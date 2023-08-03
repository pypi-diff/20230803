# Comparing `tmp/flytekit-1.8.3.tar.gz` & `tmp/flytekit-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.8.3.tar", last modified: Thu Aug  3 17:08:03 2023, max compression
+gzip compressed data, was "flytekit-1.9.0a0.tar", last modified: Thu Jul 20 18:58:06 2023, max compression
```

## Comparing `flytekit-1.8.3.tar` & `flytekit-1.9.0a0.tar`

### file list

```diff
@@ -1,257 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.520070 flytekit-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-03 17:07:50.000000 flytekit-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-03 17:07:50.000000 flytekit-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-03 17:08:03.520070 flytekit-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-03 17:07:50.000000 flytekit-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.500069 flytekit-1.8.3/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-08-03 17:08:00.000000 flytekit-1.8.3/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.500069 flytekit-1.8.3/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.500069 flytekit-1.8.3/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.500069 flytekit-1.8.3/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.500069 flytekit-1.8.3/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.500069 flytekit-1.8.3/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.500069 flytekit-1.8.3/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.504069 flytekit-1.8.3/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31873 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.504069 flytekit-1.8.3/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31360 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    18490 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    41843 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    78535 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38243 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extend/backend/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extend/backend/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.508069 flytekit-1.8.3/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.512070 flytekit-1.8.3/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.512070 flytekit-1.8.3/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.512070 flytekit-1.8.3/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.512070 flytekit-1.8.3/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.512070 flytekit-1.8.3/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.512070 flytekit-1.8.3/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.512070 flytekit-1.8.3/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.512070 flytekit-1.8.3/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    87410 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.516070 flytekit-1.8.3/flytekit/types/iterator/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/iterator/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.520070 flytekit-1.8.3/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.520070 flytekit-1.8.3/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.520070 flytekit-1.8.3/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.520070 flytekit-1.8.3/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44578 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.500069 flytekit-1.8.3/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-03 17:08:03.000000 flytekit-1.8.3/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-08-03 17:08:03.000000 flytekit-1.8.3/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:08:03.000000 flytekit-1.8.3/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-03 17:08:03.000000 flytekit-1.8.3/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-03 17:08:03.000000 flytekit-1.8.3/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 17:08:03.000000 flytekit-1.8.3/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:08:03.520070 flytekit-1.8.3/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-03 17:07:50.000000 flytekit-1.8.3/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-03 17:07:50.000000 flytekit-1.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-03 17:08:03.520070 flytekit-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-08-03 17:08:00.000000 flytekit-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.828494 flytekit-1.9.0a0/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-20 18:58:04.000000 flytekit-1.9.0a0/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.836495 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.836495 flytekit-1.9.0a0/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36184 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.844495 flytekit-1.9.0a0/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36181 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46418 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77132 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.844495 flytekit-1.9.0a0/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.844495 flytekit-1.9.0a0/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extend/backend/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extend/backend/external_plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.856495 flytekit-1.9.0a0/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.856495 flytekit-1.9.0a0/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.856495 flytekit-1.9.0a0/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86908 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-20 18:58:04.000000 flytekit-1.9.0a0/setup.py
```

### Comparing `flytekit-1.8.3/LICENSE` & `flytekit-1.9.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/MANIFEST.in` & `flytekit-1.9.0a0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/PKG-INFO` & `flytekit-1.9.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.8.3 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.9.0a0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.8.3/README.md` & `flytekit-1.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/__init__.py` & `flytekit-1.9.0a0/flytekit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,14 @@
    :toctree: generated/
 
    Description
    Documentation
    SourceCode
 
 """
-import os
 import sys
 from typing import Generator
 
 from rich import traceback
 
 from flytekit.lazy_import.lazy_module import lazy_module
 
@@ -231,23 +230,23 @@
 from flytekit.loggers import logger
 from flytekit.models.common import Annotations, AuthRole, Labels
 from flytekit.models.core.execution import WorkflowExecutionPhase
 from flytekit.models.core.types import BlobType
 from flytekit.models.documentation import Description, Documentation, SourceCode
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
-from flytekit.types import directory, file, iterator
+from flytekit.types import directory, file
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.8.3"
+__version__ = "1.9.0a0"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
@@ -300,9 +299,8 @@
         p.load()
 
 
 # Load all implicit plugins
 load_implicit_plugins()
 
 # Pretty-print exception messages
-if os.environ.get("FLYTE_SDK_RICH_TRACEBACKS") != "0":
-    traceback.install(width=None, extra_lines=0)
+traceback.install(width=None, extra_lines=0)
```

### Comparing `flytekit-1.8.3/flytekit/bin/entrypoint.py` & `flytekit-1.9.0a0/flytekit/bin/entrypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from flytekit.core import utils
 from flytekit.core.base_task import IgnoreOutputs, PythonTask
 from flytekit.core.checkpointer import SyncCheckpoint
 from flytekit.core.context_manager import ExecutionParameters, ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.data_persistence import FileAccessProvider
 from flytekit.core.map_task import MapTaskResolver
 from flytekit.core.promise import VoidPromise
-from flytekit.deck.deck import _output_deck
 from flytekit.exceptions import scopes as _scoped_exceptions
 from flytekit.exceptions import scopes as _scopes
 from flytekit.interfaces.stats.taggable import get_stats as _get_stats
 from flytekit.loggers import entrypoint_logger as logger
 from flytekit.loggers import user_space_logger
 from flytekit.models import dynamic_job as _dynamic_job
 from flytekit.models import literals as _literal_models
@@ -155,18 +154,14 @@
         logger.error("!! End Error Captured by Flyte !!")
 
     for k, v in output_file_dict.items():
         utils.write_proto_to_file(v.to_flyte_idl(), os.path.join(ctx.execution_state.engine_dir, k))
 
     ctx.file_access.put_data(ctx.execution_state.engine_dir, output_prefix, is_multipart=True)
     logger.info(f"Engine folder written successfully to the output prefix {output_prefix}")
-
-    if not getattr(task_def, "disable_deck", True):
-        _output_deck(task_def.name.split(".")[-1], ctx.user_space_params)
-
     logger.debug("Finished _dispatch_execute")
 
     if os.environ.get("FLYTE_FAIL_ON_ERROR", "").lower() == "true" and _constants.ERROR_FILE_NAME in output_file_dict:
         # This env is set by the flytepropeller
         # AWS batch job get the status from the exit code, so once we catch the error,
         # we should return the error code here
         exit(1)
@@ -184,24 +179,22 @@
             return os.environ[k]
     return ""
 
 
 @contextlib.contextmanager
 def setup_execution(
     raw_output_data_prefix: str,
-    output_metadata_prefix: Optional[str] = None,
     checkpoint_path: Optional[str] = None,
     prev_checkpoint: Optional[str] = None,
     dynamic_addl_distro: Optional[str] = None,
     dynamic_dest_dir: Optional[str] = None,
 ):
     """
 
-    :param raw_output_data_prefix: Where to write offloaded data (files, directories, dataframes).
-    :param output_metadata_prefix: Where to write primitive outputs.
+    :param raw_output_data_prefix:
     :param checkpoint_path:
     :param prev_checkpoint:
     :param dynamic_addl_distro: Works in concert with the other dynamic arg. If present, indicates that if a dynamic
       task were to run, it should set fast serialize to true and use these values in FastSerializationSettings
     :param dynamic_dest_dir: See above.
     :return:
     """
@@ -250,15 +243,14 @@
                 "exec_launchplan": exe_lp,
                 "api_version": _api_version,
             },
         ),
         logging=user_space_logger,
         tmp_dir=user_workspace_dir,
         raw_output_prefix=raw_output_data_prefix,
-        output_metadata_prefix=output_metadata_prefix,
         checkpoint=checkpointer,
         task_id=_identifier.Identifier(_identifier.ResourceType.TASK, tk_project, tk_domain, tk_name, tk_version),
     )
 
     try:
         file_access = FileAccessProvider(
             local_sandbox_dir=tempfile.mkdtemp(prefix="flyte"),
@@ -341,15 +333,14 @@
     :return:
     """
     if len(resolver_args) < 1:
         raise Exception("cannot be <1")
 
     with setup_execution(
         raw_output_data_prefix,
-        output_prefix,
         checkpoint_path,
         prev_checkpoint,
         dynamic_addl_distro,
         dynamic_dest_dir,
     ) as ctx:
         resolver_obj = load_object_from_module(resolver)
         # Use the resolver to load the actual task object
@@ -510,16 +501,15 @@
     for arg in task_execute_cmd:
         if arg == "--resolver":
             cmd.extend(["--dynamic-addl-distro", additional_distribution, "--dynamic-dest-dir", dest_dir])
         cmd.append(arg)
 
     # Use the commandline to run the task execute command rather than calling it directly in python code
     # since the current runtime bytecode references the older user code, rather than the downloaded distribution.
-    p = subprocess.run(cmd, check=False)
-    exit(p.returncode)
+    subprocess.run(cmd, check=True)
 
 
 @_pass_through.command("pyflyte-map-execute")
 @_click.option("--inputs", required=True)
 @_click.option("--output-prefix", required=True)
 @_click.option("--raw-output-data-prefix", required=False)
 @_click.option("--max-concurrency", type=int, required=False)
```

### Comparing `flytekit-1.8.3/flytekit/clients/auth/auth_client.py` & `flytekit-1.9.0a0/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clients/auth/authenticator.py` & `flytekit-1.9.0a0/flytekit/clients/auth/authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     token_endpoint: str
     authorization_endpoint: str
     redirect_uri: str
     client_id: str
     device_authorization_endpoint: typing.Optional[str] = None
     scopes: typing.List[str] = None
     header_key: str = "authorization"
-    audience: typing.Optional[str] = None
 
 
 class ClientConfigStore(object):
     """
     Client Config store retrieve client config. this can be done in multiple ways
     """
 
@@ -171,52 +170,43 @@
         client_id: str,
         client_secret: str,
         cfg_store: ClientConfigStore,
         header_key: typing.Optional[str] = None,
         scopes: typing.Optional[typing.List[str]] = None,
         http_proxy_url: typing.Optional[str] = None,
         verify: typing.Optional[typing.Union[bool, str]] = None,
-        audience: typing.Optional[str] = None,
     ):
         if not client_id or not client_secret:
             raise ValueError("Client ID and Client SECRET both are required.")
         cfg = cfg_store.get_client_config()
         self._token_endpoint = cfg.token_endpoint
         # Use scopes from `flytekit.configuration.PlatformConfig` if passed
         self._scopes = scopes or cfg.scopes
         self._client_id = client_id
         self._client_secret = client_secret
-        self._audience = audience or cfg.audience
         super().__init__(endpoint, cfg.header_key or header_key, http_proxy_url=http_proxy_url, verify=verify)
 
     def refresh_credentials(self):
         """
         This function is used by the _handle_rpc_error() decorator, depending on the AUTH_MODE config object. This handler
         is meant for SDK use-cases of auth (like pyflyte, or when users call SDK functions that require access to Admin,
         like when waiting for another workflow to complete from within a task). This function uses basic auth, which means
         the credentials for basic auth must be present from wherever this code is running.
 
         """
         token_endpoint = self._token_endpoint
         scopes = self._scopes
-        audience = self._audience
 
         # Note that unlike the Pkce flow, the client ID does not come from Admin.
         logging.debug(f"Basic authorization flow with client id {self._client_id} scope {scopes}")
         authorization_header = token_client.get_basic_authorization_header(self._client_id, self._client_secret)
 
         token, expires_in = token_client.get_token(
-            token_endpoint=token_endpoint,
-            authorization_header=authorization_header,
-            http_proxy_url=self._http_proxy_url,
-            verify=self._verify,
-            scopes=scopes,
-            audience=audience,
+            token_endpoint, scopes, authorization_header, http_proxy_url=self._http_proxy_url, verify=self._verify
         )
-
         logging.info("Retrieved new token, expires in {}".format(expires_in))
         self._creds = Credentials(token)
 
 
 class DeviceCodeAuthenticator(Authenticator):
     """
     This Authenticator implements the Device Code authorization flow useful for headless user authentication.
```

### Comparing `flytekit-1.8.3/flytekit/clients/auth/keyring.py` & `flytekit-1.9.0a0/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clients/auth/token_client.py` & `flytekit-1.9.0a0/flytekit/clients/auth/token_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 
 def get_token(
     token_endpoint: str,
     scopes: typing.Optional[typing.List[str]] = None,
     authorization_header: typing.Optional[str] = None,
     client_id: typing.Optional[str] = None,
     device_code: typing.Optional[str] = None,
-    audience: typing.Optional[str] = None,
     grant_type: GrantType = GrantType.CLIENT_CREDS,
     http_proxy_url: typing.Optional[str] = None,
     verify: typing.Optional[typing.Union[bool, str]] = None,
 ) -> typing.Tuple[str, int]:
     """
     :rtype: (Text,Int) The first element is the access token retrieved from the IDP, the second is the expiration
             in seconds
@@ -95,20 +94,17 @@
     }
     if client_id:
         body["client_id"] = client_id
     if device_code:
         body["device_code"] = device_code
     if scopes is not None:
         body["scope"] = ",".join(scopes)
-    if audience:
-        body["audience"] = audience
 
     proxies = {"https": http_proxy_url, "http": http_proxy_url} if http_proxy_url else None
     response = requests.post(token_endpoint, data=body, headers=headers, proxies=proxies, verify=verify)
-
     if not response.ok:
         j = response.json()
         if "error" in j:
             err = j["error"]
             if err == error_auth_pending or err == error_slow_down:
                 raise AuthenticationPending(f"Token not yet available, try again in some time {err}")
         logging.error("Status Code ({}) received from IDP: {}".format(response.status_code, response.text))
```

### Comparing `flytekit-1.8.3/flytekit/clients/auth_helper.py` & `flytekit-1.9.0a0/flytekit/clients/auth_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,14 @@
             token_endpoint=oauth2_metadata.token_endpoint,
             authorization_endpoint=oauth2_metadata.authorization_endpoint,
             redirect_uri=public_client_config.redirect_uri,
             client_id=public_client_config.client_id,
             scopes=public_client_config.scopes,
             header_key=public_client_config.authorization_metadata_key or None,
             device_authorization_endpoint=oauth2_metadata.device_authorization_endpoint,
-            audience=public_client_config.audience,
         )
 
 
 def get_authenticator(cfg: PlatformConfig, cfg_store: ClientConfigStore) -> Authenticator:
     """
     Returns a new authenticator based on the platform config.
     """
@@ -70,15 +69,14 @@
     elif cfg_auth == AuthType.BASIC or cfg_auth == AuthType.CLIENT_CREDENTIALS or cfg_auth == AuthType.CLIENTSECRET:
         return ClientCredentialsAuthenticator(
             endpoint=cfg.endpoint,
             client_id=cfg.client_id,
             client_secret=cfg.client_credentials_secret,
             cfg_store=cfg_store,
             scopes=cfg.scopes,
-            audience=cfg.audience,
             http_proxy_url=cfg.http_proxy_url,
             verify=verify,
         )
     elif cfg_auth == AuthType.EXTERNAL_PROCESS or cfg_auth == AuthType.EXTERNALCOMMAND:
         client_cfg = None
         if cfg_store:
             client_cfg = cfg_store.get_client_config()
@@ -174,17 +172,15 @@
         return grpc.insecure_channel(cfg.endpoint, **kwargs)
 
     credentials = None
     if "credentials" not in kwargs:
         if cfg.insecure_skip_verify:
             credentials = bootstrap_creds_from_server(cfg.endpoint)
         elif cfg.ca_cert_file_path:
-            credentials = grpc.ssl_channel_credentials(
-                crypto.dump_certificate(crypto.FILETYPE_PEM, load_cert(cfg.ca_cert_file_path))
-            )
+            credentials = grpc.ssl_channel_credentials(load_cert(cfg.ca_cert_file_path))
         else:
             credentials = grpc.ssl_channel_credentials(
                 root_certificates=kwargs.get("root_certificates", None),
                 private_key=kwargs.get("private_key", None),
                 certificate_chain=kwargs.get("certificate_chain", None),
             )
     else:
```

### Comparing `flytekit-1.8.3/flytekit/clients/friendly.py` & `flytekit-1.9.0a0/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.9.0a0/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.9.0a0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clients/helpers.py` & `flytekit-1.9.0a0/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clients/raw.py` & `flytekit-1.9.0a0/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/flyte_cli/main.py` & `flytekit-1.9.0a0/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/helpers.py` & `flytekit-1.9.0a0/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """
 
     def __init__(self, filename: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._filename = pathlib.Path(filename).resolve()
 
     def list_commands(self, ctx):
-        entities = get_entities_in_file(self._filename.__str__(), False)
+        entities = get_entities_in_file(self._filename.__str__())
         return entities.all()
 
     def get_command(self, ctx, exe_entity):
         """
         This command uses the filename with which this command was created, and the string name of the entity passed
           after the Python filename on the command line, to load the Python object, and then return the Command that
           click should run.
```

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 CTX_PACKAGES = "pkgs"
 CTX_NOTIFICATIONS = "notifications"
 CTX_CONFIG_FILE = "config_file"
 CTX_PROJECT_ROOT = "project_root"
 CTX_MODULE = "module"
 CTX_VERBOSE = "verbose"
 CTX_COPY_ALL = "copy_all"
-CTX_FILE_NAME = "file_name"
 
 
 project_option = _click.option(
     "-p",
     "--project",
     required=True,
     type=str,
```

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import typing
 
 import grpc
 import rich_click as click
 from google.protobuf.json_format import MessageToJson
 
 from flytekit import configuration
@@ -14,15 +13,14 @@
 from flytekit.clis.sdk_in_container.local_cache import local_cache
 from flytekit.clis.sdk_in_container.metrics import metrics
 from flytekit.clis.sdk_in_container.package import package
 from flytekit.clis.sdk_in_container.register import register
 from flytekit.clis.sdk_in_container.run import run
 from flytekit.clis.sdk_in_container.serialize import serialize
 from flytekit.clis.sdk_in_container.serve import serve
