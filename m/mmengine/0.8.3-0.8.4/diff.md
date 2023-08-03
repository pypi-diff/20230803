# Comparing `tmp/mmengine-0.8.3.tar.gz` & `tmp/mmengine-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-0.8.3.tar", last modified: Mon Jul 31 09:23:23 2023, max compression
+gzip compressed data, was "dist/mmengine-0.8.4.tar", last modified: Thu Aug  3 15:45:01 2023, max compression
```

## Comparing `mmengine-0.8.3.tar` & `mmengine-0.8.4.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 09:20:06.000000 mmengine-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-07-31 09:23:23.000000 mmengine-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-07-31 09:20:06.000000 mmengine-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    26838 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/_strategy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73964 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/config/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29994 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    19045 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/efficient_conv_bn_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66277 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/_flexible_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)   102028 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    53635 2023-07-31 09:20:06.000000 mmengine-0.8.3/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-07-31 09:23:22.000000 mmengine-0.8.3/mmengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-31 09:23:23.000000 mmengine-0.8.3/mmengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:23:22.000000 mmengine-0.8.3/mmengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 09:23:22.000000 mmengine-0.8.3/mmengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 09:23:22.000000 mmengine-0.8.3/mmengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-31 09:23:23.000000 mmengine-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-31 09:20:06.000000 mmengine-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 15:43:24.000000 mmengine-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-08-03 15:45:01.000000 mmengine-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-08-03 15:43:24.000000 mmengine-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/_strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/_strategy/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/_strategy/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26838 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/_strategy/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/_strategy/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/_strategy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73964 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/config/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18486 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29994 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19045 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/efficient_conv_bn_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/wrappers/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67167 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/_flexible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102028 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54112 2023-08-03 15:43:24.000000 mmengine-0.8.4/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 15:45:01.000000 mmengine-0.8.4/mmengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 15:45:01.000000 mmengine-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-03 15:43:24.000000 mmengine-0.8.4/setup.py
```

### Comparing `mmengine-0.8.3/PKG-INFO` & `mmengine-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.8.3
+Version: 0.8.4
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -62,15 +62,15 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## What's New
         
