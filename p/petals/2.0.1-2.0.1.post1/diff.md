# Comparing `tmp/petals-2.0.1.tar.gz` & `tmp/petals-2.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petals-2.0.1.tar", last modified: Sun Jul 23 14:48:31 2023, max compression
+gzip compressed data, was "petals-2.0.1.post1.tar", last modified: Thu Aug  3 00:17:40 2023, max compression
```

## Comparing `petals-2.0.1.tar` & `petals-2.0.1.post1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.315667 petals-2.0.1/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1089 2022-11-26 05:33:56.000000 petals-2.0.1/LICENSE
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    13837 2023-07-23 14:48:31.315667 petals-2.0.1/PKG-INFO
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12664 2023-07-23 12:40:54.000000 petals-2.0.1/README.md
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      333 2023-04-25 09:55:28.000000 petals-2.0.1/pyproject.toml
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1743 2023-07-23 14:48:31.315667 petals-2.0.1/setup.cfg
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.307667 petals-2.0.1/src/
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.307667 petals-2.0.1/src/petals/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      778 2023-07-23 14:46:44.000000 petals-2.0.1/src/petals/__init__.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.307667 petals-2.0.1/src/petals/cli/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2022-11-30 08:13:52.000000 petals-2.0.1/src/petals/cli/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3798 2023-01-13 00:54:42.000000 petals-2.0.1/src/petals/cli/run_dht.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14144 2023-07-23 14:46:44.000000 petals-2.0.1/src/petals/cli/run_server.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.311667 petals-2.0.1/src/petals/client/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      282 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/client/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3600 2023-07-12 11:02:03.000000 petals-2.0.1/src/petals/client/from_pretrained.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15296 2023-07-18 23:25:43.000000 petals-2.0.1/src/petals/client/inference_session.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3526 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/client/lm_head.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3493 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/client/ptune.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7128 2023-02-06 20:57:31.000000 petals-2.0.1/src/petals/client/remote_forward_backward.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14964 2023-05-09 21:02:40.000000 petals-2.0.1/src/petals/client/remote_generation.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2675 2023-07-12 12:22:35.000000 petals-2.0.1/src/petals/client/remote_sequential.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.311667 petals-2.0.1/src/petals/client/routing/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       71 2022-12-01 12:24:57.000000 petals-2.0.1/src/petals/client/routing/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4629 2023-07-17 09:46:40.000000 petals-2.0.1/src/petals/client/routing/sequence_info.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    23031 2023-07-23 12:40:54.000000 petals-2.0.1/src/petals/client/routing/sequence_manager.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      649 2022-12-01 12:24:57.000000 petals-2.0.1/src/petals/client/routing/spending_policy.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12405 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/client/sequential_autograd.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      904 2023-07-20 17:00:05.000000 petals-2.0.1/src/petals/constants.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2348 2023-07-19 16:28:49.000000 petals-2.0.1/src/petals/data_structures.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4511 2023-07-17 06:29:38.000000 petals-2.0.1/src/petals/dht_utils.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.311667 petals-2.0.1/src/petals/models/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       68 2023-07-13 20:49:11.000000 petals-2.0.1/src/petals/models/__init__.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.311667 petals-2.0.1/src/petals/models/bloom/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      556 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/models/bloom/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1414 2023-07-13 20:49:11.000000 petals-2.0.1/src/petals/models/bloom/block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1380 2023-07-19 16:28:49.000000 petals-2.0.1/src/petals/models/bloom/config.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5243 2023-07-19 01:15:47.000000 petals-2.0.1/src/petals/models/bloom/model.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.311667 petals-2.0.1/src/petals/models/llama/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      556 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/models/llama/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3582 2023-07-19 16:28:49.000000 petals-2.0.1/src/petals/models/llama/block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1893 2023-07-19 16:28:49.000000 petals-2.0.1/src/petals/models/llama/config.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5998 2023-07-19 01:15:47.000000 petals-2.0.1/src/petals/models/llama/model.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.311667 petals-2.0.1/src/petals/server/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2022-11-30 08:13:52.000000 petals-2.0.1/src/petals/server/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11814 2023-07-23 12:40:54.000000 petals-2.0.1/src/petals/server/backend.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4499 2023-04-06 15:09:40.000000 petals-2.0.1/src/petals/server/block_selection.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1893 2023-07-12 11:02:03.000000 petals-2.0.1/src/petals/server/block_utils.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6664 2023-07-23 12:40:54.000000 petals-2.0.1/src/petals/server/from_pretrained.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    35240 2023-07-23 12:40:54.000000 petals-2.0.1/src/petals/server/handler.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8216 2023-07-21 14:06:01.000000 petals-2.0.1/src/petals/server/memory_cache.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7706 2023-07-20 17:00:05.000000 petals-2.0.1/src/petals/server/reachability.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    30466 2023-07-23 14:46:44.000000 petals-2.0.1/src/petals/server/server.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8412 2023-04-06 15:09:40.000000 petals-2.0.1/src/petals/server/task_pool.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      842 2023-01-22 05:16:17.000000 petals-2.0.1/src/petals/server/task_prioritizer.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8657 2023-07-23 12:40:54.000000 petals-2.0.1/src/petals/server/throughput.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.311667 petals-2.0.1/src/petals/utils/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      182 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/utils/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      525 2022-12-29 20:33:47.000000 petals-2.0.1/src/petals/utils/asyncio.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2258 2023-07-23 12:40:54.000000 petals-2.0.1/src/petals/utils/auto_config.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6594 2023-07-19 16:28:49.000000 petals-2.0.1/src/petals/utils/convert_block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2963 2023-07-09 23:10:48.000000 petals-2.0.1/src/petals/utils/disk_cache.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5560 2023-07-18 09:05:08.000000 petals-2.0.1/src/petals/utils/generation_algorithms.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1853 2022-12-03 11:35:20.000000 petals-2.0.1/src/petals/utils/generation_constraints.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      270 2023-07-19 16:28:49.000000 petals-2.0.1/src/petals/utils/hf_auth.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      745 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/utils/logging.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      171 2023-07-19 16:28:49.000000 petals-2.0.1/src/petals/utils/misc.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12164 2023-07-19 16:28:49.000000 petals-2.0.1/src/petals/utils/peft.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2283 2023-07-18 09:05:08.000000 petals-2.0.1/src/petals/utils/ping.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      310 2023-07-18 09:05:08.000000 petals-2.0.1/src/petals/utils/random.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1438 2023-06-29 20:31:16.000000 petals-2.0.1/src/petals/utils/version.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.307667 petals-2.0.1/src/petals.egg-info/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    13837 2023-07-23 14:48:31.000000 petals-2.0.1/src/petals.egg-info/PKG-INFO
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2331 2023-07-23 14:48:31.000000 petals-2.0.1/src/petals.egg-info/SOURCES.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        1 2023-07-23 14:48:31.000000 petals-2.0.1/src/petals.egg-info/dependency_links.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      456 2023-07-23 14:48:31.000000 petals-2.0.1/src/petals.egg-info/requires.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        7 2023-07-23 14:48:31.000000 petals-2.0.1/src/petals.egg-info/top_level.txt
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-07-23 14:48:31.315667 petals-2.0.1/tests/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1646 2023-07-17 09:46:40.000000 petals-2.0.1/tests/test_aux_functions.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1603 2023-06-30 00:37:10.000000 petals-2.0.1/tests/test_block_exact_match.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2947 2023-06-29 20:31:16.000000 petals-2.0.1/tests/test_chained_calls.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      672 2023-06-29 20:31:16.000000 petals-2.0.1/tests/test_dtype.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8315 2023-07-23 12:40:54.000000 petals-2.0.1/tests/test_full_model.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1535 2023-07-12 12:22:35.000000 petals-2.0.1/tests/test_peft.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2848 2023-04-25 15:58:19.000000 petals-2.0.1/tests/test_priority_pool.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6055 2023-07-09 23:10:48.000000 petals-2.0.1/tests/test_remote_sequential.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1924 2023-07-14 15:21:17.000000 petals-2.0.1/tests/test_sequence_manager.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1707 2023-06-29 20:31:16.000000 petals-2.0.1/tests/test_server_stats.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1911 2023-06-29 20:31:16.000000 petals-2.0.1/tests/test_tensor_parallel.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      466 2023-07-12 12:22:35.000000 petals-2.0.1/tests/test_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.960434 petals-2.0.1.post1/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1089 2022-11-26 05:33:56.000000 petals-2.0.1.post1/LICENSE
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14156 2023-08-03 00:17:40.960434 petals-2.0.1.post1/PKG-INFO
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12977 2023-07-30 23:26:35.000000 petals-2.0.1.post1/README.md
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      333 2023-04-25 09:55:28.000000 petals-2.0.1.post1/pyproject.toml
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1743 2023-08-03 00:17:40.960434 petals-2.0.1.post1/setup.cfg
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.952434 petals-2.0.1.post1/src/
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      784 2023-08-03 00:17:32.000000 petals-2.0.1.post1/src/petals/__init__.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals/cli/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2022-11-30 08:13:52.000000 petals-2.0.1.post1/src/petals/cli/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3798 2023-01-13 00:54:42.000000 petals-2.0.1.post1/src/petals/cli/run_dht.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14144 2023-07-23 14:46:44.000000 petals-2.0.1.post1/src/petals/cli/run_server.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals/client/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      282 2023-06-29 20:31:16.000000 petals-2.0.1.post1/src/petals/client/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3600 2023-07-12 11:02:03.000000 petals-2.0.1.post1/src/petals/client/from_pretrained.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15296 2023-07-30 23:01:42.000000 petals-2.0.1.post1/src/petals/client/inference_session.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3526 2023-06-29 20:31:16.000000 petals-2.0.1.post1/src/petals/client/lm_head.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3493 2023-06-29 20:31:16.000000 petals-2.0.1.post1/src/petals/client/ptune.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7379 2023-07-30 23:01:42.000000 petals-2.0.1.post1/src/petals/client/remote_forward_backward.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14964 2023-05-09 21:02:40.000000 petals-2.0.1.post1/src/petals/client/remote_generation.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2675 2023-07-12 12:22:35.000000 petals-2.0.1.post1/src/petals/client/remote_sequential.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals/client/routing/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       71 2022-12-01 12:24:57.000000 petals-2.0.1.post1/src/petals/client/routing/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4629 2023-07-17 09:46:40.000000 petals-2.0.1.post1/src/petals/client/routing/sequence_info.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    22887 2023-08-03 00:02:55.000000 petals-2.0.1.post1/src/petals/client/routing/sequence_manager.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      649 2022-12-01 12:24:57.000000 petals-2.0.1.post1/src/petals/client/routing/spending_policy.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12371 2023-07-30 23:01:42.000000 petals-2.0.1.post1/src/petals/client/sequential_autograd.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      904 2023-07-20 17:00:05.000000 petals-2.0.1.post1/src/petals/constants.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2348 2023-07-19 16:28:49.000000 petals-2.0.1.post1/src/petals/data_structures.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4511 2023-07-17 06:29:38.000000 petals-2.0.1.post1/src/petals/dht_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals/models/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       68 2023-07-13 20:49:11.000000 petals-2.0.1.post1/src/petals/models/__init__.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals/models/bloom/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      556 2023-06-29 20:31:16.000000 petals-2.0.1.post1/src/petals/models/bloom/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1414 2023-07-13 20:49:11.000000 petals-2.0.1.post1/src/petals/models/bloom/block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1380 2023-07-19 16:28:49.000000 petals-2.0.1.post1/src/petals/models/bloom/config.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5243 2023-07-19 01:15:47.000000 petals-2.0.1.post1/src/petals/models/bloom/model.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals/models/llama/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      556 2023-06-29 20:31:16.000000 petals-2.0.1.post1/src/petals/models/llama/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3582 2023-07-19 16:28:49.000000 petals-2.0.1.post1/src/petals/models/llama/block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1893 2023-07-19 16:28:49.000000 petals-2.0.1.post1/src/petals/models/llama/config.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5998 2023-07-19 01:15:47.000000 petals-2.0.1.post1/src/petals/models/llama/model.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals/server/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2022-11-30 08:13:52.000000 petals-2.0.1.post1/src/petals/server/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11814 2023-07-23 12:40:54.000000 petals-2.0.1.post1/src/petals/server/backend.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4499 2023-04-06 15:09:40.000000 petals-2.0.1.post1/src/petals/server/block_selection.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1893 2023-07-12 11:02:03.000000 petals-2.0.1.post1/src/petals/server/block_utils.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6664 2023-08-01 08:47:57.000000 petals-2.0.1.post1/src/petals/server/from_pretrained.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    35240 2023-07-23 12:40:54.000000 petals-2.0.1.post1/src/petals/server/handler.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8216 2023-07-21 14:06:01.000000 petals-2.0.1.post1/src/petals/server/memory_cache.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7706 2023-07-20 17:00:05.000000 petals-2.0.1.post1/src/petals/server/reachability.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    30542 2023-08-03 00:02:55.000000 petals-2.0.1.post1/src/petals/server/server.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8412 2023-04-06 15:09:40.000000 petals-2.0.1.post1/src/petals/server/task_pool.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      842 2023-01-22 05:16:17.000000 petals-2.0.1.post1/src/petals/server/task_prioritizer.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8786 2023-08-03 00:02:55.000000 petals-2.0.1.post1/src/petals/server/throughput.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.960434 petals-2.0.1.post1/src/petals/utils/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      182 2023-06-29 20:31:16.000000 petals-2.0.1.post1/src/petals/utils/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      525 2022-12-29 20:33:47.000000 petals-2.0.1.post1/src/petals/utils/asyncio.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2258 2023-07-23 12:40:54.000000 petals-2.0.1.post1/src/petals/utils/auto_config.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6594 2023-07-19 16:28:49.000000 petals-2.0.1.post1/src/petals/utils/convert_block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2963 2023-07-09 23:10:48.000000 petals-2.0.1.post1/src/petals/utils/disk_cache.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5560 2023-07-18 09:05:08.000000 petals-2.0.1.post1/src/petals/utils/generation_algorithms.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1853 2022-12-03 11:35:20.000000 petals-2.0.1.post1/src/petals/utils/generation_constraints.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      270 2023-07-19 16:28:49.000000 petals-2.0.1.post1/src/petals/utils/hf_auth.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      745 2023-06-29 20:31:16.000000 petals-2.0.1.post1/src/petals/utils/logging.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      171 2023-07-19 16:28:49.000000 petals-2.0.1.post1/src/petals/utils/misc.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12164 2023-07-19 16:28:49.000000 petals-2.0.1.post1/src/petals/utils/peft.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2460 2023-08-03 00:17:32.000000 petals-2.0.1.post1/src/petals/utils/ping.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      310 2023-07-18 09:05:08.000000 petals-2.0.1.post1/src/petals/utils/random.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1438 2023-06-29 20:31:16.000000 petals-2.0.1.post1/src/petals/utils/version.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.956434 petals-2.0.1.post1/src/petals.egg-info/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14156 2023-08-03 00:17:40.000000 petals-2.0.1.post1/src/petals.egg-info/PKG-INFO
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2331 2023-08-03 00:17:40.000000 petals-2.0.1.post1/src/petals.egg-info/SOURCES.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        1 2023-08-03 00:17:40.000000 petals-2.0.1.post1/src/petals.egg-info/dependency_links.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      456 2023-08-03 00:17:40.000000 petals-2.0.1.post1/src/petals.egg-info/requires.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        7 2023-08-03 00:17:40.000000 petals-2.0.1.post1/src/petals.egg-info/top_level.txt
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-08-03 00:17:40.960434 petals-2.0.1.post1/tests/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1646 2023-07-17 09:46:40.000000 petals-2.0.1.post1/tests/test_aux_functions.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1603 2023-06-30 00:37:10.000000 petals-2.0.1.post1/tests/test_block_exact_match.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2947 2023-06-29 20:31:16.000000 petals-2.0.1.post1/tests/test_chained_calls.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      672 2023-06-29 20:31:16.000000 petals-2.0.1.post1/tests/test_dtype.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8315 2023-07-23 12:40:54.000000 petals-2.0.1.post1/tests/test_full_model.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1535 2023-07-12 12:22:35.000000 petals-2.0.1.post1/tests/test_peft.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2848 2023-04-25 15:58:19.000000 petals-2.0.1.post1/tests/test_priority_pool.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6055 2023-07-09 23:10:48.000000 petals-2.0.1.post1/tests/test_remote_sequential.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1924 2023-07-14 15:21:17.000000 petals-2.0.1.post1/tests/test_sequence_manager.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1707 2023-06-29 20:31:16.000000 petals-2.0.1.post1/tests/test_server_stats.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1911 2023-06-29 20:31:16.000000 petals-2.0.1.post1/tests/test_tensor_parallel.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      466 2023-07-12 12:22:35.000000 petals-2.0.1.post1/tests/test_utils.py
```

### Comparing `petals-2.0.1/LICENSE` & `petals-2.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/PKG-INFO` & `petals-2.0.1.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petals
-Version: 2.0.1
+Version: 2.0.1.post1
 Summary: Easy way to efficiently run 100B+ language models without high-end GPUs
 Home-page: https://github.com/bigscience-workshop/petals
 Author: Petals Developers
 Author-email: petals-devs@googlegroups.com
 Project-URL: Bug Tracker, https://github.com/bigscience-workshop/petals/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,27 +24,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
     <img src="https://i.imgur.com/7eR7Pan.png" width="400"><br>
     Run large language models at home, BitTorrent-style.<br>