-from flytekit.configuration.file import FLYTECTL_CONFIG_ENV_VAR, FLYTECTL_CONFIG_ENV_VAR_OVERRIDE
 from flytekit.configuration.internal import LocalSDK
 from flytekit.exceptions.base import FlyteException
 from flytekit.exceptions.user import FlyteInvalidInputException
 from flytekit.loggers import cli_logger
 
 
 def validate_package(ctx, param, values):
@@ -118,20 +116,14 @@
     ctx.obj = dict()
 
     # Handle package management - get from the command line, the environment variables, then the config file.
     pkgs = pkgs or LocalSDK.WORKFLOW_PACKAGES.read() or []
     if config:
         ctx.obj[CTX_CONFIG_FILE] = config
         cfg = configuration.ConfigFile(config)
-        # Set here so that if someone has Config.auto() in their user code, the config here will get used.
-        if FLYTECTL_CONFIG_ENV_VAR in os.environ:
-            cli_logger.info(
-                f"Config file arg {config} will override env var {FLYTECTL_CONFIG_ENV_VAR}: {os.environ[FLYTECTL_CONFIG_ENV_VAR]}"
-            )
-        os.environ[FLYTECTL_CONFIG_ENV_VAR_OVERRIDE] = config
         if not pkgs:
             pkgs = LocalSDK.WORKFLOW_PACKAGES.read(cfg)
             if pkgs is None:
                 pkgs = []
     ctx.obj[CTX_PACKAGES] = pkgs
     ctx.obj[CTX_VERBOSE] = verbose
```

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from typing_extensions import get_args
 
 from flytekit import BlobType, Literal, Scalar
 from flytekit.clis.sdk_in_container.constants import (
     CTX_CONFIG_FILE,
     CTX_COPY_ALL,
     CTX_DOMAIN,
-    CTX_FILE_NAME,
     CTX_MODULE,
     CTX_PROJECT,
     CTX_PROJECT_ROOT,
 )
 from flytekit.clis.sdk_in_container.helpers import (
     FLYTE_REMOTE_INSTANCE_KEY,
     get_and_save_remote_with_click_context,
@@ -108,23 +107,21 @@
 
 class PickleParamType(click.ParamType):
     name = "pickle"
 
     def convert(
         self, value: typing.Any, param: typing.Optional[click.Parameter], ctx: typing.Optional[click.Context]
     ) -> typing.Any:
-
         uri = FlyteContextManager.current_context().file_access.get_random_local_path()
         with open(uri, "w+b") as outfile:
             cloudpickle.dump(value, outfile)
         return FileParam(filepath=str(pathlib.Path(uri).resolve()))
 
 
 class DateTimeType(click.DateTime):
-
     _NOW_FMT = "now"
     _ADDITONAL_FORMATS = [_NOW_FMT]
 
     def __init__(self):
         super().__init__()
         self.formats.extend(self._ADDITONAL_FORMATS)
 
@@ -273,15 +270,14 @@
             uri = native_url[: -len(remote_filename)]
 
         return uri
 
     def convert_to_structured_dataset(
         self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: Directory
     ) -> Literal:
-
         uri = self.get_uri_for_dir(ctx, value, "00000.parquet")
 
         lit = Literal(
             scalar=Scalar(
                 structured_dataset=literals.StructuredDataset(
                     uri=uri,
                     metadata=literals.StructuredDatasetMetadata(
@@ -335,15 +331,15 @@
             )
             try:
                 # Here we use click converter to convert the input in command line to native python type,
                 # and then use flyte converter to convert it to literal.
                 python_val = converter._click_type.convert(value, param, ctx)
                 literal = converter.convert_to_literal(ctx, param, python_val)
                 return Literal(scalar=Scalar(union=Union(literal, variant)))
-            except (Exception or AttributeError) as e:
+            except Exception or AttributeError as e:
                 logging.debug(f"Failed to convert python type {python_type} to literal type {variant}", e)
         raise ValueError(f"Failed to convert python type {self._python_type} to literal type {lt}")
 
     def convert_to_list(
         self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: list
     ) -> Literal:
         """
@@ -396,15 +392,18 @@
         param: typing.Optional[click.Parameter],
         value: typing.Union[dict, typing.Any],
     ) -> Literal:
         """
         Convert the loaded json object to a Flyte Literal struct type.
         """
         if type(value) != self._python_type:
-            o = cast(DataClassJsonMixin, self._python_type).from_json(json.dumps(value))
+            if is_pydantic_basemodel(self._python_type):
+                o = self._python_type.parse_raw(json.dumps(value))  # type: ignore
+            else:
+                o = cast(DataClassJsonMixin, self._python_type).from_json(json.dumps(value))
         else:
             o = value
         return TypeEngine.to_literal(self._flyte_ctx, o, self._python_type, self._literal_type)
 
     def convert_to_literal(
         self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: typing.Any
     ) -> Literal:
@@ -443,14 +442,23 @@
             return lit
         except click.BadParameter:
             raise
         except Exception as e:
             raise click.BadParameter(f"Failed to convert param {param}, {value} to {self._python_type}") from e
 
 
+def is_pydantic_basemodel(python_type: typing.Type) -> bool:
+    try:
+        import pydantic
+    except ImportError:
+        return False
+    else:
+        return issubclass(python_type, pydantic.BaseModel)
+
+
 def to_click_option(
     ctx: click.Context,
     flyte_ctx: FlyteContext,
     input_name: str,
     literal_var: Variable,
     python_type: typing.Type,
     default_val: typing.Any,
@@ -623,15 +631,15 @@
     def all(self) -> typing.List[str]:
         e = []
         e.extend(self.workflows)
         e.extend(self.tasks)
         return e
 
 
-def get_entities_in_file(filename: pathlib.Path, should_delete: bool) -> Entities:
+def get_entities_in_file(filename: str) -> Entities:
     """
     Returns a list of flyte workflow names and list of Flyte tasks in a file.
     """
     flyte_ctx = context_manager.FlyteContextManager.current_context().new_builder()
     module_name = os.path.splitext(os.path.relpath(filename))[0].replace(os.path.sep, ".")
     with context_manager.FlyteContextManager.with_context(flyte_ctx):
         with module_loader.add_sys_path(os.getcwd()):
@@ -643,16 +651,14 @@
     for name in dir(module):
         o = module.__dict__[name]
         if isinstance(o, WorkflowBase):
             workflows.append(name)
         elif isinstance(o, PythonTask):
             tasks.append(name)
 
-    if should_delete and os.path.exists(filename):
-        os.remove(filename)
     return Entities(workflows, tasks)
 
 
 def run_command(ctx: click.Context, entity: typing.Union[PythonFunctionWorkflow, PythonTask]):
     """
     Returns a function that is used to implement WorkflowCommand and execute a flyte workflow.
     """
@@ -665,16 +671,14 @@
         inputs = {}
         for input_name, _ in entity.python_interface.inputs.items():
             inputs[input_name] = kwargs.get(input_name)
 
         if not ctx.obj[REMOTE_FLAG_KEY]:
             output = entity(**inputs)
             click.echo(output)
-            if ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME):
-                os.remove(ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME))
             return
 
         remote = ctx.obj[FLYTE_REMOTE_INSTANCE_KEY]
         config_file = ctx.obj.get(CTX_CONFIG_FILE)
 
         image_config = run_level_params.get("image_config")
         image_config = patch_image_config(config_file, image_config)
@@ -712,40 +716,28 @@
 
         console_url = remote.generate_console_url(execution)
         click.secho(f"Go to {console_url} to see execution in the console.")
 
         if run_level_params.get("dump_snippet"):
             dump_flyte_remote_snippet(execution, project, domain)
 
-        if ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME):
-            os.remove(ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME))
-
     return _run
 
 
 class WorkflowCommand(click.RichGroup):
     """
     click multicommand at the python file layer, subcommands should be all the workflows in the file.
     """
 
     def __init__(self, filename: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
-
-        ctx = context_manager.FlyteContextManager.current_context()
-        if ctx.file_access.is_remote(filename):
-            local_path = os.path.join(os.path.curdir, filename.rsplit("/", 1)[1])
-            ctx.file_access.download(filename, local_path)
-            self._filename = pathlib.Path(local_path).resolve()
-            self._should_delete = True
-        else:
-            self._filename = pathlib.Path(filename).resolve()
-            self._should_delete = False
+        self._filename = pathlib.Path(filename).resolve()
 
     def list_commands(self, ctx):
-        entities = get_entities_in_file(self._filename, self._should_delete)
+        entities = get_entities_in_file(self._filename)
         return entities.all()
 
     def get_command(self, ctx, exe_entity):
         """
         This command uses the filename with which this command was created, and the string name of the entity passed
           after the Python filename on the command line, to load the Python object, and then return the Command that
           click should run.
@@ -767,16 +759,15 @@
         # N.B.: by construction project_root will necessarily be an ancestor of the filename passed in as
         # a parameter.
         rel_path = self._filename.relative_to(project_root)
         module = os.path.splitext(rel_path)[0].replace(os.path.sep, ".")
 
         ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_PROJECT_ROOT] = project_root
         ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_MODULE] = module
-        if self._should_delete:
-            ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_FILE_NAME] = self._filename
+
         entity = load_naive_entity(module, exe_entity, project_root)
 
         # If this is a remote execution, which we should know at this point, then create the remote object
         p = ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_PROJECT)
         d = ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_DOMAIN)
         r = get_and_save_remote_with_click_context(ctx, p, d)
         get_upload_url_fn = functools.partial(r.client.get_upload_signed_url, project=p, domain=d)
@@ -815,18 +806,19 @@
     def get_command(self, ctx, filename):
         if ctx.obj:
             ctx.obj[RUN_LEVEL_PARAMS_KEY] = ctx.params
         return WorkflowCommand(filename, name=filename, help="Run a [workflow|task] in a file using script mode")
 
 
 _run_help = """
-This command can execute either a workflow or a task from the command line, allowing for fully self-contained scripts.
-Tasks and workflows can be imported from other files.
+This command can execute either a workflow or a task from the command line, for fully self-contained scripts.
+Tasks and workflows cannot be imported from other files currently. Please use ``pyflyte package`` or
+``pyflyte register`` to handle those and then launch from the Flyte UI or ``flytectl``.
 
-Note: This command is compatible with regular Python packages, but not with namespace packages.
-When determining the root of your project, it identifies the first folder without an ``__init__.py`` file.
+Note: This command only works on regular Python packages, not namespace packages. When determining
+the root of your project, it finds the first folder that does not have an ``__init__.py`` file.
 """
 
 run = RunCommand(
     name="run",
     help=_run_help,
 )
```

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 @system_entry_point
 def serialize_all(
     pkgs: typing.List[str] = None,
     local_source_root: typing.Optional[str] = None,
     folder: typing.Optional[str] = None,
     mode: typing.Optional[SerializationMode] = None,
-    image_config: typing.Optional[ImageConfig] = None,
+    image: typing.Optional[str] = None,
     flytekit_virtualenv_root: typing.Optional[str] = None,
     python_interpreter: typing.Optional[str] = None,
     config_file: typing.Optional[str] = None,
 ):
     """
     This function will write to the folder specified the following protobuf types ::
         flyteidl.admin.launch_plan_pb2.LaunchPlan
@@ -45,48 +45,40 @@
 
     See :py:class:`flytekit.models.core.identifier.ResourceType` to match the trailing index in the file name with the
     entity type.
     :param pkgs: Dot-delimited Python packages/subpackages to look into for serialization.
     :param local_source_root: Where to start looking for the code.
     :param folder: Where to write the output protobuf files
     :param mode: Regular vs fast
-    :param image_config: ImageConfig object to use
+    :param image: The fully qualified and versioned default image to use
     :param flytekit_virtualenv_root: The full path of the virtual env in the container.
     """
 
     if not (mode == SerializationMode.DEFAULT or mode == SerializationMode.FAST):
         raise AssertionError(f"Unrecognized serialization mode: {mode}")
 
     serialization_settings = SerializationSettings(
-        image_config=image_config or ImageConfig.auto(config_file),
+        image_config=ImageConfig.auto(config_file, img_name=image),
         fast_serialization_settings=FastSerializationSettings(
             enabled=mode == SerializationMode.FAST,
             # TODO: if we want to move the destination dir as a serialization argument, we should initialize it here
         ),
         flytekit_virtualenv_root=flytekit_virtualenv_root,
         python_interpreter=python_interpreter,
     )
 
     serialize_to_folder(pkgs, serialization_settings, local_source_root, folder)
 
 
 @click.group("serialize", cls=click.RichGroup)
 @click.option(
-    "-i",
     "--image",
-    "image_config",
     required=False,
-    multiple=True,
-    type=click.UNPROCESSED,
-    callback=ImageConfig.validate_image,
-    help="A fully qualified tag for an docker image, for example ``somedocker.com/myimage:someversion123``. This is a "
-    "multi-option and can be of the form ``--image xyz.io/docker:latest"
-    " --image my_image=xyz.io/docker2:latest``. Note, the ``name=image_uri``. The name is optional, if not "
-    "provided the image will be used as the default image. All the names have to be unique, and thus "
-    "there can only be one ``--image`` option with no name.",
+    default=lambda: os.environ.get("FLYTE_INTERNAL_IMAGE", ""),
+    help="Text tag, for example ``somedocker.com/myimage:someversion123``",
 )
 @click.option(
     "--local-source-root",
     required=False,
     default=lambda: os.getcwd(),
     help="Root dir for Python code containing workflow definitions to operate on when not the current working directory. "
     "Optional when running ``pyflyte serialize`` in out-of-container-mode and your code lies outside of your working directory.",
@@ -103,27 +95,25 @@
     required=False,
     help="DEPRECATED: This flag is ignored! This is the root of the flytekit virtual env in your container. "
     "The reason it needs to be a separate option is because this pyflyte utility cannot know where flytekit is "
     "installed inside your container. Required for running `pyflyte serialize` in out of container mode when "
     "your container installs the flytekit virtualenv outside of the default `/opt/venv`",
 )
 @click.pass_context
-def serialize(
-    ctx, image_config: ImageConfig, local_source_root, in_container_config_path, in_container_virtualenv_root
-):
+def serialize(ctx, image, local_source_root, in_container_config_path, in_container_virtualenv_root):
     """
     This command produces protobufs for tasks and templates.
     For tasks, one pb file is produced for each task, representing one TaskTemplate object.
     For workflows, one pb file is produced for each workflow, representing a WorkflowClosure object. The closure
     object contains the WorkflowTemplate, along with the relevant tasks for that workflow. In lieu of Admin,
     this serialization step will set the URN of the tasks to the fully qualified name of the task function.
     """
-    ctx.obj[CTX_IMAGE] = image_config
+    ctx.obj[CTX_IMAGE] = image
     ctx.obj[CTX_LOCAL_SRC_ROOT] = local_source_root
-    click.echo(f"Serializing Flyte elements with image {image_config}")
+    click.echo("Serializing Flyte elements with image {}".format(image))
 
     if in_container_virtualenv_root:
         ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT] = in_container_virtualenv_root
         ctx.obj[CTX_PYTHON_INTERPRETER] = os.path.join(in_container_virtualenv_root, "/bin/python3")
     else:
         # For in container serialize we make sure to never accept an override the entrypoint path and determine it here
         # instead.
@@ -147,15 +137,15 @@
     pkgs = ctx.obj[CTX_PACKAGES]
     dir = ctx.obj[CTX_LOCAL_SRC_ROOT]
     serialize_all(
         pkgs,
         dir,
         folder,
         SerializationMode.DEFAULT,
-        image_config=ctx.obj[CTX_IMAGE],
+        image=ctx.obj[CTX_IMAGE],
         flytekit_virtualenv_root=ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT],
         python_interpreter=ctx.obj[CTX_PYTHON_INTERPRETER],
         config_file=ctx.obj.get(constants.CTX_CONFIG_FILE, None),
     )
 
 
 @click.group("fast", cls=click.RichGroup)
@@ -186,15 +176,15 @@
     pkgs = ctx.obj[CTX_PACKAGES]
     dir = ctx.obj[CTX_LOCAL_SRC_ROOT]
     serialize_all(
         pkgs,
         dir,
         folder,
         SerializationMode.FAST,
-        image_config=ctx.obj[CTX_IMAGE],
+        image=ctx.obj[CTX_IMAGE],
         flytekit_virtualenv_root=ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT],
         python_interpreter=ctx.obj[CTX_PYTHON_INTERPRETER],
         config_file=ctx.obj.get(constants.CTX_CONFIG_FILE, None),
     )
 
 
 fast.add_command(fast_workflows)
```

### Comparing `flytekit-1.8.3/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/serve.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from concurrent import futures
 
 import click
 import grpc
-from flyteidl.service.agent_pb2_grpc import add_AsyncAgentServiceServicer_to_server
+from flyteidl.service.external_plugin_service_pb2_grpc import add_ExternalPluginServiceServicer_to_server
 
-from flytekit.extend.backend.agent_service import AgentService
+from flytekit.extend.backend.external_plugin_service import BackendPluginServer
 
-_serve_help = """Start a grpc server for the agent service."""
+_serve_help = """Start a grpc server for the external plugin service."""
 
 
 @click.command("serve", help=_serve_help)
 @click.option(
     "--port",
     default="8000",
     is_flag=False,
     type=int,
-    help="Grpc port for the agent service",
+    help="Grpc port for the external plugin service",
 )
 @click.option(
     "--worker",
     default="10",
     is_flag=False,
     type=int,
     help="Number of workers for the grpc server",
@@ -31,16 +31,16 @@
     type=int,
     help="It will wait for the specified number of seconds before shutting down grpc server. It should only be used "
     "for testing.",
 )
 @click.pass_context
 def serve(_: click.Context, port, worker, timeout):
     """
-    Start a grpc server for the agent service.
+    Start a grpc server for the external plugin service.
     """