-        v0.8.3 was released on 2023-07-31.
+        v0.8.4 was released on 2023-08-03.
         
         Highlights:
         
         - Support enabling `efficient_conv_bn_eval` for efficient convolution and batch normalization. See [save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#save-memory-on-gpu) for more details
         
         - Add an [example](./examples/llama2/) to finetune Llama2.
         
@@ -84,15 +84,15 @@
           - Support inheriting two configuration files containing the same field
           - Load the configuration file without other third-party requirements
         
           Refer to the [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) for more detailed usages.
         
           ![new-config-en](https://github.com/open-mmlab/mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1)
         
-        Read [Changelog](./docs/en/notes/changelog.md#v083-07312023) for more details.
+        Read [Changelog](./docs/en/notes/changelog.md#v083-08032023) for more details.
         
         ## Table of Contents
         
         - [Introduction](#introduction)
         - [Installation](#installation)
         - [Get Started](#get-started)
         - [Learn More](#learn-more)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.8.3 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.8.4 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
@@ -17,15 +17,15 @@
    badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/
 mmengine/issues) [ðDocumentation](https://mmengine.readthedocs.io/en/latest/
      ) | [ð ï¸Installation](https://mmengine.readthedocs.io/en/latest/
   get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
                     open-mmlab/mmengine/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-## What's New v0.8.3 was released on 2023-07-31. Highlights: - Support enabling
+## What's New v0.8.4 was released on 2023-08-03. Highlights: - Support enabling
 `efficient_conv_bn_eval` for efficient convolution and batch normalization. See
 [save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/
 save_gpu_memory.html#save-memory-on-gpu) for more details - Add an [example](./
 examples/llama2/) to finetune Llama2. - Support training with [FSDP](https://
 pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp)
 and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large
 Models](https://mmengine.readthedocs.io/en/latest/common_usage/
@@ -34,15 +34,15 @@
 file in IDE - Support navigating to base variable in IDE - Support navigating
 to source code of class in IDE - Support inheriting two configuration files
 containing the same field - Load the configuration file without other third-
 party requirements Refer to the [tutorial](https://mmengine.readthedocs.io/en/
 latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-
 beta) for more detailed usages. ![new-config-en](https://github.com/open-mmlab/
 mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1) Read [Changelog]
-(./docs/en/notes/changelog.md#v083-07312023) for more details. ## Table of
+(./docs/en/notes/changelog.md#v083-08032023) for more details. ## Table of
 Contents - [Introduction](#introduction) - [Installation](#installation) - [Get
 Started](#get-started) - [Learn More](#learn-more) - [Contributing]
 (#contributing) - [Citation](#citation) - [License](#license) - [Ecosystem]
 (#ecosystem) - [Projects in OpenMMLab](#projects-in-openmmlab) ## Introduction
 MMEngine is a foundational library for training deep learning models based on
 PyTorch. It provides a solid engineering foundation and frees developers from
 writing redundant codes on workflows. It serves as the training engine of all
```

### Comparing `mmengine-0.8.3/README.md` & `mmengine-0.8.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
 </div>
 
 ## What's New
 
-v0.8.3 was released on 2023-07-31.
+v0.8.4 was released on 2023-08-03.
 
 Highlights:
 
 - Support enabling `efficient_conv_bn_eval` for efficient convolution and batch normalization. See [save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#save-memory-on-gpu) for more details
 
 - Add an [example](./examples/llama2/) to finetune Llama2.
 
@@ -76,15 +76,15 @@
   - Support inheriting two configuration files containing the same field
   - Load the configuration file without other third-party requirements
 
   Refer to the [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) for more detailed usages.
 
   ![new-config-en](https://github.com/open-mmlab/mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1)
 
-Read [Changelog](./docs/en/notes/changelog.md#v083-07312023) for more details.
+Read [Changelog](./docs/en/notes/changelog.md#v083-08032023) for more details.
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
 - [Get Started](#get-started)
 - [Learn More](#learn-more)
```

### Comparing `mmengine-0.8.3/mmengine/_strategy/__init__.py` & `mmengine-0.8.4/mmengine/_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/_strategy/base.py` & `mmengine-0.8.4/mmengine/_strategy/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/_strategy/deepspeed.py` & `mmengine-0.8.4/mmengine/_strategy/deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/_strategy/distributed.py` & `mmengine-0.8.4/mmengine/_strategy/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/_strategy/fsdp.py` & `mmengine-0.8.4/mmengine/_strategy/fsdp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/_strategy/single_device.py` & `mmengine-0.8.4/mmengine/_strategy/single_device.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/_strategy/utils.py` & `mmengine-0.8.4/mmengine/_strategy/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/analysis/complexity_analysis.py` & `mmengine-0.8.4/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/analysis/jit_analysis.py` & `mmengine-0.8.4/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/analysis/jit_handles.py` & `mmengine-0.8.4/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/analysis/print_helper.py` & `mmengine-0.8.4/mmengine/analysis/print_helper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/config/config.py` & `mmengine-0.8.4/mmengine/config/config.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/config/lazy.py` & `mmengine-0.8.4/mmengine/config/lazy.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/config/utils.py` & `mmengine-0.8.4/mmengine/config/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     # Module not found
     if spec is None:
         return False
     origin_path = getattr(spec, 'origin', None)
     if origin_path is None:
         return False
     origin_path = osp.abspath(origin_path)
-    if ('site-package' in origin_path
+    if ('site-package' in origin_path or 'dist-package' in origin_path
             or not origin_path.startswith(PYTHON_ROOT_DIR)):
         return False
     else:
         return True
 
 
 class ImportTransformer(ast.NodeTransformer):
```

### Comparing `mmengine-0.8.3/mmengine/dataset/__init__.py` & `mmengine-0.8.4/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/dataset/base_dataset.py` & `mmengine-0.8.4/mmengine/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/dataset/dataset_wrapper.py` & `mmengine-0.8.4/mmengine/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/dataset/sampler.py` & `mmengine-0.8.4/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/dataset/utils.py` & `mmengine-0.8.4/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/device/utils.py` & `mmengine-0.8.4/mmengine/device/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/dist/__init__.py` & `mmengine-0.8.4/mmengine/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/dist/dist.py` & `mmengine-0.8.4/mmengine/dist/dist.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/dist/utils.py` & `mmengine-0.8.4/mmengine/dist/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/evaluator/evaluator.py` & `mmengine-0.8.4/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/evaluator/metric.py` & `mmengine-0.8.4/mmengine/evaluator/metric.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/evaluator/utils.py` & `mmengine-0.8.4/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/__init__.py` & `mmengine-0.8.4/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/backends/__init__.py` & `mmengine-0.8.4/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/backends/base.py` & `mmengine-0.8.4/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/backends/http_backend.py` & `mmengine-0.8.4/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-0.8.4/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/backends/local_backend.py` & `mmengine-0.8.4/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/backends/memcached_backend.py` & `mmengine-0.8.4/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/backends/petrel_backend.py` & `mmengine-0.8.4/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/backends/registry_utils.py` & `mmengine-0.8.4/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/file_client.py` & `mmengine-0.8.4/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/handlers/base.py` & `mmengine-0.8.4/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/handlers/json_handler.py` & `mmengine-0.8.4/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-0.8.4/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/handlers/registry_utils.py` & `mmengine-0.8.4/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-0.8.4/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/io.py` & `mmengine-0.8.4/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/fileio/parse.py` & `mmengine-0.8.4/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/__init__.py` & `mmengine-0.8.4/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/checkpoint_hook.py` & `mmengine-0.8.4/mmengine/hooks/checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/early_stopping_hook.py` & `mmengine-0.8.4/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/ema_hook.py` & `mmengine-0.8.4/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/empty_cache_hook.py` & `mmengine-0.8.4/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/hook.py` & `mmengine-0.8.4/mmengine/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/iter_timer_hook.py` & `mmengine-0.8.4/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/logger_hook.py` & `mmengine-0.8.4/mmengine/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/naive_visualization_hook.py` & `mmengine-0.8.4/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/param_scheduler_hook.py` & `mmengine-0.8.4/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/profiler_hook.py` & `mmengine-0.8.4/mmengine/hooks/profiler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/runtime_info_hook.py` & `mmengine-0.8.4/mmengine/hooks/runtime_info_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/sampler_seed_hook.py` & `mmengine-0.8.4/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/sync_buffer_hook.py` & `mmengine-0.8.4/mmengine/hooks/sync_buffer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hooks/test_time_aug_hook.py` & `mmengine-0.8.4/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hub/hub.py` & `mmengine-0.8.4/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hub/mmcls.json` & `mmengine-0.8.4/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hub/openmmlab.json` & `mmengine-0.8.4/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/hub/torchvision_0.12.json` & `mmengine-0.8.4/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/infer/infer.py` & `mmengine-0.8.4/mmengine/infer/infer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/logging/history_buffer.py` & `mmengine-0.8.4/mmengine/logging/history_buffer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/logging/logger.py` & `mmengine-0.8.4/mmengine/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/logging/message_hub.py` & `mmengine-0.8.4/mmengine/logging/message_hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/__init__.py` & `mmengine-0.8.4/mmengine/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/averaged_model.py` & `mmengine-0.8.4/mmengine/model/averaged_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/base_model/base_model.py` & `mmengine-0.8.4/mmengine/model/base_model/base_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/base_model/data_preprocessor.py` & `mmengine-0.8.4/mmengine/model/base_model/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/base_module.py` & `mmengine-0.8.4/mmengine/model/base_module.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/efficient_conv_bn_eval.py` & `mmengine-0.8.4/mmengine/model/efficient_conv_bn_eval.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/test_time_aug.py` & `mmengine-0.8.4/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/utils.py` & `mmengine-0.8.4/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/weight_init.py` & `mmengine-0.8.4/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/wrappers/__init__.py` & `mmengine-0.8.4/mmengine/model/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/wrappers/_deepspeed.py` & `mmengine-0.8.4/mmengine/model/wrappers/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/wrappers/distributed.py` & `mmengine-0.8.4/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/wrappers/fully_sharded_distributed.py` & `mmengine-0.8.4/mmengine/model/wrappers/fully_sharded_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-0.8.4/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/model/wrappers/utils.py` & `mmengine-0.8.4/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/__init__.py` & `mmengine-0.8.4/mmengine/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/__init__.py` & `mmengine-0.8.4/mmengine/optim/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/_deepspeed.py` & `mmengine-0.8.4/mmengine/optim/optimizer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-0.8.4/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-0.8.4/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/base.py` & `mmengine-0.8.4/mmengine/optim/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/builder.py` & `mmengine-0.8.4/mmengine/optim/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/default_constructor.py` & `mmengine-0.8.4/mmengine/optim/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-0.8.4/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-0.8.4/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-0.8.4/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/scheduler/__init__.py` & `mmengine-0.8.4/mmengine/optim/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-0.8.4/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-0.8.4/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-0.8.4/mmengine/optim/scheduler/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/registry/__init__.py` & `mmengine-0.8.4/mmengine/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/registry/build_functions.py` & `mmengine-0.8.4/mmengine/registry/build_functions.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/registry/default_scope.py` & `mmengine-0.8.4/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/registry/registry.py` & `mmengine-0.8.4/mmengine/registry/registry.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/registry/root.py` & `mmengine-0.8.4/mmengine/registry/root.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/registry/utils.py` & `mmengine-0.8.4/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/__init__.py` & `mmengine-0.8.4/mmengine/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/_flexible_runner.py` & `mmengine-0.8.4/mmengine/runner/_flexible_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import torch.nn as nn
 from torch.utils.data import DataLoader
 
 import mmengine
 from mmengine._strategy import BaseStrategy
 from mmengine.config import Config, ConfigDict
-from mmengine.dataset import worker_init_fn
+from mmengine.dataset import worker_init_fn as default_worker_init_fn
 from mmengine.dist import get_rank, infer_launcher, master_only
 from mmengine.evaluator import Evaluator
 from mmengine.fileio import FileClient, join_path
 from mmengine.hooks import Hook
 from mmengine.logging import MessageHub, print_log
 from mmengine.optim import OptimWrapper, OptimWrapperDict, _ParamScheduler
 from mmengine.registry import (DATA_SAMPLERS, DATASETS, EVALUATOR, FUNCTIONS,
@@ -853,30 +853,36 @@
         else:
             # fallback to raise error in dataloader
             # if `batch_sampler_cfg` is not a valid type
             batch_sampler = batch_sampler_cfg
 
         # build dataloader
         init_fn: Optional[partial]
-
-        if seed is not None:
-            disable_subprocess_warning = dataloader_cfg.pop(
-                'disable_subprocess_warning', False)
-            assert isinstance(
-                disable_subprocess_warning,
-                bool), ('disable_subprocess_warning should be a bool, but got '
-                        f'{type(disable_subprocess_warning)}')
-            init_fn = partial(
-                worker_init_fn,
-                num_workers=dataloader_cfg.get('num_workers'),
-                rank=get_rank(),
-                seed=seed,
-                disable_subprocess_warning=disable_subprocess_warning)
-        else:
-            init_fn = None
+        if 'worker_init_fn' in dataloader_cfg:
+            worker_init_fn_cfg = dataloader_cfg.pop('worker_init_fn')
+            worker_init_fn_type = worker_init_fn_cfg.pop('type')
+            worker_init_fn = FUNCTIONS.get(worker_init_fn_type)
+            assert callable(worker_init_fn)
+            init_fn = partial(worker_init_fn,
+                              **worker_init_fn_cfg)  # type: ignore
+        else:
+            if seed is not None:
+                disable_subprocess_warning = dataloader_cfg.pop(
+                    'disable_subprocess_warning', False)
+                assert isinstance(disable_subprocess_warning, bool), (
+                    'disable_subprocess_warning should be a bool, but got '
+                    f'{type(disable_subprocess_warning)}')
+                init_fn = partial(
+                    default_worker_init_fn,
+                    num_workers=dataloader_cfg.get('num_workers'),
+                    rank=get_rank(),
+                    seed=seed,
+                    disable_subprocess_warning=disable_subprocess_warning)
+            else:
+                init_fn = None
 
         # `persistent_workers` requires pytorch version >= 1.7
         if ('persistent_workers' in dataloader_cfg
                 and digit_version(TORCH_VERSION) < digit_version('1.7.0')):
             print_log(
                 '`persistent_workers` is only available when '
                 'pytorch version >= 1.7',
@@ -887,17 +893,27 @@
         # The default behavior of `collat_fn` in dataloader is to
         # merge a list of samples to form a mini-batch of Tensor(s).
         # However, in mmengine, if `collate_fn` is not defined in
         # dataloader_cfg, `pseudo_collate` will only convert the list of
         # samples into a dict without stacking the batch tensor.
         collate_fn_cfg = dataloader_cfg.pop('collate_fn',
                                             dict(type='pseudo_collate'))
-        collate_fn_type = collate_fn_cfg.pop('type')
-        collate_fn = FUNCTIONS.get(collate_fn_type)
-        collate_fn = partial(collate_fn, **collate_fn_cfg)  # type: ignore
+        if isinstance(collate_fn_cfg, dict):
+            collate_fn_type = collate_fn_cfg.pop('type')
+            if isinstance(collate_fn_type, str):
+                collate_fn = FUNCTIONS.get(collate_fn_type)
+            else:
+                collate_fn = collate_fn_type
+            collate_fn = partial(collate_fn, **collate_fn_cfg)  # type: ignore
+        elif callable(collate_fn_cfg):
+            collate_fn = collate_fn_cfg
+        else:
+            raise TypeError(
+                'collate_fn should be a dict or callable object, but got '
+                f'{collate_fn_cfg}')
         data_loader = DataLoader(
             dataset=dataset,
             sampler=sampler if batch_sampler is None else None,
             batch_sampler=batch_sampler,
             collate_fn=collate_fn,
             worker_init_fn=init_fn,
             **dataloader_cfg)
```

### Comparing `mmengine-0.8.3/mmengine/runner/amp.py` & `mmengine-0.8.4/mmengine/runner/amp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/base_loop.py` & `mmengine-0.8.4/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/checkpoint.py` & `mmengine-0.8.4/mmengine/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/log_processor.py` & `mmengine-0.8.4/mmengine/runner/log_processor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/loops.py` & `mmengine-0.8.4/mmengine/runner/loops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/priority.py` & `mmengine-0.8.4/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/runner.py` & `mmengine-0.8.4/mmengine/runner/runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/runner/utils.py` & `mmengine-0.8.4/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/structures/base_data_element.py` & `mmengine-0.8.4/mmengine/structures/base_data_element.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/structures/instance_data.py` & `mmengine-0.8.4/mmengine/structures/instance_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/structures/label_data.py` & `mmengine-0.8.4/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/structures/pixel_data.py` & `mmengine-0.8.4/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/testing/__init__.py` & `mmengine-0.8.4/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/testing/_internal/distributed.py` & `mmengine-0.8.4/mmengine/testing/_internal/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/testing/compare.py` & `mmengine-0.8.4/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/testing/runner_test_case.py` & `mmengine-0.8.4/mmengine/testing/runner_test_case.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/__init__.py` & `mmengine-0.8.4/mmengine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/__init__.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/collect_env.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/hub.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/misc.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/setup_env.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/time_counter.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/trace.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/dl_utils/visualize.py` & `mmengine-0.8.4/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/manager.py` & `mmengine-0.8.4/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/misc.py` & `mmengine-0.8.4/mmengine/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/package_utils.py` & `mmengine-0.8.4/mmengine/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/path.py` & `mmengine-0.8.4/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/progressbar.py` & `mmengine-0.8.4/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/timer.py` & `mmengine-0.8.4/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/utils/version_utils.py` & `mmengine-0.8.4/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/version.py` & `mmengine-0.8.4/mmengine/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.8.3'
+__version__ = '0.8.4'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-0.8.3/mmengine/visualization/utils.py` & `mmengine-0.8.4/mmengine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/visualization/vis_backend.py` & `mmengine-0.8.4/mmengine/visualization/vis_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/mmengine/visualization/visualizer.py` & `mmengine-0.8.4/mmengine/visualization/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import inspect
 import os.path as osp
 import warnings
 from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple, Union
 
 if TYPE_CHECKING:
     from matplotlib.font_manager import FontProperties
 
@@ -11,22 +12,25 @@
 import torch
 import torch.nn.functional as F
 
 from mmengine.config import Config
 from mmengine.dist import master_only
 from mmengine.registry import VISBACKENDS, VISUALIZERS
 from mmengine.structures import BaseDataElement
-from mmengine.utils import ManagerMixin
+from mmengine.utils import ManagerMixin, is_seq_of
 from mmengine.visualization.utils import (check_type, check_type_and_length,
                                           color_str2rgb, color_val_matplotlib,
                                           convert_overlay_heatmap,
                                           img_from_canvas, tensor2ndarray,
                                           value2list, wait_continue)
 from mmengine.visualization.vis_backend import BaseVisBackend
 
+VisBackendsType = Union[List[Union[List, BaseDataElement]], BaseDataElement,
+                        dict, None]
+
 
 @VISUALIZERS.register_module()
 class Visualizer(ManagerMixin):
     """MMEngine provides a Visualizer class that uses the ``Matplotlib``
     library as the backend. It has the following functions:
 
     - Basic drawing methods
@@ -149,50 +153,60 @@
         >>>         pass
     """
 
     def __init__(
         self,
         name='visualizer',
         image: Optional[np.ndarray] = None,
-        vis_backends: Optional[List[Dict]] = None,
+        vis_backends: VisBackendsType = None,
         save_dir: Optional[str] = None,
         fig_save_cfg=dict(frameon=False),
         fig_show_cfg=dict(frameon=False)
     ) -> None:
         super().__init__(name)
         self._dataset_meta: Optional[dict] = None
-        self._vis_backends: Union[Dict, Dict[str, 'BaseVisBackend']] = dict()
+        self._vis_backends: Dict[str, BaseVisBackend] = {}
+
+        if vis_backends is None:
+            vis_backends = []
 
-        if vis_backends is not None:
-            assert len(vis_backends) > 0, 'empty list'
-            names = [vis_backend.get('name') for vis_backend in vis_backends]
-            if None in names:
-                if len(set(names)) > 1:
-                    raise RuntimeError(
-                        'If one of them has a name attribute, '
-                        'all backends must use the name attribute')
-                else:
-                    type_names = [
-                        vis_backend['type'] for vis_backend in vis_backends
-                    ]
-                    if len(set(type_names)) != len(type_names):
-                        raise RuntimeError(
-                            'The same vis backend cannot exist in '
-                            '`vis_backend` config. '
-                            'Please specify the name field.')
-
-            if None not in names and len(set(names)) != len(names):
-                raise RuntimeError('The name fields cannot be the same')
-
-            if save_dir is not None:
-                save_dir = osp.join(save_dir, 'vis_data')
-            for vis_backend in vis_backends:
-                name = vis_backend.pop('name', vis_backend['type'])
+        if isinstance(vis_backends, (dict, BaseVisBackend)):
+            vis_backends = [vis_backends]  # type: ignore
+
+        if not is_seq_of(vis_backends, (dict, BaseVisBackend)):
+            raise TypeError('vis_backends must be a list of dicts or a list '
+                            'of BaseBackend instances')
+        if save_dir is not None:
+            save_dir = osp.join(save_dir, 'vis_data')
+
+        for vis_backend in vis_backends:  # type: ignore
+            name = None
+            if isinstance(vis_backend, dict):
+                name = vis_backend.pop('name', None)
                 vis_backend.setdefault('save_dir', save_dir)
-                self._vis_backends[name] = VISBACKENDS.build(vis_backend)
+                vis_backend = VISBACKENDS.build(vis_backend)
+
+            # If vis_backend requires `save_dir` (with no default value)
+            # but is initialized with None, then don't add this
+            # vis_backend to the visualizer.
+            save_dir_arg = inspect.signature(
+                vis_backend.__class__.__init__).parameters.get('save_dir')
+            if (save_dir_arg is not None
+                    and save_dir_arg.default is save_dir_arg.empty
+                    and getattr(vis_backend, '_save_dir') is None):
+                warnings.warn(f'Failed to add {vis_backend.__class__}, '
+                              'please provide the `save_dir` argument.')
+                continue
+
+            type_name = vis_backend.__class__.__name__
+            name = name or type_name
+
+            if name in self._vis_backends:
+                raise RuntimeError(f'vis_backend name {name} already exists')
+            self._vis_backends[name] = vis_backend  # type: ignore
 
         self.fig_save = None
         self.fig_save_cfg = fig_save_cfg
         self.fig_show_cfg = fig_show_cfg
 
         (self.fig_save_canvas, self.fig_save,
          self.ax_save) = self._initialize_fig(fig_save_cfg)
```

### Comparing `mmengine-0.8.3/mmengine.egg-info/PKG-INFO` & `mmengine-0.8.4/mmengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.8.3
+Version: 0.8.4
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -62,15 +62,15 @@
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## What's New
         
-        v0.8.3 was released on 2023-07-31.
+        v0.8.4 was released on 2023-08-03.
         
         Highlights:
         
         - Support enabling `efficient_conv_bn_eval` for efficient convolution and batch normalization. See [save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/save_gpu_memory.html#save-memory-on-gpu) for more details
         
         - Add an [example](./examples/llama2/) to finetune Llama2.
         
@@ -84,15 +84,15 @@
           - Support inheriting two configuration files containing the same field
           - Load the configuration file without other third-party requirements
         
           Refer to the [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) for more detailed usages.
         
           ![new-config-en](https://github.com/open-mmlab/mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1)
         
-        Read [Changelog](./docs/en/notes/changelog.md#v083-07312023) for more details.
+        Read [Changelog](./docs/en/notes/changelog.md#v083-08032023) for more details.
         
         ## Table of Contents
         
         - [Introduction](#introduction)
         - [Installation](#installation)
         - [Get Started](#get-started)
         - [Learn More](#learn-more)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.8.3 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.8.4 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
@@ -17,15 +17,15 @@
    badge/resolution/open-mmlab/mmengine.svg)](https://github.com/open-mmlab/
 mmengine/issues) [ðDocumentation](https://mmengine.readthedocs.io/en/latest/
      ) | [ð ï¸Installation](https://mmengine.readthedocs.io/en/latest/
   get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
                     open-mmlab/mmengine/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-## What's New v0.8.3 was released on 2023-07-31. Highlights: - Support enabling
+## What's New v0.8.4 was released on 2023-08-03. Highlights: - Support enabling
 `efficient_conv_bn_eval` for efficient convolution and batch normalization. See
 [save memory on gpu](https://mmengine.readthedocs.io/en/latest/common_usage/
 save_gpu_memory.html#save-memory-on-gpu) for more details - Add an [example](./
 examples/llama2/) to finetune Llama2. - Support training with [FSDP](https://
 pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp)
 and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large
 Models](https://mmengine.readthedocs.io/en/latest/common_usage/
@@ -34,15 +34,15 @@
 file in IDE - Support navigating to base variable in IDE - Support navigating
 to source code of class in IDE - Support inheriting two configuration files
 containing the same field - Load the configuration file without other third-
 party requirements Refer to the [tutorial](https://mmengine.readthedocs.io/en/
 latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-
 beta) for more detailed usages. ![new-config-en](https://github.com/open-mmlab/
 mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1) Read [Changelog]
-(./docs/en/notes/changelog.md#v083-07312023) for more details. ## Table of
+(./docs/en/notes/changelog.md#v083-08032023) for more details. ## Table of
 Contents - [Introduction](#introduction) - [Installation](#installation) - [Get
 Started](#get-started) - [Learn More](#learn-more) - [Contributing]
 (#contributing) - [Citation](#citation) - [License](#license) - [Ecosystem]
 (#ecosystem) - [Projects in OpenMMLab](#projects-in-openmmlab) ## Introduction
 MMEngine is a foundational library for training deep learning models based on
 PyTorch. It provides a solid engineering foundation and frees developers from
 writing redundant codes on workflows. It serves as the training engine of all
```

### Comparing `mmengine-0.8.3/mmengine.egg-info/SOURCES.txt` & `mmengine-0.8.4/mmengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.3/setup.py` & `mmengine-0.8.4/setup.py`

 * *Files identical despite different names*