-    Fine-tuning and inference <a href="https://github.com/bigscience-workshop/petals#benchmarks">up to 10x faster</a> than offloading<br><br>
-    <a href="https://pypi.org/project/petals/"><img src="https://img.shields.io/pypi/v/petals.svg?color=green"></a><br>
+    Fine-tuning and inference <a href="https://github.com/bigscience-workshop/petals#benchmarks">up to 10x faster</a> than offloading
+    <br><br>
+    <a href="https://pypi.org/project/petals/"><img src="https://img.shields.io/pypi/v/petals.svg?color=green"></a>
+    <a href="https://discord.gg/tfHfe8B34k"><img src="https://img.shields.io/discord/865254854262652969?label=discord&logo=discord&logoColor=white"></a>
+    <br>
 </p>
 
-Generate text with distributed [LLaMA 2](https://ai.meta.com/llama/) ([70B](https://huggingface.co/meta-llama/Llama-2-70b-hf), [70B-Chat](https://huggingface.co/meta-llama/Llama-2-70b-chat-hf)), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and fine‑tune them for your own tasks &mdash; right from your desktop computer or Google Colab:
+Generate text with distributed [LLaMA 2 (70B)](https://huggingface.co/meta-llama/Llama-2-70b-hf), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and fine‑tune them for your own tasks &mdash; right from your desktop computer or Google Colab:
 
 ```python
 from transformers import AutoTokenizer
 from petals import AutoDistributedModelForCausalLM
 
-model_name = "enoch/llama-65b-hf"
+model_name = "stabilityai/StableBeluga2"
 # You can also use "meta-llama/Llama-2-70b-hf", "meta-llama/Llama-2-70b-chat-hf",
-# "bigscience/bloom", or "bigscience/bloomz"
+# repos with LLaMA-65B, "bigscience/bloom", or "bigscience/bloomz"
 
 tokenizer = AutoTokenizer.from_pretrained(model_name)
 model = AutoDistributedModelForCausalLM.from_pretrained(model_name)
 # Embeddings & prompts are on your device, transformer blocks are distributed across the Internet
 
 inputs = tokenizer("A cat sat", return_tensors="pt")["input_ids"]
 outputs = model.generate(inputs, max_new_tokens=5)
@@ -53,48 +56,50 @@
 
 <p align="center">
     🚀 &nbsp;<b><a href="https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing">Try now in Colab</a></b>
 </p>
 
 🦙 **Want to run LLaMA 2?** Request access to its weights at the ♾️ [Meta AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and 🤗 [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), then run `huggingface-cli login` in the terminal before loading the model. Or just try it in our [chatbot app](https://chat.petals.dev).
 
-📋 **Terms of use.** Make sure you follow the model license (see the ones for [LLaMA 2](https://bit.ly/llama2-license), [LLaMA](https://bit.ly/llama-license) and [BLOOM](https://bit.ly/bloom-license)).
+📋 **Terms of use.** Make sure you follow the model license (see [LLaMA 2](https://bit.ly/llama2-license), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2/blob/main/LICENSE.txt), [LLaMA](https://bit.ly/llama-license), and [BLOOM](https://bit.ly/bloom-license)).
 
 🔏 **Privacy.** Your data will be processed by other people in the public swarm. Learn more about privacy [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety). For sensitive data, you can set up a [private swarm](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm) among people you trust.
 
+💬 **Any questions?** Ping us in [our Discord](https://discord.gg/J29mCBNBvm)!
+
 ### Connect your GPU and increase Petals capacity
 
 Petals is a community-run system &mdash; we rely on people sharing their GPUs. You can check out available servers on our [swarm monitor](https://health.petals.dev) and connect your GPU to help serving one of the models!
 
 🐍 **Linux + Anaconda.** Run these commands:
 
 ```bash
 conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
 pip install git+https://github.com/bigscience-workshop/petals
-python -m petals.cli.run_server enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
+python -m petals.cli.run_server stabilityai/StableBeluga2 --torch_dtype float16
 ```
 
 🪟 **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/bigscience-workshop/petals/wiki/Run-Petals-server-on-Windows).
 
 🐋 **Any OS + Docker.** Run our [Docker](https://www.docker.com) image:
 
 ```bash
 sudo docker run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm learningathome/petals:main \
-    python -m petals.cli.run_server --port 31330 enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
+    python -m petals.cli.run_server --port 31330 stabilityai/StableBeluga2 --torch_dtype float16
 ```
 
-These commands host a part of LLaMA-65B with optional [Guanaco](https://huggingface.co/timdettmers/guanaco-65b) adapters on your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, `bigscience/bloom`, `bigscience/bloomz`, and other compatible models from 🤗 [Model Hub](https://huggingface.co/models), or [add support](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model architectures.
+These commands will host a part of [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2) on your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, repos with LLaMA-65B, `bigscience/bloom`, `bigscience/bloomz`, and other compatible models from 🤗 [Model Hub](https://huggingface.co/models), or [add support](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model architectures.
 
 🦙 **Want to host LLaMA 2?** Request access to its weights at the ♾️ [Meta AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and 🤗 [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), generate an 🔑 [access token](https://huggingface.co/settings/tokens), then use this command for `petals.cli.run_server`:
 
 ```bash
 python -m petals.cli.run_server meta-llama/Llama-2-70b-chat-hf --token YOUR_TOKEN_HERE
 ```
 
-💬 **FAQ.** Check out our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to use multple GPUs, restart the server on reboot, etc. If you have any issues or feedback, ping us in [our Discord](https://discord.gg/D9MwApKgWa)!
+💬 **FAQ.** Check out our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to use multple GPUs, restart the server on reboot, etc. If you have any issues, ping us in [our Discord](https://discord.gg/D9MwApKgWa)!
 
 🔒 **Security.** Hosting a server does not allow others to run custom code on your computer. Learn more [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
 
 🏆 **Thank you!** Once you load and host 10+ blocks, we can show your name or link on the [swarm monitor](https://health.petals.dev) as a way to say thanks. You can specify them with `--public_name YOUR_NAME`.
 
 ### Check out tutorials, examples, and more
 
@@ -102,16 +107,16 @@
 
 - Getting started: [tutorial](https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-sst2.ipynb)
 - Prompt-tune BLOOM to create a personified chatbot: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-personachat.ipynb)
 
 Useful tools and advanced guides:
 
-- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.dev)
-- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/borzunov/health.petals.dev)
+- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/petals-infra/chat.petals.dev)
+- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/petals-infra/health.petals.dev)
 - Launch your own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm)
 - Run a custom foundation model: [guide](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals)
 
 Learning more:
 
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions)
 - In-depth system description: [paper](https://arxiv.org/abs/2209.01188)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petals Version: 2.0.1 Summary: Easy way to
+Metadata-Version: 2.1 Name: petals Version: 2.0.1.post1 Summary: Easy way to
 efficiently run 100B+ language models without high-end GPUs Home-page: https://
 github.com/bigscience-workshop/petals Author: Petals Developers Author-email:
 petals-devs@googlegroups.com Project-URL: Bug Tracker, https://github.com/
 bigscience-workshop/petals/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -14,92 +14,94 @@
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Provides-Extra: dev License-File: LICENSE
                        [https://i.imgur.com/7eR7Pan.png]
              Run large language models at home, BitTorrent-style.
           Fine-tuning and inference up_to_10x_faster than offloading
 
-            [https://img.shields.io/pypi/v/petals.svg?color=green]
-Generate text with distributed [LLaMA 2](https://ai.meta.com/llama/) ([70B]
-(https://huggingface.co/meta-llama/Llama-2-70b-hf), [70B-Chat](https://
-huggingface.co/meta-llama/Llama-2-70b-chat-hf)), [LLaMA-65B](https://
-github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B]
-(https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://
-huggingface.co/bigscience/bloom) and fineâtune them for your own tasks —
-right from your desktop computer or Google Colab: ```python from transformers
-import AutoTokenizer from petals import AutoDistributedModelForCausalLM
-model_name = "enoch/llama-65b-hf" # You can also use "meta-llama/Llama-2-70b-
-hf", "meta-llama/Llama-2-70b-chat-hf", # "bigscience/bloom", or "bigscience/
-bloomz" tokenizer = AutoTokenizer.from_pretrained(model_name) model =
+[https://img.shields.io/pypi/v/petals.svg?color=green] [https://img.shields.io/
+    discord/865254854262652969?label=discord&logo=discord&logoColor=white]
+Generate text with distributed [LLaMA 2 (70B)](https://huggingface.co/meta-
+llama/Llama-2-70b-hf), [Stable Beluga 2](https://huggingface.co/stabilityai/
+StableBeluga2), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/
+llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/
+guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and
+fineâtune them for your own tasks — right from your desktop computer or
+Google Colab: ```python from transformers import AutoTokenizer from petals
+import AutoDistributedModelForCausalLM model_name = "stabilityai/StableBeluga2"
+# You can also use "meta-llama/Llama-2-70b-hf", "meta-llama/Llama-2-70b-chat-
+hf", # repos with LLaMA-65B, "bigscience/bloom", or "bigscience/bloomz"
+tokenizer = AutoTokenizer.from_pretrained(model_name) model =
 AutoDistributedModelForCausalLM.from_pretrained(model_name) # Embeddings &
 prompts are on your device, transformer blocks are distributed across the
 Internet inputs = tokenizer("A cat sat", return_tensors="pt")["input_ids"]
 outputs = model.generate(inputs, max_new_tokens=5) print(tokenizer.decode
 (outputs[0])) # A cat sat on a mat... ```
                             ð  Try_now_in_Colab
 ð¦ **Want to run LLaMA 2?** Request access to its weights at the â¾ï¸ [Meta
 AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/
 ) and ð¤ [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), then
 run `huggingface-cli login` in the terminal before loading the model. Or just
 try it in our [chatbot app](https://chat.petals.dev). ð **Terms of use.**
-Make sure you follow the model license (see the ones for [LLaMA 2](https://
-bit.ly/llama2-license), [LLaMA](https://bit.ly/llama-license) and [BLOOM]
+Make sure you follow the model license (see [LLaMA 2](https://bit.ly/llama2-
+license), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2/
+blob/main/LICENSE.txt), [LLaMA](https://bit.ly/llama-license), and [BLOOM]
 (https://bit.ly/bloom-license)). ð **Privacy.** Your data will be processed
 by other people in the public swarm. Learn more about privacy [here](https://
 github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
 For sensitive data, you can set up a [private swarm](https://github.com/
 bigscience-workshop/petals/wiki/Launch-your-own-swarm) among people you trust.
-### Connect your GPU and increase Petals capacity Petals is a community-run
-system — we rely on people sharing their GPUs. You can check out available
-servers on our [swarm monitor](https://health.petals.dev) and connect your GPU
-to help serving one of the models! ð **Linux + Anaconda.** Run these
-commands: ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
-pip install git+https://github.com/bigscience-workshop/petals python -
-m petals.cli.run_server enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
-``` ðª **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/
+ð¬ **Any questions?** Ping us in [our Discord](https://discord.gg/
+J29mCBNBvm)! ### Connect your GPU and increase Petals capacity Petals is a
+community-run system — we rely on people sharing their GPUs. You can check out
+available servers on our [swarm monitor](https://health.petals.dev) and connect
+your GPU to help serving one of the models! ð **Linux + Anaconda.** Run
+these commands: ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -
+c nvidia pip install git+https://github.com/bigscience-workshop/petals python -
+m petals.cli.run_server stabilityai/StableBeluga2 --torch_dtype float16 ```
+ðª **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/
 bigscience-workshop/petals/wiki/Run-Petals-server-on-Windows). ð **Any OS +
 Docker.** Run our [Docker](https://www.docker.com) image: ```bash sudo docker
 run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm
 learningathome/petals:main \ python -m petals.cli.run_server --port 31330
-enoch/llama-65b-hf --adapters timdettmers/guanaco-65b ``` These commands host a
-part of LLaMA-65B with optional [Guanaco](https://huggingface.co/timdettmers/
-guanaco-65b) adapters on your machine. You can also host `meta-llama/Llama-2-
-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, `bigscience/bloom`, `bigscience/
-bloomz`, and other compatible models from ð¤ [Model Hub](https://
-huggingface.co/models), or [add support](https://github.com/bigscience-
-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model
-architectures. ð¦ **Want to host LLaMA 2?** Request access to its weights at
-the â¾ï¸ [Meta AI website](https://ai.meta.com/resources/models-and-
-libraries/llama-downloads/) and ð¤ [Model Hub](https://huggingface.co/meta-
-llama/Llama-2-70b-hf), generate an ð [access token](https://huggingface.co/
-settings/tokens), then use this command for `petals.cli.run_server`: ```bash
-python -m petals.cli.run_server meta-llama/Llama-2-70b-chat-hf --token
-YOUR_TOKEN_HERE ``` ð¬ **FAQ.** Check out our [Wiki](https://github.com/
-bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-
-server) to learn how to use multple GPUs, restart the server on reboot, etc. If
-you have any issues or feedback, ping us in [our Discord](https://discord.gg/
-D9MwApKgWa)! ð **Security.** Hosting a server does not allow others to run
-custom code on your computer. Learn more [here](https://github.com/bigscience-
-workshop/petals/wiki/Security,-privacy,-and-AI-safety). ð **Thank you!**
-Once you load and host 10+ blocks, we can show your name or link on the [swarm
-monitor](https://health.petals.dev) as a way to say thanks. You can specify
-them with `--public_name YOUR_NAME`. ### Check out tutorials, examples, and
-more Basic tutorials: - Getting started: [tutorial](https://
+stabilityai/StableBeluga2 --torch_dtype float16 ``` These commands will host a
+part of [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2) on
+your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-
+2-70b-chat-hf`, repos with LLaMA-65B, `bigscience/bloom`, `bigscience/bloomz`,
+and other compatible models from ð¤ [Model Hub](https://huggingface.co/
+models), or [add support](https://github.com/bigscience-workshop/petals/wiki/
+Run-a-custom-model-with-Petals) for new model architectures. ð¦ **Want to
+host LLaMA 2?** Request access to its weights at the â¾ï¸ [Meta AI website]
+(https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and ð¤
+[Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), generate an ð
+[access token](https://huggingface.co/settings/tokens), then use this command
+for `petals.cli.run_server`: ```bash python -m petals.cli.run_server meta-
+llama/Llama-2-70b-chat-hf --token YOUR_TOKEN_HERE ``` ð¬ **FAQ.** Check out
+our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-
+asked-questions#running-a-server) to learn how to use multple GPUs, restart the
+server on reboot, etc. If you have any issues, ping us in [our Discord](https:/
+/discord.gg/D9MwApKgWa)! ð **Security.** Hosting a server does not allow
+others to run custom code on your computer. Learn more [here](https://
+github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
+ð **Thank you!** Once you load and host 10+ blocks, we can show your name or
+link on the [swarm monitor](https://health.petals.dev) as a way to say thanks.
+You can specify them with `--public_name YOUR_NAME`. ### Check out tutorials,
+examples, and more Basic tutorials: - Getting started: [tutorial](https://
 colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://
 colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/
 prompt-tuning-sst2.ipynb) - Prompt-tune BLOOM to create a personified chatbot:
 [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/
 blob/main/examples/prompt-tuning-personachat.ipynb) Useful tools and advanced
 guides: - [Chatbot web app](https://chat.petals.dev) (connects to Petals via an
-HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/
+HTTP/WebSocket endpoint): [source code](https://github.com/petals-infra/
 chat.petals.dev) - [Monitor](https://health.petals.dev) for the public swarm:
-[source code](https://github.com/borzunov/health.petals.dev) - Launch your own
-swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-
-own-swarm) - Run a custom foundation model: [guide](https://github.com/
+[source code](https://github.com/petals-infra/health.petals.dev) - Launch your
+own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-
+your-own-swarm) - Run a custom foundation model: [guide](https://github.com/
 bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) Learning more:
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/
 petals/wiki/FAQ:-Frequently-asked-questions) - In-depth system description:
 [paper](https://arxiv.org/abs/2209.01188) ## How does it work? - Petals runs
 large language models like [LLaMA](https://github.com/facebookresearch/llama/
 blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom)
 **collaboratively** â you load a small part of the model, then team up with
```

### Comparing `petals-2.0.1/README.md` & `petals-2.0.1.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 <p align="center">
     <img src="https://i.imgur.com/7eR7Pan.png" width="400"><br>
     Run large language models at home, BitTorrent-style.<br>
-    Fine-tuning and inference <a href="https://github.com/bigscience-workshop/petals#benchmarks">up to 10x faster</a> than offloading<br><br>
-    <a href="https://pypi.org/project/petals/"><img src="https://img.shields.io/pypi/v/petals.svg?color=green"></a><br>
+    Fine-tuning and inference <a href="https://github.com/bigscience-workshop/petals#benchmarks">up to 10x faster</a> than offloading
+    <br><br>
+    <a href="https://pypi.org/project/petals/"><img src="https://img.shields.io/pypi/v/petals.svg?color=green"></a>
+    <a href="https://discord.gg/tfHfe8B34k"><img src="https://img.shields.io/discord/865254854262652969?label=discord&logo=discord&logoColor=white"></a>
+    <br>
 </p>
 
-Generate text with distributed [LLaMA 2](https://ai.meta.com/llama/) ([70B](https://huggingface.co/meta-llama/Llama-2-70b-hf), [70B-Chat](https://huggingface.co/meta-llama/Llama-2-70b-chat-hf)), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and fine‑tune them for your own tasks &mdash; right from your desktop computer or Google Colab:
+Generate text with distributed [LLaMA 2 (70B)](https://huggingface.co/meta-llama/Llama-2-70b-hf), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and fine‑tune them for your own tasks &mdash; right from your desktop computer or Google Colab:
 
 ```python
 from transformers import AutoTokenizer
 from petals import AutoDistributedModelForCausalLM
 
-model_name = "enoch/llama-65b-hf"
+model_name = "stabilityai/StableBeluga2"
 # You can also use "meta-llama/Llama-2-70b-hf", "meta-llama/Llama-2-70b-chat-hf",
-# "bigscience/bloom", or "bigscience/bloomz"
+# repos with LLaMA-65B, "bigscience/bloom", or "bigscience/bloomz"
 
 tokenizer = AutoTokenizer.from_pretrained(model_name)
 model = AutoDistributedModelForCausalLM.from_pretrained(model_name)
 # Embeddings & prompts are on your device, transformer blocks are distributed across the Internet
 
 inputs = tokenizer("A cat sat", return_tensors="pt")["input_ids"]
 outputs = model.generate(inputs, max_new_tokens=5)
@@ -26,48 +29,50 @@
 
 <p align="center">
     🚀 &nbsp;<b><a href="https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing">Try now in Colab</a></b>
 </p>
 
 🦙 **Want to run LLaMA 2?** Request access to its weights at the ♾️ [Meta AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and 🤗 [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), then run `huggingface-cli login` in the terminal before loading the model. Or just try it in our [chatbot app](https://chat.petals.dev).
 
-📋 **Terms of use.** Make sure you follow the model license (see the ones for [LLaMA 2](https://bit.ly/llama2-license), [LLaMA](https://bit.ly/llama-license) and [BLOOM](https://bit.ly/bloom-license)).
+📋 **Terms of use.** Make sure you follow the model license (see [LLaMA 2](https://bit.ly/llama2-license), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2/blob/main/LICENSE.txt), [LLaMA](https://bit.ly/llama-license), and [BLOOM](https://bit.ly/bloom-license)).
 
 🔏 **Privacy.** Your data will be processed by other people in the public swarm. Learn more about privacy [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety). For sensitive data, you can set up a [private swarm](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm) among people you trust.
 
+💬 **Any questions?** Ping us in [our Discord](https://discord.gg/J29mCBNBvm)!
+
 ### Connect your GPU and increase Petals capacity
 
 Petals is a community-run system &mdash; we rely on people sharing their GPUs. You can check out available servers on our [swarm monitor](https://health.petals.dev) and connect your GPU to help serving one of the models!
 
 🐍 **Linux + Anaconda.** Run these commands:
 
 ```bash
 conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
 pip install git+https://github.com/bigscience-workshop/petals
-python -m petals.cli.run_server enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
+python -m petals.cli.run_server stabilityai/StableBeluga2 --torch_dtype float16
 ```
 
 🪟 **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/bigscience-workshop/petals/wiki/Run-Petals-server-on-Windows).
 
 🐋 **Any OS + Docker.** Run our [Docker](https://www.docker.com) image:
 
 ```bash
 sudo docker run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm learningathome/petals:main \
-    python -m petals.cli.run_server --port 31330 enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
+    python -m petals.cli.run_server --port 31330 stabilityai/StableBeluga2 --torch_dtype float16
 ```
 
-These commands host a part of LLaMA-65B with optional [Guanaco](https://huggingface.co/timdettmers/guanaco-65b) adapters on your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, `bigscience/bloom`, `bigscience/bloomz`, and other compatible models from 🤗 [Model Hub](https://huggingface.co/models), or [add support](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model architectures.
+These commands will host a part of [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2) on your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, repos with LLaMA-65B, `bigscience/bloom`, `bigscience/bloomz`, and other compatible models from 🤗 [Model Hub](https://huggingface.co/models), or [add support](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model architectures.
 
 🦙 **Want to host LLaMA 2?** Request access to its weights at the ♾️ [Meta AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and 🤗 [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), generate an 🔑 [access token](https://huggingface.co/settings/tokens), then use this command for `petals.cli.run_server`:
 
 ```bash
 python -m petals.cli.run_server meta-llama/Llama-2-70b-chat-hf --token YOUR_TOKEN_HERE
 ```
 
-💬 **FAQ.** Check out our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to use multple GPUs, restart the server on reboot, etc. If you have any issues or feedback, ping us in [our Discord](https://discord.gg/D9MwApKgWa)!
+💬 **FAQ.** Check out our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to use multple GPUs, restart the server on reboot, etc. If you have any issues, ping us in [our Discord](https://discord.gg/D9MwApKgWa)!
 
 🔒 **Security.** Hosting a server does not allow others to run custom code on your computer. Learn more [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
 
 🏆 **Thank you!** Once you load and host 10+ blocks, we can show your name or link on the [swarm monitor](https://health.petals.dev) as a way to say thanks. You can specify them with `--public_name YOUR_NAME`.
 
 ### Check out tutorials, examples, and more
 
@@ -75,16 +80,16 @@
 
 - Getting started: [tutorial](https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-sst2.ipynb)
 - Prompt-tune BLOOM to create a personified chatbot: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-personachat.ipynb)
 
 Useful tools and advanced guides:
 
-- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.dev)
-- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/borzunov/health.petals.dev)
+- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/petals-infra/chat.petals.dev)
+- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/petals-infra/health.petals.dev)
 - Launch your own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm)
 - Run a custom foundation model: [guide](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals)
 
 Learning more:
 
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions)
 - In-depth system description: [paper](https://arxiv.org/abs/2209.01188)
```

#### html2text {}

```diff
@@ -1,89 +1,91 @@
                        [https://i.imgur.com/7eR7Pan.png]
              Run large language models at home, BitTorrent-style.
           Fine-tuning and inference up_to_10x_faster than offloading
 
-            [https://img.shields.io/pypi/v/petals.svg?color=green]
-Generate text with distributed [LLaMA 2](https://ai.meta.com/llama/) ([70B]
-(https://huggingface.co/meta-llama/Llama-2-70b-hf), [70B-Chat](https://
-huggingface.co/meta-llama/Llama-2-70b-chat-hf)), [LLaMA-65B](https://
-github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B]
-(https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://
-huggingface.co/bigscience/bloom) and fineâtune them for your own tasks —
-right from your desktop computer or Google Colab: ```python from transformers
-import AutoTokenizer from petals import AutoDistributedModelForCausalLM
-model_name = "enoch/llama-65b-hf" # You can also use "meta-llama/Llama-2-70b-
-hf", "meta-llama/Llama-2-70b-chat-hf", # "bigscience/bloom", or "bigscience/
-bloomz" tokenizer = AutoTokenizer.from_pretrained(model_name) model =
+[https://img.shields.io/pypi/v/petals.svg?color=green] [https://img.shields.io/
+    discord/865254854262652969?label=discord&logo=discord&logoColor=white]
+Generate text with distributed [LLaMA 2 (70B)](https://huggingface.co/meta-
+llama/Llama-2-70b-hf), [Stable Beluga 2](https://huggingface.co/stabilityai/
+StableBeluga2), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/
+llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/
+guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and
+fineâtune them for your own tasks — right from your desktop computer or
+Google Colab: ```python from transformers import AutoTokenizer from petals
+import AutoDistributedModelForCausalLM model_name = "stabilityai/StableBeluga2"
+# You can also use "meta-llama/Llama-2-70b-hf", "meta-llama/Llama-2-70b-chat-
+hf", # repos with LLaMA-65B, "bigscience/bloom", or "bigscience/bloomz"
+tokenizer = AutoTokenizer.from_pretrained(model_name) model =
 AutoDistributedModelForCausalLM.from_pretrained(model_name) # Embeddings &
 prompts are on your device, transformer blocks are distributed across the
 Internet inputs = tokenizer("A cat sat", return_tensors="pt")["input_ids"]
 outputs = model.generate(inputs, max_new_tokens=5) print(tokenizer.decode
 (outputs[0])) # A cat sat on a mat... ```
                             ð  Try_now_in_Colab
 ð¦ **Want to run LLaMA 2?** Request access to its weights at the â¾ï¸ [Meta
 AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/
 ) and ð¤ [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), then
 run `huggingface-cli login` in the terminal before loading the model. Or just
 try it in our [chatbot app](https://chat.petals.dev). ð **Terms of use.**
-Make sure you follow the model license (see the ones for [LLaMA 2](https://
-bit.ly/llama2-license), [LLaMA](https://bit.ly/llama-license) and [BLOOM]
+Make sure you follow the model license (see [LLaMA 2](https://bit.ly/llama2-
+license), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2/
+blob/main/LICENSE.txt), [LLaMA](https://bit.ly/llama-license), and [BLOOM]
 (https://bit.ly/bloom-license)). ð **Privacy.** Your data will be processed
 by other people in the public swarm. Learn more about privacy [here](https://
 github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
 For sensitive data, you can set up a [private swarm](https://github.com/
 bigscience-workshop/petals/wiki/Launch-your-own-swarm) among people you trust.
-### Connect your GPU and increase Petals capacity Petals is a community-run
-system — we rely on people sharing their GPUs. You can check out available
-servers on our [swarm monitor](https://health.petals.dev) and connect your GPU
-to help serving one of the models! ð **Linux + Anaconda.** Run these
-commands: ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
-pip install git+https://github.com/bigscience-workshop/petals python -
-m petals.cli.run_server enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
-``` ðª **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/
+ð¬ **Any questions?** Ping us in [our Discord](https://discord.gg/
+J29mCBNBvm)! ### Connect your GPU and increase Petals capacity Petals is a
+community-run system — we rely on people sharing their GPUs. You can check out
+available servers on our [swarm monitor](https://health.petals.dev) and connect
+your GPU to help serving one of the models! ð **Linux + Anaconda.** Run
+these commands: ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -
+c nvidia pip install git+https://github.com/bigscience-workshop/petals python -
+m petals.cli.run_server stabilityai/StableBeluga2 --torch_dtype float16 ```
+ðª **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/
 bigscience-workshop/petals/wiki/Run-Petals-server-on-Windows). ð **Any OS +
 Docker.** Run our [Docker](https://www.docker.com) image: ```bash sudo docker
 run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm
 learningathome/petals:main \ python -m petals.cli.run_server --port 31330
-enoch/llama-65b-hf --adapters timdettmers/guanaco-65b ``` These commands host a
-part of LLaMA-65B with optional [Guanaco](https://huggingface.co/timdettmers/
-guanaco-65b) adapters on your machine. You can also host `meta-llama/Llama-2-
-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, `bigscience/bloom`, `bigscience/
-bloomz`, and other compatible models from ð¤ [Model Hub](https://
-huggingface.co/models), or [add support](https://github.com/bigscience-
-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model
-architectures. ð¦ **Want to host LLaMA 2?** Request access to its weights at
-the â¾ï¸ [Meta AI website](https://ai.meta.com/resources/models-and-
-libraries/llama-downloads/) and ð¤ [Model Hub](https://huggingface.co/meta-
-llama/Llama-2-70b-hf), generate an ð [access token](https://huggingface.co/
-settings/tokens), then use this command for `petals.cli.run_server`: ```bash
-python -m petals.cli.run_server meta-llama/Llama-2-70b-chat-hf --token
-YOUR_TOKEN_HERE ``` ð¬ **FAQ.** Check out our [Wiki](https://github.com/
-bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-
-server) to learn how to use multple GPUs, restart the server on reboot, etc. If
-you have any issues or feedback, ping us in [our Discord](https://discord.gg/
-D9MwApKgWa)! ð **Security.** Hosting a server does not allow others to run
-custom code on your computer. Learn more [here](https://github.com/bigscience-
-workshop/petals/wiki/Security,-privacy,-and-AI-safety). ð **Thank you!**
-Once you load and host 10+ blocks, we can show your name or link on the [swarm
-monitor](https://health.petals.dev) as a way to say thanks. You can specify
-them with `--public_name YOUR_NAME`. ### Check out tutorials, examples, and
-more Basic tutorials: - Getting started: [tutorial](https://
+stabilityai/StableBeluga2 --torch_dtype float16 ``` These commands will host a
+part of [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2) on
+your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-
+2-70b-chat-hf`, repos with LLaMA-65B, `bigscience/bloom`, `bigscience/bloomz`,
+and other compatible models from ð¤ [Model Hub](https://huggingface.co/
+models), or [add support](https://github.com/bigscience-workshop/petals/wiki/
+Run-a-custom-model-with-Petals) for new model architectures. ð¦ **Want to
+host LLaMA 2?** Request access to its weights at the â¾ï¸ [Meta AI website]
+(https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and ð¤
+[Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), generate an ð
+[access token](https://huggingface.co/settings/tokens), then use this command
+for `petals.cli.run_server`: ```bash python -m petals.cli.run_server meta-
+llama/Llama-2-70b-chat-hf --token YOUR_TOKEN_HERE ``` ð¬ **FAQ.** Check out
+our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-
+asked-questions#running-a-server) to learn how to use multple GPUs, restart the
+server on reboot, etc. If you have any issues, ping us in [our Discord](https:/
+/discord.gg/D9MwApKgWa)! ð **Security.** Hosting a server does not allow
+others to run custom code on your computer. Learn more [here](https://
+github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
+ð **Thank you!** Once you load and host 10+ blocks, we can show your name or
+link on the [swarm monitor](https://health.petals.dev) as a way to say thanks.
+You can specify them with `--public_name YOUR_NAME`. ### Check out tutorials,
+examples, and more Basic tutorials: - Getting started: [tutorial](https://
 colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://
 colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/
 prompt-tuning-sst2.ipynb) - Prompt-tune BLOOM to create a personified chatbot:
 [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/
 blob/main/examples/prompt-tuning-personachat.ipynb) Useful tools and advanced
 guides: - [Chatbot web app](https://chat.petals.dev) (connects to Petals via an
-HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/
+HTTP/WebSocket endpoint): [source code](https://github.com/petals-infra/
 chat.petals.dev) - [Monitor](https://health.petals.dev) for the public swarm:
-[source code](https://github.com/borzunov/health.petals.dev) - Launch your own
-swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-
-own-swarm) - Run a custom foundation model: [guide](https://github.com/
+[source code](https://github.com/petals-infra/health.petals.dev) - Launch your
+own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-
+your-own-swarm) - Run a custom foundation model: [guide](https://github.com/
 bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) Learning more:
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/
 petals/wiki/FAQ:-Frequently-asked-questions) - In-depth system description:
 [paper](https://arxiv.org/abs/2209.01188) ## How does it work? - Petals runs
 large language models like [LLaMA](https://github.com/facebookresearch/llama/
 blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom)
 **collaboratively** â you load a small part of the model, then team up with
```

### Comparing `petals-2.0.1/setup.cfg` & `petals-2.0.1.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/__init__.py` & `petals-2.0.1.post1/src/petals/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from packaging import version
 
 from petals.client import *
 from petals.models import *
 from petals.utils import *
 from petals.utils.logging import initialize_logs as _initialize_logs
 
-__version__ = "2.0.1"
+__version__ = "2.0.1.post1"
 
 
 if not os.getenv("PETALS_IGNORE_DEPENDENCY_VERSION"):
     assert (
         version.parse("4.31.0") <= version.parse(transformers.__version__) < version.parse("5.0.0")
     ), "Please install a proper transformers version: pip install transformers>=4.31.0,<5.0.0"
```

### Comparing `petals-2.0.1/src/petals/cli/run_dht.py` & `petals-2.0.1.post1/src/petals/cli/run_dht.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/cli/run_server.py` & `petals-2.0.1.post1/src/petals/cli/run_server.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/client/from_pretrained.py` & `petals-2.0.1.post1/src/petals/client/from_pretrained.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/client/inference_session.py` & `petals-2.0.1.post1/src/petals/client/inference_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         **metadata,
     ) -> _ServerInferenceSession:
         """Create a new session for a given remote module. This code is meant to be run inside RemoteExpertWorker"""
         stub = TransformerConnectionHandler.get_stub(p2p, span.peer_id)
         inputs_queue = asyncio.Queue()
         outputs_stream = await asyncio.wait_for(
             stub.rpc_inference(cls._read_inputs_from_queue(inputs_queue)),
-            config.request_timeout,
+            config.connect_timeout,
         )
         return cls(config, span, uid, rpc_info, inputs_queue, outputs_stream, **metadata)
 
     @staticmethod
     async def _read_inputs_from_queue(queue: asyncio.Queue, input_timeout: Optional[float] = None) -> AsyncIterator:
         while True:
             next_input_message = await asyncio.wait_for(queue.get(), input_timeout)
```

### Comparing `petals-2.0.1/src/petals/client/lm_head.py` & `petals-2.0.1.post1/src/petals/client/lm_head.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/client/ptune.py` & `petals-2.0.1.post1/src/petals/client/ptune.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/client/remote_forward_backward.py` & `petals-2.0.1.post1/src/petals/client/remote_forward_backward.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,69 +9,70 @@
 from hivemind.compression.serialization import deserialize_tensor_stream, deserialize_torch_tensor
 from hivemind.p2p import StubBase
 from hivemind.p2p.p2p_daemon_bindings.control import DEFAULT_MAX_MSG_SIZE, MAX_UNARY_PAYLOAD_SIZE
 from hivemind.proto import runtime_pb2
 from hivemind.utils.asyncio import aiter_with_timeout, iter_as_aiter
 from hivemind.utils.streaming import split_for_streaming
 
+from petals.client.routing.sequence_manager import SequenceManagerConfig
 from petals.data_structures import ModuleUID, RPCInfo
 
 
 async def _forward_unary(
-    uid: str, serialized_tensors: Iterable[runtime_pb2.Tensor], stub, timeout: float, **kwargs
+    uid: str, serialized_tensors: Iterable[runtime_pb2.Tensor], stub, config: SequenceManagerConfig, **kwargs
 ) -> List[torch.Tensor]:
     outputs: runtime_pb2.ExpertResponse = await stub.rpc_forward(
         runtime_pb2.ExpertRequest(uid=uid, tensors=list(serialized_tensors), **kwargs),
-        timeout=timeout,
+        timeout=config.request_timeout,
     )
     return [deserialize_torch_tensor(t) for t in outputs.tensors]
 
 
 async def _backward_unary(
-    uid: str, serialized_tensors: Iterable[runtime_pb2.Tensor], stub, timeout: float, **kwargs
+    uid: str, serialized_tensors: Iterable[runtime_pb2.Tensor], stub, config: SequenceManagerConfig, **kwargs
 ) -> List[torch.Tensor]:
     grad_inputs: runtime_pb2.ExpertResponse = await stub.rpc_backward(
         runtime_pb2.ExpertRequest(uid=uid, tensors=list(serialized_tensors), **kwargs),
-        timeout=timeout,
+        timeout=config.request_timeout,
     )
     return [deserialize_torch_tensor(t) for t in grad_inputs.tensors]
 
 
 async def _forward_stream(
-    uid: str, serialized_tensors: Iterable[runtime_pb2.Tensor], stub, timeout: float, **kwargs
+    uid: str, serialized_tensors: Iterable[runtime_pb2.Tensor], stub, config: SequenceManagerConfig, **kwargs
 ) -> List[torch.Tensor]:
     parts = (
         runtime_pb2.ExpertRequest(uid=uid, tensors=[part], **kwargs)
         for tensor in serialized_tensors
         for part in split_for_streaming(tensor, DEFAULT_MAX_MSG_SIZE)
     )
-    outputs = await asyncio.wait_for(stub.rpc_forward_stream(iter_as_aiter(parts)), timeout)
-    outputs = aiter_with_timeout(outputs, timeout)
+    outputs = await asyncio.wait_for(stub.rpc_forward_stream(iter_as_aiter(parts)), config.connect_timeout)
+    outputs = aiter_with_timeout(outputs, config.request_timeout)
     return await deserialize_tensor_stream(msg.tensors async for msg in outputs)
 
 
 async def _backward_stream(
-    uid: str, serialized_tensors: Iterable[runtime_pb2.Tensor], stub, timeout: float, **kwargs
+    uid: str, serialized_tensors: Iterable[runtime_pb2.Tensor], stub, config: SequenceManagerConfig, **kwargs
 ) -> List[torch.Tensor]:
     parts = (
         runtime_pb2.ExpertRequest(uid=uid, tensors=[part], **kwargs)
         for tensor in serialized_tensors
         for part in split_for_streaming(tensor, DEFAULT_MAX_MSG_SIZE)
     )
-    grad_inputs = await asyncio.wait_for(stub.rpc_backward_stream(iter_as_aiter(parts)), timeout)
-    grad_inputs = aiter_with_timeout(grad_inputs, timeout)
+    grad_inputs = await asyncio.wait_for(stub.rpc_backward_stream(iter_as_aiter(parts)), config.connect_timeout)
+    grad_inputs = aiter_with_timeout(grad_inputs, config.request_timeout)
     return await deserialize_tensor_stream(msg.tensors async for msg in grad_inputs)
 
 
 async def run_remote_forward(
     uid: ModuleUID,
     stub: StubBase,
     rpc_info: RPCInfo,
     *inputs: torch.Tensor,
-    timeout: float,
+    config: SequenceManagerConfig,
     metadata: Optional[bytes] = None,
     **kwargs,
 ) -> Tuple[torch.Tensor, ...]:
     """
     Serializes input tensors and calls "rpc_forward" on a remote server.
     Mostly adapted from https://github.com/learning-at-home/hivemind/blob/7a7c93aefffc9494c39e7b170c07cb06d8c09c4c/hivemind/moe/client/expert.py#L198
     but without RemoteExpertWorker.run_coroutine() call that leads to deadlock here.
@@ -106,26 +107,26 @@
         )
     )
 
     # call RPC on remote server
     size = sum(t.element_size() * t.nelement() for t in inputs)
     forward_fn = _forward_stream if size > MAX_UNARY_PAYLOAD_SIZE // 2 else _forward_unary
     # Hotfix: we use "// 2" since hivemind==1.1.5 serializes bfloat16 tensors in float32, so they take 2x more space
-    deserialized_outputs = await forward_fn(uid, serialized_tensors, stub, timeout, metadata=metadata, **kwargs)
+    deserialized_outputs = await forward_fn(uid, serialized_tensors, stub, config, metadata=metadata, **kwargs)
     return nested_pack(deserialized_outputs, structure=rpc_info["outputs_schema"])
 
 
 async def run_remote_backward(
     uid: ModuleUID,
     stub: StubBase,
     rpc_info: RPCInfo,
     inputs: torch.Tensor,
     grad_outputs: List[torch.Tensor],
     *extra_tensors: torch.Tensor,
-    timeout: float,
+    config: SequenceManagerConfig,
     metadata: Optional[bytes] = None,
     **kwargs,
 ) -> Sequence[torch.Tensor]:
     """
     Serializes grad outputs and calls "rpc_backward" on a remote server.
     Mostly adapted from https://github.com/learning-at-home/hivemind/blob/7a7c93aefffc9494c39e7b170c07cb06d8c09c4c/hivemind/moe/client/expert.py#L221
     but without RemoteExpertWorker.run_coroutine() call that leads to deadlock here.
@@ -149,9 +150,9 @@
             for tensor, proto in zip(inputs_and_grad_outputs, backward_schema)
         )
     )
 
     size = sum(t.element_size() * t.nelement() for t in inputs_and_grad_outputs)
     backward_fn = _backward_stream if size > MAX_UNARY_PAYLOAD_SIZE // 2 else _backward_unary
     # Hotfix: we use "// 2" since hivemind==1.1.5 serializes bfloat16 tensors in float32, so they take 2x more space
-    deserialized_grad_inputs = await backward_fn(uid, serialized_tensors, stub, timeout, metadata=metadata, **kwargs)
+    deserialized_grad_inputs = await backward_fn(uid, serialized_tensors, stub, config, metadata=metadata, **kwargs)
     return deserialized_grad_inputs
```

### Comparing `petals-2.0.1/src/petals/client/remote_generation.py` & `petals-2.0.1.post1/src/petals/client/remote_generation.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/client/remote_sequential.py` & `petals-2.0.1.post1/src/petals/client/remote_sequential.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/client/routing/sequence_info.py` & `petals-2.0.1.post1/src/petals/client/routing/sequence_info.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/client/routing/sequence_manager.py` & `petals-2.0.1.post1/src/petals/client/routing/sequence_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     dht_prefix: Optional[str] = None  # a prefix for all dht keys that correspond to this model (default: model name)
     daemon_startup_timeout: int = 60  # timeout for the libp2p daemon connecting to initial peers
 
     show_route: Union[str, bool] = "inference"  # show chosen route through servers. one of [False, "inference", True]
     allowed_servers: Optional[Collection[Union[PeerID, str]]] = None  # if defined, send requests only to these servers
     use_server_to_server: bool = True  # Use direct server-to-server communication
 
+    connect_timeout: float = 5  # timeout for opening a connection
     request_timeout: float = 3 * 60  # timeout for forward/backward/inference requests
     update_period: float = 60  # refresh DHT information once in this many seconds
 
     max_retries: Optional[int] = None  # max number retries before the client raises an exception (default: inf)
     min_backoff: float = 1  # after a repeated failure, sleep for this many seconds times 2 ** (num_failures - 1)
     max_backoff: float = 60  # limit maximal sleep time between retries to this value
     ban_timeout: float = 15  # when a remote peer fails to respond, prevent routing to that peer for this many seconds
@@ -287,31 +288,23 @@
 
         # Here, `span` contains all blocks hosted by a server - but we won't necessarily run all of them through
         # this particular server in our path. It is difficult to estimate how many blocks we'll use at this stage,
         # so we assume that we'll use all of them (the worst case for the cache size) and get a pessimistic estimate.
         # This is okay since false positives are more costly than false negatives here.
         return cache_tokens_needed * 2 * span.length <= span.server_info.cache_tokens_left
 
-    def _make_sequence_with_max_throughput(
-        self, start_index: int, end_index: int, *, relay_penalty: float = 0.5
-    ) -> List[RemoteSpanInfo]:
+    def _make_sequence_with_max_throughput(self, start_index: int, end_index: int) -> List[RemoteSpanInfo]:
         span_sequence = []
         current_index = start_index
         while current_index < end_index:
             candidate_spans = self.state.sequence_info.spans_containing_block[current_index]
             if not candidate_spans:
                 raise MissingBlocksError(current_index)
 
-            span_weights = np.array(
-                [
-                    span.server_info.throughput * (1 if not span.server_info.using_relay else relay_penalty)
-                    for span in candidate_spans
-                ],
-                dtype=np.float64,
-            )
+            span_weights = np.array([span.server_info.throughput for span in candidate_spans], dtype=np.float64)
             chosen_span = np.random.choice(candidate_spans, p=span_weights / span_weights.sum())
 
             assert chosen_span.start <= current_index < chosen_span.end
             span_sequence.append(dataclasses.replace(chosen_span, start=current_index))
             current_index = chosen_span.end
         return span_sequence
```

### Comparing `petals-2.0.1/src/petals/client/routing/spending_policy.py` & `petals-2.0.1.post1/src/petals/client/routing/spending_policy.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/client/sequential_autograd.py` & `petals-2.0.1.post1/src/petals/client/sequential_autograd.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 span_uids = CHAIN_DELIMITER.join(sequence_manager.block_uids[span.start : span.end])
                 metadata = sequence_manager.get_request_metadata("rpc_forward", span_uids, *inputs_and_prompts)
                 (outputs,) = await run_remote_forward(
                     span_uids,
                     stub,
                     sequence_manager.rpc_info,
                     *inputs_and_prompts,
-                    timeout=sequence_manager.config.request_timeout,
+                    config=sequence_manager.config,
                     metadata=MSGPackSerializer.dumps(metadata),
                 )
 
                 assert isinstance(outputs, torch.Tensor)
                 assert outputs.shape == inputs.shape, f"Expected output {inputs.shape}, got {outputs.shape}"
 
                 # Save intermediate inputs and subsequences if the forward is already done for them
@@ -157,15 +157,15 @@
                 grad_outputs, *span_grad_prompts = await run_remote_backward(
                     span_uids,
                     stub,
                     sequence_manager.rpc_info,
                     inputs,
                     grad_outputs,
                     prompts[span.start : span.end],
-                    timeout=sequence_manager.config.request_timeout,
+                    config=sequence_manager.config,
                     metadata=MSGPackSerializer.dumps(metadata),
                 )
                 grad_outputs = [grad_outputs]
                 grad_prompts_reversed.extend(span_grad_prompts)
                 sequence_manager.on_request_success(span.peer_id)
                 break
             except Exception as e:
```

### Comparing `petals-2.0.1/src/petals/constants.py` & `petals-2.0.1.post1/src/petals/constants.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/data_structures.py` & `petals-2.0.1.post1/src/petals/data_structures.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/dht_utils.py` & `petals-2.0.1.post1/src/petals/dht_utils.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/models/bloom/__init__.py` & `petals-2.0.1.post1/src/petals/models/bloom/__init__.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/models/bloom/block.py` & `petals-2.0.1.post1/src/petals/models/bloom/block.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/models/bloom/config.py` & `petals-2.0.1.post1/src/petals/models/bloom/config.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/models/bloom/model.py` & `petals-2.0.1.post1/src/petals/models/bloom/model.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/models/llama/__init__.py` & `petals-2.0.1.post1/src/petals/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/models/llama/block.py` & `petals-2.0.1.post1/src/petals/models/llama/block.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/models/llama/config.py` & `petals-2.0.1.post1/src/petals/models/llama/config.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/models/llama/model.py` & `petals-2.0.1.post1/src/petals/models/llama/model.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/backend.py` & `petals-2.0.1.post1/src/petals/server/backend.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/block_selection.py` & `petals-2.0.1.post1/src/petals/server/block_selection.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/block_utils.py` & `petals-2.0.1.post1/src/petals/server/block_utils.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/from_pretrained.py` & `petals-2.0.1.post1/src/petals/server/from_pretrained.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/handler.py` & `petals-2.0.1.post1/src/petals/server/handler.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/memory_cache.py` & `petals-2.0.1.post1/src/petals/server/memory_cache.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/reachability.py` & `petals-2.0.1.post1/src/petals/server/reachability.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/server.py` & `petals-2.0.1.post1/src/petals/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         balance_quality: float = 0.75,
         mean_balance_check_period: float = 120,
         mean_block_selection_delay: float = 2.5,
         token: Optional[Union[str, bool]] = None,
         quant_type: Optional[QuantType] = None,
         tensor_parallel_devices: Optional[Sequence[torch.device]] = None,
         skip_reachability_check: bool = False,
-        dht_client_mode: Optional[bool] = None,
+        reachable_via_relay: Optional[bool] = None,
         use_relay: bool = True,
         use_auto_relay: bool = True,
         adapters: Sequence[str] = (),
         **kwargs,
     ):
         """Create a server with one or more bloom blocks. See run_server.py for documentation."""
 
@@ -125,28 +125,28 @@
         self.session_timeout, self.step_timeout = session_timeout, step_timeout
 
         self.module_uids = [
             f"{self.dht_prefix}{UID_DELIMITER}{block_index}"
             for block_index in range(self.block_config.num_hidden_layers)
         ]
 
-        if dht_client_mode is None:
+        if reachable_via_relay is None:
             is_reachable = check_direct_reachability(initial_peers=initial_peers, use_relay=False, **kwargs)
-            dht_client_mode = is_reachable is False  # if could not check reachability (returns None), run a full peer
-            logger.info(f"This server is accessible {'via relays' if dht_client_mode else 'directly'}")
+            reachable_via_relay = is_reachable is False  # if can't check reachability (returns None), run a full peer
+            logger.info(f"This server is accessible {'via relays' if reachable_via_relay else 'directly'}")
         self.dht = DHT(
             initial_peers=initial_peers,
             start=True,
             num_workers=self.block_config.num_hidden_layers,
             use_relay=use_relay,
             use_auto_relay=use_auto_relay,
-            client_mode=dht_client_mode,
+            client_mode=reachable_via_relay,
             **kwargs,
         )
-        self.reachability_protocol = ReachabilityProtocol.attach_to_dht(self.dht) if not dht_client_mode else None
+        self.reachability_protocol = ReachabilityProtocol.attach_to_dht(self.dht) if not reachable_via_relay else None
 
         visible_maddrs_str = [str(a) for a in self.dht.get_visible_maddrs()]
         if initial_peers == PUBLIC_INITIAL_PEERS:
             logger.info("Connecting to the public swarm")
         else:
             logger.info(f"Connecting to a private swarm, initial peers: {initial_peers}")
         logger.info(f"Running a server on {visible_maddrs_str}")
@@ -223,27 +223,28 @@
                 converted_model_name_or_path,
                 self.block_config,
                 device,
                 torch_dtype,
                 num_blocks=num_blocks,
                 quant_type=quant_type,
                 tensor_parallel_devices=self.tensor_parallel_devices,
+                reachable_via_relay=reachable_via_relay,
                 force_eval=(throughput == "eval"),
                 cache_dir=cache_dir,
             )
         else:
             throughput_info = {"throughput": throughput}
         self.server_info = ServerInfo(
             state=ServerState.JOINING,
             public_name=public_name,
             version=petals.__version__,
             adapters=tuple(adapters),
             torch_dtype=str(torch_dtype).replace("torch.", ""),
             quant_type=quant_type.name.lower(),
-            using_relay=self.dht.client_mode,
+            using_relay=reachable_via_relay,
             **throughput_info,
         )
 
         self.balance_quality = balance_quality
         self.mean_balance_check_period = mean_balance_check_period
         self.mean_block_selection_delay = mean_block_selection_delay
```

### Comparing `petals-2.0.1/src/petals/server/task_pool.py` & `petals-2.0.1.post1/src/petals/server/task_pool.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/task_prioritizer.py` & `petals-2.0.1.post1/src/petals/server/task_prioritizer.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/server/throughput.py` & `petals-2.0.1.post1/src/petals/server/throughput.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     config: PretrainedConfig,
     device: torch.device,
     dtype: Union[str, torch.dtype],
     *,
     num_blocks: int,
     quant_type: QuantType,
     tensor_parallel_devices: Sequence[torch.device],
+    reachable_via_relay: bool,
+    relay_penalty: float = 0.2,
     force_eval: bool = False,
     cache_dir: Optional[str] = None,
 ) -> Dict[str, float]:
     dtype = resolve_block_dtype(config, dtype)
 
     if cache_dir is None:
         cache_dir = DEFAULT_CACHE_DIR
@@ -90,15 +92,18 @@
     throughput_info = cache[cache_key]
 
     # Most requests start at some block hosted by a server, then use all next blocks hosted on this server.
     # Assuming the start block index is distributed uniformly, the average number of blocks used per request is
     # E[Uniform{1, 2, ..., num_blocks}] = (num_blocks + 1) / 2
     average_blocks_used = (num_blocks + 1) / 2
     throughput = throughput_info["forward_rps"] / average_blocks_used
-    throughput = min(throughput, throughput_info.get("network_rps", math.inf))
+
+    network_rps = throughput_info["network_rps"] * (relay_penalty if reachable_via_relay else 1)
+    throughput = min(throughput, network_rps)
+
     throughput_info["throughput"] = throughput
     logger.info(f"Reporting throughput: {throughput:.1f} tokens/sec for {num_blocks} blocks")
 
     return throughput_info
 
 
 def measure_throughput_info(
```

### Comparing `petals-2.0.1/src/petals/utils/asyncio.py` & `petals-2.0.1.post1/src/petals/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/utils/auto_config.py` & `petals-2.0.1.post1/src/petals/utils/auto_config.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/utils/convert_block.py` & `petals-2.0.1.post1/src/petals/utils/convert_block.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/utils/disk_cache.py` & `petals-2.0.1.post1/src/petals/utils/disk_cache.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/utils/generation_algorithms.py` & `petals-2.0.1.post1/src/petals/utils/generation_algorithms.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/utils/generation_constraints.py` & `petals-2.0.1.post1/src/petals/utils/generation_constraints.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/utils/logging.py` & `petals-2.0.1.post1/src/petals/utils/logging.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/utils/peft.py` & `petals-2.0.1.post1/src/petals/utils/peft.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals/utils/ping.py` & `petals-2.0.1.post1/src/petals/utils/ping.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,18 @@
     wait_timeout: float = 5,
 ) -> float:
     try:
         ping_request = dht_pb2.PingRequest(peer=node.protocol.node_info)
         start_time = time.perf_counter()
         await node.protocol.get_stub(peer_id).rpc_ping(ping_request, timeout=wait_timeout)
         return time.perf_counter() - start_time
-    except Exception:
+    except Exception as e:
+        if str(e) == "protocol not supported":  # Happens on servers with client-mode DHT (e.g., reachable via relays)
+            return time.perf_counter() - start_time
+
         logger.debug(f"Failed to ping {peer_id}:", exc_info=True)
         return math.inf
 
 
 async def ping_parallel(peer_ids: Sequence[hivemind.PeerID], *args, **kwargs) -> Dict[hivemind.PeerID, float]:
     rpc_infos = await asyncio.gather(*[ping(peer_id, *args, **kwargs) for peer_id in peer_ids])
     return dict(zip(peer_ids, rpc_infos))
```

### Comparing `petals-2.0.1/src/petals/utils/version.py` & `petals-2.0.1.post1/src/petals/utils/version.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/src/petals.egg-info/PKG-INFO` & `petals-2.0.1.post1/src/petals.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petals
-Version: 2.0.1
+Version: 2.0.1.post1
 Summary: Easy way to efficiently run 100B+ language models without high-end GPUs
 Home-page: https://github.com/bigscience-workshop/petals
 Author: Petals Developers
 Author-email: petals-devs@googlegroups.com
 Project-URL: Bug Tracker, https://github.com/bigscience-workshop/petals/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,27 +24,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
     <img src="https://i.imgur.com/7eR7Pan.png" width="400"><br>
     Run large language models at home, BitTorrent-style.<br>
-    Fine-tuning and inference <a href="https://github.com/bigscience-workshop/petals#benchmarks">up to 10x faster</a> than offloading<br><br>
-    <a href="https://pypi.org/project/petals/"><img src="https://img.shields.io/pypi/v/petals.svg?color=green"></a><br>
+    Fine-tuning and inference <a href="https://github.com/bigscience-workshop/petals#benchmarks">up to 10x faster</a> than offloading
+    <br><br>
+    <a href="https://pypi.org/project/petals/"><img src="https://img.shields.io/pypi/v/petals.svg?color=green"></a>
+    <a href="https://discord.gg/tfHfe8B34k"><img src="https://img.shields.io/discord/865254854262652969?label=discord&logo=discord&logoColor=white"></a>
+    <br>
 </p>
 
-Generate text with distributed [LLaMA 2](https://ai.meta.com/llama/) ([70B](https://huggingface.co/meta-llama/Llama-2-70b-hf), [70B-Chat](https://huggingface.co/meta-llama/Llama-2-70b-chat-hf)), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and fine‑tune them for your own tasks &mdash; right from your desktop computer or Google Colab:
+Generate text with distributed [LLaMA 2 (70B)](https://huggingface.co/meta-llama/Llama-2-70b-hf), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and fine‑tune them for your own tasks &mdash; right from your desktop computer or Google Colab:
 
 ```python
 from transformers import AutoTokenizer
 from petals import AutoDistributedModelForCausalLM
 
-model_name = "enoch/llama-65b-hf"
+model_name = "stabilityai/StableBeluga2"
 # You can also use "meta-llama/Llama-2-70b-hf", "meta-llama/Llama-2-70b-chat-hf",
-# "bigscience/bloom", or "bigscience/bloomz"
+# repos with LLaMA-65B, "bigscience/bloom", or "bigscience/bloomz"
 
 tokenizer = AutoTokenizer.from_pretrained(model_name)
 model = AutoDistributedModelForCausalLM.from_pretrained(model_name)
 # Embeddings & prompts are on your device, transformer blocks are distributed across the Internet
 
 inputs = tokenizer("A cat sat", return_tensors="pt")["input_ids"]
 outputs = model.generate(inputs, max_new_tokens=5)
@@ -53,48 +56,50 @@
 
 <p align="center">
     🚀 &nbsp;<b><a href="https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing">Try now in Colab</a></b>
 </p>
 
 🦙 **Want to run LLaMA 2?** Request access to its weights at the ♾️ [Meta AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and 🤗 [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), then run `huggingface-cli login` in the terminal before loading the model. Or just try it in our [chatbot app](https://chat.petals.dev).
 
-📋 **Terms of use.** Make sure you follow the model license (see the ones for [LLaMA 2](https://bit.ly/llama2-license), [LLaMA](https://bit.ly/llama-license) and [BLOOM](https://bit.ly/bloom-license)).
+📋 **Terms of use.** Make sure you follow the model license (see [LLaMA 2](https://bit.ly/llama2-license), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2/blob/main/LICENSE.txt), [LLaMA](https://bit.ly/llama-license), and [BLOOM](https://bit.ly/bloom-license)).
 
 🔏 **Privacy.** Your data will be processed by other people in the public swarm. Learn more about privacy [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety). For sensitive data, you can set up a [private swarm](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm) among people you trust.
 
+💬 **Any questions?** Ping us in [our Discord](https://discord.gg/J29mCBNBvm)!
+
 ### Connect your GPU and increase Petals capacity
 
 Petals is a community-run system &mdash; we rely on people sharing their GPUs. You can check out available servers on our [swarm monitor](https://health.petals.dev) and connect your GPU to help serving one of the models!
 
 🐍 **Linux + Anaconda.** Run these commands:
 
 ```bash
 conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
 pip install git+https://github.com/bigscience-workshop/petals
-python -m petals.cli.run_server enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
+python -m petals.cli.run_server stabilityai/StableBeluga2 --torch_dtype float16
 ```
 
 🪟 **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/bigscience-workshop/petals/wiki/Run-Petals-server-on-Windows).
 
 🐋 **Any OS + Docker.** Run our [Docker](https://www.docker.com) image:
 
 ```bash
 sudo docker run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm learningathome/petals:main \
-    python -m petals.cli.run_server --port 31330 enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
+    python -m petals.cli.run_server --port 31330 stabilityai/StableBeluga2 --torch_dtype float16
 ```
 
-These commands host a part of LLaMA-65B with optional [Guanaco](https://huggingface.co/timdettmers/guanaco-65b) adapters on your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, `bigscience/bloom`, `bigscience/bloomz`, and other compatible models from 🤗 [Model Hub](https://huggingface.co/models), or [add support](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model architectures.
+These commands will host a part of [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2) on your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, repos with LLaMA-65B, `bigscience/bloom`, `bigscience/bloomz`, and other compatible models from 🤗 [Model Hub](https://huggingface.co/models), or [add support](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model architectures.
 
 🦙 **Want to host LLaMA 2?** Request access to its weights at the ♾️ [Meta AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and 🤗 [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), generate an 🔑 [access token](https://huggingface.co/settings/tokens), then use this command for `petals.cli.run_server`:
 
 ```bash
 python -m petals.cli.run_server meta-llama/Llama-2-70b-chat-hf --token YOUR_TOKEN_HERE
 ```
 
-💬 **FAQ.** Check out our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to use multple GPUs, restart the server on reboot, etc. If you have any issues or feedback, ping us in [our Discord](https://discord.gg/D9MwApKgWa)!
+💬 **FAQ.** Check out our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-server) to learn how to use multple GPUs, restart the server on reboot, etc. If you have any issues, ping us in [our Discord](https://discord.gg/D9MwApKgWa)!
 
 🔒 **Security.** Hosting a server does not allow others to run custom code on your computer. Learn more [here](https://github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
 
 🏆 **Thank you!** Once you load and host 10+ blocks, we can show your name or link on the [swarm monitor](https://health.petals.dev) as a way to say thanks. You can specify them with `--public_name YOUR_NAME`.
 
 ### Check out tutorials, examples, and more
 
@@ -102,16 +107,16 @@
 
 - Getting started: [tutorial](https://colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-sst2.ipynb)
 - Prompt-tune BLOOM to create a personified chatbot: [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/prompt-tuning-personachat.ipynb)
 
 Useful tools and advanced guides:
 
-- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/chat.petals.dev)
-- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/borzunov/health.petals.dev)
+- [Chatbot web app](https://chat.petals.dev) (connects to Petals via an HTTP/WebSocket endpoint): [source code](https://github.com/petals-infra/chat.petals.dev)
+- [Monitor](https://health.petals.dev) for the public swarm: [source code](https://github.com/petals-infra/health.petals.dev)
 - Launch your own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-own-swarm)
 - Run a custom foundation model: [guide](https://github.com/bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals)
 
 Learning more:
 
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions)
 - In-depth system description: [paper](https://arxiv.org/abs/2209.01188)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petals Version: 2.0.1 Summary: Easy way to
+Metadata-Version: 2.1 Name: petals Version: 2.0.1.post1 Summary: Easy way to
 efficiently run 100B+ language models without high-end GPUs Home-page: https://
 github.com/bigscience-workshop/petals Author: Petals Developers Author-email:
 petals-devs@googlegroups.com Project-URL: Bug Tracker, https://github.com/
 bigscience-workshop/petals/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -14,92 +14,94 @@
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Provides-Extra: dev License-File: LICENSE
                        [https://i.imgur.com/7eR7Pan.png]
              Run large language models at home, BitTorrent-style.
           Fine-tuning and inference up_to_10x_faster than offloading
 
-            [https://img.shields.io/pypi/v/petals.svg?color=green]
-Generate text with distributed [LLaMA 2](https://ai.meta.com/llama/) ([70B]
-(https://huggingface.co/meta-llama/Llama-2-70b-hf), [70B-Chat](https://
-huggingface.co/meta-llama/Llama-2-70b-chat-hf)), [LLaMA-65B](https://
-github.com/facebookresearch/llama/blob/llama_v1/MODEL_CARD.md), [Guanaco-65B]
-(https://huggingface.co/timdettmers/guanaco-65b) or [BLOOM-176B](https://
-huggingface.co/bigscience/bloom) and fineâtune them for your own tasks —
-right from your desktop computer or Google Colab: ```python from transformers
-import AutoTokenizer from petals import AutoDistributedModelForCausalLM
-model_name = "enoch/llama-65b-hf" # You can also use "meta-llama/Llama-2-70b-
-hf", "meta-llama/Llama-2-70b-chat-hf", # "bigscience/bloom", or "bigscience/
-bloomz" tokenizer = AutoTokenizer.from_pretrained(model_name) model =
+[https://img.shields.io/pypi/v/petals.svg?color=green] [https://img.shields.io/
+    discord/865254854262652969?label=discord&logo=discord&logoColor=white]
+Generate text with distributed [LLaMA 2 (70B)](https://huggingface.co/meta-
+llama/Llama-2-70b-hf), [Stable Beluga 2](https://huggingface.co/stabilityai/
+StableBeluga2), [LLaMA-65B](https://github.com/facebookresearch/llama/blob/
+llama_v1/MODEL_CARD.md), [Guanaco-65B](https://huggingface.co/timdettmers/
+guanaco-65b) or [BLOOM-176B](https://huggingface.co/bigscience/bloom) and
+fineâtune them for your own tasks — right from your desktop computer or
+Google Colab: ```python from transformers import AutoTokenizer from petals
+import AutoDistributedModelForCausalLM model_name = "stabilityai/StableBeluga2"
+# You can also use "meta-llama/Llama-2-70b-hf", "meta-llama/Llama-2-70b-chat-
+hf", # repos with LLaMA-65B, "bigscience/bloom", or "bigscience/bloomz"
+tokenizer = AutoTokenizer.from_pretrained(model_name) model =
 AutoDistributedModelForCausalLM.from_pretrained(model_name) # Embeddings &
 prompts are on your device, transformer blocks are distributed across the
 Internet inputs = tokenizer("A cat sat", return_tensors="pt")["input_ids"]
 outputs = model.generate(inputs, max_new_tokens=5) print(tokenizer.decode
 (outputs[0])) # A cat sat on a mat... ```
                             ð  Try_now_in_Colab
 ð¦ **Want to run LLaMA 2?** Request access to its weights at the â¾ï¸ [Meta
 AI website](https://ai.meta.com/resources/models-and-libraries/llama-downloads/
 ) and ð¤ [Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), then
 run `huggingface-cli login` in the terminal before loading the model. Or just
 try it in our [chatbot app](https://chat.petals.dev). ð **Terms of use.**
-Make sure you follow the model license (see the ones for [LLaMA 2](https://
-bit.ly/llama2-license), [LLaMA](https://bit.ly/llama-license) and [BLOOM]
+Make sure you follow the model license (see [LLaMA 2](https://bit.ly/llama2-
+license), [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2/
+blob/main/LICENSE.txt), [LLaMA](https://bit.ly/llama-license), and [BLOOM]
 (https://bit.ly/bloom-license)). ð **Privacy.** Your data will be processed
 by other people in the public swarm. Learn more about privacy [here](https://
 github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
 For sensitive data, you can set up a [private swarm](https://github.com/
 bigscience-workshop/petals/wiki/Launch-your-own-swarm) among people you trust.
-### Connect your GPU and increase Petals capacity Petals is a community-run
-system — we rely on people sharing their GPUs. You can check out available
-servers on our [swarm monitor](https://health.petals.dev) and connect your GPU
-to help serving one of the models! ð **Linux + Anaconda.** Run these
-commands: ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -c nvidia
-pip install git+https://github.com/bigscience-workshop/petals python -
-m petals.cli.run_server enoch/llama-65b-hf --adapters timdettmers/guanaco-65b
-``` ðª **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/
+ð¬ **Any questions?** Ping us in [our Discord](https://discord.gg/
+J29mCBNBvm)! ### Connect your GPU and increase Petals capacity Petals is a
+community-run system — we rely on people sharing their GPUs. You can check out
+available servers on our [swarm monitor](https://health.petals.dev) and connect
+your GPU to help serving one of the models! ð **Linux + Anaconda.** Run
+these commands: ```bash conda install pytorch pytorch-cuda=11.7 -c pytorch -
+c nvidia pip install git+https://github.com/bigscience-workshop/petals python -
+m petals.cli.run_server stabilityai/StableBeluga2 --torch_dtype float16 ```
+ðª **Windows + WSL.** Follow the guide on our [Wiki](https://github.com/
 bigscience-workshop/petals/wiki/Run-Petals-server-on-Windows). ð **Any OS +
 Docker.** Run our [Docker](https://www.docker.com) image: ```bash sudo docker
 run -p 31330:31330 --ipc host --gpus all --volume petals-cache:/cache --rm
 learningathome/petals:main \ python -m petals.cli.run_server --port 31330
-enoch/llama-65b-hf --adapters timdettmers/guanaco-65b ``` These commands host a
-part of LLaMA-65B with optional [Guanaco](https://huggingface.co/timdettmers/
-guanaco-65b) adapters on your machine. You can also host `meta-llama/Llama-2-
-70b-hf`, `meta-llama/Llama-2-70b-chat-hf`, `bigscience/bloom`, `bigscience/
-bloomz`, and other compatible models from ð¤ [Model Hub](https://
-huggingface.co/models), or [add support](https://github.com/bigscience-
-workshop/petals/wiki/Run-a-custom-model-with-Petals) for new model
-architectures. ð¦ **Want to host LLaMA 2?** Request access to its weights at
-the â¾ï¸ [Meta AI website](https://ai.meta.com/resources/models-and-
-libraries/llama-downloads/) and ð¤ [Model Hub](https://huggingface.co/meta-
-llama/Llama-2-70b-hf), generate an ð [access token](https://huggingface.co/
-settings/tokens), then use this command for `petals.cli.run_server`: ```bash
-python -m petals.cli.run_server meta-llama/Llama-2-70b-chat-hf --token
-YOUR_TOKEN_HERE ``` ð¬ **FAQ.** Check out our [Wiki](https://github.com/
-bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-
-server) to learn how to use multple GPUs, restart the server on reboot, etc. If
-you have any issues or feedback, ping us in [our Discord](https://discord.gg/
-D9MwApKgWa)! ð **Security.** Hosting a server does not allow others to run
-custom code on your computer. Learn more [here](https://github.com/bigscience-
-workshop/petals/wiki/Security,-privacy,-and-AI-safety). ð **Thank you!**
-Once you load and host 10+ blocks, we can show your name or link on the [swarm
-monitor](https://health.petals.dev) as a way to say thanks. You can specify
-them with `--public_name YOUR_NAME`. ### Check out tutorials, examples, and
-more Basic tutorials: - Getting started: [tutorial](https://
+stabilityai/StableBeluga2 --torch_dtype float16 ``` These commands will host a
+part of [Stable Beluga 2](https://huggingface.co/stabilityai/StableBeluga2) on
+your machine. You can also host `meta-llama/Llama-2-70b-hf`, `meta-llama/Llama-
+2-70b-chat-hf`, repos with LLaMA-65B, `bigscience/bloom`, `bigscience/bloomz`,
+and other compatible models from ð¤ [Model Hub](https://huggingface.co/
+models), or [add support](https://github.com/bigscience-workshop/petals/wiki/
+Run-a-custom-model-with-Petals) for new model architectures. ð¦ **Want to
+host LLaMA 2?** Request access to its weights at the â¾ï¸ [Meta AI website]
+(https://ai.meta.com/resources/models-and-libraries/llama-downloads/) and ð¤
+[Model Hub](https://huggingface.co/meta-llama/Llama-2-70b-hf), generate an ð
+[access token](https://huggingface.co/settings/tokens), then use this command
+for `petals.cli.run_server`: ```bash python -m petals.cli.run_server meta-
+llama/Llama-2-70b-chat-hf --token YOUR_TOKEN_HERE ``` ð¬ **FAQ.** Check out
+our [Wiki](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-
+asked-questions#running-a-server) to learn how to use multple GPUs, restart the
+server on reboot, etc. If you have any issues, ping us in [our Discord](https:/
+/discord.gg/D9MwApKgWa)! ð **Security.** Hosting a server does not allow
+others to run custom code on your computer. Learn more [here](https://
+github.com/bigscience-workshop/petals/wiki/Security,-privacy,-and-AI-safety).
+ð **Thank you!** Once you load and host 10+ blocks, we can show your name or
+link on the [swarm monitor](https://health.petals.dev) as a way to say thanks.
+You can specify them with `--public_name YOUR_NAME`. ### Check out tutorials,
+examples, and more Basic tutorials: - Getting started: [tutorial](https://
 colab.research.google.com/drive/1uCphNY7gfAUkdDrTx21dZZwCOUDCMPw8?usp=sharing)
 - Prompt-tune LLaMA-65B for text semantic classification: [tutorial](https://
 colab.research.google.com/github/bigscience-workshop/petals/blob/main/examples/
 prompt-tuning-sst2.ipynb) - Prompt-tune BLOOM to create a personified chatbot:
 [tutorial](https://colab.research.google.com/github/bigscience-workshop/petals/
 blob/main/examples/prompt-tuning-personachat.ipynb) Useful tools and advanced
 guides: - [Chatbot web app](https://chat.petals.dev) (connects to Petals via an
-HTTP/WebSocket endpoint): [source code](https://github.com/borzunov/
+HTTP/WebSocket endpoint): [source code](https://github.com/petals-infra/
 chat.petals.dev) - [Monitor](https://health.petals.dev) for the public swarm:
-[source code](https://github.com/borzunov/health.petals.dev) - Launch your own
-swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-your-
-own-swarm) - Run a custom foundation model: [guide](https://github.com/
+[source code](https://github.com/petals-infra/health.petals.dev) - Launch your
+own swarm: [guide](https://github.com/bigscience-workshop/petals/wiki/Launch-
+your-own-swarm) - Run a custom foundation model: [guide](https://github.com/
 bigscience-workshop/petals/wiki/Run-a-custom-model-with-Petals) Learning more:
 - Frequently asked questions: [FAQ](https://github.com/bigscience-workshop/
 petals/wiki/FAQ:-Frequently-asked-questions) - In-depth system description:
 [paper](https://arxiv.org/abs/2209.01188) ## How does it work? - Petals runs
 large language models like [LLaMA](https://github.com/facebookresearch/llama/
 blob/main/MODEL_CARD.md) and [BLOOM](https://huggingface.co/bigscience/bloom)
 **collaboratively** â you load a small part of the model, then team up with
```

### Comparing `petals-2.0.1/src/petals.egg-info/SOURCES.txt` & `petals-2.0.1.post1/src/petals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_aux_functions.py` & `petals-2.0.1.post1/tests/test_aux_functions.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_block_exact_match.py` & `petals-2.0.1.post1/tests/test_block_exact_match.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_chained_calls.py` & `petals-2.0.1.post1/tests/test_chained_calls.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_dtype.py` & `petals-2.0.1.post1/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_full_model.py` & `petals-2.0.1.post1/tests/test_full_model.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_peft.py` & `petals-2.0.1.post1/tests/test_peft.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_priority_pool.py` & `petals-2.0.1.post1/tests/test_priority_pool.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_remote_sequential.py` & `petals-2.0.1.post1/tests/test_remote_sequential.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_sequence_manager.py` & `petals-2.0.1.post1/tests/test_sequence_manager.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_server_stats.py` & `petals-2.0.1.post1/tests/test_server_stats.py`

 * *Files identical despite different names*

### Comparing `petals-2.0.1/tests/test_tensor_parallel.py` & `petals-2.0.1.post1/tests/test_tensor_parallel.py`

 * *Files identical despite different names*