-    click.secho("Starting the agent service...", fg="blue")
+    click.secho("Starting the external plugin service...", fg="blue")
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=worker))
-    add_AsyncAgentServiceServicer_to_server(AgentService(), server)
+    add_ExternalPluginServiceServicer_to_server(BackendPluginServer(), server)
 
     server.add_insecure_port(f"[::]:{port}")
     server.start()
     server.wait_for_termination(timeout=timeout)
```

### Comparing `flytekit-1.8.3/flytekit/configuration/__init__.py` & `flytekit-1.9.0a0/flytekit/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,17 +278,14 @@
                     f"Only one default image can be specified. Received multiple {default_image} & {img} for {param}"
                 )
             if img.name == DEFAULT_IMAGE_NAME:
                 default_image = img
             else:
                 images.append(img)
 
-        if default_image is None:
-            default_image_str = os.environ.get("FLYTE_INTERNAL_IMAGE", DefaultImages.default_image())
-            default_image = Image.look_up_image_info(DEFAULT_IMAGE_NAME, default_image_str, False)
         return ImageConfig.create_from(default_image=default_image, other_images=images)
 
     @classmethod
     def create_from(
         cls, default_image: Optional[Image], other_images: typing.Optional[typing.List[Image]] = None
     ) -> ImageConfig:
         if default_image and not isinstance(default_image, Image):
@@ -427,15 +424,14 @@
             "client_credentials_secret",
             client_credentials_secret,
         )
         kwargs = set_if_exists(kwargs, "scopes", _internal.Credentials.SCOPES.read(config_file))
         kwargs = set_if_exists(kwargs, "auth_mode", _internal.Credentials.AUTH_MODE.read(config_file))
         kwargs = set_if_exists(kwargs, "endpoint", _internal.Platform.URL.read(config_file))
         kwargs = set_if_exists(kwargs, "console_endpoint", _internal.Platform.CONSOLE_ENDPOINT.read(config_file))
-
         kwargs = set_if_exists(kwargs, "http_proxy_url", _internal.Platform.HTTP_PROXY_URL.read(config_file))
         return PlatformConfig(**kwargs)
 
     @classmethod
     def for_endpoint(cls, endpoint: str, insecure: bool = False) -> PlatformConfig:
         return PlatformConfig(endpoint=endpoint, insecure=insecure)
```

### Comparing `flytekit-1.8.3/flytekit/configuration/default_images.py` & `flytekit-1.9.0a0/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/configuration/feature_flags.py` & `flytekit-1.9.0a0/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/configuration/file.py` & `flytekit-1.9.0a0/flytekit/configuration/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 import yaml
 
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.loggers import logger
 
 # This is the env var that the flytectl sandbox instructions say to set
 FLYTECTL_CONFIG_ENV_VAR = "FLYTECTL_CONFIG"
-# This is an explicit override only to be used by pyflyte and takes precedence in get_config_file over the main
-# environment variable.
-# This env var should not be set by users
-FLYTECTL_CONFIG_ENV_VAR_OVERRIDE = "_FLYTECTL_CONFIG_PYFLYTE_OVERRIDE"
 
 
 def _exists(val: typing.Any) -> bool:
     """Check if a value is defined."""
     return isinstance(val, bool) or bool(val is not None and val)
 
 
@@ -239,39 +235,33 @@
 
 
 def get_config_file(c: typing.Union[str, ConfigFile, None]) -> typing.Optional[ConfigFile]:
     """
     Checks if the given argument is a file or a configFile and returns a loaded configFile else returns None
     """
     if c is None:
-        # Pyflyte override env var takes highest precedence
-        # Env var takes second highest precedence
-        flytectl_path_from_env = getenv(FLYTECTL_CONFIG_ENV_VAR_OVERRIDE, getenv(FLYTECTL_CONFIG_ENV_VAR, None))
-        if flytectl_path_from_env:
-            flytectl_path = Path(flytectl_path_from_env)
-            if flytectl_path.exists():
-                logger.info(f"Using flytectl/YAML config {flytectl_path.absolute()}")
-                return ConfigFile(str(flytectl_path.absolute()))
-            else:
-                logger.warning(f"flytectl config file {flytectl_path.absolute()} does not exist, ignoring...")
-
         # See if there's a config file in the current directory where Python is being run from
         current_location_config = Path("flytekit.config")
         if current_location_config.exists():
             logger.info(f"Using configuration from Python process root {current_location_config.absolute()}")
             return ConfigFile(str(current_location_config.absolute()))
 
         # If not, see if there's a config in the user's home directory
         home_dir_config = Path(Path.home(), ".flyte", "config")  # _default_config_file_name in main.py
         if home_dir_config.exists():
             logger.info(f"Using configuration from home directory {home_dir_config.absolute()}")
             return ConfigFile(str(home_dir_config.absolute()))
 
-        # If not see if there's something in the default home directory location
+        # If not, see if the env var that flytectl sandbox tells the user to set is set,
+        # or see if there's something in the default home directory location
         flytectl_path = Path(Path.home(), ".flyte", "config.yaml")
+        flytectl_path_from_env = getenv(FLYTECTL_CONFIG_ENV_VAR, None)
+
+        if flytectl_path_from_env:
+            flytectl_path = Path(flytectl_path_from_env)
         if flytectl_path.exists():
             logger.info(f"Using flytectl/YAML config {flytectl_path.absolute()}")
             return ConfigFile(str(flytectl_path.absolute()))
 
         # If not, then return None and let caller handle
         return None
     if isinstance(c, str):
```

### Comparing `flytekit-1.8.3/flytekit/configuration/internal.py` & `flytekit-1.9.0a0/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/annotation.py` & `flytekit-1.9.0a0/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/base_sql_task.py` & `flytekit-1.9.0a0/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/base_task.py` & `flytekit-1.9.0a0/flytekit/core/base_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,17 +598,15 @@
                 for k, v in native_inputs.items():
                     input_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_input_var(k, v)))
 
                 output_deck = Deck(OUTPUT)
                 for k, v in native_outputs_as_map.items():
                     output_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_output_var(k, v)))
 
-                if ctx.execution_state and ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
-                    # When we run the workflow remotely, flytekit outputs decks at the end of _dispatch_execute
-                    _output_deck(self.name.split(".")[-1], new_user_params)
+                _output_deck(self.name.split(".")[-1], new_user_params)
 
             outputs_literal_map = _literal_models.LiteralMap(literals=literals)
             # After the execute has been successfully completed
             return outputs_literal_map
 
     def pre_execute(self, user_params: Optional[ExecutionParameters]) -> Optional[ExecutionParameters]:  # type: ignore
         """
```

### Comparing `flytekit-1.8.3/flytekit/core/checkpointer.py` & `flytekit-1.9.0a0/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/class_based_resolver.py` & `flytekit-1.9.0a0/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/condition.py` & `flytekit-1.9.0a0/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/constants.py` & `flytekit-1.9.0a0/flytekit/core/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 INPUT_FILE_NAME = "inputs.pb"
 OUTPUT_FILE_NAME = "outputs.pb"
 FUTURES_FILE_NAME = "futures.pb"
 ERROR_FILE_NAME = "error.pb"
-REQUIREMENTS_FILE_NAME = "requirements.txt"
 
 
 class SdkTaskType(object):
     PYTHON_TASK = "python-task"
     DYNAMIC_TASK = "dynamic-task"
     CONTAINER_ARRAY_TASK = "container_array"
     SPARK_TASK = "spark"
```

### Comparing `flytekit-1.8.3/flytekit/core/container_task.py` & `flytekit-1.9.0a0/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/context_manager.py` & `flytekit-1.9.0a0/flytekit/core/context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,14 @@
         self,
         execution_date,
         tmp_dir,
         stats,
         execution_id: typing.Optional[_identifier.WorkflowExecutionIdentifier],
         logging,
         raw_output_prefix,
-        output_metadata_prefix=None,
         checkpoint=None,
         decks=None,
         task_id: typing.Optional[_identifier.Identifier] = None,
         **kwargs,
     ):
         """
         Args:
@@ -170,15 +169,14 @@
             decks = []
         self._stats = stats
         self._execution_date = execution_date
         self._working_directory = tmp_dir
         self._execution_id = execution_id
         self._logging = logging
         self._raw_output_prefix = raw_output_prefix
-        self._output_metadata_prefix = output_metadata_prefix
         # AutoDeletingTempDir's should be used with a with block, which creates upon entry
         self._attrs = kwargs
         # It is safe to recreate the Secrets Manager
         self._secrets_manager = SecretsManager()
         self._checkpoint = checkpoint
         self._decks = decks
         self._task_id = task_id
@@ -200,18 +198,14 @@
         return self._logging
 
     @property
     def raw_output_prefix(self) -> str:
         return self._raw_output_prefix
 
     @property
-    def output_metadata_prefix(self) -> str:
-        return self._output_metadata_prefix
-
-    @property
     def working_directory(self) -> str:
         """
         A handle to a special working directory for easily producing temporary files.
         TODO: Usage examples
         """
         return self._working_directory
```

### Comparing `flytekit-1.8.3/flytekit/core/data_persistence.py` & `flytekit-1.9.0a0/flytekit/core/data_persistence.py`

 * *Files 5% similar despite different names*

```diff
@@ -199,29 +199,29 @@
             logger.debug(f"Error in getting {from_path} to {to_path} rec {recursive} {oe}")
             file_system = self.get_filesystem(get_protocol(from_path), anonymous=True)
             if file_system is not None:
                 logger.debug(f"Attempting anonymous get with {file_system}")
                 return file_system.get(from_path, to_path, recursive=recursive)
             raise oe
 
-    def put(self, from_path: str, to_path: str, recursive: bool = False, **kwargs):
+    def put(self, from_path: str, to_path: str, recursive: bool = False):
         file_system = self.get_filesystem_for_path(to_path)
         from_path = self.strip_file_header(from_path)
         if recursive:
             # Only check this for the local filesystem
             if file_system.protocol == "file" and not file_system.isdir(from_path):
                 raise FlyteAssertion(f"Source path {from_path} is not a directory")
             if os.name == "nt" and file_system.protocol == "file":
                 import shutil
 
                 return shutil.copytree(
                     self.strip_file_header(from_path), self.strip_file_header(to_path), dirs_exist_ok=True
                 )
             from_path, to_path = self.recursive_paths(from_path, to_path)
-        return file_system.put(from_path, to_path, recursive=recursive, **kwargs)
+        return file_system.put(from_path, to_path, recursive=recursive)
 
     def get_random_remote_path(self, file_path_or_file_name: typing.Optional[str] = None) -> str:
         """
         Constructs a randomized path on the configured raw_output_prefix (persistence layer). the random bit is a UUID
         and allows for disambiguating paths within the same directory.
 
         Use file_path_or_file_name, when you want a random directory, but want to preserve the leaf file name
@@ -283,43 +283,44 @@
     def upload_directory(self, local_path: str, remote_path: str):
         """
         :param Text local_path:
         :param Text remote_path:
         """
         return self.put_data(local_path, remote_path, is_multipart=True)
 
+    @timeit("Download data to local from remote")
     def get_data(self, remote_path: str, local_path: str, is_multipart: bool = False):
         """
         :param remote_path:
         :param local_path:
         :param is_multipart:
         """
         try:
             pathlib.Path(local_path).parent.mkdir(parents=True, exist_ok=True)
-            with timeit(f"Download data to local from {remote_path}"):
-                self.get(remote_path, to_path=local_path, recursive=is_multipart)
+            self.get(remote_path, to_path=local_path, recursive=is_multipart)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to get data from {remote_path} to {local_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             )
 
-    def put_data(self, local_path: Union[str, os.PathLike], remote_path: str, is_multipart: bool = False, **kwargs):
+    @timeit("Upload data to remote")
+    def put_data(self, local_path: Union[str, os.PathLike], remote_path: str, is_multipart: bool = False):
         """
         The implication here is that we're always going to put data to the remote location, so we .remote to ensure
         we don't use the true local proxy if the remote path is a file://
 
         :param local_path:
         :param remote_path:
         :param is_multipart:
         """
         try:
             local_path = str(local_path)
-            with timeit(f"Upload data to {remote_path}"):
-                self.put(cast(str, local_path), remote_path, recursive=is_multipart, **kwargs)
+
+            self.put(cast(str, local_path), remote_path, recursive=is_multipart)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to put data from {local_path} to {remote_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             ) from ex
```

### Comparing `flytekit-1.8.3/flytekit/core/docstring.py` & `flytekit-1.9.0a0/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.9.0a0/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/gate.py` & `flytekit-1.9.0a0/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/interface.py` & `flytekit-1.9.0a0/flytekit/core/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import collections
 import copy
 import inspect
 import typing
 from collections import OrderedDict
 from typing import Any, Dict, Generator, List, Optional, Tuple, Type, TypeVar, Union, cast
 
-from typing_extensions import get_args, get_origin, get_type_hints
+from typing_extensions import Annotated, get_args, get_origin, get_type_hints
 
 from flytekit.core import context_manager
 from flytekit.core.docstring import Docstring
 from flytekit.core.type_engine import TypeEngine
 from flytekit.exceptions.user import FlyteValidationException
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models.literals import Void
+from flytekit.types.pickle import FlytePickle
 
 T = typing.TypeVar("T")
 
 
 def repr_kv(k: str, v: Union[Type, Tuple[Type, Any]]) -> str:
     if isinstance(v, tuple):
         if v[1]:
@@ -245,20 +246,18 @@
         )
 
     inputs_map = transform_variable_map(interface.inputs, input_descriptions)
     outputs_map = transform_variable_map(interface.outputs, output_descriptions)
     return _interface_models.TypedInterface(inputs_map, outputs_map)
 
 
-def transform_types_to_list_of_type(
-    m: Dict[str, type], bound_inputs: typing.Set[str], list_as_optional: bool = False
-) -> Dict[str, type]:
+def transform_types_to_list_of_type(m: Dict[str, type], bound_inputs: typing.Set[str]) -> Dict[str, type]:
     """
-    Converts unbound inputs into the equivalent (optional) collections. This is useful for array jobs / map style code.
-    It will create a collection of types even if any one these types is not a collection type.
+    Converts a given variables to be collections of their type. This is useful for array jobs / map style code.
+    It will create a collection of types even if any one these types is not a collection type
     """
     if m is None:
         return {}
 
     all_types_are_collection = True
     for k, v in m.items():
         if k in bound_inputs:
@@ -274,54 +273,77 @@
         return m
 
     om = {}
     for k, v in m.items():
         if k in bound_inputs:
             om[k] = v
         else:
-            om[k] = typing.List[typing.Optional[v] if list_as_optional else v]  # type: ignore
+            om[k] = typing.List[v]  # type: ignore
     return om  # type: ignore
 
 
-def transform_interface_to_list_interface(
-    interface: Interface, bound_inputs: typing.Set[str], optional_outputs: bool = False
-) -> Interface:
+def transform_interface_to_list_interface(interface: Interface, bound_inputs: typing.Set[str]) -> Interface:
     """
     Takes a single task interface and interpolates it to an array interface - to allow performing distributed python map
     like functions
     :param interface: Interface to be upgraded toa list interface
     :param bound_inputs: fixed inputs that should not upgraded to a list and will be maintained as scalars.
     """
     map_inputs = transform_types_to_list_of_type(interface.inputs, bound_inputs)
-    map_outputs = transform_types_to_list_of_type(interface.outputs, set(), optional_outputs)
+    map_outputs = transform_types_to_list_of_type(interface.outputs, set())
 
     return Interface(inputs=map_inputs, outputs=map_outputs)
 
 
+def _change_unrecognized_type_to_pickle(t: Type[T]) -> typing.Union[Tuple[Type[T]], Type[T]]:
+    try:
+        if hasattr(t, "__origin__") and hasattr(t, "__args__"):
+            ot = get_origin(t)
+            args = getattr(t, "__args__")
+            if ot is list:
+                return typing.List[_change_unrecognized_type_to_pickle(args[0])]  # type: ignore
+            elif ot is dict and args[0] == str:
+                return typing.Dict[str, _change_unrecognized_type_to_pickle(args[1])]  # type: ignore
+            elif ot is typing.Union:
+                return typing.Union[tuple(_change_unrecognized_type_to_pickle(v) for v in get_args(t))]  # type: ignore
+            elif ot is Annotated:
+                base_type, *config = get_args(t)
+                return Annotated[(_change_unrecognized_type_to_pickle(base_type), *config)]  # type: ignore
+        TypeEngine.get_transformer(t)
+    except ValueError:
+        logger.warning(
+            f"Unsupported Type {t} found, Flyte will default to use PickleFile as the transport. "
+            f"Pickle can only be used to send objects between the exact same version of Python, "
+            f"and we strongly recommend to use python type that flyte support."
+        )
+        return FlytePickle[t]
+    return t
+
+
 def transform_function_to_interface(fn: typing.Callable, docstring: Optional[Docstring] = None) -> Interface:
     """
     From the annotations on a task function that the user should have provided, and the output names they want to use
     for each output parameter, construct the TypedInterface object
 
     For now the fancy object, maybe in the future a dumb object.
 
     """
     type_hints = get_type_hints(fn, include_extras=True)
     signature = inspect.signature(fn)
     return_annotation = type_hints.get("return", None)
 
     outputs = extract_return_annotation(return_annotation)
     for k, v in outputs.items():
-        outputs[k] = v  # type: ignore
+        outputs[k] = _change_unrecognized_type_to_pickle(v)  # type: ignore
     inputs: Dict[str, Tuple[Type, Any]] = OrderedDict()
     for k, v in signature.parameters.items():  # type: ignore
         annotation = type_hints.get(k, None)
         default = v.default if v.default is not inspect.Parameter.empty else None
         # Inputs with default values are currently ignored, we may want to look into that in the future
-        inputs[k] = (annotation, default)  # type: ignore
+        inputs[k] = (_change_unrecognized_type_to_pickle(annotation), default)  # type: ignore
 
     # This is just for typing.NamedTuples - in those cases, the user can select a name to call the NamedTuple. We
     # would like to preserve that name in our custom collections.namedtuple.
     custom_name = None
     if hasattr(return_annotation, "__bases__"):
         bases = return_annotation.__bases__
         if len(bases) == 1 and bases[0] == tuple and hasattr(return_annotation, "_fields"):
@@ -339,14 +361,28 @@
     Given a map of str (names of inputs for instance) to their Python native types, return a map of the name to a
     Flyte Variable object with that type.
     """
     res = OrderedDict()
     if variable_map:
         for k, v in variable_map.items():
             res[k] = transform_type(v, descriptions.get(k, k))
