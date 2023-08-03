# Comparing `tmp/vllm-0.1.2.tar.gz` & `tmp/vllm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm-0.1.2.tar", last modified: Wed Jul  5 04:52:32 2023, max compression
+gzip compressed data, was "vllm-0.1.3.tar", last modified: Wed Aug  2 23:57:25 2023, max compression
```

## Comparing `vllm-0.1.2.tar` & `vllm-0.1.3.tar`

### file list

```diff
@@ -1,103 +1,108 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.593359 vllm-0.1.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-05-19 19:30:16.000000 vllm-0.1.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-06-06 03:07:23.000000 vllm-0.1.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5512 2023-07-05 04:52:32.590359 vllm-0.1.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4794 2023-07-05 04:42:28.000000 vllm-0.1.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.035305 vllm-0.1.2/csrc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-04-02 07:37:46.000000 vllm-0.1.2/csrc/activation.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/activation_kernels.cu
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.104312 vllm-0.1.2/csrc/attention/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      135 2023-06-03 11:19:52.000000 vllm-0.1.2/csrc/attention/attention_dtypes.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1721 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/attention_generic.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20688 2023-07-05 04:42:28.000000 vllm-0.1.2/csrc/attention/attention_kernels.cu
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1850 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/attention_utils.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10962 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/dtype_bfloat16.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10793 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/dtype_float16.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5559 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/dtype_float32.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      595 2023-07-03 20:41:37.000000 vllm-0.1.2/csrc/attention.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-05-19 19:30:17.000000 vllm-0.1.2/csrc/cache.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14699 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/cache_kernels.cu
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2023-03-31 16:51:49.000000 vllm-0.1.2/csrc/layernorm.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/layernorm_kernels.cu
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-05-19 19:30:17.000000 vllm-0.1.2/csrc/pos_encoding.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2901 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/pos_encoding_kernels.cu
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1592 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/reduction_utils.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      153 2023-06-06 03:07:24.000000 vllm-0.1.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-07-05 04:42:28.000000 vllm-0.1.2/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-05 04:52:32.594359 vllm-0.1.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6038 2023-06-29 15:14:11.000000 vllm-0.1.2/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.173318 vllm-0.1.2/vllm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1852 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/block.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9369 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.239325 vllm-0.1.2/vllm/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/core/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10443 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/core/block_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      896 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/core/policy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18979 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/core/scheduler.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.276328 vllm-0.1.2/vllm/engine/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/engine/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8079 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/engine/arg_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9653 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/engine/async_llm_engine.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14359 2023-07-03 21:53:08.000000 vllm-0.1.2/vllm/engine/llm_engine.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/engine/ray_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.298330 vllm-0.1.2/vllm/entrypoints/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/entrypoints/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2983 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/entrypoints/api_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6279 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/entrypoints/llm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.320332 vllm-0.1.2/vllm/entrypoints/openai/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/entrypoints/openai/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22383 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/entrypoints/openai/api_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5299 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/entrypoints/openai/protocol.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1615 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.360336 vllm-0.1.2/vllm/model_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      246 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2618 2023-07-03 20:41:37.000000 vllm-0.1.2/vllm/model_executor/input_metadata.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.399340 vllm-0.1.2/vllm/model_executor/layers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/model_executor/layers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1164 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/layers/activation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15036 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/model_executor/layers/attention.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      773 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/model_executor/layers/layernorm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16825 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/layers/sampler.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1965 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/model_executor/model_loader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.465346 vllm-0.1.2/vllm/model_executor/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/model_executor/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12489 2023-07-03 21:53:08.000000 vllm-0.1.2/vllm/model_executor/models/bloom.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12944 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/models/gpt2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14532 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/models/gpt_bigcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11460 2023-07-03 20:41:37.000000 vllm-0.1.2/vllm/model_executor/models/gpt_neox.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12189 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/models/llama.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/model_executor/models/mpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13635 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/models/opt.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.481348 vllm-0.1.2/vllm/model_executor/parallel_utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22861 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/parallel_state.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.522352 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18207 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/layers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8586 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/random.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2460 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4472 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/weight_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4139 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/outputs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6702 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/sampling_params.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9648 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/sequence.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.543354 vllm-0.1.2/vllm/transformers_utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 15:14:11.000000 vllm-0.1.2/vllm/transformers_utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      479 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/transformers_utils/config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.558355 vllm-0.1.2/vllm/transformers_utils/configs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/transformers_utils/configs/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2261 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/transformers_utils/configs/mpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3907 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/transformers_utils/tokenizer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      893 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.580358 vllm-0.1.2/vllm/worker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/worker/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5980 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/worker/cache_engine.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12438 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/worker/worker.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.209322 vllm-0.1.2/vllm.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5512 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2561 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      120 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/top_level.txt
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.164969 vllm-0.1.3/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    11357 2023-08-02 23:22:26.000000 vllm-0.1.3/LICENSE
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)       67 2023-08-02 23:22:26.000000 vllm-0.1.3/MANIFEST.in
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     5883 2023-08-02 23:57:25.164969 vllm-0.1.3/PKG-INFO
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     5165 2023-08-02 23:47:36.000000 vllm-0.1.3/README.md
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.152968 vllm-0.1.3/csrc/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      234 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/activation.cpp
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1359 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/activation_kernels.cu
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.156968 vllm-0.1.3/csrc/attention/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      135 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/attention/attention_dtypes.h
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1721 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/attention/attention_generic.cuh
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    21396 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/attention/attention_kernels.cu
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1850 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/attention/attention_utils.cuh
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    10962 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/attention/dtype_bfloat16.cuh
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    10793 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/attention/dtype_float16.cuh
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     5559 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/attention/dtype_float32.cuh
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      626 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/attention.cpp
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1151 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/cache.cpp
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    14699 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/cache_kernels.cu
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      292 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/layernorm.cpp
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1904 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/layernorm_kernels.cu
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      357 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/pos_encoding.cpp
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     3687 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/pos_encoding_kernels.cu
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1592 2023-08-02 23:22:26.000000 vllm-0.1.3/csrc/reduction_utils.cuh
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      153 2023-08-02 23:22:26.000000 vllm-0.1.3/pyproject.toml
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      243 2023-08-02 23:22:26.000000 vllm-0.1.3/requirements.txt
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)       38 2023-08-02 23:57:25.164969 vllm-0.1.3/setup.cfg
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     6038 2023-08-02 23:22:26.000000 vllm-0.1.3/setup.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.156968 vllm-0.1.3/vllm/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      658 2023-08-02 23:47:36.000000 vllm-0.1.3/vllm/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1852 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/block.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    11090 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/config.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.156968 vllm-0.1.3/vllm/core/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/core/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    10443 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/core/block_manager.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      896 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/core/policy.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    17313 2023-08-02 23:42:52.000000 vllm-0.1.3/vllm/core/scheduler.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.156968 vllm-0.1.3/vllm/engine/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/engine/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     8210 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/engine/arg_utils.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     9669 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/engine/async_llm_engine.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    20274 2023-08-02 23:42:52.000000 vllm-0.1.3/vllm/engine/llm_engine.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     4134 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/engine/ray_utils.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.156968 vllm-0.1.3/vllm/entrypoints/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/entrypoints/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     2981 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/entrypoints/api_server.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     6714 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/entrypoints/llm.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.156968 vllm-0.1.3/vllm/entrypoints/openai/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/entrypoints/openai/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    22653 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/entrypoints/openai/api_server.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     5299 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/entrypoints/openai/protocol.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1615 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/logger.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.160969 vllm-0.1.3/vllm/model_executor/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      246 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     2618 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/input_metadata.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.160969 vllm-0.1.3/vllm/model_executor/layers/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/layers/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1164 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/layers/activation.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    17209 2023-08-02 23:42:52.000000 vllm-0.1.3/vllm/model_executor/layers/attention.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      773 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/layers/layernorm.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    16956 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/layers/sampler.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     2216 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/model_loader.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.160969 vllm-0.1.3/vllm/model_executor/models/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      992 2023-08-02 23:47:36.000000 vllm-0.1.3/vllm/model_executor/models/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    14835 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/baichuan.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    12839 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/bloom.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    20636 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/falcon.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    12944 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/gpt2.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    14990 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/gpt_bigcode.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    10162 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/gpt_j.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    11460 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/gpt_neox.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    13670 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/llama.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    11099 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/mpt.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    13635 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/models/opt.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.160969 vllm-0.1.3/vllm/model_executor/parallel_utils/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      175 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/parallel_utils/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    20617 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/parallel_utils/parallel_state.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.160969 vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1463 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    18239 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/layers.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     8586 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     6056 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/random.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     2460 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/utils.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      546 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/utils.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     4546 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/model_executor/weight_utils.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     4139 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/outputs.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     6702 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/sampling_params.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     9729 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/sequence.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.160969 vllm-0.1.3/vllm/transformers_utils/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/transformers_utils/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     1255 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/transformers_utils/config.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.160969 vllm-0.1.3/vllm/transformers_utils/configs/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      466 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/transformers_utils/configs/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     2266 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/transformers_utils/configs/baichuan.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     2878 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/transformers_utils/configs/falcon.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     2261 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/transformers_utils/configs/mpt.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     4874 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/transformers_utils/tokenizer.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      893 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/utils.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.164969 vllm-0.1.3/vllm/worker/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/worker/__init__.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     5980 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/worker/cache_engine.py
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)    13499 2023-08-02 23:22:26.000000 vllm-0.1.3/vllm/worker/worker.py
+drwxr-xr-x   0 gcpuser   (1008) gcpuser   (1009)        0 2023-08-02 23:57:25.156968 vllm-0.1.3/vllm.egg-info/
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     5883 2023-08-02 23:57:25.000000 vllm-0.1.3/vllm.egg-info/PKG-INFO
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)     2759 2023-08-02 23:57:25.000000 vllm-0.1.3/vllm.egg-info/SOURCES.txt
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        1 2023-08-02 23:57:25.000000 vllm-0.1.3/vllm.egg-info/dependency_links.txt
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)      122 2023-08-02 23:57:25.000000 vllm-0.1.3/vllm.egg-info/requires.txt
+-rw-r--r--   0 gcpuser   (1008) gcpuser   (1009)        5 2023-08-02 23:57:25.000000 vllm-0.1.3/vllm.egg-info/top_level.txt
```

### Comparing `vllm-0.1.2/LICENSE` & `vllm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/PKG-INFO` & `vllm-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vllm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A high-throughput and memory-efficient inference and serving engine for LLMs
 Home-page: https://github.com/vllm-project/vllm
 Author: vLLM Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/vllm-project/vllm
 Project-URL: Documentation, https://vllm.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
@@ -31,14 +31,15 @@
 | <a href="https://vllm.readthedocs.io/en/latest/"><b>Documentation</b></a> | <a href="https://vllm.ai"><b>Blog</b></a> | <a href="https://github.com/vllm-project/vllm/discussions"><b>Discussions</b></a> |
 
 </p>
 
 ---
 
 *Latest News* 🔥
+- [2023/07] Added support for LLaMA-2! You can run and serve 7B/13B/70B LLaMA-2s on vLLM with a single command!
 - [2023/06] Serving vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo, and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the clouds.
 - [2023/06] We officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog post](https://vllm.ai).
 
 ---
 
 vLLM is a fast and easy-to-use library for LLM inference and serving.
 
@@ -55,19 +56,22 @@
 - High-throughput serving with various decoding algorithms, including *parallel sampling*, *beam search*, and more
 - Tensor parallelism support for distributed inference
 - Streaming outputs
 - OpenAI-compatible API server
 
 vLLM seamlessly supports many Huggingface models, including the following architectures:
 
+- Baichuan (`baichuan-inc/Baichuan-7B`, `baichuan-inc/Baichuan-13B-Chat`, etc.)
 - BLOOM (`bigscience/bloom`, `bigscience/bloomz`, etc.)
+- Falcon (`tiiuae/falcon-7b`, `tiiuae/falcon-40b`, `tiiuae/falcon-rw-7b`, etc.)
 - GPT-2 (`gpt2`, `gpt2-xl`, etc.)
 - GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.)
+- GPT-J (`EleutherAI/gpt-j-6b`, `nomic-ai/gpt4all-j`, etc.)
 - GPT-NeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
-- LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
+- LLaMA & LLaMA-2 (`meta-llama/Llama-2-70b-hf`, `lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
 - MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.)
 - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
 
 Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-source):
 
 ```bash
 pip install vllm
```

#### html2text {}

```diff
@@ -1,53 +1,58 @@
-Metadata-Version: 2.1 Name: vllm Version: 0.1.2 Summary: A high-throughput and
+Metadata-Version: 2.1 Name: vllm Version: 0.1.3 Summary: A high-throughput and
 memory-efficient inference and serving engine for LLMs Home-page: https://
 github.com/vllm-project/vllm Author: vLLM Team License: Apache 2.0 Project-URL:
 Homepage, https://github.com/vllm-project/vllm Project-URL: Documentation,
 https://vllm.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE
                                      [vLLM]
            **** Easy, fast, and cheap LLM serving for everyone ****
                     | Documentation | Blog | Discussions |
---- *Latest News* ð¥ - [2023/06] Serving vLLM On any Cloud with SkyPilot.
-Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/
-master/llm/vllm) to start the vLLM demo, and the [blog post](https://
-blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/
-) for the story behind vLLM development on the clouds. - [2023/06] We
-officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna
-and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog
-post](https://vllm.ai). --- vLLM is a fast and easy-to-use library for LLM
-inference and serving. vLLM is fast with: - State-of-the-art serving throughput
-- Efficient management of attention key and value memory with
-**PagedAttention** - Continuous batching of incoming requests - Optimized CUDA
-kernels vLLM is flexible and easy to use with: - Seamless integration with
-popular HuggingFace models - High-throughput serving with various decoding
-algorithms, including *parallel sampling*, *beam search*, and more - Tensor
-parallelism support for distributed inference - Streaming outputs - OpenAI-
-compatible API server vLLM seamlessly supports many Huggingface models,
-including the following architectures: - BLOOM (`bigscience/bloom`,
-`bigscience/bloomz`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) - GPT BigCode
-(`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) - GPT-NeoX
+--- *Latest News* ð¥ - [2023/07] Added support for LLaMA-2! You can run and
+serve 7B/13B/70B LLaMA-2s on vLLM with a single command! - [2023/06] Serving
+vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://
+github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo,
+and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-
+cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the
+clouds. - [2023/06] We officially released vLLM! FastChat-vLLM integration has
+powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-
+April. Check out our [blog post](https://vllm.ai). --- vLLM is a fast and easy-
+to-use library for LLM inference and serving. vLLM is fast with: - State-of-
+the-art serving throughput - Efficient management of attention key and value
+memory with **PagedAttention** - Continuous batching of incoming requests -
+Optimized CUDA kernels vLLM is flexible and easy to use with: - Seamless
+integration with popular HuggingFace models - High-throughput serving with
+various decoding algorithms, including *parallel sampling*, *beam search*, and
+more - Tensor parallelism support for distributed inference - Streaming outputs
+- OpenAI-compatible API server vLLM seamlessly supports many Huggingface
+models, including the following architectures: - Baichuan (`baichuan-inc/
+Baichuan-7B`, `baichuan-inc/Baichuan-13B-Chat`, etc.) - BLOOM (`bigscience/
+bloom`, `bigscience/bloomz`, etc.) - Falcon (`tiiuae/falcon-7b`, `tiiuae/
+falcon-40b`, `tiiuae/falcon-rw-7b`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) -
+GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) -
+GPT-J (`EleutherAI/gpt-j-6b`, `nomic-ai/gpt4all-j`, etc.) - GPT-NeoX
 (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-
-tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`,
-`openlm-research/open_llama_13b`, etc.) - MPT (`mosaicml/mpt-7b`, `mosaicml/
-mpt-30b`, etc.) - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
-Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/
-getting_started/installation.html#build-from-source): ```bash pip install vllm
-``` ## Getting Started Visit our [documentation](https://vllm.readthedocs.io/
-en/latest/) to get started. - [Installation](https://vllm.readthedocs.io/en/
-latest/getting_started/installation.html) - [Quickstart](https://
-vllm.readthedocs.io/en/latest/getting_started/quickstart.html) - [Supported
-Models](https://vllm.readthedocs.io/en/latest/models/supported_models.html) ##
-Performance vLLM outperforms HuggingFace Transformers (HF) by up to 24x and
-Text Generation Inference (TGI) by up to 3.5x, in terms of throughput. For
-details, check out our [blog post](https://vllm.ai).
+tuned-alpha-7b`, etc.) - LLaMA & LLaMA-2 (`meta-llama/Llama-2-70b-hf`, `lmsys/
+vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.) -
+MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.) - OPT (`facebook/opt-66b`,
+`facebook/opt-iml-max-30b`, etc.) Install vLLM with pip or [from source](https:
+//vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-
+source): ```bash pip install vllm ``` ## Getting Started Visit our
+[documentation](https://vllm.readthedocs.io/en/latest/) to get started. -
+[Installation](https://vllm.readthedocs.io/en/latest/getting_started/
+installation.html) - [Quickstart](https://vllm.readthedocs.io/en/latest/
+getting_started/quickstart.html) - [Supported Models](https://
+vllm.readthedocs.io/en/latest/models/supported_models.html) ## Performance vLLM
+outperforms HuggingFace Transformers (HF) by up to 24x and Text Generation
+Inference (TGI) by up to 3.5x, in terms of throughput. For details, check out
+our [blog post](https://vllm.ai).
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n1_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n1_light.png]
       Serving throughput when each request asks for 1 output completion.
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n3_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n3_light.png]
```

### Comparing `vllm-0.1.2/README.md` & `vllm-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 | <a href="https://vllm.readthedocs.io/en/latest/"><b>Documentation</b></a> | <a href="https://vllm.ai"><b>Blog</b></a> | <a href="https://github.com/vllm-project/vllm/discussions"><b>Discussions</b></a> |
 
 </p>
 
 ---
 
 *Latest News* 🔥
+- [2023/07] Added support for LLaMA-2! You can run and serve 7B/13B/70B LLaMA-2s on vLLM with a single command!
 - [2023/06] Serving vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo, and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the clouds.
 - [2023/06] We officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog post](https://vllm.ai).
 
 ---
 
 vLLM is a fast and easy-to-use library for LLM inference and serving.
 
@@ -37,19 +38,22 @@
 - High-throughput serving with various decoding algorithms, including *parallel sampling*, *beam search*, and more
 - Tensor parallelism support for distributed inference
 - Streaming outputs
 - OpenAI-compatible API server
 
 vLLM seamlessly supports many Huggingface models, including the following architectures:
 
+- Baichuan (`baichuan-inc/Baichuan-7B`, `baichuan-inc/Baichuan-13B-Chat`, etc.)
 - BLOOM (`bigscience/bloom`, `bigscience/bloomz`, etc.)
+- Falcon (`tiiuae/falcon-7b`, `tiiuae/falcon-40b`, `tiiuae/falcon-rw-7b`, etc.)
 - GPT-2 (`gpt2`, `gpt2-xl`, etc.)
 - GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.)
+- GPT-J (`EleutherAI/gpt-j-6b`, `nomic-ai/gpt4all-j`, etc.)
 - GPT-NeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
-- LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
+- LLaMA & LLaMA-2 (`meta-llama/Llama-2-70b-hf`, `lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
 - MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.)
 - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
 
 Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-source):
 
 ```bash
 pip install vllm
```

#### html2text {}

```diff
@@ -1,43 +1,48 @@
                                      [vLLM]
            **** Easy, fast, and cheap LLM serving for everyone ****
                     | Documentation | Blog | Discussions |
---- *Latest News* ð¥ - [2023/06] Serving vLLM On any Cloud with SkyPilot.
-Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/
-master/llm/vllm) to start the vLLM demo, and the [blog post](https://
-blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/
-) for the story behind vLLM development on the clouds. - [2023/06] We
-officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna
-and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog
-post](https://vllm.ai). --- vLLM is a fast and easy-to-use library for LLM
-inference and serving. vLLM is fast with: - State-of-the-art serving throughput
-- Efficient management of attention key and value memory with
-**PagedAttention** - Continuous batching of incoming requests - Optimized CUDA
-kernels vLLM is flexible and easy to use with: - Seamless integration with
-popular HuggingFace models - High-throughput serving with various decoding
-algorithms, including *parallel sampling*, *beam search*, and more - Tensor
-parallelism support for distributed inference - Streaming outputs - OpenAI-
-compatible API server vLLM seamlessly supports many Huggingface models,
-including the following architectures: - BLOOM (`bigscience/bloom`,
-`bigscience/bloomz`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) - GPT BigCode
-(`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) - GPT-NeoX
+--- *Latest News* ð¥ - [2023/07] Added support for LLaMA-2! You can run and
+serve 7B/13B/70B LLaMA-2s on vLLM with a single command! - [2023/06] Serving
+vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://
+github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo,
+and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-
+cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the
+clouds. - [2023/06] We officially released vLLM! FastChat-vLLM integration has
+powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-
+April. Check out our [blog post](https://vllm.ai). --- vLLM is a fast and easy-
+to-use library for LLM inference and serving. vLLM is fast with: - State-of-
+the-art serving throughput - Efficient management of attention key and value
+memory with **PagedAttention** - Continuous batching of incoming requests -
+Optimized CUDA kernels vLLM is flexible and easy to use with: - Seamless
+integration with popular HuggingFace models - High-throughput serving with
+various decoding algorithms, including *parallel sampling*, *beam search*, and
+more - Tensor parallelism support for distributed inference - Streaming outputs
+- OpenAI-compatible API server vLLM seamlessly supports many Huggingface
+models, including the following architectures: - Baichuan (`baichuan-inc/
+Baichuan-7B`, `baichuan-inc/Baichuan-13B-Chat`, etc.) - BLOOM (`bigscience/
+bloom`, `bigscience/bloomz`, etc.) - Falcon (`tiiuae/falcon-7b`, `tiiuae/
+falcon-40b`, `tiiuae/falcon-rw-7b`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) -
+GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) -
+GPT-J (`EleutherAI/gpt-j-6b`, `nomic-ai/gpt4all-j`, etc.) - GPT-NeoX
 (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-
-tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`,
-`openlm-research/open_llama_13b`, etc.) - MPT (`mosaicml/mpt-7b`, `mosaicml/
-mpt-30b`, etc.) - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
-Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/
-getting_started/installation.html#build-from-source): ```bash pip install vllm
-``` ## Getting Started Visit our [documentation](https://vllm.readthedocs.io/
-en/latest/) to get started. - [Installation](https://vllm.readthedocs.io/en/
-latest/getting_started/installation.html) - [Quickstart](https://
-vllm.readthedocs.io/en/latest/getting_started/quickstart.html) - [Supported
-Models](https://vllm.readthedocs.io/en/latest/models/supported_models.html) ##
-Performance vLLM outperforms HuggingFace Transformers (HF) by up to 24x and
-Text Generation Inference (TGI) by up to 3.5x, in terms of throughput. For
-details, check out our [blog post](https://vllm.ai).
+tuned-alpha-7b`, etc.) - LLaMA & LLaMA-2 (`meta-llama/Llama-2-70b-hf`, `lmsys/
+vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.) -
+MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.) - OPT (`facebook/opt-66b`,
+`facebook/opt-iml-max-30b`, etc.) Install vLLM with pip or [from source](https:
+//vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-
+source): ```bash pip install vllm ``` ## Getting Started Visit our
+[documentation](https://vllm.readthedocs.io/en/latest/) to get started. -
+[Installation](https://vllm.readthedocs.io/en/latest/getting_started/
+installation.html) - [Quickstart](https://vllm.readthedocs.io/en/latest/
+getting_started/quickstart.html) - [Supported Models](https://
+vllm.readthedocs.io/en/latest/models/supported_models.html) ## Performance vLLM
+outperforms HuggingFace Transformers (HF) by up to 24x and Text Generation
+Inference (TGI) by up to 3.5x, in terms of throughput. For details, check out
+our [blog post](https://vllm.ai).
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n1_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n1_light.png]
       Serving throughput when each request asks for 1 output completion.
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n3_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n3_light.png]
```

### Comparing `vllm-0.1.2/csrc/activation_kernels.cu` & `vllm-0.1.3/csrc/activation_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/attention/attention_generic.cuh` & `vllm-0.1.3/csrc/attention/attention_generic.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/attention/attention_kernels.cu` & `vllm-0.1.3/csrc/attention/attention_kernels.cu`

 * *Files 6% similar despite different names*

```diff
@@ -70,31 +70,35 @@
   typename scalar_t,
   int HEAD_SIZE,
   int BLOCK_SIZE,
   int NUM_THREADS>
 __global__ void single_query_cached_kv_attention_kernel(
   scalar_t* __restrict__ out,             // [num_seqs, num_heads, head_size]
   const scalar_t* __restrict__ q,         // [num_seqs, num_heads, head_size]
-  const scalar_t* __restrict__ k_cache,   // [num_blocks, num_heads, head_size/x, block_size, x]
-  const scalar_t* __restrict__ v_cache,   // [num_blocks, num_heads, head_size, block_size]
+  const scalar_t* __restrict__ k_cache,   // [num_blocks, num_kv_heads, head_size/x, block_size, x]
+  const scalar_t* __restrict__ v_cache,   // [num_blocks, num_kv_heads, head_size, block_size]
+  const int* __restrict__ head_mapping,   // [num_heads]
   const float scale,
   const int* __restrict__ block_tables,   // [num_seqs, max_num_blocks_per_seq]
   const int* __restrict__ context_lens,   // [num_seqs]
   const int max_num_blocks_per_seq,
   const float* __restrict__ alibi_slopes, // [num_heads]
-  const int q_stride) {
+  const int q_stride,
+  const int kv_block_stride,
+  const int kv_head_stride) {
   constexpr int THREAD_GROUP_SIZE = MAX(WARP_SIZE / BLOCK_SIZE, 1);
   constexpr int NUM_TOKENS_PER_THREAD_GROUP = (BLOCK_SIZE + WARP_SIZE - 1) / WARP_SIZE;
   constexpr int NUM_WARPS = NUM_THREADS / WARP_SIZE;
   const int thread_idx = threadIdx.x;
   const int warp_idx = thread_idx / WARP_SIZE;
   const int lane = thread_idx % WARP_SIZE;
 
   const int head_idx = blockIdx.x;
   const int num_heads = gridDim.x;
+  const int kv_head_idx = head_mapping[head_idx];
   const int seq_idx = blockIdx.y;
   const float alibi_slope = alibi_slopes == nullptr ? 0.f : alibi_slopes[head_idx];
 
   // A vector type to store a part of a key or a query.
   // The vector size is configured in such a way that the threads in a thread group
   // fetch or compute 16 bytes at a time.
   // For example, if the size of a thread group is 4 and the data type is half,
@@ -154,16 +158,16 @@
     for (int i = 0; i < NUM_TOKENS_PER_THREAD_GROUP; i++) {
       const int physical_block_offset = (thread_group_idx + i * WARP_SIZE) % BLOCK_SIZE;
       const int token_idx = block_idx * BLOCK_SIZE + physical_block_offset;
       K_vec k_vecs[NUM_VECS_PER_THREAD];
 
 #pragma unroll
       for (int j = 0; j < NUM_VECS_PER_THREAD; j++) {
-        const scalar_t* k_ptr = k_cache + physical_block_number * num_heads * HEAD_SIZE * BLOCK_SIZE
-                                        + head_idx * HEAD_SIZE * BLOCK_SIZE
+        const scalar_t* k_ptr = k_cache + physical_block_number * kv_block_stride
+                                        + kv_head_idx * kv_head_stride
                                         + physical_block_offset * x;
         const int vec_idx = thread_group_offset + j * THREAD_GROUP_SIZE;
         const int offset1 = (vec_idx * VEC_SIZE) / x;
         const int offset2 = (vec_idx * VEC_SIZE) % x;
         k_vecs[j] = *reinterpret_cast<const K_vec*>(k_ptr + offset1 * BLOCK_SIZE * x + offset2);
       }
 
@@ -242,16 +246,16 @@
   for (int block_idx = warp_idx; block_idx < num_blocks; block_idx += NUM_WARPS) {
     const int physical_block_number = block_table[block_idx];
     const int physical_block_offset = (lane % NUM_V_VECS_PER_ROW) * V_VEC_SIZE;
     const int token_idx = block_idx * BLOCK_SIZE + physical_block_offset;
     L_vec logits_vec;
     from_float(logits_vec, *reinterpret_cast<Float_L_vec*>(logits + token_idx));
 
-    const scalar_t* v_ptr = v_cache + physical_block_number * num_heads * HEAD_SIZE * BLOCK_SIZE
-                                    + head_idx * HEAD_SIZE * BLOCK_SIZE;
+    const scalar_t* v_ptr = v_cache + physical_block_number * kv_block_stride
+                                    + kv_head_idx * kv_head_stride;
 #pragma unroll
     for (int i = 0; i < NUM_ROWS_PER_THREAD; i++) {
       const int row_idx = lane / NUM_V_VECS_PER_ROW + i * NUM_ROWS_PER_ITER;
       if (row_idx < HEAD_SIZE) {
         const int offset = row_idx * BLOCK_SIZE + physical_block_offset;
         V_vec v_vec = *reinterpret_cast<const V_vec*>(v_ptr + offset);
         accs[i] += dot(logits_vec, v_vec);
@@ -324,69 +328,76 @@
 #define LAUNCH_ATTENTION_KERNEL(T, HEAD_SIZE, BLOCK_SIZE, NUM_THREADS)                        \
   vllm::single_query_cached_kv_attention_kernel<T, HEAD_SIZE, BLOCK_SIZE, NUM_THREADS>        \
   <<<grid, block, shared_mem_size, stream>>>(                                                 \
     out_ptr,                                                                                  \
     query_ptr,                                                                                \
     key_cache_ptr,                                                                            \
     value_cache_ptr,                                                                          \
+    head_mapping_ptr,                                                                         \
     scale,                                                                                    \
     block_tables_ptr,                                                                         \
     context_lens_ptr,                                                                         \
     max_num_blocks_per_seq,                                                                   \
     alibi_slopes_ptr,                                                                         \
-    query_stride);
+    q_stride,                                                                                 \
+    kv_block_stride,                                                                          \
+    kv_head_stride);
 
 // TODO(woosuk): Tune NUM_THREADS.
 template<
   typename T,
   int BLOCK_SIZE,
   int NUM_THREADS = 128>
 void single_query_cached_kv_attention_launcher(
   torch::Tensor& out,
   torch::Tensor& query,
   torch::Tensor& key_cache,
   torch::Tensor& value_cache,
+  torch::Tensor& head_mapping,
   float scale,
   torch::Tensor& block_tables,
   torch::Tensor& context_lens,
   int max_context_len,
   const c10::optional<torch::Tensor>& alibi_slopes) {
   int num_seqs = query.size(0);
   int num_heads = query.size(1);
   int head_size = query.size(2);
   int max_num_blocks_per_seq = block_tables.size(1);
-  int query_stride = query.stride(0);
+  int q_stride = query.stride(0);
+  int kv_block_stride = key_cache.stride(0);
+  int kv_head_stride = key_cache.stride(1);
 
   int thread_group_size = MAX(WARP_SIZE / BLOCK_SIZE, 1);
   assert(head_size % thread_group_size == 0);
 
   // NOTE: alibi_slopes is optional.
   const float* alibi_slopes_ptr = alibi_slopes ?
     reinterpret_cast<const float*>(alibi_slopes.value().data_ptr())
     : nullptr;
 
   T* out_ptr = reinterpret_cast<T*>(out.data_ptr());
   T* query_ptr = reinterpret_cast<T*>(query.data_ptr());
   T* key_cache_ptr = reinterpret_cast<T*>(key_cache.data_ptr());
   T* value_cache_ptr = reinterpret_cast<T*>(value_cache.data_ptr());
+  int* head_mapping_ptr = reinterpret_cast<int*>(head_mapping.data_ptr());
   int* block_tables_ptr = block_tables.data_ptr<int>();
   int* context_lens_ptr = context_lens.data_ptr<int>();
 
   constexpr int NUM_WARPS = NUM_THREADS / WARP_SIZE;
   int padded_max_context_len = ((max_context_len + BLOCK_SIZE - 1) / BLOCK_SIZE) * BLOCK_SIZE;
   int logits_size = padded_max_context_len * sizeof(float);
   int outputs_size = (NUM_WARPS / 2) * head_size * sizeof(float);
   int shared_mem_size = std::max(logits_size, outputs_size);
 
   dim3 grid(num_heads, num_seqs);
   dim3 block(NUM_THREADS);
   const cudaStream_t stream = at::cuda::getCurrentCUDAStream();
   switch (head_size) {
     // NOTE(woosuk): To reduce the compilation time, we omitted head sizes
-    // 32, 160, 192, 256.
+    // 32, 160, 192.
     // case 32:
     //   LAUNCH_ATTENTION_KERNEL(T, 32, BLOCK_SIZE, NUM_THREADS);
     //   break;
     case 64:
       LAUNCH_ATTENTION_KERNEL(T, 64, BLOCK_SIZE, NUM_THREADS);
       break;
     case 80:
@@ -403,29 +414,30 @@
       break;
     // case 160:
     //   LAUNCH_ATTENTION_KERNEL(T, 160, BLOCK_SIZE, NUM_THREADS);
     //   break;
     // case 192:
     //   LAUNCH_ATTENTION_KERNEL(T, 192, BLOCK_SIZE, NUM_THREADS);
     //   break;
-    // case 256:
-    //   LAUNCH_ATTENTION_KERNEL(T, 256, BLOCK_SIZE, NUM_THREADS);
-    //   break;
+    case 256:
+      LAUNCH_ATTENTION_KERNEL(T, 256, BLOCK_SIZE, NUM_THREADS);
+      break;
     default:
       TORCH_CHECK(false, "Unsupported head size: ", head_size);
       break;
   }
 }
 
 #define CALL_KERNEL_LAUNCHER(T, BLOCK_SIZE)                         \
   single_query_cached_kv_attention_launcher<T, BLOCK_SIZE>(         \
     out,                                                            \
     query,                                                          \
     key_cache,                                                      \
     value_cache,                                                    \
+    head_mapping,                                                   \
     scale,                                                          \
     block_tables,                                                   \
     context_lens,                                                   \
     max_context_len,                                                \
     alibi_slopes);
 
 // NOTE(woosuk): To reduce the compilation time, we omitted block sizes
@@ -465,14 +477,15 @@
   }
 
 void single_query_cached_kv_attention(
   torch::Tensor& out,             // [num_seqs, num_heads, head_size]
   torch::Tensor& query,           // [num_seqs, num_heads, head_size]
   torch::Tensor& key_cache,       // [num_blocks, num_heads, head_size/x, block_size, x]
   torch::Tensor& value_cache,     // [num_blocks, num_heads, head_size, block_size]
+  torch::Tensor& head_mapping,    // [num_heads]
   float scale,
   torch::Tensor& block_tables,    // [num_seqs, max_num_blocks_per_seq]
   torch::Tensor& context_lens,    // [num_seqs]
   int block_size,
   int max_context_len,
   const c10::optional<torch::Tensor>& alibi_slopes) {
   if (query.dtype() == at::ScalarType::Float) {
```

### Comparing `vllm-0.1.2/csrc/attention/attention_utils.cuh` & `vllm-0.1.3/csrc/attention/attention_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/attention/dtype_bfloat16.cuh` & `vllm-0.1.3/csrc/attention/dtype_bfloat16.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/attention/dtype_float16.cuh` & `vllm-0.1.3/csrc/attention/dtype_float16.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/attention/dtype_float32.cuh` & `vllm-0.1.3/csrc/attention/dtype_float32.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/attention.cpp` & `vllm-0.1.3/csrc/attention.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include <c10/util/Optional.h>
 
 void single_query_cached_kv_attention(
   torch::Tensor& out,
   torch::Tensor& query,
   torch::Tensor& key_cache,
   torch::Tensor& value_cache,
+  torch::Tensor& head_mapping,
   float scale,
   torch::Tensor& block_tables,
   torch::Tensor& context_lens,
   int block_size,
   int max_context_len,
   const c10::optional<torch::Tensor>& alibi_slopes);
```

### Comparing `vllm-0.1.2/csrc/cache.cpp` & `vllm-0.1.3/csrc/cache.cpp`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/cache_kernels.cu` & `vllm-0.1.3/csrc/cache_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/layernorm_kernels.cu` & `vllm-0.1.3/csrc/layernorm_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/csrc/pos_encoding_kernels.cu` & `vllm-0.1.3/csrc/pos_encoding_kernels.cu`

 * *Files 13% similar despite different names*

```diff
@@ -3,67 +3,86 @@
 
 namespace vllm {
 
 template<typename scalar_t>
 __global__ void rotary_embedding_neox_kernel(
   const int64_t* __restrict__ positions,        // [num_tokens]
   scalar_t* __restrict__ query,                 // [num_tokens, num_heads, head_size]
-  scalar_t* __restrict__ key,                   // [num_tokens, num_heads, head_size]
+  scalar_t* __restrict__ key,                   // [num_tokens, num_kv_heads, head_size]
   const scalar_t* __restrict__ cos_sin_cache,   // [max_position, 2, rot_dim // 2]
   const int rot_dim,
-  const int stride,
+  const int query_stride,
+  const int key_stride,
   const int num_heads,
+  const int num_kv_heads,
   const int head_size) {
   // Each thread block is responsible for one token.
   const int token_idx = blockIdx.x;
   int64_t pos = positions[token_idx];
   const scalar_t* cache_ptr = cos_sin_cache + pos * rot_dim;
 
   const int embed_dim = rot_dim / 2;
-  const int n = num_heads * embed_dim;
-  for (int i = threadIdx.x; i < n; i += blockDim.x) {
+  const int nq = num_heads * embed_dim;
+  for (int i = threadIdx.x; i < nq; i += blockDim.x) {
     const int head_idx = i / embed_dim;
-    const int token_head = token_idx * stride + head_idx * head_size;
+    const int token_head = token_idx * query_stride + head_idx * head_size;
 
     const int rot_offset = i % embed_dim;
     const int x_index = rot_offset;
     const int y_index = embed_dim + rot_offset;
 
-    const int out_x = token_idx * stride + head_idx * head_size + x_index;
-    const int out_y = token_idx * stride + head_idx * head_size + y_index;
+    const int out_x = token_idx * query_stride + head_idx * head_size + x_index;
+    const int out_y = token_idx * query_stride + head_idx * head_size + y_index;
 
     const scalar_t cos = __ldg(cache_ptr + x_index);
     const scalar_t sin = __ldg(cache_ptr + y_index);
 
     const scalar_t q_x = query[token_head + x_index];
     const scalar_t q_y = query[token_head + y_index];
     query[out_x] = q_x * cos - q_y * sin;
     query[out_y] = q_y * cos + q_x * sin;
+  }
+
+  const int nk = num_kv_heads * embed_dim;
+  for (int i = threadIdx.x; i < nk; i += blockDim.x) {
+    const int head_idx = i / embed_dim;
+    const int token_head = token_idx * key_stride + head_idx * head_size;
+
+    const int rot_offset = i % embed_dim;
+    const int x_index = rot_offset;
+    const int y_index = embed_dim + rot_offset;
+
+    const int out_x = token_idx * key_stride + head_idx * head_size + x_index;
+    const int out_y = token_idx * key_stride + head_idx * head_size + y_index;
+
+    const scalar_t cos = __ldg(cache_ptr + x_index);
+    const scalar_t sin = __ldg(cache_ptr + y_index);
 
     const scalar_t k_x = key[token_head + x_index];
     const scalar_t k_y = key[token_head + y_index];
     key[out_x] = k_x * cos - k_y * sin;
     key[out_y] = k_y * cos + k_x * sin;
   }
 }
 
 } // namespace vllm
 
 void rotary_embedding_neox(
   torch::Tensor& positions,         // [num_tokens]
   torch::Tensor& query,             // [num_tokens, num_heads * head_size]
-  torch::Tensor& key,               // [num_tokens, num_heads * head_size]
+  torch::Tensor& key,               // [num_tokens, num_kv_heads * head_size]
   int head_size,
   torch::Tensor& cos_sin_cache)     // [max_position, rot_dim]
 {
   int num_tokens = query.size(0);
   int rot_dim = cos_sin_cache.size(1);
   int num_heads = query.size(1) / head_size;
-  int stride = query.stride(0);
-  TORCH_CHECK(stride == key.stride(0));
+  int num_kv_heads = key.size(1) / head_size;
+  int query_stride = query.stride(0);
+  int key_stride = key.stride(0);
 
   dim3 grid(num_tokens);
   dim3 block(std::min(num_heads * rot_dim / 2, 512));
   const cudaStream_t stream = at::cuda::getCurrentCUDAStream();
   AT_DISPATCH_FLOATING_TYPES_AND2(
     at::ScalarType::Half,
     at::ScalarType::BFloat16,
@@ -72,12 +91,14 @@
     [&] {
       vllm::rotary_embedding_neox_kernel<scalar_t><<<grid, block, 0, stream>>>(
         positions.data_ptr<int64_t>(),
         query.data_ptr<scalar_t>(),
         key.data_ptr<scalar_t>(),
         cos_sin_cache.data_ptr<scalar_t>(),
         rot_dim,
-        stride,
+        query_stride,
+        key_stride,
         num_heads,
+        num_kv_heads,
         head_size);
     });
 }
```

### Comparing `vllm-0.1.2/csrc/reduction_utils.cuh` & `vllm-0.1.3/csrc/reduction_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/setup.py` & `vllm-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/__init__.py` & `vllm-0.1.3/vllm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.engine.llm_engine import LLMEngine
 from vllm.engine.ray_utils import initialize_cluster
 from vllm.entrypoints.llm import LLM
 from vllm.outputs import CompletionOutput, RequestOutput
 from vllm.sampling_params import SamplingParams
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 __all__ = [
     "LLM",
     "SamplingParams",
     "RequestOutput",
     "CompletionOutput",
     "LLMEngine",
```

### Comparing `vllm-0.1.2/vllm/block.py` & `vllm-0.1.3/vllm/block.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/config.py` & `vllm-0.1.3/vllm/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     """Configuration for the model.
 
     Args:
         model: Name or path of the huggingface model to use.
         tokenizer: Name or path of the huggingface tokenizer to use.
         tokenizer_mode: Tokenizer mode. "auto" will use the fast tokenizer if
             available, and "slow" will always use the slow tokenizer.
+        trust_remote_code: Trust remote code (e.g., from HuggingFace) when
+            downloading the model and tokenizer.
         download_dir: Directory to download and load the weights, default to the
             default cache directory of huggingface.
         use_np_weights: Save a numpy copy of model weights for faster loading.
             This can increase the disk usage by up to 2x.
         use_dummy_weights: Use dummy values for model weights (for profiling).
         dtype: Data type for model weights and activations. The "auto" option
             will use FP16 precision for FP32 and FP16 models, and BF16 precision
@@ -32,29 +34,31 @@
     """
 
     def __init__(
         self,
         model: str,
         tokenizer: str,
         tokenizer_mode: str,
+        trust_remote_code: bool,
         download_dir: Optional[str],
         use_np_weights: bool,
         use_dummy_weights: bool,
         dtype: str,
         seed: int,
     ) -> None:
         self.model = model
         self.tokenizer = tokenizer
         self.tokenizer_mode = tokenizer_mode
+        self.trust_remote_code = trust_remote_code
         self.download_dir = download_dir
         self.use_np_weights = use_np_weights
         self.use_dummy_weights = use_dummy_weights
         self.seed = seed
 
-        self.hf_config = get_config(model)
+        self.hf_config = get_config(model, trust_remote_code)
         self.dtype = _get_and_verify_dtype(self.hf_config, dtype)
         self._verify_tokenizer_mode()
 
     def _verify_tokenizer_mode(self) -> None:
         tokenizer_mode = self.tokenizer_mode.lower()
         if tokenizer_mode not in ["auto", "slow"]:
             raise ValueError(
@@ -86,17 +90,54 @@
         return self.hf_config.hidden_size
 
     def get_head_size(self) -> int:
         # FIXME(woosuk): This may not be true for all models.
         return self.hf_config.hidden_size // self.hf_config.num_attention_heads
 
     def get_num_heads(self, parallel_config: "ParallelConfig") -> int:
+        # For GPTBigCode & Falcon:
+        # Note: for falcon, when new_decoder_architecture is True, the
+        # multi_query flag is ignored and we use n_head_kv for the number of
+        # KV heads.
+        if (getattr(self.hf_config, "multi_query", False) and
+            (self.hf_config.model_type == "falcon" and
+             not getattr(self.hf_config, "new_decoder_architecture", False))):
+            # Multi-query attention, only one KV head.
+            return 1
+        # For Falcon:
+        if getattr(self.hf_config, "n_head_kv", None) is not None:
+            return (self.hf_config.n_head_kv //
+                    parallel_config.tensor_parallel_size)
+        # For LLaMA-2:
+        if getattr(self.hf_config, "num_key_value_heads", None) is not None:
+            return (self.hf_config.num_key_value_heads //
+                    parallel_config.tensor_parallel_size)
         total_num_attention_heads = self.hf_config.num_attention_heads
         return total_num_attention_heads // parallel_config.tensor_parallel_size
 
+    def get_max_model_len(self) -> int:
+        max_model_len = float("inf")
+        possible_keys = [
+            # OPT
+            "max_position_embeddings",
+            # GPT-2
+            "n_positions",
+            # MPT
+            "max_seq_len",
+            # Others
+            "max_sequence_length",
+            "max_seq_length",
+            "seq_len",
+        ]
+        for key in possible_keys:
+            max_len_key = getattr(self.hf_config, key, None)
+            if max_len_key is not None:
+                max_model_len = min(max_model_len, max_len_key)
+        return max_model_len
+
     def get_num_layers(self, parallel_config: "ParallelConfig") -> int:
         total_num_hidden_layers = self.hf_config.num_hidden_layers
         return total_num_hidden_layers // parallel_config.pipeline_parallel_size
 
 
 class CacheConfig:
     """Configuration for the KV cache.
@@ -184,23 +225,23 @@
     """Scheduler configuration.
 
     Args:
         max_num_batched_tokens: Maximum number of tokens to be processed in
             a single iteration.
         max_num_seqs: Maximum number of sequences to be processed in a single
             iteration.
-        max_seq_len: Maximum length of a sequence (including prompt
+        max_model_len: Maximum length of a sequence (including prompt
             and generated text).
     """
 
     def __init__(self, max_num_batched_tokens: int, max_num_seqs: int,
-                 max_seq_len: int) -> None:
+                 max_model_len: int) -> None:
         self.max_num_batched_tokens = max_num_batched_tokens
         self.max_num_seqs = max_num_seqs
-        self.max_seq_len = max_seq_len
+        self.max_model_len = max_model_len
 
 
 _STR_DTYPE_TO_TORCH_DTYPE = {
     "half": torch.float16,
     "float16": torch.float16,
     "float": torch.float32,
     "float32": torch.float32,
```

### Comparing `vllm-0.1.2/vllm/core/block_manager.py` & `vllm-0.1.3/vllm/core/block_manager.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/core/policy.py` & `vllm-0.1.3/vllm/core/policy.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/core/scheduler.py` & `vllm-0.1.3/vllm/core/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from vllm.logger import init_logger
 from vllm.sequence import (Sequence, SequenceData, SequenceGroup,
                            SequenceGroupMetadata, SequenceOutputs,
                            SequenceStatus)
 
 logger = init_logger(__name__)
 
-_LOGGING_INTERVAL_SEC = 5
-
 
 class PreemptionMode(enum.Enum):
     """Preemption modes.
 
     1. Swapping: Swap out the blocks of the preempted sequences to CPU memory
     and swap them back in when the sequences are resumed.
     2. Recomputation: Discard the blocks of the preempted sequences and
@@ -28,40 +26,47 @@
     RECOMPUTE = enum.auto()
 
 
 class SchedulerOutputs:
 
     def __init__(
         self,
+        scheduled_seq_groups: List[SequenceGroup],
+        prompt_run: bool,
+        num_batched_tokens: int,
         blocks_to_swap_in: Dict[int, int],
         blocks_to_swap_out: Dict[int, int],
         blocks_to_copy: Dict[int, List[int]],
+        ignored_seq_groups: List[SequenceGroup],
     ) -> None:
+        self.scheduled_seq_groups = scheduled_seq_groups
+        self.prompt_run = prompt_run
+        self.num_batched_tokens = num_batched_tokens
         self.blocks_to_swap_in = blocks_to_swap_in
         self.blocks_to_swap_out = blocks_to_swap_out
         self.blocks_to_copy = blocks_to_copy
         # Swap in and swap out should never happen at the same time.
         assert not (blocks_to_swap_in and blocks_to_swap_out)
+        self.ignored_seq_groups = ignored_seq_groups
 
     def is_empty(self) -> bool:
-        return (not self.blocks_to_swap_in and not self.blocks_to_swap_out
-                and not self.blocks_to_copy)
+        # NOTE: We do not consider the ignored sequence groups.
+        return (not self.scheduled_seq_groups and not self.blocks_to_swap_in
+                and not self.blocks_to_swap_out and not self.blocks_to_copy)
 
 
 class Scheduler:
 
     def __init__(
         self,
         scheduler_config: SchedulerConfig,
         cache_config: CacheConfig,
-        log_stats: bool,
     ) -> None:
         self.scheduler_config = scheduler_config
         self.cache_config = cache_config
-        self.log_stats = log_stats
 
         # Instantiate the scheduling policy.
         self.policy = PolicyFactory.get_policy(policy_name="fcfs")
         # Create the block space manager.
         self.block_manager = BlockSpaceManager(
             block_size=self.cache_config.block_size,
             num_gpu_blocks=self.cache_config.num_gpu_blocks,
@@ -71,18 +76,14 @@
         # Sequence groups in the WAITING state.
         self.waiting: List[SequenceGroup] = []
         # Sequence groups in the RUNNING state.
         self.running: List[SequenceGroup] = []
         # Sequence groups in the SWAPPED state.
         self.swapped: List[SequenceGroup] = []
 
-        self.last_logging_time: float = 0.0
-        # List[timestamp, num_tokens]
-        self.num_input_tokens: List[Tuple[float, int]] = []
-
     def add_seq_group(self, seq_group: SequenceGroup) -> None:
         # Add sequence groups to the waiting queue.
         self.waiting.append(seq_group)
 
     def abort_seq_group(self, request_id: str) -> None:
         for state_queue in [self.waiting, self.running, self.swapped]:
             for seq_group in state_queue:
@@ -97,29 +98,88 @@
 
     def has_unfinished_seqs(self) -> bool:
         return self.waiting or self.running or self.swapped
 
     def get_num_unfinished_seq_groups(self) -> int:
         return len(self.waiting) + len(self.running) + len(self.swapped)
 
-    def _schedule(
-            self) -> Tuple[SchedulerOutputs, List[str], List[SequenceGroup]]:
+    def _schedule(self) -> SchedulerOutputs:
         # Blocks that need to be swaped or copied before model execution.
         blocks_to_swap_in: Dict[int, int] = {}
         blocks_to_swap_out: Dict[int, int] = {}
         blocks_to_copy: Dict[int, List[int]] = {}
-        ignored_seq_groups: List[SequenceGroup] = []
 
         # Fix the current time.
         now = time.time()
 
-        # NOTE(woosuk): We prioritize the sequence groups in the RUNNING state
-        # in order to minimize the preemption overheads.
-        # Preemption happens only when there is no available slot to keep all
-        # the sequence groups in the RUNNING state.
+        # Join waiting sequences if possible.
+        if not self.swapped:
+            ignored_seq_groups: List[SequenceGroup] = []
+            scheduled: List[SequenceGroup] = []
+            num_batched_tokens = 0
+            # Optimization: We do not sort the waiting queue since the preempted
+            # sequence groups are added to the front and the new sequence groups
+            # are added to the back.
+            while self.waiting:
+                seq_group = self.waiting[0]
+
+                num_prompt_tokens = seq_group.get_seqs()[0].get_len()
+                prompt_limit = min(
+                    self.scheduler_config.max_model_len,
+                    self.scheduler_config.max_num_batched_tokens)
+                if num_prompt_tokens > prompt_limit:
+                    logger.warning(
+                        f"Input prompt ({num_prompt_tokens} tokens) is too long"
+                        f" and exceeds limit of {prompt_limit}")
+                    for seq in seq_group.get_seqs():
+                        seq.status = SequenceStatus.FINISHED_IGNORED
+                    ignored_seq_groups.append(seq_group)
+                    self.waiting.pop(0)
+                    break
+
+                # If the sequence group cannot be allocated, stop.
+                if not self.block_manager.can_allocate(seq_group):
+                    break
+
+                # If the number of batched tokens exceeds the limit, stop.
+                if (num_batched_tokens + num_prompt_tokens >
+                        self.scheduler_config.max_num_batched_tokens):
+                    break
+
+                # The total number of sequences in the RUNNING state should not
+                # exceed the maximum number of sequences.
+                num_new_seqs = seq_group.num_seqs(
+                    status=SequenceStatus.WAITING)
+                num_curr_seqs = sum(
+                    seq_group.num_seqs(status=SequenceStatus.RUNNING)
+                    for seq_group in self.running)
+                if (num_curr_seqs + num_new_seqs >
+                        self.scheduler_config.max_num_seqs):
+                    break
+
+                seq_group = self.waiting.pop(0)
+                self._allocate(seq_group)
+                self.running.append(seq_group)
+                num_batched_tokens += num_prompt_tokens
+                scheduled.append(seq_group)
+
+            if scheduled:
+                scheduler_outputs = SchedulerOutputs(
+                    scheduled_seq_groups=scheduled,
+                    prompt_run=True,
+                    num_batched_tokens=num_batched_tokens,
+                    blocks_to_swap_in=blocks_to_swap_in,
+                    blocks_to_swap_out=blocks_to_swap_out,
+                    blocks_to_copy=blocks_to_copy,
+                    ignored_seq_groups=ignored_seq_groups,
+                )
+                return scheduler_outputs
+
+        # NOTE(woosuk): Preemption happens only when there is no available slot
+        # to keep all the sequence groups in the RUNNING state.
         # In this case, the policy is responsible for deciding which sequence
         # groups to preempt.
         self.running = self.policy.sort_by_priority(now, self.running)
 
         # Reserve new token slots for the running sequence groups.
         running: List[SequenceGroup] = []
         preempted: List[SequenceGroup] = []
@@ -169,153 +229,64 @@
             self._append_slot(seq_group, blocks_to_copy)
             self.running.append(seq_group)
 
         num_batched_tokens = sum(
             seq_group.num_seqs(status=SequenceStatus.RUNNING)
             for seq_group in self.running)
 
-        # Join waiting sequences if possible.
-        prompt_group_ids: List[str] = []
-        # NOTE(woosuk): The sequence groups in the SWAPPED state are strictly
-        # prioritized over the sequence groups in the WAITING state.
-        # This is because we want to bound the amount of CPU memory taken by
-        # the swapped sequence groups.
-        if not self.swapped:
-            # Optimization: We do not sort the waiting queue since the preempted
-            # sequence groups are added to the front and the new sequence groups
-            # are added to the back.
-            while self.waiting:
-                seq_group = self.waiting[0]
-                # If the sequence group has been preempted in this step, stop.
-                if seq_group in preempted:
-                    break
-
-                num_prompt_tokens = seq_group.get_seqs()[0].get_len()
-                if num_prompt_tokens >= self.scheduler_config.max_seq_len:
-                    logger.warning(
-                        f"Input prompt ({num_prompt_tokens} tokens) is too long"
-                        " and exceeds limit of "
-                        f"{self.scheduler_config.max_seq_len}")
-                    for seq in seq_group.get_seqs():
-                        seq.status = SequenceStatus.FINISHED_IGNORED
-                    ignored_seq_groups.append(seq_group)
-                    self.waiting.pop(0)
-                    break
-
-                # If the sequence group cannot be allocated, stop.
-                if not self.block_manager.can_allocate(seq_group):
-                    break
-
-                # If the number of batched tokens exceeds the limit, stop.
-                if (num_batched_tokens + num_prompt_tokens >
-                        self.scheduler_config.max_num_batched_tokens):
-                    break
-
-                # The total number of sequences in the RUNNING state should not
-                # exceed the maximum number of sequences.
-                num_new_seqs = seq_group.num_seqs(
-                    status=SequenceStatus.WAITING)
-                num_curr_seqs = sum(
-                    seq_group.num_seqs(status=SequenceStatus.RUNNING)
-                    for seq_group in self.running)
-                if (num_curr_seqs + num_new_seqs >
-                        self.scheduler_config.max_num_seqs):
-                    break
-
-                seq_group = self.waiting.pop(0)
-                self._allocate(seq_group)
-                self.running.append(seq_group)
-                num_batched_tokens += num_prompt_tokens
-                prompt_group_ids.append(seq_group.request_id)
-
         scheduler_outputs = SchedulerOutputs(
+            scheduled_seq_groups=self.running,
+            prompt_run=False,
+            num_batched_tokens=num_batched_tokens,
             blocks_to_swap_in=blocks_to_swap_in,
             blocks_to_swap_out=blocks_to_swap_out,
             blocks_to_copy=blocks_to_copy,
+            ignored_seq_groups=[],
         )
-        if not self.log_stats:
-            return scheduler_outputs, prompt_group_ids, ignored_seq_groups
-
-        # TODO(woosuk): Move the below code to the engine.
-        now = time.time()
-        if num_batched_tokens > 0:
-            self.num_input_tokens.append((now, num_batched_tokens))
-        elapsed_time = now - self.last_logging_time
-        if elapsed_time > _LOGGING_INTERVAL_SEC:
-            self.last_logging_time = now
-            self.num_input_tokens = [(t, n) for t, n in self.num_input_tokens
-                                     if now - t < _LOGGING_INTERVAL_SEC]
-            if len(self.num_input_tokens) > 1:
-                total_num_tokens = sum(n
-                                       for _, n in self.num_input_tokens[:-1])
-                window = now - self.num_input_tokens[0][0]
-                avg_throughput = total_num_tokens / window
-            else:
-                avg_throughput = 0.0
-
-            total_num_gpu_blocks = self.cache_config.num_gpu_blocks
-            num_free_gpu_blocks = self.block_manager.get_num_free_gpu_blocks()
-            num_used_gpu_blocks = total_num_gpu_blocks - num_free_gpu_blocks
-            gpu_cache_usage = num_used_gpu_blocks / total_num_gpu_blocks
-
-            total_num_cpu_blocks = self.cache_config.num_cpu_blocks
-            if total_num_cpu_blocks > 0:
-                num_free_cpu_blocks = (
-                    self.block_manager.get_num_free_cpu_blocks())
-                num_used_cpu_blocks = total_num_cpu_blocks - num_free_cpu_blocks
-                cpu_cache_usage = num_used_cpu_blocks / total_num_cpu_blocks
-            else:
-                cpu_cache_usage = 0.0
+        return scheduler_outputs
 
-            logger.info(f"Throughput: {avg_throughput:.1f} tokens/s, "
-                        f"Running: {len(self.running)} reqs, "
-                        f"Swapped: {len(self.swapped)} reqs, "
-                        f"Pending: {len(self.waiting)} reqs, "
-                        f"GPU KV cache usage: {gpu_cache_usage * 100:.1f}%, "
-                        f"CPU KV cache usage: {cpu_cache_usage * 100:.1f}%")
-        return scheduler_outputs, prompt_group_ids, ignored_seq_groups
-
-    def schedule(
-        self
-    ) -> Tuple[List[SequenceGroupMetadata], SchedulerOutputs,
-               List[SequenceGroup]]:
+    def schedule(self) -> Tuple[List[SequenceGroupMetadata], SchedulerOutputs]:
         # Schedule sequence groups.
         # This function call changes the internal states of the scheduler
         # such as self.running, self.swapped, and self.waiting.
-        (scheduler_outputs, prompt_group_ids,
-         ignored_seq_groups) = self._schedule()
+        scheduler_outputs = self._schedule()
 
         # Create input data structures.
         seq_group_metadata_list: List[SequenceGroupMetadata] = []
-        for seq_group in self.running:
-            is_prompt = seq_group.request_id in prompt_group_ids
-
+        for seq_group in scheduler_outputs.scheduled_seq_groups:
             seq_data: Dict[int, List[SequenceData]] = {}
             block_tables: Dict[int, List[int]] = {}
             for seq in seq_group.get_seqs(status=SequenceStatus.RUNNING):
                 seq_id = seq.seq_id
                 seq_data[seq_id] = seq.data
                 block_tables[seq_id] = self.block_manager.get_block_table(seq)
 
             seq_group_metadata = SequenceGroupMetadata(
                 request_id=seq_group.request_id,
-                is_prompt=is_prompt,
+                is_prompt=scheduler_outputs.prompt_run,
                 seq_data=seq_data,
                 sampling_params=seq_group.sampling_params,
                 block_tables=block_tables,
             )
             seq_group_metadata_list.append(seq_group_metadata)
-        return seq_group_metadata_list, scheduler_outputs, ignored_seq_groups
+        return seq_group_metadata_list, scheduler_outputs
 
     def update(
         self,
         seq_outputs: Dict[int, SequenceOutputs],
     ) -> List[SequenceGroup]:
-        # Update the running sequences and free blocks.
+        scheduled: List[SequenceGroup] = []
         for seq_group in self.running:
+            for seq in seq_group.get_seqs(status=SequenceStatus.RUNNING):
+                if seq.seq_id in seq_outputs:
+                    scheduled.append(seq_group)
+                    break
+
+        # Update the scheduled sequences and free blocks.
+        for seq_group in scheduled:
             # Process beam search results before processing the new tokens.
             for seq in seq_group.get_seqs(status=SequenceStatus.RUNNING):
                 output = seq_outputs[seq.seq_id]
                 if seq.seq_id != output.parent_seq_id:
                     # The sequence is a fork of the parent sequence (beam
                     # search). Free the current sequence.
                     self.block_manager.free(seq)
@@ -325,17 +296,15 @@
                     self.block_manager.fork(parent_seq, seq)
 
             # Process the new tokens.
             for seq in seq_group.get_seqs(status=SequenceStatus.RUNNING):
                 # Append a new token to the sequence.
                 output = seq_outputs[seq.seq_id]
                 seq.append_token_id(output.output_token, output.logprobs)
-        # Return a shallow copy of the running queue to prevent the queue
-        # from being modified by the caller.
-        return self.running.copy()
+        return scheduled
 
     def free_seq(self, seq: Sequence, finish_status: SequenceStatus) -> None:
         seq.status = finish_status
         self.block_manager.free(seq)
 
     def free_finished_seq_groups(self) -> None:
         self.running = [
```

### Comparing `vllm-0.1.2/vllm/engine/arg_utils.py` & `vllm-0.1.3/vllm/engine/arg_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 @dataclass
 class EngineArgs:
     """Arguments for vLLM engine."""
     model: str
     tokenizer: Optional[str] = None
     tokenizer_mode: str = 'auto'
+    trust_remote_code: bool = False
     download_dir: Optional[str] = None
     use_np_weights: bool = False
     use_dummy_weights: bool = False
     dtype: str = 'auto'
     seed: int = 0
     worker_use_ray: bool = False
     pipeline_parallel_size: int = 1
@@ -51,14 +52,17 @@
         parser.add_argument('--tokenizer-mode',
                             type=str,
                             default=EngineArgs.tokenizer_mode,
                             choices=['auto', 'slow'],
                             help='tokenizer mode. "auto" will use the fast '
                             'tokenizer if available, and "slow" will '
                             'always use the slow tokenizer.')
+        parser.add_argument('--trust-remote-code',
+                            action='store_true',
+                            help='trust remote code from huggingface')
         parser.add_argument('--download-dir',
                             type=str,
                             default=EngineArgs.download_dir,
                             help='directory to download and load the weights, '
                             'default to the default cache dir of '
                             'huggingface')
         parser.add_argument('--use-np-weights',
@@ -137,28 +141,27 @@
         return engine_args
 
     def create_engine_configs(
         self,
     ) -> Tuple[ModelConfig, CacheConfig, ParallelConfig, SchedulerConfig]:
         # Initialize the configs.
         model_config = ModelConfig(self.model, self.tokenizer,
-                                   self.tokenizer_mode, self.download_dir,
-                                   self.use_np_weights, self.use_dummy_weights,
-                                   self.dtype, self.seed)
+                                   self.tokenizer_mode, self.trust_remote_code,
+                                   self.download_dir, self.use_np_weights,
+                                   self.use_dummy_weights, self.dtype,
+                                   self.seed)
         cache_config = CacheConfig(self.block_size,
                                    self.gpu_memory_utilization,
                                    self.swap_space)
         parallel_config = ParallelConfig(self.pipeline_parallel_size,
                                          self.tensor_parallel_size,
                                          self.worker_use_ray)
-        model_max_len = getattr(model_config.hf_config,
-                                'max_position_embeddings', float('inf'))
-        max_seq_len = min(self.max_num_batched_tokens, model_max_len)
         scheduler_config = SchedulerConfig(self.max_num_batched_tokens,
-                                           self.max_num_seqs, max_seq_len)
+                                           self.max_num_seqs,
+                                           model_config.get_max_model_len())
         return model_config, cache_config, parallel_config, scheduler_config
 
 
 @dataclass
 class AsyncEngineArgs(EngineArgs):
     """Arguments for asynchronous vLLM engine."""
     engine_use_ray: bool = False
```

### Comparing `vllm-0.1.2/vllm/engine/async_llm_engine.py` & `vllm-0.1.3/vllm/engine/async_llm_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,18 +222,18 @@
     def from_engine_args(cls,
                          engine_args: AsyncEngineArgs) -> "AsyncLLMEngine":
         """Creates an async LLM engine from the engine arguments."""
         # Create the engine configs.
         engine_configs = engine_args.create_engine_configs()
         parallel_config = engine_configs[2]
         # Initialize the cluster.
-        distributed_init_method, devices = initialize_cluster(
+        distributed_init_method, placement_group = initialize_cluster(
             parallel_config, engine_args.engine_use_ray)
         # Create the async LLM engine.
         engine = cls(engine_args.worker_use_ray,
                      engine_args.engine_use_ray,
                      *engine_configs,
                      distributed_init_method,
-                     devices,
+                     placement_group,
                      log_requests=not engine_args.disable_log_requests,
                      log_stats=not engine_args.disable_log_stats)
         return engine
```

### Comparing `vllm-0.1.2/vllm/engine/llm_engine.py` & `vllm-0.1.3/vllm/engine/llm_engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import time
-from typing import Any, List, Optional
+import copy
+from functools import partial
+from typing import Any, List, Optional, Tuple, TYPE_CHECKING
 
 from vllm.config import (CacheConfig, ModelConfig, ParallelConfig,
                          SchedulerConfig)
 from vllm.core.scheduler import Scheduler
 from vllm.engine.arg_utils import EngineArgs
-from vllm.engine.ray_utils import DeviceID, initialize_cluster, ray
+from vllm.engine.ray_utils import initialize_cluster, ray, RayWorker
 from vllm.logger import init_logger
 from vllm.outputs import RequestOutput
 from vllm.sampling_params import SamplingParams
 from vllm.sequence import Sequence, SequenceGroup, SequenceStatus
 from vllm.transformers_utils.tokenizer import (detokenize_incrementally,
                                                get_tokenizer)
 from vllm.utils import Counter
-from vllm.worker.worker import Worker
+
+if ray:
+    from ray.air.util.torch_dist import init_torch_dist_process_group
+    from ray.util.scheduling_strategies import PlacementGroupSchedulingStrategy
+
+if TYPE_CHECKING:
+    from ray.util.placement_group import PlacementGroup
 
 logger = init_logger(__name__)
 
+_LOGGING_INTERVAL_SEC = 5
+
 
 class LLMEngine:
     """An LLM engine that receives requests and generates texts.
 
     This is the main class for the vLLM engine. It receives requests
     from clients and generates texts from the LLM. It includes a tokenizer, a
     language model (possibly distributed across multiple GPUs), and GPU memory
@@ -50,22 +60,23 @@
     def __init__(
         self,
         model_config: ModelConfig,
         cache_config: CacheConfig,
         parallel_config: ParallelConfig,
         scheduler_config: SchedulerConfig,
         distributed_init_method: str,
-        stage_devices: List[List[DeviceID]],
+        placement_group: Optional["PlacementGroup"],
         log_stats: bool,
     ) -> None:
         logger.info(
             "Initializing an LLM engine with config: "
             f"model={model_config.model!r}, "
             f"tokenizer={model_config.tokenizer!r}, "
             f"tokenizer_mode={model_config.tokenizer_mode}, "
+            f"trust_remote_code={model_config.trust_remote_code}, "
             f"dtype={model_config.dtype}, "
             f"use_dummy_weights={model_config.use_dummy_weights}, "
             f"download_dir={model_config.download_dir!r}, "
             f"use_np_weights={model_config.use_np_weights}, "
             f"tensor_parallel_size={parallel_config.tensor_parallel_size}, "
             f"seed={model_config.seed})")
         # TODO(woosuk): Print more configs in debug mode.
@@ -74,42 +85,96 @@
         self.cache_config = cache_config
         self.parallel_config = parallel_config
         self.scheduler_config = scheduler_config
         self.log_stats = log_stats
         self._verify_args()
 
         self.tokenizer = get_tokenizer(
-            model_config.tokenizer, tokenizer_mode=model_config.tokenizer_mode)
+            model_config.tokenizer,
+            tokenizer_mode=model_config.tokenizer_mode,
+            trust_remote_code=model_config.trust_remote_code)
         self.seq_counter = Counter()
 
         # Create the parallel GPU workers.
-        self.workers: List[Worker] = []
-        assert len(stage_devices) == 1, "Only support one stage for now."
-        for rank, node_resource, _ in stage_devices[0]:
-            worker_cls = Worker
-            if self.parallel_config.worker_use_ray:
-                worker_cls = ray.remote(
-                    num_cpus=0,
-                    num_gpus=1,
-                    resources={node_resource: 1e-3},
-                )(worker_cls).remote
-
-            worker = worker_cls(
-                model_config,
-                parallel_config,
-                scheduler_config,
-                rank,
-                distributed_init_method,
-            )
-            self.workers.append(worker)
+        if self.parallel_config.worker_use_ray:
+            self._init_workers_ray(placement_group)
+        else:
+            self._init_workers(distributed_init_method)
+
         # Profile the memory usage and initialize the cache.
         self._init_cache()
 
         # Create the scheduler.
-        self.scheduler = Scheduler(scheduler_config, cache_config, log_stats)
+        self.scheduler = Scheduler(scheduler_config, cache_config)
+
+        # Logging.
+        self.last_logging_time = 0.0
+        # List of (timestamp, num_tokens)
+        self.num_prompt_tokens: List[Tuple[float, int]] = []
+        # List of (timestamp, num_tokens)
+        self.num_generation_tokens: List[Tuple[float, int]] = []
+
+    def _init_workers(self, distributed_init_method: str):
+        # Lazy import the Worker to avoid importing torch.cuda/xformers
+        # before CUDA_VISIBLE_DEVICES is set in the Worker
+        from vllm.worker.worker import Worker  # pylint: disable=import-outside-toplevel
+
+        assert self.parallel_config.world_size == 1, (
+            "Ray is required if parallel_config.world_size > 1.")
+
+        self.workers: List[Worker] = []
+        worker = Worker(
+            self.model_config,
+            self.parallel_config,
+            self.scheduler_config,
+            0,
+            distributed_init_method,
+        )
+        self.workers.append(worker)
+        self._run_workers(
+            "init_model",
+            get_all_outputs=True,
+        )
+
+    def _init_workers_ray(self, placement_group: "PlacementGroup"):
+        # Lazy import the Worker to avoid importing torch.cuda/xformers
+        # before CUDA_VISIBLE_DEVICES is set in the Worker
+        from vllm.worker.worker import Worker  # pylint: disable=import-outside-toplevel
+
+        self.workers: List[Worker] = []
+        for bundle in placement_group.bundle_specs:
+            if not bundle.get("GPU", 0):
+                continue
+            worker = ray.remote(
+                num_cpus=0,
+                num_gpus=1,
+                scheduling_strategy=PlacementGroupSchedulingStrategy(
+                    placement_group=placement_group,
+                    placement_group_capture_child_tasks=True),
+            )(RayWorker).remote()
+            self.workers.append(worker)
+
+        # Initialize torch distributed process group for the workers.
+        init_torch_dist_process_group(self.workers, backend="nccl")
+        model_config = copy.deepcopy(self.model_config)
+        parallel_config = copy.deepcopy(self.parallel_config)
+        scheduler_config = copy.deepcopy(self.scheduler_config)
+        self._run_workers("init_worker",
+                          get_all_outputs=True,
+                          worker_init_fn=lambda: Worker(
+                              model_config,
+                              parallel_config,
+                              scheduler_config,
+                              None,
+                              None,
+                          ))
+        self._run_workers(
+            "init_model",
+            get_all_outputs=True,
+        )
 
     def _verify_args(self) -> None:
         self.model_config.verify_with_parallel_config(self.parallel_config)
         self.cache_config.verify_with_parallel_config(self.parallel_config)
 
     def _init_cache(self) -> None:
         """Profiles the memory usage and initializes the KV cache."""
@@ -145,19 +210,20 @@
     @classmethod
     def from_engine_args(cls, engine_args: EngineArgs) -> "LLMEngine":
         """Creates an LLM engine from the engine arguments."""
         # Create the engine configs.
         engine_configs = engine_args.create_engine_configs()
         parallel_config = engine_configs[2]
         # Initialize the cluster.
-        distributed_init_method, devices = initialize_cluster(parallel_config)
+        distributed_init_method, placement_group = initialize_cluster(
+            parallel_config)
         # Create the LLM engine.
         engine = cls(*engine_configs,
                      distributed_init_method,
-                     devices,
+                     placement_group,
                      log_stats=not engine_args.disable_log_stats)
         return engine
 
     def add_request(
         self,
         request_id: str,
         prompt: Optional[str],
@@ -227,20 +293,25 @@
 
         This function performs one decoding iteration of the engine. It first
         schedules the sequences to be executed in the next iteration and the
         token blocks to be swapped in/out/copy. Then, it executes the model
         and updates the scheduler with the model outputs. Finally, it decodes
         the sequences and returns the newly generated results.
         """
-        (seq_group_metadata_list, scheduler_outputs,
-         ignored_seq_groups) = self.scheduler.schedule()
-        if ((not seq_group_metadata_list) and scheduler_outputs.is_empty()
-                and (not ignored_seq_groups)):
-            # Nothing to do.
-            return []
+        seq_group_metadata_list, scheduler_outputs = self.scheduler.schedule()
+        if scheduler_outputs.is_empty():
+            if not scheduler_outputs.ignored_seq_groups:
+                # Nothing to do.
+                return []
+            # If there are ignored seq groups, we need to return them as the
+            # request outputs.
+            return [
+                RequestOutput.from_seq_group(seq_group)
+                for seq_group in scheduler_outputs.ignored_seq_groups
+            ]
 
         # Execute the model.
         output = self._run_workers(
             "execute_model",
             seq_group_metadata_list=seq_group_metadata_list,
             blocks_to_swap_in=scheduler_outputs.blocks_to_swap_in,
             blocks_to_swap_out=scheduler_outputs.blocks_to_swap_out,
@@ -254,31 +325,100 @@
         # Stop the sequences that meet the stopping criteria.
         self._stop_sequences(seq_groups)
         # Free the finished sequence groups.
         self.scheduler.free_finished_seq_groups()
 
         # Create the outputs.
         request_outputs: List[RequestOutput] = []
-        for seq_group in seq_groups + ignored_seq_groups:
+        for seq_group in seq_groups + scheduler_outputs.ignored_seq_groups:
             request_output = RequestOutput.from_seq_group(seq_group)
             request_outputs.append(request_output)
+
+        if self.log_stats:
+            # Log the system stats.
+            self._log_system_stats(scheduler_outputs.prompt_run,
+                                   scheduler_outputs.num_batched_tokens)
         return request_outputs
 
+    def _log_system_stats(
+        self,
+        prompt_run: bool,
+        num_batched_tokens: int,
+    ) -> None:
+        now = time.time()
+        # Log the number of batched input tokens.
+        if prompt_run:
+            self.num_prompt_tokens.append((now, num_batched_tokens))
+        else:
+            self.num_generation_tokens.append((now, num_batched_tokens))
+
+        elapsed_time = now - self.last_logging_time
+        if elapsed_time < _LOGGING_INTERVAL_SEC:
+            return
+
+        # Discard the old stats.
+        self.num_prompt_tokens = [(t, n) for t, n in self.num_prompt_tokens
+                                  if now - t < _LOGGING_INTERVAL_SEC]
+        self.num_generation_tokens = [(t, n)
+                                      for t, n in self.num_generation_tokens
+                                      if now - t < _LOGGING_INTERVAL_SEC]
+
+        if len(self.num_prompt_tokens) > 1:
+            total_num_tokens = sum(n for _, n in self.num_prompt_tokens[:-1])
+            window = now - self.num_prompt_tokens[0][0]
+            avg_prompt_throughput = total_num_tokens / window
+        else:
+            avg_prompt_throughput = 0.0
+        if len(self.num_generation_tokens) > 1:
+            total_num_tokens = sum(n
+                                   for _, n in self.num_generation_tokens[:-1])
+            window = now - self.num_generation_tokens[0][0]
+            avg_generation_throughput = total_num_tokens / window
+        else:
+            avg_generation_throughput = 0.0
+
+        total_num_gpu_blocks = self.cache_config.num_gpu_blocks
+        num_free_gpu_blocks = (
+            self.scheduler.block_manager.get_num_free_gpu_blocks())
+        num_used_gpu_blocks = total_num_gpu_blocks - num_free_gpu_blocks
+        gpu_cache_usage = num_used_gpu_blocks / total_num_gpu_blocks
+
+        total_num_cpu_blocks = self.cache_config.num_cpu_blocks
+        if total_num_cpu_blocks > 0:
+            num_free_cpu_blocks = (
+                self.scheduler.block_manager.get_num_free_cpu_blocks())
+            num_used_cpu_blocks = total_num_cpu_blocks - num_free_cpu_blocks
+            cpu_cache_usage = num_used_cpu_blocks / total_num_cpu_blocks
+        else:
+            cpu_cache_usage = 0.0
+
+        logger.info("Avg prompt throughput: "
+                    f"{avg_prompt_throughput:.1f} tokens/s, "
+                    "Avg generation throughput: "
+                    f"{avg_generation_throughput:.1f} tokens/s, "
+                    f"Running: {len(self.scheduler.running)} reqs, "
+                    f"Swapped: {len(self.scheduler.swapped)} reqs, "
+                    f"Pending: {len(self.scheduler.waiting)} reqs, "
+                    f"GPU KV cache usage: {gpu_cache_usage * 100:.1f}%, "
+                    f"CPU KV cache usage: {cpu_cache_usage * 100:.1f}%")
+        self.last_logging_time = now
+
     def _decode_sequences(self, seq_groups: List[SequenceGroup]) -> None:
         """Decodes the sequence outputs."""
         for seq_group in seq_groups:
             for seq in seq_group.get_seqs(status=SequenceStatus.RUNNING):
                 new_token, new_output_text = detokenize_incrementally(
                     self.tokenizer,
                     seq.output_tokens,
                     seq.get_last_token_id(),
                     skip_special_tokens=True,
                 )
-                seq.output_tokens.append(new_token)
-                seq.output_text = new_output_text
+                if new_token is not None:
+                    seq.output_tokens.append(new_token)
+                    seq.output_text = new_output_text
 
     def _stop_sequences(self, seq_groups: List[SequenceGroup]) -> None:
         """Stop the finished sequences."""
         for seq_group in seq_groups:
             sampling_params = seq_group.sampling_params
             for seq in seq_group.get_seqs(status=SequenceStatus.RUNNING):
                 # Check if the sequence has generated a stop string.
@@ -291,17 +431,16 @@
                         self.scheduler.free_seq(
                             seq, SequenceStatus.FINISHED_STOPPED)
                         stopped = True
                         break
                 if stopped:
                     continue
 
-                # Check if the sequence has reached max_seq_len.
-                if (seq.get_len() >=
-                        self.scheduler.scheduler_config.max_seq_len):
+                # Check if the sequence has reached max_model_len.
+                if seq.get_len() > self.scheduler_config.max_model_len:
                     self.scheduler.free_seq(
                         seq, SequenceStatus.FINISHED_LENGTH_CAPPED)
                     continue
                 # Check if the sequence has reached max_tokens.
                 if seq.get_output_len() == sampling_params.max_tokens:
                     self.scheduler.free_seq(
                         seq, SequenceStatus.FINISHED_LENGTH_CAPPED)
@@ -319,17 +458,18 @@
         *args,
         get_all_outputs: bool = False,
         **kwargs,
     ) -> Any:
         """Runs the given method on all workers."""
         all_outputs = []
         for worker in self.workers:
-            executor = getattr(worker, method)
             if self.parallel_config.worker_use_ray:
-                executor = executor.remote
+                executor = partial(worker.execute_method.remote, method)
+            else:
+                executor = getattr(worker, method)
 
             output = executor(*args, **kwargs)
             all_outputs.append(output)
 
         if self.parallel_config.worker_use_ray:
             all_outputs = ray.get(all_outputs)
```

### Comparing `vllm-0.1.2/vllm/entrypoints/api_server.py` & `vllm-0.1.3/vllm/entrypoints/api_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import json
 from typing import AsyncGenerator
 
 from fastapi import BackgroundTasks, FastAPI, Request
-from fastapi.responses import Response, StreamingResponse
+from fastapi.responses import JSONResponse, Response, StreamingResponse
 import uvicorn
 
 from vllm.engine.arg_utils import AsyncEngineArgs
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.sampling_params import SamplingParams
 from vllm.utils import random_uuid
 
@@ -60,15 +60,15 @@
             return Response(status_code=499)
         final_output = request_output
 
     assert final_output is not None
     prompt = final_output.prompt
     text_outputs = [prompt + output.text for output in final_output.outputs]
     ret = {"text": text_outputs}
-    return Response(content=json.dumps(ret))
+    return JSONResponse(ret)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=8000)
     parser = AsyncEngineArgs.add_cli_args(parser)
```

### Comparing `vllm-0.1.2/vllm/entrypoints/llm.py` & `vllm-0.1.3/vllm/entrypoints/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     NOTE: For the comprehensive list of arguments, see `EngineArgs`.
 
     Args:
         model: The name or path of a HuggingFace Transformers model.
         tokenizer: The name or path of a HuggingFace Transformers tokenizer.
         tokenizer_mode: The tokenizer mode. "auto" will use the fast tokenizer
             if available, and "slow" will always use the slow tokenizer.
+        trust_remote_code: Trust remote code (e.g., from HuggingFace) when
+            downloading the model and tokenizer.
         tensor_parallel_size: The number of GPUs to use for distributed
             execution with tensor parallelism.
         dtype: The data type for the model weights and activations. Currently,
             we support `float32`, `float16`, and `bfloat16`. If `auto`, we use
             the `torch_dtype` attribute specified in the model config file.
             However, if the `torch_dtype` in the config is `float32`, we will
             use `float16` instead.
@@ -39,25 +41,27 @@
     """
 
     def __init__(
         self,
         model: str,
         tokenizer: Optional[str] = None,
         tokenizer_mode: str = "auto",
+        trust_remote_code: bool = False,
         tensor_parallel_size: int = 1,
         dtype: str = "auto",
         seed: int = 0,
         **kwargs,
     ) -> None:
         if "disable_log_stats" not in kwargs:
             kwargs["disable_log_stats"] = True
         engine_args = EngineArgs(
             model=model,
             tokenizer=tokenizer,
             tokenizer_mode=tokenizer_mode,
+            trust_remote_code=trust_remote_code,
             tensor_parallel_size=tensor_parallel_size,
             dtype=dtype,
             seed=seed,
             **kwargs,
         )
         self.llm_engine = LLMEngine.from_engine_args(engine_args)
         self.request_counter = Counter()
@@ -147,8 +151,12 @@
             for output in step_outputs:
                 if output.finished:
                     outputs.append(output)
                     if use_tqdm:
                         pbar.update(1)
         if use_tqdm:
             pbar.close()
+        # Sort the outputs by request ID.
+        # This is necessary because some requests may be finished earlier than
+        # its previous requests.
+        outputs = sorted(outputs, key=lambda x: int(x.request_id))
         return outputs
```

### Comparing `vllm-0.1.2/vllm/entrypoints/openai/api_server.py` & `vllm-0.1.3/vllm/entrypoints/openai/api_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 
 import argparse
 import asyncio
 from http import HTTPStatus
 import json
 import time
 from typing import AsyncGenerator, Dict, List, Optional
+from packaging import version
 
 import fastapi
 from fastapi import BackgroundTasks, Request
 from fastapi.exceptions import RequestValidationError
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse, StreamingResponse
-from fastchat.conversation import Conversation, SeparatorStyle
-from fastchat.model.model_adapter import get_conversation_template
-
 import uvicorn
 
 from vllm.engine.arg_utils import AsyncEngineArgs
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.entrypoints.openai.protocol import (
     CompletionRequest, CompletionResponse, CompletionResponseChoice,
     CompletionResponseStreamChoice, CompletionStreamResponse,
@@ -29,14 +27,22 @@
     LogProbs, ModelCard, ModelList, ModelPermission, UsageInfo)
 from vllm.logger import init_logger
 from vllm.outputs import RequestOutput
 from vllm.sampling_params import SamplingParams
 from vllm.transformers_utils.tokenizer import get_tokenizer
 from vllm.utils import random_uuid
 
+try:
+    import fastchat
+    from fastchat.conversation import Conversation, SeparatorStyle
+    from fastchat.model.model_adapter import get_conversation_template
+    _fastchat_available = True
+except ImportError:
+    _fastchat_available = False
+
 TIMEOUT_KEEP_ALIVE = 5  # seconds
 
 logger = init_logger(__name__)
 served_model = None
 app = fastapi.FastAPI()
 
 
@@ -59,18 +65,29 @@
         HTTPStatus.NOT_FOUND,
         f"The model `{request.model}` does not exist.",
     )
     return ret
 
 
 async def get_gen_prompt(request) -> str:
+    if not _fastchat_available:
+        raise ModuleNotFoundError(
+            "fastchat is not installed. Please install fastchat to use "
+            "the chat completion and conversation APIs: `$ pip install fschat`"
+        )
+    if version.parse(fastchat.__version__) < version.parse("0.2.23"):
+        raise ImportError(
+            f"fastchat version is low. Current version: {fastchat.__version__} "
+            "Please upgrade fastchat to use: `$ pip install -U fschat`")
+
     conv = get_conversation_template(request.model)
     conv = Conversation(
         name=conv.name,
-        system=conv.system,
+        system_template=conv.system_template,
+        system_message=conv.system_message,
         roles=conv.roles,
         messages=list(conv.messages),  # prevent in-place modification
         offset=conv.offset,
         sep_style=SeparatorStyle(conv.sep_style),
         sep=conv.sep,
         sep2=conv.sep2,
         stop_str=conv.stop_str,
@@ -79,48 +96,37 @@
 
     if isinstance(request.messages, str):
         prompt = request.messages
     else:
         for message in request.messages:
             msg_role = message["role"]
             if msg_role == "system":
-                conv.system = message["content"]
+                conv.system_message = message["content"]
             elif msg_role == "user":
                 conv.append_message(conv.roles[0], message["content"])
             elif msg_role == "assistant":
                 conv.append_message(conv.roles[1], message["content"])
             else:
                 raise ValueError(f"Unknown role: {msg_role}")
 
         # Add a blank message for the assistant.
         conv.append_message(conv.roles[1], None)
         prompt = conv.get_prompt()
 
     return prompt
 
 
-async def check_length(request, prompt, model_config):
-    if hasattr(model_config.hf_config, "max_sequence_length"):
-        context_len = model_config.hf_config.max_sequence_length
-    elif hasattr(model_config.hf_config, "seq_length"):
-        context_len = model_config.hf_config.seq_length
-    elif hasattr(model_config.hf_config, "max_position_embeddings"):
-        context_len = model_config.hf_config.max_position_embeddings
-    elif hasattr(model_config.hf_config, "seq_length"):
-        context_len = model_config.hf_config.seq_length
-    else:
-        context_len = 2048
-
+async def check_length(request, prompt):
     input_ids = tokenizer(prompt).input_ids
     token_num = len(input_ids)
 
-    if token_num + request.max_tokens > context_len:
+    if token_num + request.max_tokens > max_model_len:
         return create_error_response(
             HTTPStatus.BAD_REQUEST,
-            f"This model's maximum context length is {context_len} tokens. "
+            f"This model's maximum context length is {max_model_len} tokens. "
             f"However, you requested {request.max_tokens + token_num} tokens "
             f"({token_num} in the messages, "
             f"{request.max_tokens} in the completion). "
             f"Please reduce the length of the messages or completion.",
         )
     else:
         return None
@@ -181,15 +187,15 @@
 
     if request.logit_bias is not None:
         # TODO: support logit_bias in vLLM engine.
         return create_error_response(HTTPStatus.BAD_REQUEST,
                                      "logit_bias is not currently supported")
 
     prompt = await get_gen_prompt(request)
-    error_check_ret = await check_length(request, prompt, engine_model_config)
+    error_check_ret = await check_length(request, prompt)
     if error_check_ret is not None:
         return error_check_ret
 
     model_name = request.model
     request_id = f"cmpl-{random_uuid()}"
     created_time = int(time.time())
     try:
@@ -265,15 +271,15 @@
                 if output.finish_reason is not None:
                     response_json = create_stream_response_json(
                         index=i,
                         text="",
                         finish_reason=output.finish_reason,
                     )
                     yield f"data: {response_json}\n\n"
-            yield "data: [DONE]\n\n"
+        yield "data: [DONE]\n\n"
 
     # Streaming response
     if request.stream:
         background_tasks = BackgroundTasks()
         # Abort the request if the client disconnects.
         background_tasks.add_task(abort_request)
         return StreamingResponse(completion_stream_generator(),
@@ -461,15 +467,15 @@
                     response_json = create_stream_response_json(
                         index=i,
                         text="",
                         logprobs=logprobs,
                         finish_reason=output.finish_reason,
                     )
                     yield f"data: {response_json}\n\n"
-            yield "data: [DONE]\n\n"
+        yield "data: [DONE]\n\n"
 
     # Streaming response
     if stream:
         background_tasks = BackgroundTasks()
         # Abort the request if the client disconnects.
         background_tasks.add_task(abort_request)
         return StreamingResponse(completion_stream_generator(),
@@ -578,17 +584,19 @@
         served_model = args.served_model_name
     else:
         served_model = args.model
 
     engine_args = AsyncEngineArgs.from_cli_args(args)
     engine = AsyncLLMEngine.from_engine_args(engine_args)
     engine_model_config = asyncio.run(engine.get_model_config())
+    max_model_len = engine_model_config.get_max_model_len()
 
     # A separate tokenizer to map token IDs to strings.
     tokenizer = get_tokenizer(engine_args.tokenizer,
-                              tokenizer_mode=engine_args.tokenizer_mode)
+                              tokenizer_mode=engine_args.tokenizer_mode,
+                              trust_remote_code=engine_args.trust_remote_code)
 
     uvicorn.run(app,
                 host=args.host,
                 port=args.port,
                 log_level="info",
                 timeout_keep_alive=TIMEOUT_KEEP_ALIVE)
```

### Comparing `vllm-0.1.2/vllm/entrypoints/openai/protocol.py` & `vllm-0.1.3/vllm/entrypoints/openai/protocol.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/logger.py` & `vllm-0.1.3/vllm/logger.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/input_metadata.py` & `vllm-0.1.3/vllm/model_executor/input_metadata.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/layers/activation.py` & `vllm-0.1.3/vllm/model_executor/layers/activation.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/layers/attention.py` & `vllm-0.1.3/vllm/model_executor/layers/attention.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,36 @@
                                          LowerTriangularMaskWithTensorBias)
 
 from vllm import attention_ops
 from vllm import cache_ops
 from vllm import pos_encoding_ops
 from vllm.model_executor.input_metadata import InputMetadata
 
-_SUPPORTED_HEAD_SIZES = [64, 80, 96, 112, 128]
+_SUPPORTED_HEAD_SIZES = [64, 80, 96, 112, 128, 256]
 
 
 class PagedAttention(nn.Module):
     # pylint: disable=line-too-long
     """GPT-style multi-head PagedAttention.
 
     This class takes flattened 1D query, key, and value tensors as input. The
-    input 1D tensors can be split into three parts: the prompt tokens, the
-    generation tokens, and the paddings.
+    input 1D tensors can either contain prompt tokens or generation tokens, in
+    addition to paddings.
 
-    |<------------------------------------- num_valid_tokens ------------------------------------->|
-    |<--------------- num_prompt_tokens -------------->|<------- num_generation_tokens (M) ------->|
-    |<--prompt_0-->|<--prompt_1-->|...|<--prompt_N-1-->|<--generation_0-->|...|<--generation_M-1-->|<--padding-->|
+    If the input tensors contain prompt tokens, the layout is as follows:
+
+    |<---------------------- num_valid_tokens ---------------------->|
+    |<--------------- num_prompt_tokens -------------->|
+    |<--prompt_0-->|<--prompt_1-->|...|<--prompt_N-1-->|<--padding-->|
+
+    Otherwise, the layout is as follows:
+
+    |<------------------ num_valid_tokens ------------------->|
+    |<------- num_generation_tokens (M) ------->|
+    |<--generation_0-->|...|<--generation_M-1-->|<--padding-->|
 
     The prompts might have different lengths, while the generation tokens always
     have length 1. The paddings are appended to make the input length a multiple
     of 8, which is desirable for Tensor Cores.
 
     The class does the following:
     1. Perform multi_query_kv_attention for the prompts. This operation does
@@ -40,20 +48,31 @@
     3. Reshape and store the input key and value tensors in the KV cache.
     4. Perform single_query_cached_kv_attention for the generation tokens.
         This operation reads the previous key and value tensors from the KV
         cache.
     5. Output a flattened 1D tensor.
     """
 
-    def __init__(self, num_heads: int, head_size: int, scale: float) -> None:
+    def __init__(self,
+                 num_heads: int,
+                 head_size: int,
+                 scale: float,
+                 num_kv_heads: Optional[int] = None) -> None:
         super().__init__()
         self.num_heads = num_heads
         self.head_size = head_size
         self.scale = float(scale)
         self.attn_op = xops.fmha.cutlass.FwOp()
+        self.num_kv_heads = num_heads if num_kv_heads is None else num_kv_heads
+
+        assert self.num_heads % self.num_kv_heads == 0
+        self.num_queries_per_kv = self.num_heads // self.num_kv_heads
+        self.head_mapping = torch.repeat_interleave(
+            torch.arange(self.num_kv_heads, dtype=torch.int32, device="cuda"),
+            self.num_queries_per_kv)
 
         if self.head_size not in _SUPPORTED_HEAD_SIZES:
             raise ValueError(f"head_size ({self.head_size}) is not supported. "
                              f"Supported head sizes: {_SUPPORTED_HEAD_SIZES}.")
 
     def set_attn_bias(self, input_metadata: InputMetadata) -> None:
         if input_metadata.attn_bias:
@@ -72,18 +91,26 @@
         input_metadata: InputMetadata,
     ) -> torch.Tensor:
         """Normal attention for the prompt tokens.
 
         Args:
             output: shape = [num_prompt_tokens, num_heads, head_size]
             query: shape = [num_prompt_tokens, num_heads, head_size]
-            key: shape = [num_prompt_tokens, num_heads, head_size]
-            value: shape = [num_prompt_tokens, num_heads, head_size]
+            key: shape = [num_prompt_tokens, num_kv_heads, head_size]
+            value: shape = [num_prompt_tokens, num_kv_heads, head_size]
             input_metadata: metadata for paged attention.
         """
+
+        if self.num_kv_heads != self.num_heads:
+            # Project the key and value tensors to the desired number of heads.
+            key = torch.repeat_interleave(key, self.num_queries_per_kv, dim=1)
+            value = torch.repeat_interleave(value,
+                                            self.num_queries_per_kv,
+                                            dim=1)
+
         # TODO(woosuk): The unsqueeze op may incur some CPU overhead. Optimize.
         out = xops.memory_efficient_attention_forward(
             query.unsqueeze(0),
             key.unsqueeze(0),
             value.unsqueeze(0),
             attn_bias=input_metadata.attn_bias[0],
             p=0.0,
@@ -103,25 +130,27 @@
         input_metadata: InputMetadata,
     ) -> None:
         """PagedAttention for the generation tokens.
 
         Args:
             output: shape = [num_generation_tokens, num_heads, head_size]
             query: shape = [num_generation_tokens, num_heads, head_size]
-            key_cache: shape = [num_blocks, num_heads, head_size/x,
+            key_cache: shape = [num_blocks, num_kv_heads, head_size/x,
                 block_size, x]
-            value_cache: shape = [num_blocks, num_heads, head_size, block_size]
+            value_cache: shape = [num_blocks, num_kv_heads, head_size,
+                block_size]
             input_metadata: metadata for paged attention.
         """
         block_size = value_cache.shape[3]
         attention_ops.single_query_cached_kv_attention(
             output,
             query,
             key_cache,
             value_cache,
+            self.head_mapping,
             self.scale,
             input_metadata.block_tables,
             input_metadata.context_lens,
             block_size,
             input_metadata.max_context_len,
             None,  # alibi_slopes
         )
@@ -139,37 +168,40 @@
         """PagedAttention forward pass.
 
         NOTE: The query, key, and value tensors must be sliced from a qkv
         tensor of shape [num_tokens, 3 * num_heads * head_size].
 
         Args:
             query: shape = [num_tokens, num_heads * head_size]
-            key: shape = [num_tokens, num_heads * head_size]
-            value: shape = [num_tokens, num_heads * head_size]
-            key_cache: shape = [num_blocks, num_heads, head_size/x,
+            key: shape = [num_tokens, num_kv_heads * head_size]
+            value: shape = [num_tokens, num_kv_heads * head_size]
+            key_cache: shape = [num_blocks, num_kv_heads, head_size/x,
                 block_size, x]
-            value_cache: shape = [num_blocks, num_heads, head_size, block_size]
+            value_cache: shape = [num_blocks, num_kv_heads, head_size,
+                block_size]
             input_metadata: metadata for paged attention.
             cache_event: event to wait for the cache operations to finish.
 
         Returns:
             shape = [num_tokens, num_heads * head_size]
         """
 
         # Reshape the query, key, and value tensors.
         query = query.view(-1, self.num_heads, self.head_size)
-        key = key.view(-1, self.num_heads, self.head_size)
-        value = value.view(-1, self.num_heads, self.head_size)
+        key = key.view(-1, self.num_kv_heads, self.head_size)
+        value = value.view(-1, self.num_kv_heads, self.head_size)
 
         # Pre-allocate the output tensor.
         output = torch.empty_like(query)
 
         # Compute the attention op for prompts.
         num_prompt_tokens = input_metadata.num_prompt_tokens
         if num_prompt_tokens > 0:
+            # Prompt run.
+            assert input_metadata.num_generation_tokens == 0
             self.set_attn_bias(input_metadata)
             self.multi_query_kv_attention(
                 output[:num_prompt_tokens],
                 query[:num_prompt_tokens],
                 key[:num_prompt_tokens],
                 value[:num_prompt_tokens],
                 input_metadata,
@@ -191,14 +223,16 @@
                 value[:num_valid_tokens],
                 key_cache,
                 value_cache,
                 input_metadata.slot_mapping,
             )
 
         if input_metadata.num_generation_tokens > 0:
+            # Decoding run.
+            assert input_metadata.num_prompt_tokens == 0
             assert key_cache is not None and value_cache is not None, (
                 "key_cache and value_cache must be provided when "
                 "generating tokens.")
             # Compute the attention op for generation tokens.
             self.single_query_cached_kv_attention(
                 output[num_prompt_tokens:num_valid_tokens],
                 query[num_prompt_tokens:num_valid_tokens], key_cache,
@@ -216,16 +250,17 @@
         self,
         num_heads: int,
         head_size: int,
         scale: float,
         rotary_dim: int,
         max_position: int = 8192,
         base: int = 10000,
+        num_kv_heads: Optional[int] = None,
     ) -> None:
-        super().__init__(num_heads, head_size, scale)
+        super().__init__(num_heads, head_size, scale, num_kv_heads)
 
         # Create the cos and sin cache.
         inv_freq = 1.0 / (base**(torch.arange(0, rotary_dim, 2) / rotary_dim))
         t = torch.arange(max_position).float()
         freqs = torch.einsum("i,j -> ij", t, inv_freq.float())
         cos = freqs.cos()
         sin = freqs.sin()
@@ -251,19 +286,20 @@
         cache_event: Optional[torch.cuda.Event],
     ) -> torch.Tensor:
         """ PagedAttention forward pass with rotary embedding.
 
         Args:
             positions: shape = [num_tokens]
                         query: shape = [num_tokens, num_heads * head_size]
-            key: shape = [num_tokens, num_heads * head_size]
-            value: shape = [num_tokens, num_heads * head_size]
-            key_cache: shape = [num_blocks, num_heads, head_size/x,
+            key: shape = [num_tokens, num_kv_heads * head_size]
+            value: shape = [num_tokens, num_kv_heads * head_size]
+            key_cache: shape = [num_blocks, num_kv_heads, head_size/x,
                 block_size, x]
-            value_cache: shape = [num_blocks, num_heads, head_size, block_size]
+            value_cache: shape = [num_blocks, num_kv_heads, head_size,
+                block_size]
             input_metadata: metadata for paged attention.
             cache_event: event to wait for the cache operations to finish.
 
         Returns:
             shape = [num_tokens, num_heads * head_size]
         """
 
@@ -286,34 +322,38 @@
             cache_event,
         )
 
 
 class PagedAttentionWithALiBi(PagedAttention):
     """PagedAttention with ALiBi attention bias."""
 
-    def __init__(
-        self,
-        num_heads: int,
-        head_size: int,
-        scale: float,
-        slopes: List[float],
-    ) -> None:
-        super().__init__(num_heads, head_size, scale)
+    def __init__(self,
+                 num_heads: int,
+                 head_size: int,
+                 scale: float,
+                 slopes: List[float],
+                 num_kv_heads: Optional[int] = None) -> None:
+        super().__init__(num_heads, head_size, scale, num_kv_heads)
         assert len(slopes) == num_heads
 
         slopes = torch.tensor(slopes, dtype=torch.float32)
         self.register_buffer("alibi_slopes", slopes, persistent=False)
 
     def set_attn_bias(self, input_metadata: InputMetadata) -> None:
         if input_metadata.attn_bias:
             # Already set by a previous layer.
             return
         # Generates ALiBi mask for each prompt.
         for prompt_len in input_metadata.prompt_lens:
             bias = torch.arange(prompt_len)
+            # Note(zhuohan): HF uses
+            #     `bias = bias[None, :].repeat(prompt_len, 1)`
+            # here. We find that both biases give the same results, but
+            # the bias below more accurately follows the original ALiBi
+            # paper.
             bias = bias[None, :] - bias[:, None]
             bias = bias.to(self.alibi_slopes.device)
 
             # When using custom attention bias, xformers requires the bias to
             # be sliced from a tensor whose length is a multiple of 8.
             padded_len = (prompt_len + 7) // 8 * 8
             bias = torch.empty(
@@ -335,18 +375,25 @@
         input_metadata: InputMetadata,
     ) -> torch.Tensor:
         """Attention with ALiBi bias for the prompt tokens.
 
         Args:
             output: shape = [num_prompt_tokens, num_heads, head_size]
             query: shape = [num_prompt_tokens, num_heads, head_size]
-            key: shape = [num_prompt_tokens, num_heads, head_size]
-            value: shape = [num_prompt_tokens, num_heads, head_size]
+            key: shape = [num_prompt_tokens, num_kv_heads, head_size]
+            value: shape = [num_prompt_tokens, num_kv_heads, head_size]
             input_metadata: metadata for paged attention.
         """
+        if self.num_kv_heads != self.num_heads:
+            # Project the key and value tensors to the desired number of heads.
+            key = torch.repeat_interleave(key, self.num_queries_per_kv, dim=1)
+            value = torch.repeat_interleave(value,
+                                            self.num_queries_per_kv,
+                                            dim=1)
+
         # FIXME(woosuk): Because xformers does not support dynamic sequence
         # lengths with custom attention bias, we process each prompt one by
         # one. This is inefficient, especially when we have many short prompts.
         start = 0
         for i, prompt_len in enumerate(input_metadata.prompt_lens):
             end = start + prompt_len
             out = xops.memory_efficient_attention_forward(
@@ -372,25 +419,27 @@
         input_metadata: InputMetadata,
     ) -> None:
         """PagedAttention with ALiBi bias for the generation tokens.
 
         Args:
             output: shape = [num_generation_tokens, num_heads, head_size]
             query: shape = [num_generation_tokens, num_heads, head_size]
-            key_cache: shape = [num_blocks, num_heads, head_size/x,
+            key_cache: shape = [num_blocks, num_kv_heads, head_size/x,
                 block_size, x]
-            value_cache: shape = [num_blocks, num_heads, head_size, block_size]
+            value_cache: shape = [num_blocks, num_kv_heads, head_size,
+                block_size]
             input_metadata: metadata for paged attention.
         """
         block_size = value_cache.shape[3]
         attention_ops.single_query_cached_kv_attention(
             output,
             query,
             key_cache,
             value_cache,
+            self.head_mapping,
             self.scale,
             input_metadata.block_tables,
             input_metadata.context_lens,
             block_size,
             input_metadata.max_context_len,
             self.alibi_slopes,
         )
```

### Comparing `vllm-0.1.2/vllm/model_executor/layers/layernorm.py` & `vllm-0.1.3/vllm/model_executor/layers/layernorm.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/layers/sampler.py` & `vllm-0.1.3/vllm/model_executor/layers/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,23 @@
         self.vocab_size = vocab_size
 
     def forward(
         self,
         embedding: torch.Tensor,
         hidden_states: torch.Tensor,
         input_metadata: InputMetadata,
+        embedding_bias: Optional[torch.Tensor] = None,
     ) -> Dict[int, SequenceOutputs]:
         # Get the hidden states that we use for sampling.
         hidden_states = _prune_hidden_states(hidden_states, input_metadata)
 
         # Get the logits for the next tokens.
         logits = torch.matmul(hidden_states, embedding.t())
+        if embedding_bias is not None:
+            logits += embedding_bias
         logits = gather_from_tensor_model_parallel_region(logits)
         # Remove paddings in vocab (if any).
         logits = logits[:, :self.vocab_size]
 
         # Apply presence and frequency penalties.
         output_tokens = _get_output_tokens(input_metadata)
         assert len(output_tokens) == logits.shape[0]
```

### Comparing `vllm-0.1.2/vllm/model_executor/model_loader.py` & `vllm-0.1.3/vllm/model_executor/model_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 
 from vllm.config import ModelConfig
 from vllm.model_executor.models import *  # pylint: disable=wildcard-import
 from vllm.model_executor.weight_utils import initialize_dummy_weights
 
 # TODO(woosuk): Lazy-load the model classes.
 _MODEL_REGISTRY = {
+    "BaiChuanForCausalLM": BaiChuanForCausalLM,  # baichuan-7b
+    "BaichuanForCausalLM": BaichuanForCausalLM,  # baichuan-13b
     "BloomForCausalLM": BloomForCausalLM,
+    "FalconForCausalLM": FalconForCausalLM,
     "GPT2LMHeadModel": GPT2LMHeadModel,
     "GPTBigCodeForCausalLM": GPTBigCodeForCausalLM,
+    "GPTJForCausalLM": GPTJForCausalLM,
     "GPTNeoXForCausalLM": GPTNeoXForCausalLM,
     "LlamaForCausalLM": LlamaForCausalLM,
     "LLaMAForCausalLM": LlamaForCausalLM,  # For decapoda-research/llama-*
     "MPTForCausalLM": MPTForCausalLM,
     "OPTForCausalLM": OPTForCausalLM,
+    "RWForCausalLM": FalconForCausalLM,
 }
 
 
 def _get_model_architecture(config: PretrainedConfig) -> Type[nn.Module]:
     architectures = getattr(config, "architectures", [])
     for arch in architectures:
         if arch in _MODEL_REGISTRY:
```

### Comparing `vllm-0.1.2/vllm/model_executor/models/__init__.py` & `vllm-0.1.3/vllm/model_executor/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+from vllm.model_executor.models.baichuan import (BaiChuanForCausalLM,
+                                                 BaichuanForCausalLM)
 from vllm.model_executor.models.bloom import BloomForCausalLM
+from vllm.model_executor.models.falcon import FalconForCausalLM
 from vllm.model_executor.models.gpt2 import GPT2LMHeadModel
 from vllm.model_executor.models.gpt_bigcode import GPTBigCodeForCausalLM
+from vllm.model_executor.models.gpt_j import GPTJForCausalLM
 from vllm.model_executor.models.gpt_neox import GPTNeoXForCausalLM
 from vllm.model_executor.models.llama import LlamaForCausalLM
 from vllm.model_executor.models.mpt import MPTForCausalLM
 from vllm.model_executor.models.opt import OPTForCausalLM
 
 __all__ = [
+    "BaiChuanForCausalLM",
+    "BaichuanForCausalLM",
     "BloomForCausalLM",
+    "FalconForCausalLM",
     "GPT2LMHeadModel",
     "GPTBigCodeForCausalLM",
+    "GPTJForCausalLM",
     "GPTNeoXForCausalLM",
     "LlamaForCausalLM",
     "MPTForCausalLM",
     "OPTForCausalLM",
 ]
```

### Comparing `vllm-0.1.2/vllm/model_executor/models/bloom.py` & `vllm-0.1.3/vllm/model_executor/models/bloom.py`

 * *Files 4% similar despite different names*

```diff
@@ -280,18 +280,25 @@
                      model_name_or_path: str,
                      cache_dir: Optional[str] = None,
                      use_np_cache: bool = False):
         tp_rank = get_tensor_model_parallel_rank()
         state_dict = self.state_dict()
         for name, loaded_weight in hf_model_weights_iterator(
                 model_name_or_path, cache_dir, use_np_cache):
-            if not name.startswith("transformer."):
-                name = "transformer." + name
+            if name == "lm_head.weight":
+                # Since hidden_states are parallelized, we need to
+                # load lm_head.weight in parallel.
+                self._column_parallel_weights.append(name)
+                # If lm_head is provided, use it instead.
+                param = self.lm_head_weight
+            else:
+                if not name.startswith("transformer."):
+                    name = "transformer." + name
+                param = state_dict[name]
 
-            param = state_dict[name]
             if "query_key_value" in name:
                 # NOTE(woosuk): BLOOM's fused QKV has the shape of
                 # [num_heads * 3 * head_size, hidden_size], while the
                 # required shape is [3 * num_heads * head_size, hidden_size].
                 # Thus, we need weight conversion.
                 shard_size = param.shape[0]
                 start = shard_size * tp_rank
```

### Comparing `vllm-0.1.2/vllm/model_executor/models/gpt2.py` & `vllm-0.1.3/vllm/model_executor/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/models/gpt_bigcode.py` & `vllm-0.1.3/vllm/model_executor/models/gpt_bigcode.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 The input of the model is flattened to a 1D tensor of tokens. The model uses
 InputMetadata to extract the original 2D shape of the input.
 """
 from typing import Dict, List, Optional, Tuple
 
 import torch
 from torch import nn
-import numpy as np
 from transformers import GPTBigCodeConfig
 
 from vllm.model_executor.input_metadata import InputMetadata
 from vllm.model_executor.layers.activation import get_act_fn
 from vllm.model_executor.layers.attention import PagedAttention
 from vllm.model_executor.layers.sampler import Sampler
 from vllm.model_executor.weight_utils import (hf_model_weights_iterator,
@@ -53,37 +52,61 @@
         tensor_model_parallel_world_size = (
             get_tensor_model_parallel_world_size())
         assert total_num_heads % tensor_model_parallel_world_size == 0
         self.num_heads = total_num_heads // tensor_model_parallel_world_size
         self.head_dim = self.hidden_size // total_num_heads
         self.scale = self.head_dim**-0.5
 
-        self.c_attn = ColumnParallelLinear(self.hidden_size,
-                                           3 * self.hidden_size,
-                                           bias=True,
-                                           gather_output=False,
-                                           perform_initialization=False)
+        self.multi_query = config.multi_query
+        if self.multi_query:
+            self.num_kv_heads = 1
+            self.kv_dim = self.head_dim
+            self.c_attn_q = ColumnParallelLinear(self.hidden_size,
+                                                 self.hidden_size,
+                                                 bias=True,
+                                                 gather_output=False,
+                                                 perform_initialization=False)
+            self.c_attn_kv = nn.Linear(self.hidden_size,
+                                       2 * self.kv_dim,
+                                       bias=True)
+        else:
+            self.num_kv_heads = self.num_heads
+            self.kv_dim = self.num_kv_heads * self.head_dim
+            self.c_attn = ColumnParallelLinear(self.hidden_size,
+                                               self.hidden_size +
+                                               2 * self.kv_dim,
+                                               bias=True,
+                                               gather_output=False,
+                                               perform_initialization=False)
+
         self.c_proj = RowParallelLinear(self.hidden_size,
                                         self.hidden_size,
                                         bias=True,
                                         input_is_parallel=True,
                                         perform_initialization=False)
         self.attn = PagedAttention(self.num_heads,
                                    self.head_dim,
-                                   scale=self.scale)
+                                   scale=self.scale,
+                                   num_kv_heads=self.num_kv_heads)
 
     def forward(
         self,
         hidden_states: torch.Tensor,
         kv_cache: KVCache,
         input_metadata: InputMetadata,
         cache_event: Optional[torch.cuda.Event],
     ) -> torch.Tensor:
-        qkv, _ = self.c_attn(hidden_states)
-        q, k, v = qkv.chunk(chunks=3, dim=-1)
+        if self.multi_query:
+            q, _ = self.c_attn_q(hidden_states)
+            kv = self.c_attn_kv(hidden_states)
+            k, v = kv.split([self.kv_dim, self.kv_dim], dim=-1)
+        else:
+            qkv, _ = self.c_attn(hidden_states)
+            q, k, v = qkv.split([self.hidden_size, self.kv_dim, self.kv_dim],
+                                dim=-1)
         key_cache, value_cache = kv_cache
         attn_output = self.attn(q, k, v, key_cache, value_cache,
                                 input_metadata, cache_event)
         attn_output, _ = self.c_proj(attn_output)
         return attn_output
 
 
@@ -244,88 +267,73 @@
                 # linear layer.
                 continue
             if ".attn.bias" in name:
                 # Skip attention mask.
                 # NOTE: "c_attn.bias" should not be skipped.
                 continue
 
-            param = state_dict[name]
-
             if not name.startswith("transformer."):
                 name = "transformer." + name
 
-            if name == "transformer.wte.weight":
-                # Consider padding in the vocab size.
-                padded_vocab_size = param.shape[
-                    0] * tensor_model_parallel_world_size
-                num_extra_rows = padded_vocab_size - self.config.vocab_size
-                extra_rows = torch.empty(num_extra_rows,
-                                         loaded_weight.shape[1])
-                extra_rows = extra_rows.to(loaded_weight)
-                loaded_weight = torch.cat([loaded_weight, extra_rows], dim=0)
-
-            def _expand_mqa_mha(qkv_array, n_head, head_dim):
-                """manipulates along axis=0 from MQA to MHA
-                inputs: qkv_array.shape=((n_heads + 2) * head_dim, hidden_dim)
-                    with n_heads for q, then 1 for k, 1 for 1 v, times head dim
-                return: qkv_array.shape=(3 * n_heads * head_dim, hidden_dim)
-
-                TODO: this function is no longer needed once vllm supports MQA.
-                """
-                qkv_array = qkv_array.numpy()
-
-                dims_q = n_head * head_dim
-                # pylint: disable=unbalanced-tuple-unpacking
-                q, k, v = np.split(qkv_array, (dims_q, dims_q + head_dim),
-                                   axis=0)
-                # q is fine, but k & v have not replicated shape along the first
-                # axis as long as MQA is not nativly supported, increase memory
-                # and replicated (head_dim, hidden_dim) to
-                # (n_heads * head_dim, hidden_dim)
-                if k.ndim == 2 and v.ndim == 2:
-                    replication = (n_head, 1)  # weights
-                else:
-                    replication = n_head  # biases
-                # replicate n_head times for q, v
-                k, v = np.tile(k, replication), np.tile(v, replication)
-                # concat q, k, v along the first axis
-                # (n_heads * head_dim, hidden_dim)
-                # to (3 * n_heads * head_dim, hidden_dim)
-                qkv_array = np.concatenate((q, k, v), axis=0)
-                return torch.from_numpy(qkv_array)
-
             # For the fused QKV linear layer, manually shard the weights.
             if "c_attn" in name:
                 # GPT-2's fused QKV has the shape of
                 # [3 * num_heads * head_size, hidden_size].
                 # When tensor parallelism is used, we shard the weights along
                 # the head dimension.
                 total_num_heads = self.config.num_attention_heads
+                total_num_kv_heads = (1 if self.config.multi_query else
+                                      total_num_heads)
                 hidden_size = self.config.hidden_size
                 head_size = hidden_size // total_num_heads
+                total_kv_size = head_size * total_num_kv_heads
                 num_heads = total_num_heads // tensor_model_parallel_world_size
                 head_start = tensor_model_parallel_rank * num_heads
                 head_end = (tensor_model_parallel_rank + 1) * num_heads
 
-                if name.endswith(".weight"):
-                    loaded_weight = _expand_mqa_mha(loaded_weight,
-                                                    n_head=total_num_heads,
-                                                    head_dim=head_size)
-                    loaded_weight = loaded_weight.view(3, total_num_heads,
-                                                       head_size, hidden_size)
-                    loaded_weight = loaded_weight[:, head_start:head_end, :, :]
-                    loaded_weight = loaded_weight.reshape(-1, hidden_size)
-                elif name.endswith(".bias"):
-                    loaded_weight = _expand_mqa_mha(loaded_weight,
-                                                    n_head=total_num_heads,
-                                                    head_dim=head_size)
-                    loaded_weight = loaded_weight.view(3, total_num_heads,
-                                                       head_size)
-                    loaded_weight = loaded_weight[:, head_start:head_end, :]
-                    loaded_weight = loaded_weight.reshape(-1)
+                wq, wk, wv = torch.split(
+                    loaded_weight, [hidden_size, total_kv_size, total_kv_size],
+                    dim=0)
+
+                wq = wq[head_size * head_start:head_size * head_end]
+                if not self.config.multi_query:
+                    # Split the heads when using normal multi-head attention
+                    wk = wk[head_size * head_start:head_size * head_end]
+                    wv = wv[head_size * head_start:head_size * head_end]
+                    loaded_weight = torch.cat([wq, wk, wv], dim=0)
                 else:
-                    raise ValueError(f"Unexpected parameter name {name}")
+                    # For multi-query attention, we split the query
+                    # but replicate the key and value.
+                    loaded_weight_q = wq
+                    loaded_weight_kv = torch.cat([wk, wv], dim=0)
+                    q_weight_name = name.replace("c_attn", "c_attn_q")
+                    kv_weight_name = name.replace("c_attn", "c_attn_kv")
+                    load_tensor_parallel_weights(state_dict[q_weight_name],
+                                                 loaded_weight_q,
+                                                 q_weight_name,
+                                                 self._column_parallel_weights,
+                                                 self._row_parallel_weights,
+                                                 tensor_model_parallel_rank)
+                    load_tensor_parallel_weights(state_dict[kv_weight_name],
+                                                 loaded_weight_kv,
+                                                 kv_weight_name,
+                                                 self._column_parallel_weights,
+                                                 self._row_parallel_weights,
+                                                 tensor_model_parallel_rank)
+                    continue
+
+            param = state_dict[name]
+
+            if name == "transformer.wte.weight":
+                # Consider padding in the vocab size.
+                padded_vocab_size = param.shape[
+                    0] * tensor_model_parallel_world_size
+                num_extra_rows = padded_vocab_size - self.config.vocab_size
+                extra_rows = torch.empty(num_extra_rows,
+                                         loaded_weight.shape[1])
+                extra_rows = extra_rows.to(loaded_weight)
+                loaded_weight = torch.cat([loaded_weight, extra_rows], dim=0)
 
             load_tensor_parallel_weights(param, loaded_weight, name,
                                          self._column_parallel_weights,
                                          self._row_parallel_weights,
                                          tensor_model_parallel_rank)
```

### Comparing `vllm-0.1.2/vllm/model_executor/models/gpt_neox.py` & `vllm-0.1.3/vllm/model_executor/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/models/llama.py` & `vllm-0.1.3/vllm/model_executor/models/llama.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,55 +80,61 @@
 
 class LlamaAttention(nn.Module):
 
     def __init__(
         self,
         hidden_size: int,
         num_heads: int,
+        num_kv_heads: int,
     ):
         super().__init__()
         self.hidden_size = hidden_size
-        tensor_model_parallel_world_size = (
-            get_tensor_model_parallel_world_size())
+        tp_size = get_tensor_model_parallel_world_size()
         self.total_num_heads = num_heads
-        assert self.total_num_heads % tensor_model_parallel_world_size == 0
-        self.num_heads = (self.total_num_heads //
-                          tensor_model_parallel_world_size)
+        assert self.total_num_heads % tp_size == 0
+        self.num_heads = self.total_num_heads // tp_size
+        self.total_num_kv_heads = num_kv_heads
+        assert self.total_num_kv_heads % tp_size == 0
+        self.num_kv_heads = self.total_num_kv_heads // tp_size
         self.head_dim = hidden_size // self.total_num_heads
+        self.q_size = self.num_heads * self.head_dim
+        self.kv_size = self.num_kv_heads * self.head_dim
         self.scaling = self.head_dim**-0.5
 
         self.qkv_proj = ColumnParallelLinear(
             hidden_size,
-            3 * self.total_num_heads * self.head_dim,
+            (self.total_num_heads + 2 * self.total_num_kv_heads) *
+            self.head_dim,
             bias=False,
             gather_output=False,
             perform_initialization=False,
         )
         self.o_proj = RowParallelLinear(
             self.total_num_heads * self.head_dim,
             hidden_size,
             bias=False,
             input_is_parallel=True,
             perform_initialization=False,
         )
         self.attn = PagedAttentionWithRoPE(self.num_heads,
                                            self.head_dim,
                                            self.scaling,
-                                           rotary_dim=self.head_dim)
+                                           rotary_dim=self.head_dim,
+                                           num_kv_heads=self.num_kv_heads)
 
     def forward(
         self,
         positions: torch.Tensor,
         hidden_states: torch.Tensor,
         kv_cache: KVCache,
         input_metadata: InputMetadata,
         cache_event: Optional[torch.cuda.Event],
     ) -> torch.Tensor:
         qkv, _ = self.qkv_proj(hidden_states)
-        q, k, v = qkv.chunk(chunks=3, dim=-1)
+        q, k, v = qkv.split([self.q_size, self.kv_size, self.kv_size], dim=-1)
         k_cache, v_cache = kv_cache
         attn_output = self.attn(positions, q, k, v, k_cache, v_cache,
                                 input_metadata, cache_event)
         output, _ = self.o_proj(attn_output)
         return output
 
 
@@ -136,14 +142,15 @@
 
     def __init__(self, config: LlamaConfig):
         super().__init__()
         self.hidden_size = config.hidden_size
         self.self_attn = LlamaAttention(
             hidden_size=self.hidden_size,
             num_heads=config.num_attention_heads,
+            num_kv_heads=config.num_key_value_heads,
         )
         self.mlp = LlamaMLP(
             hidden_size=self.hidden_size,
             intermediate_size=config.intermediate_size,
             hidden_act=config.hidden_act,
         )
         self.input_layernorm = RMSNorm(config.hidden_size,
@@ -183,18 +190,17 @@
 
     def __init__(self, config: LlamaConfig):
         super().__init__()
         self.config = config
         self.padding_idx = config.pad_token_id
         self.vocab_size = config.vocab_size
 
+        vocab_size = ((config.vocab_size + 63) // 64) * 64
         self.embed_tokens = VocabParallelEmbedding(
-            config.vocab_size,
-            config.hidden_size,
-            perform_initialization=False)
+            vocab_size, config.hidden_size, perform_initialization=False)
         self.layers = nn.ModuleList([
             LlamaDecoderLayer(config) for _ in range(config.num_hidden_layers)
         ])
         self.norm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
     def forward(
         self,
@@ -224,16 +230,17 @@
 
 class LlamaForCausalLM(nn.Module):
 
     def __init__(self, config):
         super().__init__()
         self.config = config
         self.model = LlamaModel(config)
+        vocab_size = ((config.vocab_size + 63) // 64) * 64
         self.lm_head = ColumnParallelLinear(config.hidden_size,
-                                            config.vocab_size,
+                                            vocab_size,
                                             bias=False,
                                             gather_output=False,
                                             perform_initialization=False)
         self.sampler = Sampler(config.vocab_size)
 
     def forward(
         self,
@@ -255,35 +262,56 @@
     ]
     _row_parallel_weights = ["o_proj.weight", "down_proj.weight"]
 
     def load_weights(self,
                      model_name_or_path: str,
                      cache_dir: Optional[str] = None,
                      use_np_cache: bool = False):
+        tp_size = get_tensor_model_parallel_world_size()
         tensor_model_parallel_rank = get_tensor_model_parallel_rank()
+        q_proj_shard_size = (self.config.hidden_size // tp_size)
+        kv_proj_shard_size = (self.config.hidden_size //
+                              self.config.num_attention_heads *
+                              self.config.num_key_value_heads // tp_size)
+        attention_weight_specs = [
+            # (weight_name, shard_size, offset)
+            ("q_proj", q_proj_shard_size, 0),
+            ("k_proj", kv_proj_shard_size, q_proj_shard_size),
+            ("v_proj", kv_proj_shard_size,
+             q_proj_shard_size + kv_proj_shard_size),
+        ]
         state_dict = self.state_dict()
 
         for name, loaded_weight in hf_model_weights_iterator(
                 model_name_or_path, cache_dir, use_np_cache):
             if "rotary_emb.inv_freq" in name:
                 continue
 
+            if "embed_tokens" in name or "lm_head" in name:
+                param = state_dict[name]
+                # Consider padding in the vocab size.
+                padded_vocab_size = (param.shape[0] * tp_size)
+                num_extra_rows = padded_vocab_size - self.config.vocab_size
+                extra_rows = torch.empty(num_extra_rows,
+                                         loaded_weight.shape[1])
+                extra_rows = extra_rows.to(loaded_weight)
+                loaded_weight = torch.cat([loaded_weight, extra_rows], dim=0)
+
             is_attention_weight = False
-            for stride_id, att_weight_name in enumerate(
-                ["q_proj", "k_proj", "v_proj"]):
-                if att_weight_name not in name:
+            for weight_name, shard_size, offset in attention_weight_specs:
+                if weight_name not in name:
                     continue
-                param = state_dict[name.replace(att_weight_name, "qkv_proj")]
-                shard_size = param.shape[0] // 3
+                param = state_dict[name.replace(weight_name, "qkv_proj")]
+
                 loaded_weight = loaded_weight[
                     shard_size * tensor_model_parallel_rank:shard_size *
                     (tensor_model_parallel_rank + 1)]
-                param_slice = param.data[shard_size * stride_id:shard_size *
-                                         (stride_id + 1)]
+                param_slice = param.data[offset:offset + shard_size]
                 assert param_slice.shape == loaded_weight.shape
+
                 param_slice.copy_(loaded_weight)
                 is_attention_weight = True
                 break
             if is_attention_weight:
                 continue
 
             is_gate_up_weight = False
```

### Comparing `vllm-0.1.2/vllm/model_executor/models/mpt.py` & `vllm-0.1.3/vllm/model_executor/models/mpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 # Adapted from https://huggingface.co/mosaicml/mpt-7b/tree/main
 import math
 from typing import Dict, List, Optional, Tuple
 
 import torch
 import torch.nn as nn
```

### Comparing `vllm-0.1.2/vllm/model_executor/models/opt.py` & `vllm-0.1.3/vllm/model_executor/models/opt.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/parallel_utils/parallel_state.py` & `vllm-0.1.3/vllm/model_executor/parallel_utils/parallel_state.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 # rank when broadcasting from the first or last pipeline stage.
 _PIPELINE_GLOBAL_RANKS = None
 
 # A list of global ranks for each data parallel group to ease calculation of the source
 # rank when broadcasting weights from src to all other data parallel ranks
 _DATA_PARALLEL_GLOBAL_RANKS = None
 
-_ALL_REDUCE_LAUNCHER: Optional['GraphAllReduce'] = None
 
 def initialize_model_parallel(
     tensor_model_parallel_size: int = 1,
     pipeline_model_parallel_size: int = 1,
     virtual_pipeline_model_parallel_size: Optional[int] = None,
     pipeline_model_parallel_split_rank: Optional[int] = None,
 ) -> None:
@@ -192,28 +191,14 @@
 
         group = torch.distributed.new_group(position_embedding_ranks)
         if rank in position_embedding_ranks:
             _POSITION_EMBEDDING_GROUP = group
         if rank in ranks:
             _POSITION_EMBEDDING_GLOBAL_RANKS = position_embedding_ranks
 
-def initialize_all_reduce_launcher(
-    max_num_tokens: int,
-    hidden_size: int,
-    dtype: torch.dtype,
-    disable_graph: bool = False,
-) -> None:
-    global _ALL_REDUCE_LAUNCHER
-    _ALL_REDUCE_LAUNCHER = GraphAllReduce(
-        max_num_tokens=max_num_tokens,
-        hidden_size=hidden_size,
-        dtype=dtype,
-        disable_graph=disable_graph,
-    )
-
 def model_parallel_is_initialized():
     """Check if model and data parallel groups are initialized."""
     if _TENSOR_MODEL_PARALLEL_GROUP is None or \
         _PIPELINE_MODEL_PARALLEL_GROUP is None or \
         _DATA_PARALLEL_GROUP is None:
         return False
     return True
@@ -454,14 +439,15 @@
     """Return the global rank of the last process in the pipeline for the
     current tensor parallel group"""
     assert _PIPELINE_GLOBAL_RANKS is not None, \
         "Pipeline parallel group is not initialized"
     last_rank_local = get_pipeline_model_parallel_world_size() - 1
     return _PIPELINE_GLOBAL_RANKS[last_rank_local]
 
+
 def get_pipeline_model_parallel_next_rank():
     """Return the global rank that follows the caller in the pipeline"""
     assert _PIPELINE_GLOBAL_RANKS is not None, \
         "Pipeline parallel group is not initialized"
     rank_in_pipeline = get_pipeline_model_parallel_rank()
     world_size = get_pipeline_model_parallel_world_size()
     return _PIPELINE_GLOBAL_RANKS[(rank_in_pipeline + 1) % world_size]
@@ -481,18 +467,14 @@
     return torch.distributed.get_world_size(group=get_data_parallel_group())
 
 
 def get_data_parallel_rank():
     """Return my rank for the data parallel group."""
     return torch.distributed.get_rank(group=get_data_parallel_group())
 
-def get_all_reduce_launcher() -> 'GraphAllReduce':
-    assert _ALL_REDUCE_LAUNCHER is not None, 'all reduce launcher is not initialized'
-    return _ALL_REDUCE_LAUNCHER
-
 def destroy_model_parallel():
     """Set the groups to none."""
     global _MODEL_PARALLEL_GROUP
     _MODEL_PARALLEL_GROUP = None
     global _TENSOR_MODEL_PARALLEL_GROUP
     _TENSOR_MODEL_PARALLEL_GROUP = None
     global _PIPELINE_MODEL_PARALLEL_GROUP
@@ -511,60 +493,7 @@
     _MPU_TENSOR_MODEL_PARALLEL_WORLD_SIZE = None
     global _MPU_PIPELINE_MODEL_PARALLEL_WORLD_SIZE
     _MPU_PIPELINE_MODEL_PARALLEL_WORLD_SIZE = None
     global _MPU_TENSOR_MODEL_PARALLEL_RANK
     _MPU_TENSOR_MODEL_PARALLEL_RANK = None
     global _MPU_PIPELINE_MODEL_PARALLEL_RANK
     _MPU_PIPELINE_MODEL_PARALLEL_RANK = None
-
-
-class GraphAllReduce:
-
-    def __init__(
-        self,
-        max_num_tokens: int,
-        hidden_size: int,
-        dtype: torch.dtype,
-        disable_graph: bool = False,
-    ) -> None:
-        self.max_num_tokens = max_num_tokens
-        self.hidden_size = hidden_size
-        self.disable_graph = disable_graph
-
-        tp_world_size = get_tensor_model_parallel_world_size()
-        if tp_world_size == 1:
-            return
-
-        self.group = get_tensor_model_parallel_group()
-        self.buffer = torch.empty(
-            size=(max_num_tokens, hidden_size),
-            dtype=dtype,
-            device='cuda',
-        )
-
-        # Build graphs for different number of tokens.
-        if not self.disable_graph:
-            self.graphs = {}
-            for num_tokens in range(8, max_num_tokens + 1, 8):
-                self.graphs[num_tokens] = self._build_graph(num_tokens)
-
-    def _build_graph(self, num_tokens: int) -> torch.cuda.CUDAGraph:
-        # Warm up.
-        torch.distributed.all_reduce(self.buffer[:num_tokens], group=self.group)
-        torch.cuda.synchronize()
-
-        # Build graph.
-        graph = torch.cuda.CUDAGraph()
-        with torch.cuda.graph(graph):
-            torch.distributed.all_reduce(
-                self.buffer[:num_tokens], group=self.group)
-        torch.cuda.synchronize()
-        return graph
-
-    def launch(self, x: torch.Tensor) -> torch.Tensor:
-        # NOTE: x must be a slice of self.buffer.
-        num_tokens = x.shape[0]
-        if self.disable_graph:
-            torch.distributed.all_reduce(x, group=self.group)
-        else:
-            self.graphs[num_tokens].replay()
-        return x
```

### Comparing `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py` & `vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     param_is_not_tensor_parallel_duplicate,
 )
 
 from .mappings import (
     copy_to_tensor_model_parallel_region,
     gather_from_tensor_model_parallel_region,
     gather_from_sequence_parallel_region,
+    reduce_from_tensor_model_parallel_region,
     scatter_to_tensor_model_parallel_region,
     scatter_to_sequence_parallel_region,
 )
 
 from .random import (
     get_cuda_rng_tracker,
     model_parallel_cuda_manual_seed,
@@ -34,15 +35,15 @@
     "set_defaults_if_not_set_tensor_model_parallel_attributes",
     "copy_tensor_model_parallel_attributes",
     "param_is_not_tensor_parallel_duplicate",
     # mappings.py
     "copy_to_tensor_model_parallel_region",
     "gather_from_tensor_model_parallel_region",
     "gather_from_sequence_parallel_region",
-#    "reduce_from_tensor_model_parallel_region",
+    "reduce_from_tensor_model_parallel_region",
     "scatter_to_tensor_model_parallel_region",
     "scatter_to_sequence_parallel_region",
     # random.py
     "get_cuda_rng_tracker",
     "model_parallel_cuda_manual_seed",
     # utils.py
     "split_tensor_along_last_dim",
```

### Comparing `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/layers.py` & `vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import torch.nn.functional as F
 import torch.nn.init as init
 from torch.nn.parameter import Parameter
 
 from vllm.model_executor.parallel_utils.parallel_state import (
     get_tensor_model_parallel_rank,
     get_tensor_model_parallel_world_size,
-    get_all_reduce_launcher,
 )
 from .mappings import (
     copy_to_tensor_model_parallel_region,
     gather_from_tensor_model_parallel_region,
     reduce_from_tensor_model_parallel_region,
     scatter_to_tensor_model_parallel_region,
 )
@@ -244,16 +243,16 @@
         super(ColumnParallelLinear, self).__init__()
 
         # Keep input parameters
         self.input_size = input_size
         self.output_size = output_size
         self.gather_output = gather_output
         # Divide the weight matrix along the last dimension.
-        world_size = get_tensor_model_parallel_world_size()
-        self.output_size_per_partition = divide(output_size, world_size)
+        self.world_size = get_tensor_model_parallel_world_size()
+        self.output_size_per_partition = divide(output_size, self.world_size)
         self.skip_bias_add = skip_bias_add
 
         if params_dtype is None:
             params_dtype = torch.get_default_dtype()
 
         # Parameters.
         # Note: torch.nn.functional.linear performs XA^T + b and as a result
@@ -346,39 +345,46 @@
                                      used for initialization.
         skip_bias_add: This was added to enable performance optimization where bias
                        can be fused with other elementwise operations. We skip
                        adding bias but instead return it.
         params_dtype:
         use_cpu_initialization:
         perform_initialization:
+        reduce_results:
     """
 
     def __init__(self, input_size, output_size, *,
                  bias=True, input_is_parallel=False,
                  init_method=init.xavier_normal_, stride=1,
                  keep_master_weight_for_test=False,
                  skip_bias_add=False,
                  params_dtype=None,
                  use_cpu_initialization=False,
                  perform_initialization=True,
+                 reduce_results=True,
                  ):
         super(RowParallelLinear, self).__init__()
 
         # Keep input parameters
         self.input_size = input_size
         self.output_size = output_size
         self.input_is_parallel = input_is_parallel
+        self.reduce_results = reduce_results
         if params_dtype is None:
             params_dtype = torch.get_default_dtype()
 
         # Divide the weight matrix along the last dimension.
-        world_size = get_tensor_model_parallel_world_size()
-        self.input_size_per_partition = divide(input_size, world_size)
+        self.world_size = get_tensor_model_parallel_world_size()
+        self.input_size_per_partition = divide(input_size, self.world_size)
         self.skip_bias_add = skip_bias_add
 
+        if not reduce_results and (bias and not skip_bias_add):
+            raise ValueError("When not reduce the results, adding bias to the "
+                             "results can lead to incorrect results")
+
         # Parameters.
         # Note: torch.nn.functional.linear performs XA^T + b and as a result
         # we allocate the transpose.
         # Initialize weight.
         if use_cpu_initialization:
             self.weight = Parameter(torch.empty(self.output_size,
                                                 self.input_size_per_partition,
@@ -423,25 +429,20 @@
             - bias
         """
         # Set up backprop all-reduce.
         if self.input_is_parallel:
             input_parallel = input_
         else:
             input_parallel = scatter_to_tensor_model_parallel_region(input_)
-        if get_tensor_model_parallel_world_size() == 1:
-            # Matrix multiply.
-            output_ = F.linear(input_parallel, self.weight)
+        # Matrix multiply.
+        output_parallel = F.linear(input_parallel, self.weight)
+        if self.reduce_results and self.world_size > 1:
+            output_ = reduce_from_tensor_model_parallel_region(output_parallel)
         else:
-            # Matrix multiply.
-            all_reduce_launcher = get_all_reduce_launcher()
-            num_tokens = input_parallel.shape[0]
-            output_buffer = all_reduce_launcher.buffer[:num_tokens]
-            torch.matmul(input_parallel, self.weight_t, out=output_buffer)
-            # All-reduce across all the partitions.
-            output_ = all_reduce_launcher.launch(output_buffer)
+            output_ = output_parallel
 
         if not self.skip_bias_add:
             output = output_ + self.bias if self.bias is not None else output_
             output_bias = None
         else:
             output = output_
             output_bias = self.bias
```

### Comparing `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py` & `vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/random.py` & `vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/random.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/utils.py` & `vllm-0.1.3/vllm/model_executor/parallel_utils/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/utils.py` & `vllm-0.1.3/vllm/model_executor/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/model_executor/weight_utils.py` & `vllm-0.1.3/vllm/model_executor/weight_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,18 @@
             hf_folder = snapshot_download(model_name_or_path,
                                           allow_patterns="*.bin",
                                           cache_dir=cache_dir,
                                           tqdm_class=Disabledtqdm)
     else:
         hf_folder = model_name_or_path
 
-    hf_bin_files = glob.glob(os.path.join(hf_folder, "*.bin"))
+    hf_bin_files = [
+        x for x in glob.glob(os.path.join(hf_folder, "*.bin"))
+        if not x.endswith("training_args.bin")
+    ]
 
     if use_np_cache:
         # Convert the model weights from torch tensors to numpy arrays for
         # faster loading.
         np_folder = os.path.join(hf_folder, "np")
         os.makedirs(np_folder, exist_ok=True)
         weight_names_file = os.path.join(np_folder, "weight_names.json")
```

### Comparing `vllm-0.1.2/vllm/outputs.py` & `vllm-0.1.3/vllm/outputs.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/sampling_params.py` & `vllm-0.1.3/vllm/sampling_params.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/sequence.py` & `vllm-0.1.3/vllm/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,26 +123,28 @@
         block = LogicalTokenBlock(
             block_number=len(self.logical_token_blocks),
             block_size=self.block_size,
         )
         self.logical_token_blocks.append(block)
 
     def _append_tokens_to_blocks(self, token_ids: List[int]) -> None:
-        while token_ids:
+        cursor = 0
+        while cursor < len(token_ids):
             if not self.logical_token_blocks:
                 self._append_logical_block()
 
             last_block = self.logical_token_blocks[-1]
             if last_block.is_full():
                 self._append_logical_block()
                 last_block = self.logical_token_blocks[-1]
 
             num_empty_slots = last_block.get_num_empty_slots()
-            last_block.append_tokens(token_ids[:num_empty_slots])
-            token_ids = token_ids[num_empty_slots:]
+            last_block.append_tokens(token_ids[cursor:cursor +
+                                               num_empty_slots])
+            cursor += num_empty_slots
 
     def append_token_id(
         self,
         token_id: int,
         logprobs: Dict[int, float],
     ) -> None:
         assert token_id in logprobs
```

### Comparing `vllm-0.1.2/vllm/transformers_utils/configs/mpt.py` & `vllm-0.1.3/vllm/transformers_utils/configs/mpt.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/transformers_utils/tokenizer.py` & `vllm-0.1.3/vllm/transformers_utils/tokenizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 _FAST_LLAMA_TOKENIZER = "hf-internal-testing/llama-tokenizer"
 
 
 def get_tokenizer(
     tokenizer_name: str,
     *args,
     tokenizer_mode: str = "auto",
+    trust_remote_code: bool = False,
     **kwargs,
 ) -> Union[PreTrainedTokenizer, PreTrainedTokenizerFast]:
     """Gets a tokenizer for the given model name via Huggingface."""
     if tokenizer_mode == "slow":
         if kwargs.get("use_fast", False):
             raise ValueError(
                 "Cannot use the fast tokenizer in slow tokenizer mode.")
@@ -27,23 +28,40 @@
     if "llama" in tokenizer_name.lower() and kwargs.get("use_fast", True):
         logger.info(
             "For some LLaMA-based models, initializing the fast tokenizer may "
             "take a long time. To eliminate the initialization time, consider "
             f"using '{_FAST_LLAMA_TOKENIZER}' instead of the original "
             "tokenizer.")
     try:
-        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name, *args,
-                                                  **kwargs)
+        tokenizer = AutoTokenizer.from_pretrained(
+            tokenizer_name,
+            *args,
+            trust_remote_code=trust_remote_code,
+            **kwargs)
     except TypeError as e:
         # The LLaMA tokenizer causes a protobuf error in some environments.
         err_msg = (
             "Failed to load the tokenizer. If you are using a LLaMA-based "
             f"model, use '{_FAST_LLAMA_TOKENIZER}' instead of the original "
             "tokenizer.")
         raise RuntimeError(err_msg) from e
+    except ValueError as e:
+        # If the error pertains to the tokenizer class not existing or not
+        # currently being imported, suggest using the --trust-remote-code flag.
+        if (not trust_remote_code and
+            ("does not exist or is not currently imported." in str(e)
+             or "requires you to execute the tokenizer file" in str(e))):
+            err_msg = (
+                "Failed to load the tokenizer. If the tokenizer is a custom "
+                "tokenizer not yet available in the HuggingFace transformers "
+                "library, consider setting `trust_remote_code=True` in LLM "
+                "or using the `--trust-remote-code` flag in the CLI.")
+            raise RuntimeError(err_msg) from e
+        else:
+            raise e
 
     if not isinstance(tokenizer, PreTrainedTokenizerFast):
         logger.warning(
             "Using a slow tokenizer. This might cause a significant "
             "slowdown. Consider using a fast tokenizer instead.")
     return tokenizer
 
@@ -58,14 +76,16 @@
 
     NOTE: This function does not update prev_output_tokens.
 
     Returns:
         new_token: The new token as a string.
         output_text: The new output text as a string.
     """
+    if skip_special_tokens and (new_token_id in tokenizer.all_special_ids):
+        return None, prev_output_tokens
     new_token = tokenizer.convert_ids_to_tokens(
         new_token_id, skip_special_tokens=skip_special_tokens)
     output_tokens = prev_output_tokens + [new_token]
 
     # Convert the tokens to a string.
     # Optimization: If the tokenizer does not have `added_tokens_encoder`,
     # then we can directly use `convert_tokens_to_string`.
@@ -77,15 +97,15 @@
     # https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/tokenization_utils.py#L921
     # NOTE(woosuk): The following code is slow because it runs a for loop over
     # the output_tokens. In Python, running a for loop over a list can be slow
     # even when the loop body is very simple.
     sub_texts = []
     current_sub_text = []
     for token in output_tokens:
-        if skip_special_tokens and token in tokenizer.all_special_ids:
+        if skip_special_tokens and token in tokenizer.all_special_tokens:
             continue
         if token in tokenizer.added_tokens_encoder:
             if current_sub_text:
                 sub_text = tokenizer.convert_tokens_to_string(current_sub_text)
                 sub_texts.append(sub_text)
                 current_sub_text = []
             sub_texts.append(token)
```

### Comparing `vllm-0.1.2/vllm/utils.py` & `vllm-0.1.3/vllm/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/worker/cache_engine.py` & `vllm-0.1.3/vllm/worker/cache_engine.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.2/vllm/worker/worker.py` & `vllm-0.1.3/vllm/worker/worker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """A GPU worker class."""
-from typing import Dict, List, Tuple
+import os
+from typing import Dict, List, Tuple, Optional
 
 import torch
+import torch.distributed
 
 from vllm.config import (CacheConfig, ModelConfig, ParallelConfig,
                          SchedulerConfig)
 from vllm.model_executor import get_model, InputMetadata, set_random_seed
 from vllm.model_executor.parallel_utils.parallel_state import (
-    initialize_model_parallel, initialize_all_reduce_launcher)
+    initialize_model_parallel)
 from vllm.sampling_params import SamplingParams
 from vllm.sequence import SequenceData, SequenceGroupMetadata, SequenceOutputs
 from vllm.worker.cache_engine import CacheEngine
 from vllm.utils import get_gpu_memory
 
 
 class Worker:
@@ -23,44 +25,51 @@
     """
 
     def __init__(
         self,
         model_config: ModelConfig,
         parallel_config: ParallelConfig,
         scheduler_config: SchedulerConfig,
-        rank: int,
-        distributed_init_method: str,
+        rank: Optional[int] = None,
+        distributed_init_method: Optional[str] = None,
     ) -> None:
         self.model_config = model_config
         self.parallel_config = parallel_config
         self.scheduler_config = scheduler_config
         self.rank = rank
         self.distributed_init_method = distributed_init_method
 
-        # Initialize the distributed environment.
-        _init_distributed_environment(parallel_config, rank,
-                                      distributed_init_method)
-
-        # Initialize the model.
-        set_random_seed(self.model_config.seed)
-        self.model = get_model(model_config)
-        initialize_all_reduce_launcher(
-            self.scheduler_config.max_num_batched_tokens,
-            self.model_config.get_hidden_size(),
-            self.model_config.dtype,
-        )
-
         # Uninitialized cache engine. Will be initialized by
         # self.init_cache_engine().
         self.cache_config = None
         self.block_size = None
         self.cache_engine = None
         self.cache_events = None
         self.gpu_cache = None
 
+    def init_model(self):
+        # This env var set by Ray causes exceptions with graph building.
+        os.environ.pop("NCCL_ASYNC_ERROR_HANDLING", None)
+        # Env vars will be set by Ray.
+        self.rank = self.rank if self.rank is not None else int(
+            os.getenv("RANK", "-1"))
+        local_rank = int(os.getenv("LOCAL_RANK", "0"))
+        self.device = torch.device(f"cuda:{local_rank}")
+        if self.rank < 0:
+            raise ValueError("Invalid or unspecified rank.")
+        torch.cuda.set_device(self.device)
+
+        # Initialize the distributed environment.
+        _init_distributed_environment(self.parallel_config, self.rank,
+                                      self.distributed_init_method)
+
+        # Initialize the model.
+        set_random_seed(self.model_config.seed)
+        self.model = get_model(self.model_config)
+
     @torch.inference_mode()
     def profile_num_available_blocks(
         self,
         block_size: int,
         gpu_memory_utilization: float,
         cpu_swap_space: int,
     ) -> Tuple[int, int]:
@@ -290,23 +299,36 @@
         )
         return output
 
 
 def _init_distributed_environment(
     parallel_config: ParallelConfig,
     rank: int,
-    distributed_init_method: str,
+    distributed_init_method: Optional[str] = None,
 ) -> None:
     """Initialize the distributed environment."""
-    torch.distributed.init_process_group(
-        backend="nccl",
-        world_size=parallel_config.world_size,
-        rank=rank,
-        init_method=distributed_init_method,
-    )
+    if torch.distributed.is_initialized():
+        torch_world_size = torch.distributed.get_world_size()
+        if torch_world_size != parallel_config.world_size:
+            raise RuntimeError(
+                "torch.distributed is already initialized but the torch world "
+                "size does not match parallel_config.world_size "
+                f"({torch_world_size} vs. {parallel_config.world_size}).")
+    elif not distributed_init_method:
+        raise ValueError(
+            "distributed_init_method must be set if torch.distributed "
+            "is not already initialized")
+    else:
+        torch.distributed.init_process_group(
+            backend="nccl",
+            world_size=parallel_config.world_size,
+            rank=rank,
+            init_method=distributed_init_method,
+        )
+
     # A small all_reduce for warmup.
     torch.distributed.all_reduce(torch.zeros(1).cuda())
     initialize_model_parallel(parallel_config.tensor_parallel_size,
                               parallel_config.pipeline_parallel_size)
 
 
 def _pad_to_alignment(x: List[int], multiple_of: int) -> List[int]:
```

### Comparing `vllm-0.1.2/vllm.egg-info/PKG-INFO` & `vllm-0.1.3/vllm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vllm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A high-throughput and memory-efficient inference and serving engine for LLMs
 Home-page: https://github.com/vllm-project/vllm
 Author: vLLM Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/vllm-project/vllm
 Project-URL: Documentation, https://vllm.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
@@ -31,14 +31,15 @@
 | <a href="https://vllm.readthedocs.io/en/latest/"><b>Documentation</b></a> | <a href="https://vllm.ai"><b>Blog</b></a> | <a href="https://github.com/vllm-project/vllm/discussions"><b>Discussions</b></a> |
 
 </p>
 
 ---
 
 *Latest News* 🔥
+- [2023/07] Added support for LLaMA-2! You can run and serve 7B/13B/70B LLaMA-2s on vLLM with a single command!
 - [2023/06] Serving vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo, and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the clouds.
 - [2023/06] We officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog post](https://vllm.ai).
 
 ---
 
 vLLM is a fast and easy-to-use library for LLM inference and serving.
 
@@ -55,19 +56,22 @@
 - High-throughput serving with various decoding algorithms, including *parallel sampling*, *beam search*, and more
 - Tensor parallelism support for distributed inference
 - Streaming outputs
 - OpenAI-compatible API server
 
 vLLM seamlessly supports many Huggingface models, including the following architectures:
 
+- Baichuan (`baichuan-inc/Baichuan-7B`, `baichuan-inc/Baichuan-13B-Chat`, etc.)
 - BLOOM (`bigscience/bloom`, `bigscience/bloomz`, etc.)
+- Falcon (`tiiuae/falcon-7b`, `tiiuae/falcon-40b`, `tiiuae/falcon-rw-7b`, etc.)
 - GPT-2 (`gpt2`, `gpt2-xl`, etc.)
 - GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.)
+- GPT-J (`EleutherAI/gpt-j-6b`, `nomic-ai/gpt4all-j`, etc.)
 - GPT-NeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
-- LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
+- LLaMA & LLaMA-2 (`meta-llama/Llama-2-70b-hf`, `lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
 - MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.)
 - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
 
 Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-source):
 
 ```bash
 pip install vllm
```

#### html2text {}

```diff
@@ -1,53 +1,58 @@
-Metadata-Version: 2.1 Name: vllm Version: 0.1.2 Summary: A high-throughput and
+Metadata-Version: 2.1 Name: vllm Version: 0.1.3 Summary: A high-throughput and
 memory-efficient inference and serving engine for LLMs Home-page: https://
 github.com/vllm-project/vllm Author: vLLM Team License: Apache 2.0 Project-URL:
 Homepage, https://github.com/vllm-project/vllm Project-URL: Documentation,
 https://vllm.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE
                                      [vLLM]
            **** Easy, fast, and cheap LLM serving for everyone ****
                     | Documentation | Blog | Discussions |
---- *Latest News* ð¥ - [2023/06] Serving vLLM On any Cloud with SkyPilot.
-Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/
-master/llm/vllm) to start the vLLM demo, and the [blog post](https://
-blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/
-) for the story behind vLLM development on the clouds. - [2023/06] We
-officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna
-and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog
-post](https://vllm.ai). --- vLLM is a fast and easy-to-use library for LLM
-inference and serving. vLLM is fast with: - State-of-the-art serving throughput
-- Efficient management of attention key and value memory with
-**PagedAttention** - Continuous batching of incoming requests - Optimized CUDA
-kernels vLLM is flexible and easy to use with: - Seamless integration with
-popular HuggingFace models - High-throughput serving with various decoding
-algorithms, including *parallel sampling*, *beam search*, and more - Tensor
-parallelism support for distributed inference - Streaming outputs - OpenAI-
-compatible API server vLLM seamlessly supports many Huggingface models,
-including the following architectures: - BLOOM (`bigscience/bloom`,
-`bigscience/bloomz`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) - GPT BigCode
-(`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) - GPT-NeoX
+--- *Latest News* ð¥ - [2023/07] Added support for LLaMA-2! You can run and
+serve 7B/13B/70B LLaMA-2s on vLLM with a single command! - [2023/06] Serving
+vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://
+github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo,
+and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-
+cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the
+clouds. - [2023/06] We officially released vLLM! FastChat-vLLM integration has
+powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-
+April. Check out our [blog post](https://vllm.ai). --- vLLM is a fast and easy-
+to-use library for LLM inference and serving. vLLM is fast with: - State-of-
+the-art serving throughput - Efficient management of attention key and value
+memory with **PagedAttention** - Continuous batching of incoming requests -
+Optimized CUDA kernels vLLM is flexible and easy to use with: - Seamless
+integration with popular HuggingFace models - High-throughput serving with
+various decoding algorithms, including *parallel sampling*, *beam search*, and
+more - Tensor parallelism support for distributed inference - Streaming outputs
+- OpenAI-compatible API server vLLM seamlessly supports many Huggingface
+models, including the following architectures: - Baichuan (`baichuan-inc/
+Baichuan-7B`, `baichuan-inc/Baichuan-13B-Chat`, etc.) - BLOOM (`bigscience/
+bloom`, `bigscience/bloomz`, etc.) - Falcon (`tiiuae/falcon-7b`, `tiiuae/
+falcon-40b`, `tiiuae/falcon-rw-7b`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) -
+GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) -
+GPT-J (`EleutherAI/gpt-j-6b`, `nomic-ai/gpt4all-j`, etc.) - GPT-NeoX
 (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-
-tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`,
-`openlm-research/open_llama_13b`, etc.) - MPT (`mosaicml/mpt-7b`, `mosaicml/
-mpt-30b`, etc.) - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
-Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/
-getting_started/installation.html#build-from-source): ```bash pip install vllm
-``` ## Getting Started Visit our [documentation](https://vllm.readthedocs.io/
-en/latest/) to get started. - [Installation](https://vllm.readthedocs.io/en/
-latest/getting_started/installation.html) - [Quickstart](https://
-vllm.readthedocs.io/en/latest/getting_started/quickstart.html) - [Supported
-Models](https://vllm.readthedocs.io/en/latest/models/supported_models.html) ##
-Performance vLLM outperforms HuggingFace Transformers (HF) by up to 24x and
-Text Generation Inference (TGI) by up to 3.5x, in terms of throughput. For
-details, check out our [blog post](https://vllm.ai).
+tuned-alpha-7b`, etc.) - LLaMA & LLaMA-2 (`meta-llama/Llama-2-70b-hf`, `lmsys/
+vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.) -
+MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.) - OPT (`facebook/opt-66b`,
+`facebook/opt-iml-max-30b`, etc.) Install vLLM with pip or [from source](https:
+//vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-
+source): ```bash pip install vllm ``` ## Getting Started Visit our
+[documentation](https://vllm.readthedocs.io/en/latest/) to get started. -
+[Installation](https://vllm.readthedocs.io/en/latest/getting_started/
+installation.html) - [Quickstart](https://vllm.readthedocs.io/en/latest/
+getting_started/quickstart.html) - [Supported Models](https://
+vllm.readthedocs.io/en/latest/models/supported_models.html) ## Performance vLLM
+outperforms HuggingFace Transformers (HF) by up to 24x and Text Generation
+Inference (TGI) by up to 3.5x, in terms of throughput. For details, check out
+our [blog post](https://vllm.ai).
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n1_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n1_light.png]
       Serving throughput when each request asks for 1 output completion.
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n3_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n3_light.png]
```

### Comparing `vllm-0.1.2/vllm.egg-info/SOURCES.txt` & `vllm-0.1.3/vllm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -56,17 +56,20 @@
 vllm/model_executor/weight_utils.py
 vllm/model_executor/layers/__init__.py
 vllm/model_executor/layers/activation.py
 vllm/model_executor/layers/attention.py
 vllm/model_executor/layers/layernorm.py
 vllm/model_executor/layers/sampler.py
 vllm/model_executor/models/__init__.py
+vllm/model_executor/models/baichuan.py
 vllm/model_executor/models/bloom.py
+vllm/model_executor/models/falcon.py
 vllm/model_executor/models/gpt2.py
 vllm/model_executor/models/gpt_bigcode.py
+vllm/model_executor/models/gpt_j.py
 vllm/model_executor/models/gpt_neox.py
 vllm/model_executor/models/llama.py
 vllm/model_executor/models/mpt.py
 vllm/model_executor/models/opt.py
 vllm/model_executor/parallel_utils/__init__.py
 vllm/model_executor/parallel_utils/parallel_state.py
 vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
@@ -74,11 +77,13 @@
 vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
 vllm/model_executor/parallel_utils/tensor_parallel/random.py
 vllm/model_executor/parallel_utils/tensor_parallel/utils.py
 vllm/transformers_utils/__init__.py
 vllm/transformers_utils/config.py
 vllm/transformers_utils/tokenizer.py
 vllm/transformers_utils/configs/__init__.py
+vllm/transformers_utils/configs/baichuan.py
+vllm/transformers_utils/configs/falcon.py
 vllm/transformers_utils/configs/mpt.py
 vllm/worker/__init__.py
 vllm/worker/cache_engine.py
 vllm/worker/worker.py
```