+            sub_type: type = v
+            if hasattr(v, "__origin__") and hasattr(v, "__args__"):
+                if getattr(v, "__origin__") is list:
+                    sub_type = getattr(v, "__args__")[0]
+                elif getattr(v, "__origin__") is dict:
+                    sub_type = getattr(v, "__args__")[1]
+            if hasattr(sub_type, "__origin__") and getattr(sub_type, "__origin__") is FlytePickle:
+                original_type = cast(FlytePickle, sub_type).python_type()
+                if hasattr(original_type, "__name__"):
+                    res[k].type.metadata = {"python_class_name": original_type.__name__}
+                elif hasattr(original_type, "_name"):
+                    # If the class doesn't have the __name__ attribute, like typing.Sequence, use _name instead.
+                    res[k].type.metadata = {"python_class_name": original_type._name}
+
     return res
 
 
 def transform_type(x: type, description: Optional[str] = None) -> _interface_models.Variable:
     return _interface_models.Variable(type=TypeEngine.to_literal_type(x), description=description)
```

### Comparing `flytekit-1.8.3/flytekit/core/launch_plan.py` & `flytekit-1.9.0a0/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/local_cache.py` & `flytekit-1.9.0a0/flytekit/core/local_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 
 # Location on the filesystem where serialized objects will be stored
 # TODO: read from config
 CACHE_LOCATION = "~/.flyte/local-cache"
 
 
 def _recursive_hash_placement(literal: Literal) -> Literal:
-    # Base case, hash gets passed through always if set
-    if literal.hash is not None:
-        return Literal(hash=literal.hash)
-    elif literal.collection is not None:
-        literals = [_recursive_hash_placement(lit) for lit in literal.collection.literals]
+    if literal.collection is not None:
+        literals = [_recursive_hash_placement(literal) for literal in literal.collection.literals]
         return Literal(collection=LiteralCollection(literals=literals))
     elif literal.map is not None:
         literal_map = {}
-        for key, literal_value in literal.map.literals.items():
-            literal_map[key] = _recursive_hash_placement(literal_value)
+        for key, literal in literal.map.literals.items():
+            literal_map[key] = _recursive_hash_placement(literal)
         return Literal(map=LiteralMap(literal_map))
+
+    # Base case
+    if literal.hash is not None:
+        return Literal(hash=literal.hash)
     else:
         return literal
 
 
 def _calculate_cache_key(task_name: str, cache_version: str, input_literal_map: LiteralMap) -> str:
     # Traverse the literals and replace the literal with a new literal that only contains the hash
     literal_map_overridden = {}
```

### Comparing `flytekit-1.8.3/flytekit/core/map_task.py` & `flytekit-1.9.0a0/flytekit/core/map_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from flytekit.configuration import SerializationSettings
 from flytekit.core import tracker
 from flytekit.core.base_task import PythonTask, Task, TaskResolverMixin
 from flytekit.core.constants import SdkTaskType
 from flytekit.core.context_manager import ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.interface import transform_interface_to_list_interface
-from flytekit.core.python_function_task import PythonFunctionTask, PythonInstanceTask
+from flytekit.core.python_function_task import PythonFunctionTask
 from flytekit.core.tracker import TrackedInstance
 from flytekit.core.utils import timeit
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.models.array_job import ArrayJob
 from flytekit.models.interface import Variable
 from flytekit.models.task import Container, K8sPod, Sql
 from flytekit.tools.module_loader import load_object_from_module
@@ -30,15 +30,15 @@
     """
     A MapPythonTask defines a :py:class:`flytekit.PythonTask` which specifies how to run
     an inner :py:class:`flytekit.PythonFunctionTask` across a range of inputs in parallel.
     """
 
     def __init__(
         self,
-        python_function_task: typing.Union[PythonFunctionTask, PythonInstanceTask, functools.partial],
+        python_function_task: typing.Union[PythonFunctionTask, functools.partial],
         concurrency: Optional[int] = None,
         min_success_ratio: Optional[float] = None,
         bound_inputs: Optional[Set[str]] = None,
         **kwargs,
     ):
         """
         Wrapper that creates a MapPythonTask
@@ -61,39 +61,26 @@
                     raise ValueError("Map tasks do not support partial tasks with lists as inputs. ")
             self._partial = python_function_task
             actual_task = self._partial.func
         else:
             actual_task = python_function_task
 
         if not isinstance(actual_task, PythonFunctionTask):
-            if isinstance(actual_task, PythonInstanceTask):
-                pass
-            else:
-                raise ValueError("Map tasks can only compose of PythonFuncton and PythonInstanceTasks currently")
+            raise ValueError("Map tasks can only compose of Python Functon Tasks currently")
 
-        n_outputs = len(actual_task.python_interface.outputs.keys())
-        if n_outputs > 1:
+        if len(actual_task.python_interface.outputs.keys()) > 1:
             raise ValueError("Map tasks only accept python function tasks with 0 or 1 outputs")
 
         self._bound_inputs: typing.Set[str] = set(bound_inputs) if bound_inputs else set()
         if self._partial:
             self._bound_inputs = set(self._partial.keywords.keys())
 
-        # Transform the interface to List[Optional[T]] in case `min_success_ratio` is set
-        output_as_list_of_optionals = min_success_ratio is not None and min_success_ratio != 1 and n_outputs == 1
-        collection_interface = transform_interface_to_list_interface(
-            actual_task.python_interface, self._bound_inputs, output_as_list_of_optionals
-        )
-
-        self._run_task: typing.Union[PythonFunctionTask, PythonInstanceTask] = actual_task  # type: ignore
-        if isinstance(actual_task, PythonInstanceTask):
-            mod = actual_task.task_type
-            f = actual_task.lhs
-        else:
-            _, mod, f, _ = tracker.extract_task_module(typing.cast(PythonFunctionTask, actual_task).task_function)
+        collection_interface = transform_interface_to_list_interface(actual_task.python_interface, self._bound_inputs)
+        self._run_task: PythonFunctionTask = actual_task
+        _, mod, f, _ = tracker.extract_task_module(actual_task.task_function)
         h = hashlib.md5(collection_interface.__str__().encode("utf-8")).hexdigest()
         name = f"{mod}.map_{f}_{h}"
 
         self._cmd_prefix: typing.Optional[typing.List[str]] = None
         self._max_concurrency: typing.Optional[int] = concurrency
         self._min_success_ratio: typing.Optional[float] = min_success_ratio
         self._array_task_interface = actual_task.python_interface
@@ -170,15 +157,15 @@
     def get_custom(self, settings: SerializationSettings) -> Dict[str, Any]:
         return ArrayJob(parallelism=self._max_concurrency, min_success_ratio=self._min_success_ratio).to_dict()
 
     def get_config(self, settings: SerializationSettings) -> Optional[Dict[str, str]]:
         return self._run_task.get_config(settings)
 
     @property
-    def run_task(self) -> typing.Union[PythonFunctionTask, PythonInstanceTask]:
+    def run_task(self) -> PythonFunctionTask:
         return self._run_task
 
     def __call__(self, *args, **kwargs):
         """
         This call method modifies the kwargs and adds kwargs from partial.
         This is mostly done in the local_execute and compilation only.
         At runtime, the map_task is created with all the inputs filled in. to support this, we have modified
@@ -280,15 +267,15 @@
             if outputs_expected:
                 outputs.append(o)
 
         return outputs
 
 
 def map_task(
-    task_function: typing.Union[PythonFunctionTask, PythonInstanceTask, functools.partial],
+    task_function: typing.Union[PythonFunctionTask, functools.partial],
     concurrency: int = 0,
     min_success_ratio: float = 1.0,
     **kwargs,
 ):
     """
     Use a map task for parallelizable tasks that run across a list of an input type. A map task can be composed of
     any individual :py:class:`flytekit.PythonFunctionTask`.
```

### Comparing `flytekit-1.8.3/flytekit/core/mock_stats.py` & `flytekit-1.9.0a0/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/node.py` & `flytekit-1.9.0a0/flytekit/core/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,14 @@
             self._metadata._name = kwargs["name"]
         if "task_config" in kwargs:
             logger.warning("This override is beta. We may want to revisit this in the future.")
             new_task_config = kwargs["task_config"]
             if not isinstance(new_task_config, type(self.flyte_entity._task_config)):
                 raise ValueError("can't change the type of the task config")
             self.flyte_entity._task_config = new_task_config
-        if "container_image" in kwargs:
-            self.flyte_entity._container_image = kwargs["container_image"]
         return self
 
 
 def _convert_resource_overrides(
     resources: typing.Optional[Resources], resource_name: str
 ) -> typing.List[_resources_model.ResourceEntry]:
     if resources is None:
```

### Comparing `flytekit-1.8.3/flytekit/core/node_creation.py` & `flytekit-1.9.0a0/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/notification.py` & `flytekit-1.9.0a0/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/pod_template.py` & `flytekit-1.9.0a0/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/promise.py` & `flytekit-1.9.0a0/flytekit/core/promise.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,28 +19,29 @@
 )
 from flytekit.core.interface import Interface
 from flytekit.core.node import Node
 from flytekit.core.type_engine import DictTransformer, ListTransformer, TypeEngine, TypeTransformerFailedError
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
+from flytekit.models import literals as _literal_models
 from flytekit.models import literals as _literals_models
 from flytekit.models import types as _type_models
 from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.literals import Primitive
 from flytekit.models.types import SimpleType
 
 
 def translate_inputs_to_literals(
     ctx: FlyteContext,
     incoming_values: Dict[str, Any],
     flyte_interface_types: Dict[str, _interface_models.Variable],
     native_types: Dict[str, type],
-) -> Dict[str, _literals_models.Literal]:
+) -> Dict[str, _literal_models.Literal]:
     """
     The point of this function is to extract out Literals from a collection of either Python native values (which would
     be converted into Flyte literals) or Promises (the literals in which would just get extracted).
 
     When calling a task inside a workflow, a user might do something like this.
 
         def my_wf(in1: int) -> int:
@@ -64,25 +65,95 @@
     This helper function is used both when sorting out inputs to a task, as well as outputs of a function.
 
     :param ctx: Context needed in case a non-primitive literal needs to be translated to a Flyte literal (like a file)
     :param incoming_values: This is a map of your task's input or wf's output kwargs basically
     :param flyte_interface_types: One side of an :py:class:`flytekit.models.interface.TypedInterface` basically.
     :param native_types: Map to native Python type.
     """
+
+    def extract_value(
+        ctx: FlyteContext,
+        input_val: Any,
+        val_type: type,
+        flyte_literal_type: _type_models.LiteralType,
+    ) -> _literal_models.Literal:
+        if isinstance(input_val, list):
+            lt = flyte_literal_type
+            python_type = val_type
+            if flyte_literal_type.union_type:
+                for i in range(len(flyte_literal_type.union_type.variants)):
+                    variant = flyte_literal_type.union_type.variants[i]
+                    if variant.collection_type:
+                        lt = variant
+                        python_type = get_args(val_type)[i]
+            if lt.collection_type is None:
+                raise TypeError(f"Not a collection type {flyte_literal_type} but got a list {input_val}")
+            try:
+                sub_type: type = ListTransformer.get_sub_type(python_type)
+            except ValueError:
+                if len(input_val) == 0:
+                    raise
+                sub_type = type(input_val[0])
+            # To maintain consistency between translate_inputs_to_literals and ListTransformer.to_literal for batchable types,
+            # directly call ListTransformer.to_literal to batch process the list items. This is necessary because processing
+            # each list item separately could lead to errors since ListTransformer.to_python_value may treat the literal
+            # as it is batched for batchable types.
+            if ListTransformer.is_batchable(python_type):
+                return TypeEngine.to_literal(ctx, input_val, python_type, lt)
+            literal_list = [extract_value(ctx, v, sub_type, lt.collection_type) for v in input_val]
+            return _literal_models.Literal(collection=_literal_models.LiteralCollection(literals=literal_list))
+        elif isinstance(input_val, dict):
+            lt = flyte_literal_type
+            python_type = val_type
+            if flyte_literal_type.union_type:
+                for i in range(len(flyte_literal_type.union_type.variants)):
+                    variant = flyte_literal_type.union_type.variants[i]
+                    if variant.map_value_type:
+                        lt = variant
+                        python_type = get_args(val_type)[i]
+                    if variant.simple == _type_models.SimpleType.STRUCT:
+                        lt = variant
+                        python_type = get_args(val_type)[i]
+            if lt.map_value_type is None and lt.simple != _type_models.SimpleType.STRUCT:
+                raise TypeError(f"Not a map type {lt} but got a map {input_val}")
+            if lt.simple == _type_models.SimpleType.STRUCT:
+                return TypeEngine.to_literal(ctx, input_val, type(input_val), lt)
+            else:
+                k_type, sub_type = DictTransformer.get_dict_types(python_type)  # type: ignore
+                literal_map = {k: extract_value(ctx, v, sub_type, lt.map_value_type) for k, v in input_val.items()}
+                return _literal_models.Literal(map=_literal_models.LiteralMap(literals=literal_map))
+        elif isinstance(input_val, Promise):
+            # In the example above, this handles the "in2=a" type of argument
+            return input_val.val
+        elif isinstance(input_val, VoidPromise):
+            raise AssertionError(
+                f"Outputs of a non-output producing task {input_val.task_name} cannot be passed to another task."
+            )
+        elif isinstance(input_val, tuple):
+            raise AssertionError(
+                "Tuples are not a supported type for individual values in Flyte - got a tuple -"
+                f" {input_val}. If using named tuple in an inner task, please, de-reference the"
+                "actual attribute that you want to use. For example, in NamedTuple('OP', x=int) then"
+                "return v.x, instead of v, even if this has a single element"
+            )
+        else:
+            # This handles native values, the 5 example
+            return TypeEngine.to_literal(ctx, input_val, val_type, flyte_literal_type)
+
     if incoming_values is None:
         raise ValueError("Incoming values cannot be None, must be a dict")
 
     result = {}  # So as to not overwrite the input_kwargs
     for k, v in incoming_values.items():
         if k not in flyte_interface_types:
             raise ValueError(f"Received unexpected keyword argument {k}")
         var = flyte_interface_types[k]
         t = native_types[k]
         try:
-            result[k] = TypeEngine.to_literal(ctx, v, t, var.type)
+            result[k] = extract_value(ctx, v, t, var.type)
         except TypeTransformerFailedError as exc:
             raise TypeTransformerFailedError(f"Failed argument '{k}': {exc}") from exc
 
     return result
 
 
 def get_primitive_val(prim: Primitive) -> Any:
@@ -144,19 +215,19 @@
                     raise ValueError("Only primitive values can be used in comparison")
         if self._lhs is None:
             self._lhs = type_engine.TypeEngine.to_literal(FlyteContextManager.current_context(), lhs, type(lhs), None)
         if self._rhs is None:
             self._rhs = type_engine.TypeEngine.to_literal(FlyteContextManager.current_context(), rhs, type(rhs), None)
 
     @property
-    def rhs(self) -> Union["Promise", _literals_models.Literal]:
+    def rhs(self) -> Union["Promise", _literal_models.Literal]:
         return self._rhs
 
     @property
-    def lhs(self) -> Union["Promise", _literals_models.Literal]:
+    def lhs(self) -> Union["Promise", _literal_models.Literal]:
         return self._lhs
 
     @property
     def op(self) -> ComparisonOps:
         return self._op
 
     def eval(self) -> bool:
@@ -276,15 +347,15 @@
        If the task returns an integer or a ``(int, str)`` tuple like ``t1`` above, calling ``with_overrides`` on the
        result would throw an error. This Promise object adds that.
     #. Assorted handling for conditionals.
     """
 
     # TODO: Currently, NodeOutput we're creating is the slimmer core package Node class, but since only the
     #  id is used, it's okay for now. Let's clean all this up though.
-    def __init__(self, var: str, val: Union[NodeOutput, _literals_models.Literal]):
+    def __init__(self, var: str, val: Union[NodeOutput, _literal_models.Literal]):
         self._var = var
         self._promise_ready = True
         self._val = val
         if val and isinstance(val, NodeOutput):
             self._ref = val
             self._promise_ready = False
             self._val = None
@@ -313,15 +384,15 @@
                 print(p.val)
            else:
                 print(p.ref)
         """
         return self._promise_ready
 
     @property
-    def val(self) -> _literals_models.Literal:
+    def val(self) -> _literal_models.Literal:
         """
         If the promise is ready then this holds the actual evaluate value in Flyte's type system
         """
         return self._val
 
     @property
     def ref(self) -> NodeOutput:
@@ -518,52 +589,59 @@
         def __rshift__(self, other: Any):
             # See comment for runs_before
             return other
 
     return Output(*promises)  # type: ignore
 
 
+def binding_from_flyte_std(
+    ctx: _flyte_context.FlyteContext,
+    var_name: str,
+    expected_literal_type: _type_models.LiteralType,
+    t_value: Any,
+) -> _literals_models.Binding:
+    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type=None)
+    return _literals_models.Binding(var=var_name, binding=binding_data)
+
+
 def binding_data_from_python_std(
     ctx: _flyte_context.FlyteContext,
     expected_literal_type: _type_models.LiteralType,
     t_value: Any,
-    t_value_type: type,
-    nodes: List[Node],
+    t_value_type: Optional[type] = None,
 ) -> _literals_models.BindingData:
     # This handles the case where the given value is the output of another task
     if isinstance(t_value, Promise):
         if not t_value.is_ready:
-            nodes.append(t_value.ref.node)  # keeps track of upstream nodes
             return _literals_models.BindingData(promise=t_value.ref)
 
     elif isinstance(t_value, VoidPromise):
         raise AssertionError(
             f"Cannot pass output from task {t_value.task_name} that produces no outputs to a downstream task"
         )
 
-    elif t_value is not None and expected_literal_type.union_type is not None:
+    elif expected_literal_type.union_type is not None:
         for i in range(len(expected_literal_type.union_type.variants)):
             try:
                 lt_type = expected_literal_type.union_type.variants[i]
                 python_type = get_args(t_value_type)[i] if t_value_type else None
-                return binding_data_from_python_std(ctx, lt_type, t_value, python_type, nodes)
+                return binding_data_from_python_std(ctx, lt_type, t_value, python_type)
             except Exception:
                 logger.debug(
                     f"failed to bind data {t_value} with literal type {expected_literal_type.union_type.variants[i]}."
                 )
         raise AssertionError(
             f"Failed to bind data {t_value} with literal type {expected_literal_type.union_type.variants}."
         )
 
     elif isinstance(t_value, list):
-        sub_type: type = ListTransformer.get_sub_type(t_value_type)
+        sub_type: Optional[type] = ListTransformer.get_sub_type(t_value_type) if t_value_type else None
         collection = _literals_models.BindingDataCollection(
             bindings=[
-                binding_data_from_python_std(ctx, expected_literal_type.collection_type, t, sub_type, nodes)
-                for t in t_value
+                binding_data_from_python_std(ctx, expected_literal_type.collection_type, t, sub_type) for t in t_value
             ]
         )
 
         return _literals_models.BindingData(collection=collection)
 
     elif isinstance(t_value, dict):
         if (
@@ -573,20 +651,21 @@
             raise AssertionError(
                 f"this should be a Dictionary type and it is not: {type(t_value)} vs {expected_literal_type}"
             )
         if expected_literal_type.simple == _type_models.SimpleType.STRUCT:
             lit = TypeEngine.to_literal(ctx, t_value, type(t_value), expected_literal_type)
             return _literals_models.BindingData(scalar=lit.scalar)
         else:
-            _, v_type = DictTransformer.get_dict_types(t_value_type)
+            _, v_type = (
+                DictTransformer.get_dict_types(t_value_type) if t_value_type else None,
+                None,
+            )
             m = _literals_models.BindingDataMap(
                 bindings={
-                    k: binding_data_from_python_std(
-                        ctx, expected_literal_type.map_value_type, v, v_type or type(v), nodes
-                    )
+                    k: binding_data_from_python_std(ctx, expected_literal_type.map_value_type, v, v_type)
                     for k, v in t_value.items()
                 }
             )
         return _literals_models.BindingData(map=m)
 
     elif isinstance(t_value, tuple):
         raise AssertionError(
@@ -603,18 +682,17 @@
 
 def binding_from_python_std(
     ctx: _flyte_context.FlyteContext,
     var_name: str,
     expected_literal_type: _type_models.LiteralType,
     t_value: Any,
     t_value_type: type,
-) -> Tuple[_literals_models.Binding, List[Node]]:
-    nodes: List[Node] = []
-    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type, nodes)
-    return _literals_models.Binding(var=var_name, binding=binding_data), nodes
+) -> _literals_models.Binding:
+    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type)
+    return _literals_models.Binding(var=var_name, binding=binding_data)
 
 
 def to_binding(p: Promise) -> _literals_models.Binding:
     return _literals_models.Binding(var=p.var, binding=_literals_models.BindingData(promise=p.ref))
 
 
 class VoidPromise(object):
@@ -794,15 +872,15 @@
 
     if _inputs_not_allowed:
         inputs_not_allowed_specified = _inputs_not_allowed.intersection(kwargs.keys())
         if inputs_not_allowed_specified:
             raise _user_exceptions.FlyteAssertion(
                 f"Fixed inputs cannot be specified. Please remove the following inputs - {inputs_not_allowed_specified}"
             )
-    nodes = []
+
     for k in sorted(typed_interface.inputs):
         var = typed_interface.inputs[k]
         if k not in kwargs:
             if _inputs_not_allowed and _ignorable_inputs:
                 if k in _ignorable_inputs or k in _inputs_not_allowed:
                     continue
             # TODO to improve the error message, should we show python equivalent types for var.type?
@@ -813,37 +891,44 @@
         # into the function.
         if isinstance(v, tuple):
             raise AssertionError(
                 f"Variable({k}) for function({entity.name}) cannot receive a multi-valued tuple {v}."
                 f" Check if the predecessor function returning more than one value?"
             )
         try:
-            b, n = binding_from_python_std(
-                ctx,
-                var_name=k,
-                expected_literal_type=var.type,
-                t_value=v,
-                t_value_type=type(v),  # since we don't have the python type available
+            bindings.append(
+                binding_from_flyte_std(
+                    ctx,
+                    var_name=k,
+                    expected_literal_type=var.type,
+                    t_value=v,
+                )
             )
-            bindings.append(b)
-            nodes.extend(n)
             used_inputs.add(k)
         except Exception as e:
             raise AssertionError(f"Failed to Bind variable {k} for function {entity.name}.") from e
 
     extra_inputs = used_inputs ^ set(kwargs.keys())
     if len(extra_inputs) > 0:
         raise _user_exceptions.FlyteAssertion(
             f"Too many inputs for [{entity.name}] Expected inputs: {typed_interface.inputs.keys()} "
             f"- extra inputs: {extra_inputs}"
         )
 
     # Detect upstream nodes
     # These will be our core Nodes until we can amend the Promise to use NodeOutputs that reference our Nodes
-    upstream_nodes = list(set([n for n in nodes if n.id != _common_constants.GLOBAL_INPUT_NODE_ID]))
+    upstream_nodes = list(
+        set(
+            [
+                input_val.ref.node
+                for input_val in kwargs.values()
+                if isinstance(input_val, Promise) and input_val.ref.node_id != _common_constants.GLOBAL_INPUT_NODE_ID
+            ]
+        )
+    )
 
     flytekit_node = Node(
         id=f"{ctx.compilation_state.prefix}n{len(ctx.compilation_state.nodes)}",
         metadata=entity.construct_node_metadata(),
         bindings=sorted(bindings, key=lambda b: b.var),
         upstream_nodes=upstream_nodes,
         flyte_entity=entity,
@@ -876,15 +961,14 @@
     :return:  Optional[Union[Tuple[Promise], Promise, VoidPromise]]
     """
     if ctx.compilation_state is None:
         raise _user_exceptions.FlyteAssertion("Cannot create node when not compiling...")
 
     used_inputs = set()
     bindings = []
-    nodes = []
 
     interface = entity.python_interface
     typed_interface = flyte_interface.transform_interface_to_typed_interface(interface)
     # Mypy needs some extra help to believe that `typed_interface` will not be `None`
     assert typed_interface is not None
 
     for k in sorted(interface.inputs):
@@ -910,36 +994,44 @@
         # into the function.
         if isinstance(v, tuple):
             raise AssertionError(
                 f"Variable({k}) for function({entity.name}) cannot receive a multi-valued tuple {v}."
                 f" Check if the predecessor function returning more than one value?"
             )
         try:
-            b, n = binding_from_python_std(
-                ctx,
-                var_name=k,
-                expected_literal_type=var.type,
-                t_value=v,
-                t_value_type=interface.inputs[k],
+            bindings.append(
+                binding_from_python_std(
+                    ctx,
+                    var_name=k,
+                    expected_literal_type=var.type,
+                    t_value=v,
+                    t_value_type=interface.inputs[k],
+                )
             )
-            bindings.append(b)
-            nodes.extend(n)
             used_inputs.add(k)
         except Exception as e:
             raise AssertionError(f"Failed to Bind variable {k} for function {entity.name}.") from e
 
     extra_inputs = used_inputs ^ set(kwargs.keys())
     if len(extra_inputs) > 0:
         raise _user_exceptions.FlyteAssertion(
             "Too many inputs were specified for the interface.  Extra inputs were: {}".format(extra_inputs)
         )
 
     # Detect upstream nodes
     # These will be our core Nodes until we can amend the Promise to use NodeOutputs that reference our Nodes
-    upstream_nodes = list(set([n for n in nodes if n.id != _common_constants.GLOBAL_INPUT_NODE_ID]))
+    upstream_nodes = list(
+        set(
+            [
+                input_val.ref.node
+                for input_val in kwargs.values()
+                if isinstance(input_val, Promise) and input_val.ref.node_id != _common_constants.GLOBAL_INPUT_NODE_ID
+            ]
+        )
+    )
 
     flytekit_node = Node(
         # TODO: Better naming, probably a derivative of the function name.
         id=f"{ctx.compilation_state.prefix}n{len(ctx.compilation_state.nodes)}",
         metadata=entity.construct_node_metadata(),
         bindings=sorted(bindings, key=lambda b: b.var),
         upstream_nodes=upstream_nodes,
```

### Comparing `flytekit-1.8.3/flytekit/core/python_auto_container.py` & `flytekit-1.9.0a0/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/python_customized_container_task.py` & `flytekit-1.9.0a0/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/python_function_task.py` & `flytekit-1.9.0a0/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/reference.py` & `flytekit-1.9.0a0/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/reference_entity.py` & `flytekit-1.9.0a0/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/resources.py` & `flytekit-1.9.0a0/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/schedule.py` & `flytekit-1.9.0a0/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/shim_task.py` & `flytekit-1.9.0a0/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/task.py` & `flytekit-1.9.0a0/flytekit/core/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         if plugin_config_type in cls._PYTHONFUNCTION_TASK_PLUGINS:
             return cls._PYTHONFUNCTION_TASK_PLUGINS[plugin_config_type]
         # Defaults to returning Base PythonFunctionTask
         return PythonFunctionTask
 
 
 T = TypeVar("T")
-FuncOut = TypeVar("FuncOut")
 
 
 @overload
 def task(
     _task_function: None = ...,
     task_config: Optional[T] = ...,
     cache: bool = ...,
@@ -97,21 +96,21 @@
     secret_requests: Optional[List[Secret]] = ...,
     execution_mode: PythonFunctionTask.ExecutionBehavior = ...,
     task_resolver: Optional[TaskResolverMixin] = ...,
     docs: Optional[Documentation] = ...,
     disable_deck: bool = ...,
     pod_template: Optional["PodTemplate"] = ...,
     pod_template_name: Optional[str] = ...,
-) -> Callable[[Callable[..., FuncOut]], PythonFunctionTask[T]]:
+) -> Callable[[Callable[..., Any]], PythonFunctionTask[T]]:
     ...
 
 
 @overload
 def task(
-    _task_function: Callable[..., FuncOut],
+    _task_function: Callable[..., Any],
     task_config: Optional[T] = ...,
     cache: bool = ...,
     cache_serialize: bool = ...,
     cache_version: str = ...,
     retries: int = ...,
     interruptible: Optional[bool] = ...,
     deprecated: str = ...,
@@ -123,20 +122,20 @@
     secret_requests: Optional[List[Secret]] = ...,
     execution_mode: PythonFunctionTask.ExecutionBehavior = ...,
     task_resolver: Optional[TaskResolverMixin] = ...,
     docs: Optional[Documentation] = ...,
     disable_deck: bool = ...,
     pod_template: Optional["PodTemplate"] = ...,
     pod_template_name: Optional[str] = ...,
-) -> Union[PythonFunctionTask[T], Callable[..., FuncOut]]:
+) -> PythonFunctionTask[T]:
     ...
 
 
 def task(
-    _task_function: Optional[Callable[..., FuncOut]] = None,
+    _task_function: Optional[Callable[..., Any]] = None,
     task_config: Optional[T] = None,
     cache: bool = False,
     cache_serialize: bool = False,
     cache_version: str = "",
     retries: int = 0,
     interruptible: Optional[bool] = None,
     deprecated: str = "",
@@ -148,15 +147,15 @@
     secret_requests: Optional[List[Secret]] = None,
     execution_mode: PythonFunctionTask.ExecutionBehavior = PythonFunctionTask.ExecutionBehavior.DEFAULT,
     task_resolver: Optional[TaskResolverMixin] = None,
     docs: Optional[Documentation] = None,
     disable_deck: bool = True,
     pod_template: Optional["PodTemplate"] = None,
     pod_template_name: Optional[str] = None,
-) -> Union[Callable[[Callable[..., FuncOut]], PythonFunctionTask[T]], PythonFunctionTask[T], Callable[..., FuncOut]]:
+) -> Union[Callable[[Callable[..., Any]], PythonFunctionTask[T]], PythonFunctionTask[T]]:
     """
     This is the core decorator to use for any task type in flytekit.
 
     Tasks are the building blocks of Flyte. They represent users code. Tasks have the following properties
 
     * Versioned (usually tied to the git sha)
     * Strong interfaces (specified inputs and outputs)
```

### Comparing `flytekit-1.8.3/flytekit/core/testing.py` & `flytekit-1.9.0a0/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/tracker.py` & `flytekit-1.9.0a0/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/type_engine.py` & `flytekit-1.9.0a0/flytekit/core/type_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,16 @@
         if type(python_val) != self._type:
             raise TypeTransformerFailedError(
                 f"Expected value of type {self._type} but got '{python_val}' of type {type(python_val)}"
             )
         return self._to_literal_transformer(python_val)
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> T:
-        expected_python_type = get_underlying_type(expected_python_type)
+        if get_origin(expected_python_type) is Annotated:
+            expected_python_type = get_args(expected_python_type)[0]
 
         if expected_python_type != self._type:
             raise TypeTransformerFailedError(
                 f"Cannot convert to type {expected_python_type}, only {self._type} is supported"
             )
 
         try:  # todo(maximsmol): this is quite ugly and each transformer should really check their Literal
@@ -306,15 +307,15 @@
                 raise TypeTransformerFailedError(f"Type of Val '{original_type}' is not an instance of {expected_type}")
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
         """
         Extracts the Literal type definition for a Dataclass and returns a type Struct.
         If possible also extracts the JSONSchema for the dataclass.
         """
-        if is_annotated(t):
+        if get_origin(t) is Annotated:
             raise ValueError(
                 "Flytekit does not currently have support for FlyteAnnotations applied to Dataclass."
                 f"Type {t} cannot be parsed."
             )
 
         if not issubclass(t, DataClassJsonMixin):
             raise AssertionError(
@@ -363,15 +364,15 @@
         if get_origin(python_type) is list:
             return typing.List[self._get_origin_type_in_annotation(get_args(python_type)[0])]  # type: ignore
         elif get_origin(python_type) is dict:
             return typing.Dict[  # type: ignore
                 self._get_origin_type_in_annotation(get_args(python_type)[0]),
                 self._get_origin_type_in_annotation(get_args(python_type)[1]),
             ]
-        elif is_annotated(python_type):
+        elif get_origin(python_type) is Annotated:
             return get_args(python_type)[0]
         elif dataclasses.is_dataclass(python_type):
             for field in dataclasses.fields(copy.deepcopy(python_type)):
                 field.type = self._get_origin_type_in_annotation(field.type)
         return python_type
 
     def _fix_structured_dataset_type(self, python_type: Type[T], python_val: typing.Any) -> T:
@@ -705,15 +706,15 @@
 
     @classmethod
     def register_additional_type(cls, transformer: TypeTransformer, additional_type: Type, override=False):
         if additional_type not in cls._REGISTRY or override:
             cls._REGISTRY[additional_type] = transformer
 
     @classmethod
-    def get_transformer(cls, python_type: Type) -> TypeTransformer[T]:
+    def get_transformer(cls, python_type: Type[T]) -> TypeTransformer[T]:
         """
         The TypeEngine hierarchy for flyteKit. This method looksup and selects the type transformer. The algorithm is
         as follows
 
           d = dictionary of registered transformers, where is a python `type`
           v = lookup type
         Step 1:
@@ -732,30 +733,30 @@
             TODO lets make this deterministic by using an ordered dict
 
         Step 5:
             if v is of type data class, use the dataclass transformer
         """
         cls.lazy_import_transformers()
         # Step 1
-        if is_annotated(python_type):
+        if get_origin(python_type) is Annotated:
             args = get_args(python_type)
             for annotation in args:
                 if isinstance(annotation, TypeTransformer):
                     return annotation
 
             python_type = args[0]
 
         if python_type in cls._REGISTRY:
             return cls._REGISTRY[python_type]
 
         # Step 2
         if hasattr(python_type, "__origin__"):
             # Handling of annotated generics, eg:
             # Annotated[typing.List[int], 'foo']
-            if is_annotated(python_type):
+            if get_origin(python_type) is Annotated:
                 return cls.get_transformer(get_args(python_type)[0])
 
             if python_type.__origin__ in cls._REGISTRY:
                 return cls._REGISTRY[python_type.__origin__]
 
             raise ValueError(f"Generic Type {python_type.__origin__} not supported currently in Flytekit.")
 
@@ -775,19 +776,15 @@
                 # is the case for one of the restricted types, namely NamedTuple.
                 logger.debug(f"Invalid base type {base_type} in call to isinstance", exc_info=True)
 
         # Step 4
         if dataclasses.is_dataclass(python_type):
             return cls._DATACLASS_TRANSFORMER
 
-        # Step 5
-        display_pickle_warning(str(python_type))
-        from flytekit.types.pickle.pickle import FlytePickleTransformer
-
-        return FlytePickleTransformer()
+        raise ValueError(f"Type {python_type} not supported currently in Flytekit. Please register a new transformer")
 
     @classmethod
     def lazy_import_transformers(cls):
         """
         Only load the transformers if needed.
         """
         if cls.has_lazy_import:
@@ -822,15 +819,15 @@
     def to_literal_type(cls, python_type: Type) -> LiteralType:
         """
         Converts a python type into a flyte specific ``LiteralType``
         """
         transformer = cls.get_transformer(python_type)
         res = transformer.get_literal_type(python_type)
         data = None
-        if is_annotated(python_type):
+        if get_origin(python_type) is Annotated:
             for x in get_args(python_type)[1:]:
                 if not isinstance(x, FlyteAnnotation):
                     continue
                 if data is not None:
                     raise ValueError(
                         f"More than one FlyteAnnotation used within {python_type} typehint. Flytekit requires a max of one."
                     )
@@ -842,41 +839,25 @@
         return res
 
     @classmethod
     def to_literal(cls, ctx: FlyteContext, python_val: typing.Any, python_type: Type, expected: LiteralType) -> Literal:
         """
         Converts a python value of a given type and expected ``LiteralType`` into a resolved ``Literal`` value.
         """
-        from flytekit.core.promise import Promise, VoidPromise
-
-        if isinstance(python_val, Promise):
-            # In the example above, this handles the "in2=a" type of argument
-            return python_val.val
-        if isinstance(python_val, VoidPromise):
-            raise AssertionError(
-                f"Outputs of a non-output producing task {python_val.task_name} cannot be passed to another task."
-            )
-        if isinstance(python_val, tuple):
-            raise AssertionError(
-                "Tuples are not a supported type for individual values in Flyte - got a tuple -"
-                f" {python_val}. If using named tuple in an inner task, please, de-reference the"
-                "actual attribute that you want to use. For example, in NamedTuple('OP', x=int) then"
-                "return v.x, instead of v, even if this has a single element"
-            )
         if python_val is None and expected.union_type is None:
             raise TypeTransformerFailedError(f"Python value cannot be None, expected {python_type}/{expected}")
         transformer = cls.get_transformer(python_type)
         if transformer.type_assertions_enabled:
             transformer.assert_type(python_type, python_val)
 
         # In case the value is an annotated type we inspect the annotations and look for hash-related annotations.
         hash = None
-        if is_annotated(python_type):
+        if get_origin(python_type) is Annotated:
             # We are now dealing with one of two cases:
-            # 1. The annotated type is a `HashMethod`, which indicates that we should produce the hash using
+            # 1. The annotated type is a `HashMethod`, which indicates that we should we should produce the hash using
             #    the method indicated in the annotation.
             # 2. The annotated type is being used for a different purpose other than calculating hash values, in which case
             #    we should just continue.
             for annotation in get_args(python_type)[1:]:
                 if not isinstance(annotation, HashMethod):
                     continue
                 hash = annotation.calculate(python_val)
@@ -895,15 +876,15 @@
         """
         transformer = cls.get_transformer(expected_python_type)
         return transformer.to_python_value(ctx, lv, expected_python_type)
 
     @classmethod
     def to_html(cls, ctx: FlyteContext, python_val: typing.Any, expected_python_type: Type[typing.Any]) -> str:
         transformer = cls.get_transformer(expected_python_type)
-        if is_annotated(expected_python_type):
+        if get_origin(expected_python_type) is Annotated:
             expected_python_type, *annotate_args = get_args(expected_python_type)
             from flytekit.deck.renderer import Renderable
 
             for arg in annotate_args:
                 if isinstance(arg, Renderable):
                     return arg.to_html(python_val)
         return transformer.to_html(ctx, python_val, expected_python_type)
@@ -1019,15 +1000,15 @@
     def get_sub_type(t: Type[T]) -> Type[T]:
         """
         Return the generic Type T of the List
         """
         if hasattr(t, "__origin__"):
             # Handle annotation on list generic, eg:
             # Annotated[typing.List[int], 'foo']
-            if is_annotated(t):
+            if get_origin(t) is Annotated:
                 return ListTransformer.get_sub_type(get_args(t)[0])
 
             if getattr(t, "__origin__") is list and hasattr(t, "__args__"):
                 return getattr(t, "__args__")[0]
 
         raise ValueError("Only generic univariate typing.List[T] type is supported.")
 
@@ -1045,15 +1026,15 @@
     def is_batchable(t: Type):
         """
         This function evaluates whether the provided type is batchable or not.
         It returns True only if the type is either List or Annotated(List) and the List subtype is FlytePickle.
         """
         from flytekit.types.pickle import FlytePickle
 
-        if is_annotated(t):
+        if get_origin(t) is Annotated:
             return ListTransformer.is_batchable(get_args(t)[0])
         if get_origin(t) is list:
             subtype = get_args(t)[0]
             if subtype == FlytePickle or (hasattr(subtype, "__origin__") and subtype.__origin__ == FlytePickle):
                 return True
         return False
 
@@ -1062,15 +1043,15 @@
             raise TypeTransformerFailedError("Expected a list")
 
         if ListTransformer.is_batchable(python_type):
             from flytekit.types.pickle.pickle import BatchSize, FlytePickle
 
             batch_size = len(python_val)  # default batch size
             # parse annotated to get the number of items saved in a pickle file.
-            if is_annotated(python_type):
+            if get_origin(python_type) is Annotated:
                 for annotation in get_args(python_type)[1:]:
                     if isinstance(annotation, BatchSize):
                         batch_size = annotation.val
                         break
             if batch_size > 0:
                 lit_list = [TypeEngine.to_literal(ctx, python_val[i : i + batch_size], FlytePickle, expected.collection_type) for i in range(0, len(python_val), batch_size)]  # type: ignore
             else:
@@ -1101,24 +1082,14 @@
     def guess_python_type(self, literal_type: LiteralType) -> list:  # type: ignore
         if literal_type.collection_type:
             ct: Type = TypeEngine.guess_python_type(literal_type.collection_type)
             return typing.List[ct]  # type: ignore
         raise ValueError(f"List transformer cannot reverse {literal_type}")
 
 
-@lru_cache
-def display_pickle_warning(python_type: str):
-    # This is a warning that is only displayed once per python type
-    logger.warning(
-        f"Unsupported Type {python_type} found, Flyte will default to use PickleFile as the transport. "
-        f"Pickle can only be used to send objects between the exact same version of Python, "
-        f"and we strongly recommend to use python type that flyte support."
-    )
-
-
 def _add_tag_to_type(x: LiteralType, tag: str) -> LiteralType:
     x._structure = TypeStructure(tag=tag)
     return x
 
 
 def _type_essence(x: LiteralType) -> LiteralType:
     if x.metadata is not None or x.structure is not None or x.annotation is not None:
@@ -1216,38 +1187,40 @@
     def get_sub_type_in_optional(t: Type[T]) -> Type[T]:
         """
         Return the generic Type T of the Optional type
         """
         return get_args(t)[0]
 
     def get_literal_type(self, t: Type[T]) -> Optional[LiteralType]:
-        t = get_underlying_type(t)
+        if get_origin(t) is Annotated:
+            t = get_args(t)[0]
 
         try:
             trans: typing.List[typing.Tuple[TypeTransformer, typing.Any]] = [
                 (TypeEngine.get_transformer(x), x) for x in get_args(t)
             ]
             # must go through TypeEngine.to_literal_type instead of trans.get_literal_type
             # to handle Annotated
             variants = [_add_tag_to_type(TypeEngine.to_literal_type(x), t.name) for (t, x) in trans]
             return _type_models.LiteralType(union_type=UnionType(variants))
         except Exception as e:
             raise ValueError(f"Type of Generic Union type is not supported, {e}")
 
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
-        python_type = get_underlying_type(python_type)
+        if get_origin(python_type) is Annotated:
+            python_type = get_args(python_type)[0]
 
         found_res = False
         res = None
         res_type = None
-        for i in range(len(get_args(python_type))):
+        for t in get_args(python_type):
             try:
-                t = get_args(python_type)[i]
                 trans: TypeTransformer[T] = TypeEngine.get_transformer(t)
-                res = trans.to_literal(ctx, python_val, t, expected.union_type.variants[i])
+
+                res = trans.to_literal(ctx, python_val, t, expected)
                 res_type = _add_tag_to_type(trans.get_literal_type(t), trans.name)
                 if found_res:
                     # Should really never happen, sanity check
                     raise TypeError("Ambiguous choice of variant for union type")
                 found_res = True
             except (TypeTransformerFailedError, AttributeError, ValueError, AssertionError) as e:
                 logger.debug(f"Failed to convert from {python_val} to {t}", e)
@@ -1255,15 +1228,16 @@
 
         if found_res:
             return Literal(scalar=Scalar(union=Union(value=res, stored_type=res_type)))
 
         raise TypeTransformerFailedError(f"Cannot convert from {python_val} to {python_type}")
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> Optional[typing.Any]:
-        expected_python_type = get_underlying_type(expected_python_type)
+        if get_origin(expected_python_type) is Annotated:
+            expected_python_type = get_args(expected_python_type)[0]
 
         union_tag = None
         union_type = None
         if lv.scalar is not None and lv.scalar.union is not None:
             union_type = lv.scalar.union.stored_type
             if union_type.structure is not None:
                 union_tag = union_type.structure.tag
@@ -1490,15 +1464,15 @@
     Enables converting a python type enum.Enum to LiteralType.EnumType
     """
 
     def __init__(self):
         super().__init__(name="DefaultEnumTransformer", t=enum.Enum)
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
-        if is_annotated(t):
+        if get_origin(t) is Annotated:
             raise ValueError(
                 f"Flytekit does not currently have support \
                     for FlyteAnnotations applied to enums. {t} cannot be \
                     parsed."
             )
 
         values = [v.value for v in t]  # type: ignore
@@ -1804,18 +1778,7 @@
             self._ctx or FlyteContext.current_context(), self._literals[attr], cast(Type, as_type)
         )
         self._native_values[attr] = val
         return val
 
 
 _register_default_type_transformers()
-
-
-def is_annotated(t: Type) -> bool:
-    return get_origin(t) is Annotated
-
-
-def get_underlying_type(t: Type) -> Type:
-    """Return the underlying type for annotated types or the type itself"""
-    if is_annotated(t):
-        return get_args(t)[0]
-    return t
```

### Comparing `flytekit-1.8.3/flytekit/core/type_helpers.py` & `flytekit-1.9.0a0/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/utils.py` & `flytekit-1.9.0a0/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/core/workflow.py` & `flytekit-1.9.0a0/flytekit/core/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import typing
 from dataclasses import dataclass
 from enum import Enum
 from functools import update_wrapper
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union, cast, overload
 
+from typing_extensions import get_args
+
 from flytekit.core import constants as _common_constants
 from flytekit.core.base_task import PythonTask
 from flytekit.core.class_based_resolver import ClassStorageTaskResolver
 from flytekit.core.condition import ConditionalSection
 from flytekit.core.context_manager import CompilationState, FlyteContext, FlyteContextManager, FlyteEntities
 from flytekit.core.docstring import Docstring
 from flytekit.core.interface import (
@@ -29,33 +31,34 @@
     extract_obj_name,
     flyte_entity_call_handler,
     translate_inputs_to_literals,
 )
 from flytekit.core.python_auto_container import PythonAutoContainerTask
 from flytekit.core.reference_entity import ReferenceEntity, WorkflowReference
 from flytekit.core.tracker import extract_task_module
-from flytekit.core.type_engine import TypeEngine
+from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError, UnionTransformer
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.exceptions.user import FlyteValidationException, FlyteValueException
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
+from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.documentation import Description, Documentation
+from flytekit.models.types import TypeStructure
 
 GLOBAL_START_NODE = Node(
     id=_common_constants.GLOBAL_INPUT_NODE_ID,
     metadata=None,
     bindings=[],
     upstream_nodes=[],
     flyte_entity=None,
 )
 
 T = typing.TypeVar("T")
-FuncOut = typing.TypeVar("FuncOut")
 
 
 class WorkflowFailurePolicy(Enum):
     """
     Defines the behavior for a workflow execution in the case of an observed node execution failure. By default, a
     workflow execution will immediately enter a failed state if a component node fails.
     """
@@ -272,26 +275,71 @@
 
     def execute(self, **kwargs):
         raise Exception("Should not be called")
 
     def compile(self, **kwargs):
         pass
 
+    def ensure_literal(
+        self, ctx, py_type: Type[T], input_type: type_models.LiteralType, python_value: Any
+    ) -> _literal_models.Literal:
+        """
+        This function will attempt to convert a python value to a literal. If the python value is a promise, it will
+        return the promise's value.
+        """
+        if input_type.union_type is not None:
+            if python_value is None and UnionTransformer.is_optional_type(py_type):
+                return _literal_models.Literal(scalar=_literal_models.Scalar(none_type=_literal_models.Void()))
+            for i in range(len(input_type.union_type.variants)):
+                lt_type = input_type.union_type.variants[i]
+                python_type = get_args(py_type)[i]
+                try:
+                    final_lt = self.ensure_literal(ctx, python_type, lt_type, python_value)
+                    lt_type._structure = TypeStructure(tag=TypeEngine.get_transformer(python_type).name)
+                    return _literal_models.Literal(
+                        scalar=_literal_models.Scalar(union=_literal_models.Union(value=final_lt, stored_type=lt_type))
+                    )
+                except Exception as e:
+                    logger.debug(f"Failed to convert {python_value} to {lt_type} with error {e}")
+            raise TypeError(f"Failed to convert {python_value} to {input_type}")
+        if isinstance(python_value, list) and input_type.collection_type:
+            collection_lit_type = input_type.collection_type
+            collection_py_type = get_args(py_type)[0]
+            xx = [self.ensure_literal(ctx, collection_py_type, collection_lit_type, pv) for pv in python_value]
+            return _literal_models.Literal(collection=_literal_models.LiteralCollection(literals=xx))
+        elif isinstance(python_value, dict) and input_type.map_value_type:
+            mapped_lit_type = input_type.map_value_type
+            mapped_py_type = get_args(py_type)[1]
+            xx = {k: self.ensure_literal(ctx, mapped_py_type, mapped_lit_type, v) for k, v in python_value.items()}  # type: ignore
+            return _literal_models.Literal(map=_literal_models.LiteralMap(literals=xx))
+        # It is a scalar, convert to Promise if necessary.
+        else:
+            if isinstance(python_value, Promise):
+                return python_value.val
+            if not isinstance(python_value, Promise):
+                try:
+                    res = TypeEngine.to_literal(ctx, python_value, py_type, input_type)
+                    return res
+                except TypeTransformerFailedError as exc:
+                    raise TypeError(
+                        f"Failed to convert input '{python_value}' of workflow '{self.name}':\n  {exc}"
+                    ) from exc
+
     def local_execute(self, ctx: FlyteContext, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, None]:
         # This is done to support the invariant that Workflow local executions always work with Promise objects
         # holding Flyte literal values. Even in a wf, a user can call a sub-workflow with a Python native value.
-        literal_map = translate_inputs_to_literals(
-            ctx,
-            incoming_values=kwargs,
-            flyte_interface_types=self.interface.inputs,
-            native_types=self.python_interface.inputs,
-        )
-        kwargs_literals = {k: Promise(var=k, val=v) for k, v in literal_map.items()}
+        for k, v in kwargs.items():
+            py_type = self.python_interface.inputs[k]
+            lit_type = self.interface.inputs[k].type
+            kwargs[k] = Promise(var=k, val=self.ensure_literal(ctx, py_type, lit_type, v))
+
+            # The output of this will always be a combination of Python native values and Promises containing Flyte
+            # Literals.
         self.compile()
-        function_outputs = self.execute(**kwargs_literals)
+        function_outputs = self.execute(**kwargs)
         # First handle the empty return case.
         # A workflow function may return a task that doesn't return anything
         #   def wf():
         #       return t1()
         # or it may not return at all
         #   def wf():
         #       t1()
@@ -558,15 +606,15 @@
 
         flyte_type = TypeEngine.to_literal_type(python_type=python_type)
 
         ctx = FlyteContext.current_context()
         if ctx.compilation_state is not None:
             raise Exception("Can't already be compiling")
         with FlyteContextManager.with_context(ctx.with_compilation_state(self.compilation_state)) as ctx:
-            b, _ = binding_from_python_std(
+            b = binding_from_python_std(
                 ctx, output_name, expected_literal_type=flyte_type, t_value=p, t_value_type=python_type
             )
             self._output_bindings.append(b)
             self._python_interface = self._python_interface.with_outputs(extra_outputs={output_name: python_type})
             self._interface = transform_interface_to_typed_interface(self._python_interface)
 
     def add_task(self, task: PythonTask, **kwargs) -> Node:
@@ -681,15 +729,15 @@
                     )
                 if self.python_interface.output_tuple_name is None:
                     raise AssertionError(
                         "Outputs specification for Workflow does not define a tuple, but return value is a tuple"
                     )
                 workflow_outputs = workflow_outputs[0]
             t = self.python_interface.outputs[output_names[0]]
-            b, _ = binding_from_python_std(
+            b = binding_from_python_std(
                 ctx,
                 output_names[0],
                 self.interface.outputs[output_names[0]].type,
                 workflow_outputs,
                 t,
             )
             bindings.append(b)
@@ -698,15 +746,15 @@
                 raise AssertionError("The Workflow specification indicates multiple return values, received only one")
             if len(output_names) != len(workflow_outputs):
                 raise Exception(f"Length mismatch {len(output_names)} vs {len(workflow_outputs)}")
             for i, out in enumerate(output_names):
                 if isinstance(workflow_outputs[i], ConditionalSection):
                     raise AssertionError("A Conditional block (if-else) should always end with an `else_()` clause")
                 t = self.python_interface.outputs[out]
-                b, _ = binding_from_python_std(
+                b = binding_from_python_std(
                     ctx,
                     out,
                     self.interface.outputs[out].type,
                     workflow_outputs[i],
                     t,
                 )
                 bindings.append(b)
@@ -731,34 +779,34 @@
 
 @overload
 def workflow(
     _workflow_function: None = ...,
     failure_policy: Optional[WorkflowFailurePolicy] = ...,
     interruptible: bool = ...,
     docs: Optional[Documentation] = ...,
-) -> Callable[[Callable[..., FuncOut]], PythonFunctionWorkflow]:
+) -> Callable[[Callable[..., Any]], PythonFunctionWorkflow]:
     ...
 
 
 @overload
 def workflow(
-    _workflow_function: Callable[..., FuncOut],
+    _workflow_function: Callable[..., Any],
     failure_policy: Optional[WorkflowFailurePolicy] = ...,
     interruptible: bool = ...,
     docs: Optional[Documentation] = ...,
-) -> Union[PythonFunctionWorkflow, Callable[..., FuncOut]]:
+) -> PythonFunctionWorkflow:
     ...
 
 
 def workflow(
     _workflow_function: Optional[Callable[..., Any]] = None,
     failure_policy: Optional[WorkflowFailurePolicy] = None,
     interruptible: bool = False,
     docs: Optional[Documentation] = None,
-) -> Union[Callable[[Callable[..., FuncOut]], PythonFunctionWorkflow], PythonFunctionWorkflow, Callable[..., FuncOut]]:
+) -> Union[Callable[[Callable[..., Any]], PythonFunctionWorkflow], PythonFunctionWorkflow]:
     """
     This decorator declares a function to be a Flyte workflow. Workflows are declarative entities that construct a DAG
     of tasks using the data flow between tasks.
 
     Unlike a task, the function body of a workflow is evaluated at serialization-time (aka compile-time). This is
     because while we can determine the entire structure of a task by looking at the function's signature, workflows need
     to run through the function itself because the body of the function is what expresses the workflow structure. It's
```

### Comparing `flytekit-1.8.3/flytekit/deck/deck.py` & `flytekit-1.9.0a0/flytekit/deck/deck.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     MarkdownRenderer can convert Markdown string to HTML
 
     Flyte context saves a list of deck objects, and we use renderers in those decks to render
     the data and create an HTML file when those tasks are executed
 
     Each task has a least three decks (input, output, default). Input/output decks are
     used to render tasks' input/output data, and the default deck is used to render line plots,
-    scatter plots or Markdown text. In addition, users can create new decks to render
+    scatter plots or markdown text. In addition, users can create new decks to render
     their data with custom renderers.
 
     .. warning::
 
         This feature is in beta.
 
     .. code-block:: python
@@ -51,14 +51,15 @@
         def t2() -> Annotated[pd.DataFrame, TopFrameRenderer(10)]:
             return iris_df
 
     """
 
     def __init__(self, name: str, html: Optional[str] = ""):
         self._name = name
+        # self.renderers = renderers if isinstance(renderers, list) else [renderers]
         self._html = html
         FlyteContextManager.current_context().user_space_params.decks.append(self)
 
     def append(self, html: str) -> "Deck":
         assert isinstance(html, str)
         self._html = self._html + "\n" + html
         return self
@@ -140,30 +141,22 @@
             ...
         return HTML(raw_html)
     return raw_html
 
 
 def _output_deck(task_name: str, new_user_params: ExecutionParameters):
     ctx = FlyteContext.current_context()
-    local_dir = ctx.file_access.get_random_local_directory()
-    local_path = f"{local_dir}{os.sep}{DECK_FILE_NAME}"
-    try:
-        with open(local_path, "w", encoding="utf-8") as f:
-            f.write(_get_deck(new_user_params, ignore_jupyter=True))
-        logger.info(f"{task_name} task creates flyte deck html to file://{local_path}")
-        if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
-            fs = ctx.file_access.get_filesystem_for_path(new_user_params.output_metadata_prefix)
-            remote_path = f"{new_user_params.output_metadata_prefix}{ctx.file_access.sep(fs)}{DECK_FILE_NAME}"
-            kwargs: typing.Dict[str, str] = {
-                "ContentType": "text/html",  # For s3
-                "content_type": "text/html",  # For gcs
-            }
-            ctx.file_access.put_data(local_path, remote_path, **kwargs)
-    except Exception as e:
-        logger.error(f"Failed to write flyte deck html with error {e}.")
+    if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
+        output_dir = ctx.execution_state.engine_dir
+    else:
+        output_dir = ctx.file_access.get_random_local_directory()
+    deck_path = os.path.join(output_dir, DECK_FILE_NAME)
+    with open(deck_path, "w") as f:
+        f.write(_get_deck(new_user_params, ignore_jupyter=True))
+    logger.info(f"{task_name} task creates flyte deck html to file://{deck_path}")
 
 
 def get_deck_template() -> "Template":
     from jinja2 import Environment, FileSystemLoader, select_autoescape
 
     root = os.path.dirname(os.path.abspath(__file__))
     templates_dir = os.path.join(root, "html")
```

### Comparing `flytekit-1.8.3/flytekit/deck/html/template.html` & `flytekit-1.9.0a0/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/deck/renderer.py` & `flytekit-1.9.0a0/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/exceptions/scopes.py` & `flytekit-1.9.0a0/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/exceptions/system.py` & `flytekit-1.9.0a0/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/exceptions/user.py` & `flytekit-1.9.0a0/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extend/__init__.py` & `flytekit-1.9.0a0/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extend/backend/agent_service.py` & `flytekit-1.9.0a0/flytekit/extend/backend/external_plugin_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 import grpc
-from flyteidl.admin.agent_pb2 import (
+from flyteidl.service.external_plugin_service_pb2 import (
     PERMANENT_FAILURE,
-    CreateTaskRequest,
-    CreateTaskResponse,
-    DeleteTaskRequest,
-    DeleteTaskResponse,
-    GetTaskRequest,
-    GetTaskResponse,
-    Resource,
+    TaskCreateRequest,
+    TaskCreateResponse,
+    TaskDeleteRequest,
+    TaskDeleteResponse,
+    TaskGetRequest,
+    TaskGetResponse,
 )
-from flyteidl.service.agent_pb2_grpc import AsyncAgentServiceServicer
+from flyteidl.service.external_plugin_service_pb2_grpc import ExternalPluginServiceServicer
 
 from flytekit import logger
-from flytekit.extend.backend.base_agent import AgentRegistry
+from flytekit.extend.backend.base_plugin import BackendPluginRegistry
 from flytekit.models.literals import LiteralMap
 from flytekit.models.task import TaskTemplate
 
 
-class AgentService(AsyncAgentServiceServicer):
-    def CreateTask(self, request: CreateTaskRequest, context: grpc.ServicerContext) -> CreateTaskResponse:
+class BackendPluginServer(ExternalPluginServiceServicer):
+    def CreateTask(self, request: TaskCreateRequest, context: grpc.ServicerContext) -> TaskCreateResponse:
         try:
             tmp = TaskTemplate.from_flyte_idl(request.template)
             inputs = LiteralMap.from_flyte_idl(request.inputs) if request.inputs else None
-            agent = AgentRegistry.get_agent(context, tmp.type)
-            if agent is None:
-                return CreateTaskResponse()
-            return agent.create(context=context, inputs=inputs, output_prefix=request.output_prefix, task_template=tmp)
+            plugin = BackendPluginRegistry.get_plugin(context, tmp.type)
+            if plugin is None:
+                return TaskCreateResponse()
+            return plugin.create(context=context, inputs=inputs, output_prefix=request.output_prefix, task_template=tmp)
         except Exception as e:
             logger.error(f"failed to create task with error {e}")
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(f"failed to create task with error {e}")
 
-    def GetTask(self, request: GetTaskRequest, context: grpc.ServicerContext) -> GetTaskResponse:
+    def GetTask(self, request: TaskGetRequest, context: grpc.ServicerContext) -> TaskGetResponse:
         try:
-            agent = AgentRegistry.get_agent(context, request.task_type)
-            if agent is None:
-                return GetTaskResponse(resource=Resource(state=PERMANENT_FAILURE))
-            return agent.get(context=context, resource_meta=request.resource_meta)
+            plugin = BackendPluginRegistry.get_plugin(context, request.task_type)
+            if plugin is None:
+                return TaskGetResponse(state=PERMANENT_FAILURE)
+            return plugin.get(context=context, job_id=request.job_id)
         except Exception as e:
             logger.error(f"failed to get task with error {e}")
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(f"failed to get task with error {e}")
 
-    def DeleteTask(self, request: DeleteTaskRequest, context: grpc.ServicerContext) -> DeleteTaskResponse:
+    def DeleteTask(self, request: TaskDeleteRequest, context: grpc.ServicerContext) -> TaskDeleteResponse:
         try:
-            agent = AgentRegistry.get_agent(context, request.task_type)
-            if agent is None:
-                return DeleteTaskResponse()
-            return agent.delete(context=context, resource_meta=request.resource_meta)
+            plugin = BackendPluginRegistry.get_plugin(context, request.task_type)
+            if plugin is None:
+                return TaskDeleteResponse()
+            return plugin.delete(context=context, job_id=request.job_id)
         except Exception as e:
             logger.error(f"failed to delete task with error {e}")
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(f"failed to delete task with error {e}")
```

### Comparing `flytekit-1.8.3/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.9.0a0/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/pytorch/__init__.py` & `flytekit-1.9.0a0/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.9.0a0/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/pytorch/native.py` & `flytekit-1.9.0a0/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/sklearn/__init__.py` & `flytekit-1.9.0a0/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/sklearn/native.py` & `flytekit-1.9.0a0/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/sqlite3/task.py` & `flytekit-1.9.0a0/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/tasks/shell.py` & `flytekit-1.9.0a0/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.9.0a0/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/tensorflow/model.py` & `flytekit-1.9.0a0/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/extras/tensorflow/record.py` & `flytekit-1.9.0a0/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/image_spec/image_spec.py` & `flytekit-1.9.0a0/flytekit/image_spec/image_spec.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 import base64
 import hashlib
 import os
-import pathlib
 import typing
 from abc import abstractmethod
 from copy import copy
-from dataclasses import asdict, dataclass
+from dataclasses import dataclass
 from functools import lru_cache
 from typing import List, Optional
 
 import click
 import requests
+from dataclasses_json import dataclass_json
 
 DOCKER_HUB = "docker.io"
 _F_IMG_ID = "_F_IMG_ID"
 
 
+@dataclass_json
 @dataclass
 class ImageSpec:
     """
     This class is used to specify the docker image that will be used to run the task.
 
     Args:
         name: name of the image.
         python_version: python version of the image. Use default python in the base image if None.
         builder: Type of plugin to build the image. Use envd by default.
         source_root: source root of the image.
         env: environment variables of the image.
         registry: registry of the image.
         packages: list of python packages to install.
-        requirements: path to the requirements.txt file.
         apt_packages: list of apt packages to install.
-        cuda: version of cuda to install.
-        cudnn: version of cudnn to install.
         base_image: base image of the image.
         platform: Specify the target platforms for the build output (for example, windows/amd64 or linux/amd64,darwin/arm64
-        pip_index: Specify the custom pip index url
-        registry_config: Specify the path to a JSON registry config file
     """
 
     name: str = "flytekit"
     python_version: str = None  # Use default python in the base image if None.
     builder: str = "envd"
     source_root: Optional[str] = None
     env: Optional[typing.Dict[str, str]] = None
     registry: Optional[str] = None
     packages: Optional[List[str]] = None
-    requirements: Optional[str] = None
     apt_packages: Optional[List[str]] = None
-    cuda: Optional[str] = None
-    cudnn: Optional[str] = None
     base_image: Optional[str] = None
     platform: str = "linux/amd64"
-    pip_index: Optional[str] = None
-    registry_config: Optional[str] = None
 
     def image_name(self) -> str:
         """
         return full image name with tag.
         """
         tag = calculate_hash_from_image_spec(self)
         container_image = f"{self.name}:{tag}"
@@ -109,15 +100,15 @@
                     return False
 
             click.secho(f"Failed to check if the image exists with error : {e}", fg="red")
             click.secho("Flytekit assumes that the image already exists.", fg="blue")
             return True
 
     def __hash__(self):
-        return hash(asdict(self).__str__())
+        return hash(self.to_json())
 
 
 class ImageSpecBuilder:
     @abstractmethod
     def build_image(self, image_spec: ImageSpec):
         """
         Build the docker image and push it to the registry.
@@ -130,49 +121,42 @@
 
 class ImageBuildEngine:
     """
     ImageBuildEngine contains a list of builders that can be used to build an ImageSpec.
     """
 
     _REGISTRY: typing.Dict[str, ImageSpecBuilder] = {}
-    _BUILT_IMAGES: typing.Set[str] = set()
 
     @classmethod
     def register(cls, builder_type: str, image_spec_builder: ImageSpecBuilder):
         cls._REGISTRY[builder_type] = image_spec_builder
 
     @classmethod
     def build(cls, image_spec: ImageSpec):
         if image_spec.builder not in cls._REGISTRY:
             raise Exception(f"Builder {image_spec.builder} is not registered.")
-        img_name = image_spec.image_name()
-        if img_name in cls._BUILT_IMAGES or image_spec.exist():
-            click.secho(f"Image {img_name} found. Skip building.", fg="blue")
-        else:
-            click.secho(f"Image {img_name} not found. Building...", fg="blue")
+        if not image_spec.exist():
+            click.secho(f"Image {image_spec.image_name()} not found. Building...", fg="blue")
             cls._REGISTRY[image_spec.builder].build_image(image_spec)
-            cls._BUILT_IMAGES.add(img_name)
+        else:
+            click.secho(f"Image {image_spec.image_name()} found. Skip building.", fg="blue")
 
 
 @lru_cache
 def calculate_hash_from_image_spec(image_spec: ImageSpec):
     """
     Calculate the hash from the image spec.
     """
     # copy the image spec to avoid modifying the original image spec. otherwise, the hash will be different.
     spec = copy(image_spec)
     spec.source_root = hash_directory(image_spec.source_root) if image_spec.source_root else b""
-    if spec.requirements:
-        spec.requirements = hashlib.sha1(pathlib.Path(spec.requirements).read_bytes()).hexdigest()
-    # won't rebuild the image if we change the registry_config path
-    spec.registry_config = None
-    image_spec_bytes = asdict(spec).__str__().encode("utf-8")
+    image_spec_bytes = bytes(spec.to_json(), "utf-8")
     tag = base64.urlsafe_b64encode(hashlib.md5(image_spec_bytes).digest()).decode("ascii")
-    # replace "=" with "." and replace "-" with "_" to make it a valid tag
-    return tag.replace("=", ".").replace("-", "_")
+    # replace "=" with "." to make it a valid tag
+    return tag.replace("=", ".")
 
 
 def hash_directory(path):
     """
     Return the SHA-256 hash of the directory at the given path.
     """
     hasher = hashlib.sha256()
```

### Comparing `flytekit-1.8.3/flytekit/interaction/parse_stdin.py` & `flytekit-1.9.0a0/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.9.0a0/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/interfaces/random.py` & `flytekit-1.9.0a0/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/interfaces/stats/client.py` & `flytekit-1.9.0a0/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/interfaces/stats/taggable.py` & `flytekit-1.9.0a0/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/lazy_import/lazy_module.py` & `flytekit-1.9.0a0/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/loggers.py` & `flytekit-1.9.0a0/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/admin/common.py` & `flytekit-1.9.0a0/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/admin/task_execution.py` & `flytekit-1.9.0a0/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/admin/workflow.py` & `flytekit-1.9.0a0/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/annotation.py` & `flytekit-1.9.0a0/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/array_job.py` & `flytekit-1.9.0a0/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/common.py` & `flytekit-1.9.0a0/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/core/catalog.py` & `flytekit-1.9.0a0/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/core/compiler.py` & `flytekit-1.9.0a0/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/core/condition.py` & `flytekit-1.9.0a0/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/core/errors.py` & `flytekit-1.9.0a0/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/core/execution.py` & `flytekit-1.9.0a0/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/core/identifier.py` & `flytekit-1.9.0a0/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/core/types.py` & `flytekit-1.9.0a0/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/core/workflow.py` & `flytekit-1.9.0a0/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/documentation.py` & `flytekit-1.9.0a0/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/dynamic_job.py` & `flytekit-1.9.0a0/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/execution.py` & `flytekit-1.9.0a0/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/filters.py` & `flytekit-1.9.0a0/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/interface.py` & `flytekit-1.9.0a0/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/launch_plan.py` & `flytekit-1.9.0a0/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/literals.py` & `flytekit-1.9.0a0/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/matchable_resource.py` & `flytekit-1.9.0a0/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/named_entity.py` & `flytekit-1.9.0a0/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/node_execution.py` & `flytekit-1.9.0a0/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/presto.py` & `flytekit-1.9.0a0/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/project.py` & `flytekit-1.9.0a0/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/qubole.py` & `flytekit-1.9.0a0/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/schedule.py` & `flytekit-1.9.0a0/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/security.py` & `flytekit-1.9.0a0/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/task.py` & `flytekit-1.9.0a0/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/types.py` & `flytekit-1.9.0a0/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/models/workflow_closure.py` & `flytekit-1.9.0a0/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/remote/__init__.py` & `flytekit-1.9.0a0/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/remote/backfill.py` & `flytekit-1.9.0a0/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/remote/entities.py` & `flytekit-1.9.0a0/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/remote/executions.py` & `flytekit-1.9.0a0/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/remote/lazy_entity.py` & `flytekit-1.9.0a0/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/remote/remote.py` & `flytekit-1.9.0a0/flytekit/remote/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,19 +74,18 @@
     FlyteControlPlaneEntity,
     FlyteLocalEntity,
     Options,
     get_serializable,
     get_serializable_launch_plan,
 )
 
-if typing.TYPE_CHECKING:
-    try:
-        from IPython.core.display import HTML
-    except ImportError:
-        ...
+try:
+    from IPython.core.display import HTML
+except ImportError:
+    ...
 
 ExecutionDataResponse = typing.Union[WorkflowExecutionGetDataResponse, NodeExecutionGetDataResponse]
 
 MOST_RECENT_FIRST = admin_common_models.Sort("created_at", admin_common_models.Sort.Direction.DESCENDING)
 
 
 class RegistrationSkipped(Exception):
@@ -224,55 +223,46 @@
     @property
     def file_access(self) -> FileAccessProvider:
         """File access provider to use for offloading non-literal inputs/outputs."""
         return self._file_access
 
     def get(
         self, flyte_uri: typing.Optional[str] = None
-    ) -> typing.Optional[typing.Union[LiteralsResolver, Literal, HTML, bytes]]:
-        """
-        General function that works with flyte tiny urls. This can return outputs (in the form of LiteralsResolver, or
-        individual Literals for singular requests), or HTML if passed a deck link, or bytes containing HTML,
-        if ipython is not available locally.
-        """
+    ) -> typing.Optional[typing.Union[LiteralsResolver, HTML, bytes]]:
         if flyte_uri is None:
             raise user_exceptions.FlyteUserException("flyte_uri cannot be empty")
         ctx = self._ctx or FlyteContextManager.current_context()
         try:
             data_response = self.client.get_data(flyte_uri)
 
             if data_response.HasField("literal_map"):
                 lm = LiteralMap.from_flyte_idl(data_response.literal_map)
                 return LiteralsResolver(lm.literals)
-            elif data_response.HasField("literal"):
-                return data_response.literal
             elif data_response.HasField("pre_signed_urls"):
                 if len(data_response.pre_signed_urls.signed_url) == 0:
                     raise ValueError(f"Flyte url {flyte_uri} resolved to empty download link")
                 d = data_response.pre_signed_urls.signed_url[0]
                 remote_logger.debug(f"Download link is {d}")
                 fs = ctx.file_access.get_filesystem_for_path(d)
 
                 # If the venv has IPython, then return IPython's HTML
                 if ipython_check():
-                    from IPython.core.display import HTML
-
                     remote_logger.debug(f"IPython found, returning HTML from {flyte_uri}")
                     with fs.open(d, "rb") as r:
                         html = HTML(str(r.read()))
                         return html
                 # If not return bytes
                 else:
                     remote_logger.debug(f"IPython not found, returning HTML as bytes from {flyte_uri}")
                     return fs.open(d, "rb").read()
 
         except user_exceptions.FlyteUserException as e:
             remote_logger.info(f"Error from Flyte backend when trying to fetch data: {e.__cause__}")
 
-        remote_logger.info(f"Nothing found from {flyte_uri}")
+        remote_logger.debug(f"Nothing found from {flyte_uri}")
 
     def remote_context(self):
         """Context manager with remote-specific configuration."""
         return FlyteContextManager.with_context(
             FlyteContextManager.current_context().with_file_access(self.file_access)
         )
```

### Comparing `flytekit-1.8.3/flytekit/remote/remote_callable.py` & `flytekit-1.9.0a0/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/testing/__init__.py` & `flytekit-1.9.0a0/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/tools/fast_registration.py` & `flytekit-1.9.0a0/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/tools/ignore.py` & `flytekit-1.9.0a0/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/tools/module_loader.py` & `flytekit-1.9.0a0/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/tools/repo.py` & `flytekit-1.9.0a0/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/tools/script_mode.py` & `flytekit-1.9.0a0/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/tools/serialize_helpers.py` & `flytekit-1.9.0a0/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/tools/subprocess.py` & `flytekit-1.9.0a0/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/tools/translator.py` & `flytekit-1.9.0a0/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/types/directory/__init__.py` & `flytekit-1.9.0a0/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/types/directory/types.py` & `flytekit-1.9.0a0/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/types/file/__init__.py` & `flytekit-1.9.0a0/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/types/file/file.py` & `flytekit-1.9.0a0/flytekit/types/file/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import pathlib
 import typing
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 
 from dataclasses_json import config, dataclass_json
 from marshmallow import fields
+from typing_extensions import Annotated, get_args, get_origin
 
 from flytekit.core.context_manager import FlyteContext, FlyteContextManager
-from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError, get_underlying_type
+from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
 from flytekit.loggers import logger
 from flytekit.models.core.types import BlobType
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 from flytekit.types.pickle.pickle import FlytePickleTransformer
 
 
@@ -332,15 +333,16 @@
         remote_path = None
         should_upload = True
 
         if python_val is None:
             raise TypeTransformerFailedError("None value cannot be converted to a file.")
 
         # Correctly handle `Annotated[FlyteFile, ...]` by extracting the origin type
-        python_type = get_underlying_type(python_type)
+        if get_origin(python_type) is Annotated:
+            python_type = get_args(python_type)[0]
 
         if not (python_type is os.PathLike or issubclass(python_type, FlyteFile)):
             raise ValueError(f"Incorrect type {python_type}, must be either a FlyteFile or os.PathLike")
 
         # information used by all cases
         meta = BlobMetadata(type=self._blob_type(format=FlyteFilePathTransformer.get_format(python_type)))
 
@@ -407,17 +409,14 @@
         except AttributeError:
             raise TypeTransformerFailedError(f"Cannot convert from {lv} to {expected_python_type}")
         # In this condition, we still return a FlyteFile instance, but it's a simple one that has no downloading tricks
         # Using is instead of issubclass because FlyteFile does actually subclass it
         if expected_python_type is os.PathLike:
             return FlyteFile(uri)
 
-        # Correctly handle `Annotated[FlyteFile, ...]` by extracting the origin type
-        expected_python_type = get_underlying_type(expected_python_type)
-
         # The rest of the logic is only for FlyteFile types.
         if not issubclass(expected_python_type, FlyteFile):  # type: ignore
             raise TypeError(f"Neither os.PathLike nor FlyteFile specified {expected_python_type}")
 
         # This is a local file path, like /usr/local/my_file, don't mess with it. Certainly, downloading it doesn't
         # make any sense.
         if not ctx.file_access.is_remote(uri):
```

### Comparing `flytekit-1.8.3/flytekit/types/numpy/ndarray.py` & `flytekit-1.9.0a0/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/types/pickle/pickle.py` & `flytekit-1.9.0a0/flytekit/types/pickle/pickle.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,14 @@
             ctx.file_access.get_data(uri, local_path, False)
             uri = local_path
         with open(uri, "rb") as infile:
             data = cloudpickle.load(infile)
         return data
 
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
-        if python_val is None:
-            raise AssertionError("Cannot pickle None Value.")
         meta = BlobMetadata(
             type=_core_types.BlobType(
                 format=self.PYTHON_PICKLE_FORMAT, dimensionality=_core_types.BlobType.BlobDimensionality.SINGLE
             )
         )
         # Dump the task output into pickle
         local_dir = ctx.file_access.get_random_local_directory()
@@ -100,17 +98,15 @@
             and literal_type.blob.format == FlytePickleTransformer.PYTHON_PICKLE_FORMAT
         ):
             return FlytePickle
 
         raise ValueError(f"Transformer {self} cannot reverse {literal_type}")
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
-        lt = LiteralType(
+        return LiteralType(
             blob=_core_types.BlobType(
                 format=self.PYTHON_PICKLE_FORMAT, dimensionality=_core_types.BlobType.BlobDimensionality.SINGLE
             )
         )
-        lt.metadata = {"python_class_name": str(t)}
-        return lt
 
 
 TypeEngine.register(FlytePickleTransformer())
```

### Comparing `flytekit-1.8.3/flytekit/types/schema/types.py` & `flytekit-1.9.0a0/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/types/schema/types_pandas.py` & `flytekit-1.9.0a0/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/types/structured/__init__.py` & `flytekit-1.9.0a0/flytekit/types/structured/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,14 @@
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
     StructuredDatasetTransformerEngine,
 )
 
 
-def register_csv_handlers():
-
-    from .basic_dfs import CSVToPandasDecodingHandler, PandasToCSVEncodingHandler
-
-    StructuredDatasetTransformerEngine.register(PandasToCSVEncodingHandler(), default_format_for_type=True)
-    StructuredDatasetTransformerEngine.register(CSVToPandasDecodingHandler(), default_format_for_type=True)
-
-
 def register_pandas_handlers():
     import pandas as pd
 
     from .basic_dfs import PandasToParquetEncodingHandler, ParquetToPandasDecodingHandler
 
     StructuredDatasetTransformerEngine.register(PandasToParquetEncodingHandler(), default_format_for_type=True)
     StructuredDatasetTransformerEngine.register(ParquetToPandasDecodingHandler(), default_format_for_type=True)
```

### Comparing `flytekit-1.8.3/flytekit/types/structured/basic_dfs.py` & `flytekit-1.9.0a0/flytekit/types/structured/basic_dfs.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from flytekit import FlyteContext, logger
 from flytekit.configuration import DataConfig
 from flytekit.core.data_persistence import s3_setup_args
 from flytekit.models import literals
 from flytekit.models.literals import StructuredDatasetMetadata
 from flytekit.models.types import StructuredDatasetType
 from flytekit.types.structured.structured_dataset import (
-    CSV,
     PARQUET,
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
 )
 
 T = TypeVar("T")
@@ -32,62 +31,14 @@
     if protocol == "s3":
         kwargs = s3_setup_args(cfg.s3, anon)
         if kwargs:
             return kwargs
     return None
 
 
-class PandasToCSVEncodingHandler(StructuredDatasetEncoder):
-    def __init__(self):
-        super().__init__(pd.DataFrame, None, CSV)
-
-    def encode(
-        self,
-        ctx: FlyteContext,
-        structured_dataset: StructuredDataset,
-        structured_dataset_type: StructuredDatasetType,
-    ) -> literals.StructuredDataset:
-        uri = typing.cast(str, structured_dataset.uri) or ctx.file_access.get_random_remote_directory()
-        if not ctx.file_access.is_remote(uri):
-            Path(uri).mkdir(parents=True, exist_ok=True)
-        path = os.path.join(uri, ".csv")
-        df = typing.cast(pd.DataFrame, structured_dataset.dataframe)
-        df.to_csv(
-            path,
-            index=False,
-            storage_options=get_storage_options(ctx.file_access.data_config, path),
-        )
-        structured_dataset_type.format = CSV
-        return literals.StructuredDataset(uri=uri, metadata=StructuredDatasetMetadata(structured_dataset_type))
-
-
-class CSVToPandasDecodingHandler(StructuredDatasetDecoder):
-    def __init__(self):
-        super().__init__(pd.DataFrame, None, CSV)
-
-    def decode(
-        self,
-        ctx: FlyteContext,
-        flyte_value: literals.StructuredDataset,
-        current_task_metadata: StructuredDatasetMetadata,
-    ) -> pd.DataFrame:
-        uri = flyte_value.uri
-        columns = None
-        kwargs = get_storage_options(ctx.file_access.data_config, uri)
-        path = os.path.join(uri, ".csv")
-        if current_task_metadata.structured_dataset_type and current_task_metadata.structured_dataset_type.columns:
-            columns = [c.name for c in current_task_metadata.structured_dataset_type.columns]
-        try:
-            return pd.read_csv(path, usecols=columns, storage_options=kwargs)
-        except NoCredentialsError:
-            logger.debug("S3 source detected, attempting anonymous S3 access")
-            kwargs = get_storage_options(ctx.file_access.data_config, uri, anon=True)
-            return pd.read_csv(path, usecols=columns, storage_options=kwargs)
-
-
 class PandasToParquetEncodingHandler(StructuredDatasetEncoder):
     def __init__(self):
         super().__init__(pd.DataFrame, None, PARQUET)
 
     def encode(
         self,
         ctx: FlyteContext,
```

### Comparing `flytekit-1.8.3/flytekit/types/structured/bigquery.py` & `flytekit-1.9.0a0/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/flytekit/types/structured/structured_dataset.py` & `flytekit-1.9.0a0/flytekit/types/structured/structured_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 DF = typing.TypeVar("DF")  # Dataframe type
 
 # For specifying the storage formats of StructuredDatasets. It's just a string, nothing fancy.
 StructuredDatasetFormat: TypeAlias = str
 
 # Storage formats
 PARQUET: StructuredDatasetFormat = "parquet"
-CSV: StructuredDatasetFormat = "csv"
 GENERIC_FORMAT: StructuredDatasetFormat = ""
 GENERIC_PROTOCOL: str = "generic protocol"
 
 
 @dataclass_json
 @dataclass
 class StructuredDataset(object):
@@ -387,15 +386,15 @@
 
         except KeyError:
             ...
 
         if protocol_specific_handler or fsspec_handler or single_handler:
             return protocol_specific_handler or fsspec_handler or single_handler
         else:
-            raise ValueError(f"Failed to find a handler for {df_type}, protocol [{protocol}], fmt ['{format}']")
+            raise ValueError(f"Failed to find a handler for {df_type}, protocol {protocol}, fmt |{format}|")
 
     @classmethod
     def get_encoder(cls, df_type: Type, protocol: str, format: str):
         return cls._finder(StructuredDatasetTransformerEngine.ENCODERS, df_type, protocol, format)
 
     @classmethod
     def get_decoder(cls, df_type: Type, protocol: str, format: str):
```

### Comparing `flytekit-1.8.3/flytekit.egg-info/PKG-INFO` & `flytekit-1.9.0a0/flytekit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.8.3
+Version: 1.9.0a0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.8.3 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.9.0a0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.8.3/flytekit.egg-info/SOURCES.txt` & `flytekit-1.9.0a0/flytekit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,16 @@
 flytekit/exceptions/__init__.py
 flytekit/exceptions/base.py
 flytekit/exceptions/scopes.py
 flytekit/exceptions/system.py
 flytekit/exceptions/user.py
 flytekit/extend/__init__.py
 flytekit/extend/backend/__init__.py
-flytekit/extend/backend/agent_service.py
-flytekit/extend/backend/base_agent.py
+flytekit/extend/backend/base_plugin.py
+flytekit/extend/backend/external_plugin_service.py
 flytekit/extras/__init__.py
 flytekit/extras/cloud_pickle_resolver.py
 flytekit/extras/pytorch/__init__.py
 flytekit/extras/pytorch/checkpoint.py
 flytekit/extras/pytorch/native.py
 flytekit/extras/sklearn/__init__.py
 flytekit/extras/sklearn/native.py
@@ -191,16 +191,14 @@
 flytekit/tools/subprocess.py
 flytekit/tools/translator.py
 flytekit/types/__init__.py
 flytekit/types/directory/__init__.py
 flytekit/types/directory/types.py
 flytekit/types/file/__init__.py
 flytekit/types/file/file.py
-flytekit/types/iterator/__init__.py
-flytekit/types/iterator/iterator.py
 flytekit/types/numpy/__init__.py
 flytekit/types/numpy/ndarray.py
 flytekit/types/pickle/__init__.py
 flytekit/types/pickle/pickle.py
 flytekit/types/schema/__init__.py
 flytekit/types/schema/types.py
 flytekit/types/schema/types_pandas.py
```

### Comparing `flytekit-1.8.3/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.9.0a0/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.3/setup.py` & `flytekit-1.9.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.8.3"
+__version__ = "1.9.0a0"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -25,50 +25,50 @@
             "pyflyte-map-execute=flytekit.bin.entrypoint:map_execute_task_cmd",
             "pyflyte=flytekit.clis.sdk_in_container.pyflyte:main",
             "flyte-cli=flytekit.clis.flyte_cli.main:_flyte_cli",
         ]
     },
     install_requires=[
         "googleapis-common-protos>=1.57",
-        "flyteidl>=1.5.10",
+        "flyteidl>=1.5.4",
         "wheel>=0.30.0,<1.0.0",
         "pandas>=1.0.0,<2.0.0",
         "pyarrow>=4.0.0,<11.0.0",
         "click>=6.6,<9.0",
         "croniter>=0.3.20,<4.0.0",
         "deprecated>=1.0,<2.0",
         "docker>=4.0.0,<7.0.0",
         "python-dateutil>=2.1",
         # Restrict grpcio and grpcio-status.  Version 1.50.0 pulls in a version of protobuf that is not compatible
         # with the old protobuf library (as described in https://developers.google.com/protocol-buffers/docs/news/2022-05-06)
-        "grpcio>=1.50.0,!=1.55.0,<1.53.1,<2.0",
-        "grpcio-status>=1.50.0,!=1.55.0,<1.53.1,<2.0",
+        "grpcio>=1.50.0,<2.0",
+        "grpcio-status>=1.50.0,<2.0",
         "importlib-metadata",
         "fsspec>=2023.3.0",
         "adlfs",
         "s3fs>=0.6.0",
         "gcsfs",
         "pyopenssl",
         "joblib",
         "python-json-logger>=2.0.0",
         "pytimeparse>=1.1.8,<2.0.0",
         "pytz",
-        "pyyaml!=6.0.0,!=5.4.0,!=5.4.1",  # pyyaml is broken with cython 3: https://github.com/yaml/pyyaml/issues/601
+        "pyyaml",
         "keyring>=18.0.1",
         "requests>=2.18.4,<3.0.0",
+        "responses>=0.10.7",
         "sortedcontainers>=1.5.9,<3.0.0",
         "statsd>=3.0.0,<4.0.0",
         "urllib3>=1.22,<2.0.0",
         "wrapt>=1.0.0,<2.0.0",
-        # TODO: remove upper-bound after fixing change in contract
-        "dataclasses-json>=0.5.2,<0.5.12",
+        "dataclasses-json>=0.5.2",
         "marshmallow-jsonschema>=0.12.0",
-        "marshmallow-enum",
         "natsort>=7.0.1",
         "docker-image-py>=0.1.10",
+        "singledispatchmethod; python_version < '3.8.0'",
         "typing_extensions",
         "docstring-parser>=0.9.0",
         "diskcache>=5.2.1",
         "cloudpickle>=2.0.0",
         "cookiecutter>=1.7.3",
         "numpy",
         "gitpython",
```

