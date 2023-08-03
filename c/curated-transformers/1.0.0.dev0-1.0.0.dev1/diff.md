# Comparing `tmp/curated-transformers-1.0.0.dev0.tar.gz` & `tmp/curated-transformers-1.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-1.0.0.dev0.tar", last modified: Thu Jul 13 11:29:37 2023, max compression
+gzip compressed data, was "curated-transformers-1.0.0.dev1.tar", last modified: Tue Aug  1 08:03:38 2023, max compression
```

## Comparing `curated-transformers-1.0.0.dev0.tar` & `curated-transformers-1.0.0.dev1.tar`

### file list

```diff
@@ -1,196 +1,203 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.557990 curated-transformers-1.0.0.dev0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      116 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     4290 2023-07-13 11:29:37.557990 curated-transformers-1.0.0.dev0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3972 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.537990 curated-transformers-1.0.0.dev0/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      713 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/generation/
--rw-r--r--   0 vsts      (1001) docker     (122)      261 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2508 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3268 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3410 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/default_generator.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1917 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4281 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/generator.py
--rw-r--r--   0 vsts      (1001) docker     (122)      791 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/generator_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1183 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3298 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/logits.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4992 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/state.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2794 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/stop_conditions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2111 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/generation/string_generator.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1468 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/activations.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17092 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/attention.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1407 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10491 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3867 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/feedforward.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1511 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/normalization.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2514 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/layers/scalar_weight.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      360 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3660 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4109 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3249 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1734 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4792 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/auto_model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3497 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6957 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3561 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2619 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2852 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/bert/layer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.541990 curated-transformers-1.0.0.dev0/curated_transformers/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      681 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/camembert/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3579 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2803 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6335 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3420 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3874 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/layer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (122)      157 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2834 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6950 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3463 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3997 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4460 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (122)      140 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2796 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2823 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6528 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3893 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/llama/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4482 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/module.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4764 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/output.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3302 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2155 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2684 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       33 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      682 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/models/xlm_roberta/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/quantization/
--rw-r--r--   0 vsts      (1001) docker     (122)      126 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/
--rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2505 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5982 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/impl.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1101 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)      677 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/quantization/quantizable.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.545990 curated-transformers-1.0.0.dev0/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3002 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)      133 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      847 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4647 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4514 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4539 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_generic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2522 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_logits.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2860 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_stop.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      703 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/albert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/bert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/camembert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2550 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/falcon/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1378 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3916 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1367 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3917 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/llama/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      511 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/roberta/test_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3789 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_attention.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2008 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_auto_models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3415 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1324 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/models/xlm_roberta/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.549990 curated-transformers-1.0.0.dev0/curated_transformers/tests/quantization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/quantization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3732 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/quantization/test_generation.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10744 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10642 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      733 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10778 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (122)      977 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3909 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30593 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
--rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (122)      167 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2924 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/_hf_compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3523 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2661 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3021 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.553990 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (122)      385 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2325 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/_fairseq.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2903 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11948 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4435 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7336 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2781 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4092 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2250 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3230 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3885 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11770 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      221 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.557990 curated-transformers-1.0.0.dev0/curated_transformers/util/
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7746 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/util/hf.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1208 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/util/pytorch.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7392 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/curated_transformers/util/serde.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-13 11:29:37.537990 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     4290 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     7667 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       93 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-13 11:29:37.000000 curated-transformers-1.0.0.dev0/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)      702 2023-07-13 11:29:37.557990 curated-transformers-1.0.0.dev0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-07-13 11:29:27.000000 curated-transformers-1.0.0.dev0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.793844 curated-transformers-1.0.0.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      116 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-08-01 08:03:38.793844 curated-transformers-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4044 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.725843 curated-transformers-1.0.0.dev1/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      713 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.733843 curated-transformers-1.0.0.dev1/curated_transformers/generation/
+-rw-r--r--   0 vsts      (1001) docker     (122)      261 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2406 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4000 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3410 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/default_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1962 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1200 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4288 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/generator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      791 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/generator_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1183 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      753 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/llama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6591 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/logits.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4827 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/state.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2794 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/stop_conditions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2119 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/generation/string_generator.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.737843 curated-transformers-1.0.0.dev1/curated_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      615 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4055 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/activations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30505 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/attention.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2848 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10707 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3174 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/feedforward.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1511 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2514 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9950 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/layers/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.741843 curated-transformers-1.0.0.dev1/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      423 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.741843 curated-transformers-1.0.0.dev1/curated_transformers/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3527 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/albert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4488 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2913 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3442 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4944 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/auto_model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.745843 curated-transformers-1.0.0.dev1/curated_transformers/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      103 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3387 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/bert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3567 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4045 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/bert/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3628 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/bert/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.745843 curated-transformers-1.0.0.dev1/curated_transformers/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      681 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/camembert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3355 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/config.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.749843 curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5535 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1889 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4025 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5605 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5531 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/layer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.749843 curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (122)      109 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2972 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1885 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3855 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4388 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6217 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.753843 curated-transformers-1.0.0.dev1/curated_transformers/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (122)      103 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2769 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/llama/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1978 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/llama/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3676 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/llama/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4662 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/llama/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4390 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/module.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2695 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/output.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.753843 curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3226 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2039 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2213 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3683 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4328 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.757843 curated-transformers-1.0.0.dev1/curated_transformers/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)       33 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      682 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/models/xlm_roberta/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.757843 curated-transformers-1.0.0.dev1/curated_transformers/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (122)      126 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/quantization/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.757843 curated-transformers-1.0.0.dev1/curated_transformers/quantization/bnb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/quantization/bnb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2558 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/quantization/bnb/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5982 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/quantization/bnb/impl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1106 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/quantization/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      676 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/quantization/quantizable.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.761844 curated-transformers-1.0.0.dev1/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      444 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3002 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      133 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.765843 curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      847 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5058 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4514 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5152 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_generic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5066 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_logits.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2954 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_stop.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.765843 curated-transformers-1.0.0.dev1/curated_transformers/tests/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8882 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/layers/test_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7148 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/layers/test_embeddings.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.765843 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.769843 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1949 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/albert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.769843 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1737 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/bert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.769843 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1777 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/camembert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.769843 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4777 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/falcon/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.773844 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1845 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2236 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.773844 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2037 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/llama/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1997 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/llama/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.773844 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1761 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/roberta/test_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2008 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/test_auto_models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/test_hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10343 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.773844 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1765 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/models/xlm_roberta/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.777844 curated-transformers-1.0.0.dev1/curated_transformers/tests/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/quantization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3732 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/quantization/test_generation.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.777844 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.781844 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10775 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10673 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      733 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10809 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10482 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (122)      977 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/test_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3910 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.781844 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30593 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     1745 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.785844 curated-transformers-1.0.0.dev1/curated_transformers/tests/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2640 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/util/test_dataclass.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tests/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.785844 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      167 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2924 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/_hf_compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3561 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2661 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3021 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.793844 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)      385 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2325 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/_fairseq.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2903 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11952 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4436 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7336 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2939 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4092 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2287 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3234 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3945 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13006 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      221 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.793844 curated-transformers-1.0.0.dev1/curated_transformers/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4974 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/util/dataclass.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7712 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/util/hf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1208 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/util/pytorch.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7391 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/curated_transformers/util/serde.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-01 08:03:38.725843 curated-transformers-1.0.0.dev1/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-08-01 08:03:38.000000 curated-transformers-1.0.0.dev1/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     7881 2023-08-01 08:03:38.000000 curated-transformers-1.0.0.dev1/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-01 08:03:38.000000 curated-transformers-1.0.0.dev1/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      140 2023-08-01 08:03:38.000000 curated-transformers-1.0.0.dev1/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-08-01 08:03:38.000000 curated-transformers-1.0.0.dev1/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-01 08:03:38.000000 curated-transformers-1.0.0.dev1/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)      805 2023-08-01 08:03:38.797844 curated-transformers-1.0.0.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-08-01 08:03:25.000000 curated-transformers-1.0.0.dev1/setup.py
```

### Comparing `curated-transformers-1.0.0.dev0/LICENSE` & `curated-transformers-1.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/PKG-INFO` & `curated-transformers-1.0.0.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 1.0.0.dev0
-Summary: Curated transformer models
+Version: 1.0.0.dev1
+Summary: A PyTorch library of transformer models and components
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: quantization
 License-File: LICENSE
 
-# 🤖 Curated Transformers
+<img src="docs/source/logo.png" width="100" align="right"/>
+
+# Curated Transformers
 
 [![Documentation Status](https://readthedocs.org/projects/button/badge/?version=latest)](https://curated-transformers.readthedocs.io/en/latest/?badge=latest)
 [![pypi Version](https://img.shields.io/pypi/v/curated-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/curated-transformers/)
 
 **State-of-the-art transformers, brick by brick**
 
 Curated Transformers is a transformer library for PyTorch. It provides
@@ -51,21 +54,22 @@
 - CamemBERT
 - RoBERTa
 - XLM-RoBERTa
 
 Supported decoder-only models:
 
 - GPT-NeoX
-- LLaMA
+- LLaMA 1/2
 - Falcon
 
 Generator wrappers:
 
 - Dolly v2
 - Falcon
+- LLaMA 1/2
 
 All types of models can be loaded from Huggingface Hub.
 
 spaCy integration for curated transformers is provided by the
 [`spacy-curated-transformers`](https://github.com/explosion/spacy-curated-transformers)
 package.
```

### Comparing `curated-transformers-1.0.0.dev0/README.md` & `curated-transformers-1.0.0.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# 🤖 Curated Transformers
+<img src="docs/source/logo.png" width="100" align="right"/>
+
+# Curated Transformers
 
 [![Documentation Status](https://readthedocs.org/projects/button/badge/?version=latest)](https://curated-transformers.readthedocs.io/en/latest/?badge=latest)
 [![pypi Version](https://img.shields.io/pypi/v/curated-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/curated-transformers/)
 
 **State-of-the-art transformers, brick by brick**
 
 Curated Transformers is a transformer library for PyTorch. It provides
@@ -39,21 +41,22 @@
 - CamemBERT
 - RoBERTa
 - XLM-RoBERTa
 
 Supported decoder-only models:
 
 - GPT-NeoX
-- LLaMA
+- LLaMA 1/2
 - Falcon
 
 Generator wrappers:
 
 - Dolly v2
 - Falcon
+- LLaMA 1/2
 
 All types of models can be loaded from Huggingface Hub.
 
 spaCy integration for curated transformers is provided by the
 [`spacy-curated-transformers`](https://github.com/explosion/spacy-curated-transformers)
 package.
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/_compat.py` & `curated-transformers-1.0.0.dev1/curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/auto_generator.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/auto_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,18 +26,14 @@
             This class can currently only be used with the following models:
 
             - Models based on Dolly v2 (contain ``dolly-v2`` in the name).
             - Models based on Falcon (contain ``falcon`` in the name).
             - Models based on LLaMA (contain ``llama`` in the name).
     """
 
-    _DOLLY_V2_SUBSTRING = "dolly-v2"
-    _FALCON_SUBSTRING = "falcon"
-    _LLAMA_SUBSTRING = "llama"
-
     @classmethod
     def from_hf_hub(
         cls,
         *,
         name: str,
         revision: str = "main",
         device: Optional[torch.device] = None,
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/config.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Optional
+from typing import List, Optional, Set
 
 from .logits import (
     CompoundLogitTransforms,
     LogitsTransform,
     TemperatureTransform,
     TopKTransform,
+    TopPTransform,
+    VocabMaskTransform,
 )
 from .stop_conditions import (
     CompoundStopCondition,
     EndOfSequenceCondition,
     MaxGeneratedPiecesCondition,
     StopCondition,
 )
 
 
 @dataclass
 class GeneratorConfig(ABC):
     """
     Configuration of the generator.
 
+    :param masked_pieces:
+        Vocabulary pieces that should be masked out.
     :param eos_id:
         End-of-sequence identifier that should end the generation of a sequence
         when predicted. When this value is set to `None`, it is the
         responsibility of the generator to set it.
-
     :param max_generated_pieces:
         The maximum number of generation steps. This condition is a noop
         for values less than 1. When this value is set to `None`, it is the
         responsibility of the generator to set it.
     """
 
+    masked_pieces: Optional[Set[int]] = None
     eos_id: Optional[int] = None
     max_generated_pieces: Optional[int] = None
 
     @abstractmethod
     def logits_transform(self) -> LogitsTransform:
         """
         Get logit transform for the configuration.
 
         :returns:
             Logits transform. Usually multiple composed transforms.
         """
-        ...
+        raise NotImplementedError
 
     def stop_condition(self) -> StopCondition:
         """
         Get the stop condition for the configuration.
 
         :returns:
             Stop condition. Usually multiple composed conditions.
@@ -66,24 +70,28 @@
                     max_generated_pieces=self.max_generated_pieces
                 )
             )
 
         return conditions
 
 
+@dataclass
 class GreedyGeneratorConfig(GeneratorConfig):
     """
     Configuration for greedy generation.
 
     Greedy generation always selects the highest-probability piece, leading
     to deterministic generation.
     """
 
     def logits_transform(self) -> LogitsTransform:
-        return CompoundLogitTransforms([])
+        if self.masked_pieces is not None:
+            return VocabMaskTransform(self.masked_pieces)
+        else:
+            return CompoundLogitTransforms([])
 
 
 @dataclass
 class SampleGeneratorConfig(GeneratorConfig):
     """
     Configuration for generation with sampling.
 
@@ -96,19 +104,27 @@
 
         - ``T = 1``: the distribution is not changed.
         - ``T < 1``: the entropy of the distribution is decreased.
         - ``T > 1``: the entropy of the distribution is increased.
     :param top_k:
         Sample from top-k highest-probability pieces. ``top_k < 1`` disables top-k
         filtering.
+    :param top_p:
+        Sample from highest probability pieces the smallest set, such that their
+        cumulative probability is >= p. ``top_p = 1.0`` disables top-p filtering.
     """
 
     temperature: float = 1.0
     top_k: int = 0
+    top_p: float = 1.0
 
     def logits_transform(self) -> LogitsTransform:
-        return CompoundLogitTransforms(
-            [
-                TemperatureTransform(self.temperature),
-                TopKTransform(self.top_k),
-            ]
-        )
+        transforms: List[LogitsTransform] = []
+        if self.masked_pieces is not None:
+            transforms.append(VocabMaskTransform(self.masked_pieces))
+        transforms += [
+            TemperatureTransform(self.temperature),
+            TopKTransform(self.top_k),
+            TopPTransform(self.top_p),
+        ]
+
+        return CompoundLogitTransforms(transforms)
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/default_generator.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/default_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/dolly_v2.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/dolly_v2.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 
         """
         eos_id = tokenizer.tokenizer.token_to_id(END_KEY)
         super().__init__(
             tokenizer,
             causal_lm,
             default_config=SampleGeneratorConfig(
-                eos_id=eos_id, max_generated_pieces=256
+                eos_id=eos_id,
+                max_generated_pieces=256,
+                top_p=0.92,
             ),
         )
 
     def preprocess_prompts(self, prompts: List[str]) -> List[InputChunks]:
         return [
             InputChunks(
                 [
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/generator.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             The causal language model to generate with.
         """
         self.model = model
 
     def __call__(
         self,
         *,
-        attention_mask: Tensor,
+        attention_mask: AttentionMask,
         ids: Tensor,
         config: GeneratorConfig,
     ) -> Iterator[Tuple[Tensor, Tensor]]:
         """
         Alias for :meth:`.generate`.
         """
         return self.generate(
@@ -43,15 +43,15 @@
             ids=ids,
             config=config,
         )
 
     def generate(
         self,
         *,
-        attention_mask: Tensor,
+        attention_mask: AttentionMask,
         ids: Tensor,
         config: GeneratorConfig,
     ) -> Iterator[Tuple[Tensor, Tensor]]:
         """
         Generate text, starting from the given piece identifiers.
 
         The generator returns an iterator over tuples. Each tuple contains:
@@ -65,16 +65,14 @@
 
         :param ids:
             Batch of piece identifiers to start generating from.
 
             *Shape:* ``(batch_size, seq_len)``
         :param attention_mask:
             Attention mask that masks out pieces that should not be attended to.
-
-            *Shape:* ``(batch_size, seq_len)``
         :param config:
             Generator configuraton.
         :returns:
             An iterator over tuples. Each tuple contains a tensor with the
             sequence identifiers and a tensor with the next piece identier.
 
             *Shape:* ``(batch_unfinished,)``
@@ -97,15 +95,15 @@
             attention_mask=attention_mask, cache=cache, prompt_ids=ids
         )
 
         while True:
             with torch.no_grad():
                 output = self.model(
                     state.last_step_ids,
-                    attention_mask=AttentionMask(state.attention_mask),
+                    attention_mask=state.attention_mask,
                     cache=state.cache,
                     store_cache=True,
                     positions=state.positions,
                 )
 
             seq_ids, last_step_ids = state.step(
                 cache=output.cache,
@@ -120,15 +118,16 @@
                 return
 
     def _decode_greedy(
         self,
         logits_transform: LogitsTransform,
         output: CausalLMOutputWithCache[CacheT],
     ) -> Tensor:
-        return output.logits[:, -1:, :].argmax(-1)
+        logits = logits_transform(output.logits[:, -1:, :], inplace=True)
+        return logits.argmax(-1)
 
     def _decode_sample(
         self, logits_transform: LogitsTransform, output: CausalLMOutputWithCache[CacheT]
     ) -> Tensor:
         logits = logits_transform(output.logits[:, -1:, :], inplace=True)
         distribution = Categorical(logits=logits)
         return distribution.sample()
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/generator_wrapper.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/generator_wrapper.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/hf_hub.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/state.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 from typing import Generic, List, Optional, Tuple
 
 import torch
 from torch import Tensor
 
+from ..layers.attention import AttentionMask
 from ..models.output import CacheT
 from .stop_conditions import StopCondition
 
 
 class GeneratorState(Generic[CacheT]):
     """
     Stores the state of the generation process and tracks
     the sequences being generated.
     """
 
-    attention_mask: Tensor
+    attention_mask: AttentionMask
     cache: Optional[List[CacheT]]
     positions: Tensor
     seq_ids: Tensor
     prompt_ids: Tensor
     generated_ids: Tensor
 
     def __init__(
         self,
         *,
-        attention_mask: Tensor,
+        attention_mask: AttentionMask,
         cache: Optional[List[CacheT]],
         prompt_ids: Tensor,
     ) -> None:
         """
         Construct a generator state.
 
         :param attention_mask:
-            Atention mask for the prompts.
-
-            *Shape:* ``(batch_size, seq_len)``
+            Attention mask for the prompts.
         :param cache:
             Transformer model cache.
         :param prompt_ids:
             Batch of prompts.
 
             *Shape:* ``(batch_size, seq_len)``
         """
         device = prompt_ids.device
         assert (
             attention_mask.device == device
         ), f"Attention mask device '{attention_mask.device}' is not same as prompt ids device '{prompt_ids.device}'"
         self.attention_mask = attention_mask
-        self.positions = attention_mask.int().cumsum(-1) - 1
+        self.positions = attention_mask.bool_mask.int().cumsum(-1) - 1
         self.cache = cache
-        self.seq_ids = torch.arange(0, self.attention_mask.size(0), device=device)
+        self.seq_ids = torch.arange(0, self.attention_mask.shape[0], device=device)
         self.prompt_ids = prompt_ids
         self.generated_ids = torch.zeros(
             (prompt_ids.size(0), 0), dtype=prompt_ids.dtype, device=device
         )
 
     @property
     def is_finished(self):
@@ -101,24 +100,16 @@
 
             *Shape:* ``(batch_size), (batch_size, 1)``
         """
         # We update the state before removing completed sequences, so that
         # stopping conditions get a consistent view.
         self.cache = cache
         self.generated_ids = torch.concat([self.generated_ids, predicted_ids], 1)
-        self.attention_mask = torch.cat(
-            [
-                self.attention_mask,
-                torch.full(
-                    (self.attention_mask.size(0), 1),
-                    True,
-                    device=self.attention_mask.device,
-                ),
-            ],
-            dim=-1,
+        self.attention_mask = self.attention_mask.extend_length(
+            count=1, fill_value=True
         )
         self.positions = self.positions.max(-1, keepdim=True).values + 1
 
         # Determine which sequences are done generating and remove them.
         completed_exclude = torch.zeros_like(predicted_ids, dtype=torch.bool)
         completed_include = torch.zeros_like(predicted_ids, dtype=torch.bool)
         stop_condition.update_completed(
@@ -143,15 +134,15 @@
         :param completed:
             Tensor indicating for the active sequences whether they are completed.
 
         :meta private:
         """
         not_completed = completed.logical_not()
         self.generated_ids = self.generated_ids[not_completed]
-        self.attention_mask = self.attention_mask[not_completed]
+        self.attention_mask = self.attention_mask.filter_batch_items(not_completed)
         if self.cache is not None:
             self.cache = [
                 layer_cache.filter_batch_items(not_completed)
                 for layer_cache in self.cache
             ]
         self.prompt_ids = self.prompt_ids[not_completed]
         self.positions = self.positions[not_completed]
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/stop_conditions.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/generation/string_generator.py` & `curated-transformers-1.0.0.dev1/curated_transformers/generation/string_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,16 @@
             Generator configuraton.
         :returns:
             Strings generated for the prompts.
         """
 
         device = next(self.inner.model.parameters()).device
         pieces = self.tokenizer(prompts)
-        ids = pieces.padded_tensor(padding_id=0, pad_left=True).to(device)
-        attention_mask = pieces.attention_mask(pad_left=True).to(device)
+        ids = pieces.padded_tensor(padding_id=0, pad_left=True, device=device)
+        attention_mask = pieces.attention_mask(pad_left=True, device=device)
 
         piece_ids: List[List[int]] = [[] for _ in range(ids.size(0))]
         for seq_ids, outputs in self.inner(
             ids=ids, attention_mask=attention_mask, config=config
         ):
             for seq_id, seq_piece_ids in zip(seq_ids.tolist(), outputs.tolist()):
                 piece_ids[seq_id].extend(seq_piece_ids)
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/layers/__init__.py` & `curated-transformers-1.0.0.dev1/curated_transformers/layers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from ..layers.feedforward import PointwiseFeedForward
-from .activations import GeluFast, GeluNew
+from .activations import Activation, GELUFast, GELUNew
 from .attention import (
+    AttentionHeads,
     AttentionMask,
-    QkvHeadSharing,
     QkvMode,
-    RotaryEmbeddingConfig,
     ScaledDotProductAttention,
     SelfAttention,
     enable_torch_sdp,
 )
 from .cache import CacheProtocol, KeyValueCache
 from .embeddings import (
     QueryKeyRotaryEmbeddings,
     RotaryEmbeddings,
     SinusoidalPositionalEmbedding,
 )
 from .normalization import RMSNorm
 from .scalar_weight import ScalarWeight
+from .transformer import (
+    DecoderLayer,
+    EncoderLayer,
+    TransformerDropouts,
+    TransformerLayerNorms,
+)
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/layers/embeddings.py` & `curated-transformers-1.0.0.dev1/curated_transformers/layers/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         dim: int,
         max_len: int,
         *,
         normalize=True,
         device: Optional[torch.device] = None,
     ):
         """
-        Construct a sinosoidal positional embedding module.
+        Construct a sinusoidal positional embedding module.
 
         :param dim:
             Width of the embedding.
         :param max_len:
             Maximum length of the embedding.
         :param normalize:
             Perform L2 normalization of the embedding.
@@ -44,34 +44,34 @@
         )
 
         pe = torch.zeros(max_len, dim, device=device)
         pe[:, 0::2] = torch.sin(position * div_term)
         pe[:, 1::2] = torch.cos(position * div_term)
 
         if normalize == True:
-            l2 = torch.norm(pe, dim=-1)
+            l2 = torch.linalg.vector_norm(pe, dim=-1)
             pe /= l2.unsqueeze(-1)
 
         self.pe = pe
         self.pe.requires_grad = False
 
     def forward(self, input: Tensor) -> Tensor:
         """
         Returns the positional embedding for the input.
 
         :param input:
-            Input.
+            Input tensor.
 
             *Shape:* ``(batch_size, seq_len)``
         :returns:
             Positional embedding for the input.
 
             *Shape:* ``(seq_len, width)``
         """
-        return self.pe[input.size(1), :]
+        return self.pe[: input.size(1), :]
 
 
 class RotaryEmbeddings(Module):
     """
     Rotary embeddings (`Su et al., 2021`_).
 
     .. _Su et al., 2021: https://arxiv.org/abs/2104.09864
@@ -94,15 +94,15 @@
         will be precomputed for up to ``seq_len`` positions. The embedding
         will be recomputed when a longer sequence is found in the input.
 
         :param width:
             Rotary embedding dimensionality.
             Must be even.
         :param seq_len:
-            Number of positons to initially precompute.
+            Number of positions to initially precompute.
         :param base:
             The base used for :math:`\\theta_i`.
             Determines the cycle length of the embeddings.
         :param device:
             Device on which the module is to be initialized.
         """
         super().__init__()
@@ -201,15 +201,16 @@
 
         # Eq 34 with ordering changed for compatibility.
         return rot_cos * input + rot_sin * self._rotate(input)
 
 
 class QueryKeyRotaryEmbeddings(Module):
     """
-    Rotary embeddings (`Su et al., 2021`_) applied to key and value representations.
+    Rotary embeddings (`Su et al., 2021`_) applied to query
+    and key representations.
 
     .. _Su et al., 2021: https://arxiv.org/abs/2104.09864
     """
 
     def __init__(
         self,
         *,
@@ -273,14 +274,18 @@
             Query and key with the rotary embeddings applied.
 
             *Shape:* ``(batch_size, head, seq_len, width_per_head)``
         """
         dims_per_head = self.dims_per_head
         rotary_dims = self.rotary_dims
 
+        # The key-value is converted to a dict for traced models. Rewrap as
+        # KeyValueCache to get validation and utility methods.
+        cache = KeyValueCache.jit_rewrap(cache)
+
         # If a cache was provided, but no positions, assume that the
         # positions of the current batch continue from the cache.
         if cache is not None and positions is None:
             cache_len = cache.key.size(-2)
             seq_len = key.size(-2)
             positions = torch.arange(
                 cache_len,
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/layers/normalization.py` & `curated-transformers-1.0.0.dev1/curated_transformers/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/layers/scalar_weight.py` & `curated-transformers-1.0.0.dev1/curated_transformers/layers/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/albert/_hf.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/albert/_hf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 from types import MappingProxyType
-from typing import Any, Mapping
+from typing import Any, Callable, Dict, Mapping, Tuple, Union
 
 from torch import Tensor
 
+from ...layers.activations import Activation
+from ..hf_hub import _process_hf_keys
 from .config import ALBERTConfig
 
 HF_KEY_TO_CURATED_KEY = MappingProxyType(
     {
         "embeddings.word_embeddings.weight": "embeddings.word_embeddings.weight",
         "embeddings.token_type_embeddings.weight": "embeddings.token_type_embeddings.weight",
         "embeddings.position_embeddings.weight": "embeddings.position_embeddings.weight",
@@ -15,19 +17,18 @@
         "embeddings.LayerNorm.bias": "embeddings.layer_norm.bias",
         # Embedding projection
         "encoder.embedding_hidden_mapping_in.weight": "embeddings.projection.weight",
         "encoder.embedding_hidden_mapping_in.bias": "embeddings.projection.bias",
     }
 )
 
-HF_CONFIG_KEY_MAPPING = {
-    "pad_token_id": "padding_id",
+HF_CONFIG_KEY_MAPPING: Dict[str, Union[str, Tuple[str, Callable]]] = {
     "attention_probs_dropout_prob": "attention_probs_dropout_prob",
     "embedding_size": "embedding_width",
-    "hidden_act": "hidden_act",
+    "hidden_act": ("activation", Activation),
     "hidden_dropout_prob": "hidden_dropout_prob",
     "hidden_size": "hidden_width",
     "inner_group_num": "inner_group_num",
     "intermediate_size": "intermediate_width",
     "layer_norm_eps": "layer_norm_eps",
     "max_position_embeddings": "max_position_embeddings",
     "num_attention_heads": "num_attention_heads",
@@ -35,23 +36,15 @@
     "num_hidden_layers": "num_hidden_layers",
     "type_vocab_size": "type_vocab_size",
     "vocab_size": "vocab_size",
 }
 
 
 def convert_hf_config(hf_config: Any) -> ALBERTConfig:
-    missing_keys = tuple(
-        sorted(set(HF_CONFIG_KEY_MAPPING.keys()).difference(set(hf_config.keys())))
-    )
-    if len(missing_keys) != 0:
-        raise ValueError(
-            f"Missing keys in Hugging Face ALBERT model config: {missing_keys}"
-        )
-
-    kwargs = {curated: hf_config[hf] for hf, curated in HF_CONFIG_KEY_MAPPING.items()}
+    kwargs = _process_hf_keys("ALBERT", hf_config, HF_CONFIG_KEY_MAPPING)
     return ALBERTConfig(model_max_length=hf_config["max_position_embeddings"], **kwargs)
 
 
 def convert_hf_state_dict(params: Mapping[str, Tensor]) -> Mapping[str, Tensor]:
     # Strip the `albert` prefix from ALBERT model parameters.
     stripped_params = {re.sub(r"^albert\.", "", k): v for k, v in params.items()}
 
@@ -76,23 +69,23 @@
         name = re.sub(r"^albert_layer_groups\.", "groups.", name)
 
         # Inner layers.
         name = re.sub(r"\.albert_layers\.", ".group_layers.", name)
 
         # Attention blocks.
         name = re.sub(r"\.attention\.", ".mha.", name)
-        name = re.sub(r"\.mha\.LayerNorm", r".attn_output_layernorm", name)
+        name = re.sub(r"\.mha\.LayerNorm", r".attn_residual_layer_norm", name)
         name = re.sub(r"\.mha\.dense\.", r".mha.output.", name)
 
         # Pointwise feed-forward layers.
         name = re.sub(r"\.ffn\.", r".ffn.intermediate.", name)
         name = re.sub(r"\.ffn_output\.", r".ffn.output.", name)
         name = re.sub(
             r"\.full_layer_layer_norm\.",
-            r".ffn_output_layernorm.",
+            r".ffn_residual_layer_norm.",
             name,
         )
 
         out[name] = parameter
 
     for hf_name, curated_name in HF_KEY_TO_CURATED_KEY.items():
         if hf_name in stripped_params:
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/albert/config.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/albert/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from dataclasses import dataclass
 
-from ..bert import BERTAttentionConfig, BERTConfig, BERTEmbeddingConfig, BERTLayerConfig
+from ...layers.activations import Activation
+from ..config import (
+    TransformerAttentionLayerConfig,
+    TransformerEmbeddingLayerConfig,
+    TransformerFeedForwardLayerConfig,
+    TransformerLayerConfig,
+)
 
 
 @dataclass
-class ALBERTLayerConfig(BERTLayerConfig):
+class ALBERTLayerConfig(TransformerLayerConfig):
     """
     ALBERT (`Lan et al., 2022`_) layer configuration.
 
     .. _Lan et al., 2022: https://arxiv.org/abs/1909.11942
     """
 
     inner_group_num: int
@@ -25,15 +31,15 @@
         """
         super(ALBERTLayerConfig, self).__init__(*args, **kwargs)
         self.inner_group_num = inner_group_num
         self.num_hidden_groups = num_hidden_groups
 
 
 @dataclass
-class ALBERTConfig(BERTConfig):
+class ALBERTConfig:
     """
     ALBERT (`Lan et al., 2022`_) model configuration.
 
     .. _Lan et al., 2022: https://arxiv.org/abs/1909.11942
     """
 
     layer: ALBERTLayerConfig
@@ -46,21 +52,20 @@
         inner_group_num: int = 1,
         intermediate_width: int = 3072,
         num_attention_heads: int = 12,
         num_hidden_layers: int = 12,
         num_hidden_groups: int = 1,
         attention_probs_dropout_prob: float = 0.0,
         hidden_dropout_prob: float = 0.0,
-        hidden_act: str = "gelu_new",
+        activation: Activation = Activation.GELUNew,
         vocab_size: int = 30000,
         type_vocab_size: int = 2,
         max_position_embeddings: int = 512,
         model_max_length: int = 512,
         layer_norm_eps: float = 1e-12,
-        padding_id: int = 0,
     ):
         """
         :param embedding_width:
             Width of the embedding representations.
         :param hidden_width:
             Width of the transformer hidden layers.
         :param inner_group_num:
@@ -75,47 +80,53 @@
         :param num_hidden_groups:
             Number of hidden groups.
         :param attention_probs_dropout_prob:
             Dropout probabilty of the self-attention layers.
         :param hidden_dropout_prob:
             Dropout probabilty of the point-wise feed-forward and
             embedding layers.
-        :param hidden_act:
-            Activation used by the point-wise feed-forward layers.
+        :param activation:
+            Activation used by the pointwise feed-forward layers.
         :param vocab_size:
             Size of main vocabulary.
         :param type_vocab_size:
             Size of token type vocabulary.
         :param max_position_embeddings:
             Maximum length of position embeddings.
         :param model_max_length:
             Maximum length of model inputs.
         :param layer_norm_eps:
             Epsilon for layer normalization.
-        :param padding_id:
-            Index of the padding meta-token.
         """
-        self.embedding = BERTEmbeddingConfig(
+        self.embedding = TransformerEmbeddingLayerConfig(
             embedding_width=embedding_width,
             vocab_size=vocab_size,
             type_vocab_size=type_vocab_size,
             max_position_embeddings=max_position_embeddings,
             layer_norm_eps=layer_norm_eps,
             dropout_prob=hidden_dropout_prob,
         )
-        self.attention = BERTAttentionConfig(
-            hidden_width=hidden_width,
-            num_attention_heads=num_attention_heads,
-            dropout_prob=attention_probs_dropout_prob,
-        )
         self.layer = ALBERTLayerConfig(
-            hidden_width=hidden_width,
-            inner_group_num=inner_group_num,
-            intermediate_width=intermediate_width,
+            attention=TransformerAttentionLayerConfig(
+                hidden_width=hidden_width,
+                dropout_prob=attention_probs_dropout_prob,
+                num_key_value_heads=num_attention_heads,
+                num_query_heads=num_attention_heads,
+                parallel_attention=False,
+                rotary_embeddings=None,
+                use_alibi=False,
+                use_bias=True,
+            ),
+            feedforward=TransformerFeedForwardLayerConfig(
+                hidden_width=hidden_width,
+                intermediate_width=intermediate_width,
+                activation=activation,
+                use_bias=True,
+                use_gate=False,
+            ),
             num_hidden_layers=num_hidden_layers,
-            num_hidden_groups=num_hidden_groups,
-            hidden_act=hidden_act,
             layer_norm_eps=layer_norm_eps,
             dropout_prob=hidden_dropout_prob,
+            inner_group_num=inner_group_num,
+            num_hidden_groups=num_hidden_groups,
         )
         self.model_max_length = model_max_length
-        self.padding_id = padding_id
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/albert/encoder.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/albert/encoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         :param device:
             Device to which the module is to be moved.
         :returns:
             The encoder.
         """
         super().__init__()
 
-        self.padding_id = config.padding_id
         self.max_seq_len = config.model_max_length
         self.num_hidden_layers = config.layer.num_hidden_layers
         num_hidden_groups = config.layer.num_hidden_groups
 
         if self.num_hidden_layers % num_hidden_groups != 0:
             raise ValueError(
                 f"The number of hidden layers ({self.num_hidden_layers}) in the "
@@ -49,45 +48,37 @@
             )
 
         self.embeddings = BERTEmbeddings(config.embedding, config.layer, device=device)
 
         # Parameters are shared by groups of layers.
         self.groups = torch.nn.ModuleList(
             [
-                ALBERTLayerGroup(config.layer, config.attention, device=device)
+                ALBERTLayerGroup(config.layer, device=device)
                 for _ in range(num_hidden_groups)
             ]
         )
 
-    def _create_attention_mask(self, x: Tensor) -> AttentionMask:
-        return AttentionMask(bool_mask=x.ne(self.padding_id))
-
     def forward(
         self,
         input_ids: Tensor,
         attention_mask: Optional[AttentionMask] = None,
         token_type_ids: Optional[Tensor] = None,
     ) -> ModelOutput:
-        if attention_mask is None:
-            attention_mask = self._create_attention_mask(input_ids)
-
         embeddings = self.embeddings(input_ids, token_type_ids, None)
         layer_output = embeddings
 
         layers_per_group = self.num_hidden_layers // len(self.groups)
 
         layer_outputs = []
         for group in self.groups:
             for _ in range(layers_per_group):
-                layer_output = group(layer_output, attention_mask=attention_mask)
+                layer_output, _ = group(layer_output, attention_mask=attention_mask)
                 layer_outputs.append(layer_output)
 
-        return ModelOutput(
-            embedding_output=embeddings, layer_hidden_states=layer_outputs
-        )
+        return ModelOutput(all_outputs=[embeddings, *layer_outputs])
 
     @classmethod
     def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
         return convert_hf_state_dict(params)
 
     @classmethod
     def from_hf_config(
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/albert/layer_group.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/embeddings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 from typing import Optional
 
 import torch
 from torch import Tensor
-from torch.nn import Module, ModuleList
+from torch.nn import Module
 
-from ...layers.attention import AttentionMask
-from ..bert.config import BERTAttentionConfig
-from ..bert.layer import BERTAttentionConfig, BERTEncoderLayer
-from .config import ALBERTLayerConfig
+from ..bert import BERTEmbeddings
+from ..config import TransformerEmbeddingLayerConfig, TransformerLayerConfig
 
 
-class ALBERTLayerGroup(Module):
+class RoBERTaEmbeddings(Module):
     """
-    ALBERT (`Lan et al., 2022`_) layer group.
+    RoBERTa (`Liu et al., 2019`_) embedding layer.
 
-    .. _Lan et al., 2022: https://arxiv.org/abs/1909.11942
+    .. _Liu et al., 2019: https://arxiv.org/abs/1907.11692
     """
 
     def __init__(
         self,
-        layer_config: ALBERTLayerConfig,
-        attention_config: BERTAttentionConfig,
+        embedding_config: TransformerEmbeddingLayerConfig,
+        layer_config: TransformerLayerConfig,
         *,
+        padding_id: int,
         device: Optional[torch.device] = None
     ) -> None:
         super().__init__()
 
-        self.group_layers = ModuleList(
-            [
-                BERTEncoderLayer(layer_config, attention_config, device=device)
-                for _ in range(layer_config.inner_group_num)
-            ]
-        )
+        self.inner = BERTEmbeddings(embedding_config, layer_config, device=device)
+        self.padding_id = padding_id
 
-    def forward(self, input: Tensor, attention_mask: AttentionMask) -> Tensor:
+    def _get_position_ids(self, x: Tensor) -> Tensor:
+        # We need to generate the position IDs from the
+        # input tensor to pass to the embedding layer and
+        # handle padding, c.f https://github.com/huggingface/transformers/blob/330247ede2d8265aae9ab0b7a0d1a811c344960d/src/transformers/models/roberta/modeling_roberta.py#L1566
+
+        mask = x.ne(self.padding_id).int()
+        return (mask.cumsum(dim=1) * mask) + self.padding_id
+
+    def forward(
+        self,
+        input_ids: Tensor,
+        token_type_ids: Optional[Tensor] = None,
+        position_ids: Optional[Tensor] = None,
+    ) -> Tensor:
         """
-        Apply the ALBERT layer group to the given piece hidden representations.
+        Apply the RoBERTa embedding layer to the piece identifiers.
 
-        :param input:
-            Hidden representations to apply the layer group to.
+        :param input_ids:
+            Piece identifiers to embed.
 
-            *Shape:* ``(batch_size, seq_len, width)``
-        :param attention_mask:
-            Attention mask. Sequence elements for which the
-            corresponding mask element is set to ``False`` are ignored
-            during attention calculation.
+            *Shape:* ``(batch_size, seq_len)``
+        :param token_type_ids:
+            Token type identifiers to indicate the spans of different
+            sequences in the input. Useful when performing tasks like
+            sequence classification and question answering.
 
             *Shape:* ``(batch_size, seq_len)``
-        :returns:
-            Layer output.
+        :param position_ids:
+            Positional identifiers with which to fetch the positional
+            embeddings for the sequences.
 
-            *Shape:* ``(batch_size, seq_len, width)``
+            *Shape:* ``(batch_size, seq_len)``
         """
-        layer_output = input
-        for layer in self.group_layers:
-            layer_output = layer(layer_output, attention_mask)
-        return layer_output
+        if position_ids is None:
+            position_ids = self._get_position_ids(input_ids)
+
+        return self.inner(input_ids, token_type_ids, position_ids)
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/auto_model.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/auto_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,31 +33,31 @@
         *,
         name: str,
         revision: str = "main",
         device: Optional[torch.device] = None,
         quantization_config: Optional[BitsAndBytesConfig] = None,
     ) -> ModelT:
         """
-        Construct and load a module or a generator from Hugging Face Hub.
+        Construct and load a model or a generator from Hugging Face Hub.
 
         :param name:
             Model name.
         :param revision:
             Model revision.
         :param device:
             Device on which to initialize the model.
         :param quantization_config:
             Configuration for loading quantized weights.
         :returns:
-            Loaded module or generator.
+            Loaded model or generator.
         """
         raise NotImplementedError
 
     @classmethod
-    def _instantiate_module_from_hf_hub(
+    def _instantiate_model_from_hf_hub(
         cls,
         name: str,
         revision: str,
         device: Optional[torch.device],
         quantization_config: Optional[BitsAndBytesConfig],
         model_type_to_class_map: Mapping[str, Type],
     ) -> FromHFHub:
@@ -76,15 +76,15 @@
             quantization_config=quantization_config,
         )
         return module
 
 
 class AutoEncoder(AutoModel[EncoderModule]):
     """
-    Encoder module loaded from the Hugging Face Model Hub.
+    Encoder model loaded from the Hugging Face Model Hub.
     """
 
     _HF_MODEL_TYPE_TO_CURATED = {
         "bert": BERTEncoder,
         "albert": ALBERTEncoder,
         "camembert": CamemBERTEncoder,
         "roberta": RoBERTaEncoder,
@@ -96,15 +96,15 @@
         cls,
         *,
         name: str,
         revision: str = "main",
         device: Optional[torch.device] = None,
         quantization_config: Optional[BitsAndBytesConfig] = None,
     ) -> EncoderModule:
-        encoder = cls._instantiate_module_from_hf_hub(
+        encoder = cls._instantiate_model_from_hf_hub(
             name, revision, device, quantization_config, cls._HF_MODEL_TYPE_TO_CURATED
         )
         assert isinstance(encoder, EncoderModule)
         return encoder
 
 
 class AutoDecoder(AutoModel[DecoderModule]):
@@ -112,50 +112,54 @@
     Decoder module loaded from the Hugging Face Model Hub.
     """
 
     _HF_MODEL_TYPE_TO_CURATED = {
         "gpt_neox": GPTNeoXDecoder,
         "llama": LLaMADecoder,
         "falcon": FalconDecoder,
+        "RefinedWeb": FalconDecoder,
+        "RefinedWebModel": FalconDecoder,
     }
 
     @classmethod
     def from_hf_hub(
         cls,
         *,
         name: str,
         revision: str = "main",
         device: Optional[torch.device] = None,
         quantization_config: Optional[BitsAndBytesConfig] = None,
     ) -> DecoderModule:
-        decoder = cls._instantiate_module_from_hf_hub(
+        decoder = cls._instantiate_model_from_hf_hub(
             name, revision, device, quantization_config, cls._HF_MODEL_TYPE_TO_CURATED
         )
         assert isinstance(decoder, DecoderModule)
         return decoder
 
 
 class AutoCausalLM(AutoModel[CausalLMModule[KeyValueCache]]):
     """
-    Causal LM module loaded from the Hugging Face Model Hub.
+    Causal LM model loaded from the Hugging Face Model Hub.
     """
 
     _HF_MODEL_TYPE_TO_CURATED = {
         "gpt_neox": GPTNeoXCausalLM,
         "llama": LLaMACausalLM,
         "falcon": FalconCausalLM,
+        "RefinedWeb": FalconCausalLM,
+        "RefinedWebModel": FalconCausalLM,
     }
 
     @classmethod
     def from_hf_hub(
         cls,
         *,
         name: str,
         revision: str = "main",
         device: Optional[torch.device] = None,
         quantization_config: Optional[BitsAndBytesConfig] = None,
     ) -> CausalLMModule[KeyValueCache]:
-        causal_lm = cls._instantiate_module_from_hf_hub(
+        causal_lm = cls._instantiate_model_from_hf_hub(
             name, revision, device, quantization_config, cls._HF_MODEL_TYPE_TO_CURATED
         )
         assert isinstance(causal_lm, CausalLMModule)
         return causal_lm
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/bert/_hf.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/bert/_hf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 import re
 from types import MappingProxyType
-from typing import Any, Mapping
+from typing import Any, Callable, Dict, Mapping, Tuple, Union
 
 from torch import Tensor
 
+from ...layers.activations import Activation
+from ..hf_hub import _process_hf_keys
 from .config import BERTConfig
 
 HF_KEY_TO_CURATED_KEY = MappingProxyType(
     {
         "embeddings.word_embeddings.weight": "embeddings.word_embeddings.weight",
         "embeddings.token_type_embeddings.weight": "embeddings.token_type_embeddings.weight",
         "embeddings.position_embeddings.weight": "embeddings.position_embeddings.weight",
         "embeddings.LayerNorm.weight": "embeddings.layer_norm.weight",
         "embeddings.LayerNorm.bias": "embeddings.layer_norm.bias",
     }
 )
 
 
-HF_CONFIG_KEY_MAPPING = {
-    "pad_token_id": "padding_id",
+HF_CONFIG_KEY_MAPPING: Dict[str, Union[str, Tuple[str, Callable]]] = {
     "attention_probs_dropout_prob": "attention_probs_dropout_prob",
-    "hidden_act": "hidden_act",
+    "hidden_act": ("activation", Activation),
     "hidden_dropout_prob": "hidden_dropout_prob",
     "hidden_size": "hidden_width",
     "intermediate_size": "intermediate_width",
     "layer_norm_eps": "layer_norm_eps",
     "max_position_embeddings": "max_position_embeddings",
     "num_attention_heads": "num_attention_heads",
     "num_hidden_layers": "num_hidden_layers",
     "type_vocab_size": "type_vocab_size",
     "vocab_size": "vocab_size",
 }
 
 
 def convert_hf_config(hf_config: Any) -> BERTConfig:
-    missing_keys = tuple(
-        sorted(set(HF_CONFIG_KEY_MAPPING.keys()).difference(set(hf_config.keys())))
-    )
-    if len(missing_keys) != 0:
-        raise ValueError(
-            f"Missing keys in Hugging Face BERT model config: {missing_keys}"
-        )
+    kwargs = _process_hf_keys("BERT", hf_config, HF_CONFIG_KEY_MAPPING)
 
-    kwargs = {curated: hf_config[hf] for hf, curated in HF_CONFIG_KEY_MAPPING.items()}
     return BERTConfig(
         embedding_width=hf_config["hidden_size"],
         model_max_length=hf_config["max_position_embeddings"],
         **kwargs,
     )
 
 
@@ -69,18 +63,20 @@
         name = re.sub(r"^layer", "layers", name)
 
         # The HF model has one more level of indirection for the output layers in their
         # attention heads and the feed-forward network layers.
         name = re.sub(r"\.attention\.self\.(query|key|value)", r".mha.\1", name)
         name = re.sub(r"\.attention\.(output)\.dense", r".mha.\1", name)
         name = re.sub(
-            r"\.attention\.output\.LayerNorm", r".attn_output_layernorm", name
+            r"\.attention\.output\.LayerNorm", r".attn_residual_layer_norm", name
         )
         name = re.sub(r"\.(intermediate)\.dense", r".ffn.\1", name)
-        name = re.sub(r"(\.\d+)\.output\.LayerNorm", r"\1.ffn_output_layernorm", name)
+        name = re.sub(
+            r"(\.\d+)\.output\.LayerNorm", r"\1.ffn_residual_layer_norm", name
+        )
         name = re.sub(r"(\.\d+)\.(output)\.dense", r"\1.ffn.\2", name)
 
         out[name] = parameter
 
     for hf_name, curated_name in HF_KEY_TO_CURATED_KEY.items():
         if hf_name in stripped_params:
             out[curated_name] = stripped_params[hf_name]
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/bert/embeddings.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/bert/embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 from typing import Optional
 
 import torch
 from torch import Tensor
 from torch.nn import Dropout, Embedding, LayerNorm, Linear, Module
 
-from .config import BERTEmbeddingConfig, BERTLayerConfig
+from ..config import TransformerEmbeddingLayerConfig, TransformerLayerConfig
 
 
 class BERTEmbeddings(Module):
     """
     BERT (`Devlin et al., 2018`_) embedding layer.
 
     .. _Devlin et al., 2018 : https://arxiv.org/abs/1810.04805
     """
 
     def __init__(
         self,
-        embedding_config: BERTEmbeddingConfig,
-        layer_config: BERTLayerConfig,
+        embedding_config: TransformerEmbeddingLayerConfig,
+        layer_config: TransformerLayerConfig,
         *,
         device: Optional[torch.device] = None
     ) -> None:
         super().__init__()
 
+        if embedding_config.type_vocab_size is None:
+            raise ValueError(
+                "BERT embedding config does not contain type vocabulary size"
+            )
+        elif embedding_config.max_position_embeddings is None:
+            raise ValueError(
+                "BERT embedding config does not contain max position embeddings length"
+            )
+
         self.word_embeddings = Embedding(
             num_embeddings=embedding_config.vocab_size,
             embedding_dim=embedding_config.embedding_width,
             device=device,
         )
-        self.token_type_embeddings = Embedding(
+        self.token_type_embeddings: Embedding = Embedding(
             num_embeddings=embedding_config.type_vocab_size,
             embedding_dim=embedding_config.embedding_width,
             device=device,
         )
-        self.position_embeddings = Embedding(
+        self.position_embeddings: Embedding = Embedding(
             num_embeddings=embedding_config.max_position_embeddings,
             embedding_dim=embedding_config.embedding_width,
             device=device,
         )
 
-        if embedding_config.embedding_width != layer_config.hidden_width:
-            self.projection = Linear(
+        if embedding_config.embedding_width != layer_config.feedforward.hidden_width:
+            self.projection: Linear = Linear(
                 embedding_config.embedding_width,
-                layer_config.hidden_width,
+                layer_config.feedforward.hidden_width,
                 device=device,
             )
         else:
             self.projection = None  # type: ignore
 
-        self.layer_norm = LayerNorm(
+        self.layer_norm: LayerNorm = LayerNorm(
             embedding_config.embedding_width,
             eps=embedding_config.layer_norm_eps,
             device=device,
         )
-        self.dropout = Dropout(p=embedding_config.dropout_prob)
+        self.dropout: Dropout = Dropout(p=embedding_config.dropout_prob)
 
     def _get_position_ids(self, x: Tensor) -> Tensor:
         return torch.arange(x.shape[1], device=x.device).expand(1, -1)
 
     def _get_token_type_ids(self, x: Tensor) -> Tensor:
         return torch.zeros_like(x)
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/bert/layer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/albert/layer_group.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,92 @@
+from functools import partial
 from typing import Optional
 
 import torch
 from torch import Tensor
-from torch.nn import Module
+from torch.nn import LayerNorm, Module, ModuleList
 
-from ...layers.attention import AttentionMask, QkvHeadSharing, QkvMode, SelfAttention
+from ...layers.attention import AttentionHeads, AttentionMask, QkvMode, SelfAttention
 from ...layers.feedforward import PointwiseFeedForward
-from .config import BERTAttentionConfig, BERTLayerConfig
+from ...layers.transformer import (
+    EncoderLayer,
+    TransformerDropouts,
+    TransformerLayerNorms,
+)
+from .config import ALBERTLayerConfig
 
 
-class BERTEncoderLayer(Module):
+class ALBERTLayerGroup(Module):
     """
-    BERT (`Devlin et al., 2018`_) encoder layer.
+    ALBERT (`Lan et al., 2022`_) layer group.
 
-    .. _Devlin et al., 2018 : https://arxiv.org/abs/1810.04805
+    .. _Lan et al., 2022: https://arxiv.org/abs/1909.11942
     """
 
     def __init__(
-        self,
-        layer_config: BERTLayerConfig,
-        attention_config: BERTAttentionConfig,
-        *,
-        device: Optional[torch.device] = None
-    ):
+        self, layer_config: ALBERTLayerConfig, *, device: Optional[torch.device] = None
+    ) -> None:
         super().__init__()
 
-        self.mha = SelfAttention(
-            dropout_prob=attention_config.dropout_prob,
-            hidden_width=attention_config.hidden_width,
-            qkv_head_sharing=QkvHeadSharing.NONE,
-            num_attention_heads=attention_config.num_attention_heads,
-            qkv_mode=QkvMode.SEPARATE,
-            rotary_embeds=None,
-            use_bias=True,
+        layer_norm = partial(
+            LayerNorm,
+            layer_config.feedforward.hidden_width,
+            layer_config.layer_norm_eps,
             device=device,
         )
-        self.attn_output_layernorm = torch.nn.LayerNorm(
-            layer_config.hidden_width, eps=layer_config.layer_norm_eps, device=device
+        attention_config = layer_config.attention
+        self.group_layers = ModuleList(
+            [
+                EncoderLayer(
+                    attention_layer=SelfAttention(
+                        attention_heads=AttentionHeads.uniform(
+                            attention_config.num_query_heads
+                        ),
+                        dropout_prob=attention_config.dropout_prob,
+                        hidden_width=layer_config.feedforward.hidden_width,
+                        qkv_mode=QkvMode.SEPARATE,
+                        rotary_embeds=None,
+                        use_bias=attention_config.use_bias,
+                        device=device,
+                    ),
+                    feed_forward_layer=PointwiseFeedForward(
+                        activation=layer_config.feedforward.activation.module(),
+                        hidden_width=layer_config.feedforward.hidden_width,
+                        intermediate_width=layer_config.feedforward.intermediate_width,
+                        use_bias=layer_config.feedforward.use_bias,
+                        use_gate=layer_config.feedforward.use_gate,
+                        device=device,
+                    ),
+                    dropouts=TransformerDropouts.layer_output_dropouts(
+                        layer_config.dropout_prob
+                    ),
+                    layer_norms=TransformerLayerNorms(
+                        attn_residual_layer_norm=layer_norm(),
+                        ffn_residual_layer_norm=layer_norm(),
+                    ),
+                    parallel_attention=attention_config.parallel_attention,
+                )
+                for _ in range(layer_config.inner_group_num)
+            ]
         )
-        self.attn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
-        self.ffn = PointwiseFeedForward(
-            hidden_act=layer_config.hidden_act,
-            hidden_width=layer_config.hidden_width,
-            intermediate_width=layer_config.intermediate_width,
-            use_bias=True,
-            use_gate=False,
-            device=device,
-        )
-        self.ffn_output_layernorm = torch.nn.LayerNorm(
-            layer_config.hidden_width, eps=layer_config.layer_norm_eps, device=device
-        )
-        self.ffn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
 
     def forward(self, input: Tensor, attention_mask: AttentionMask) -> Tensor:
         """
-        Apply the BERT encoder layer to the given piece hidden representations.
+        Apply the ALBERT layer group to the given piece hidden representations.
 
         :param input:
-            Hidden representations to apply the layer to.
+            Hidden representations to apply the layer group to.
 
             *Shape:* ``(batch_size, seq_len, width)``
         :param attention_mask:
             Attention mask. Sequence elements for which the
             corresponding mask element is set to ``False`` are ignored
             during attention calculation.
-
-            *Shape:* ``(batch_size, seq_len)``
         :returns:
             Layer output.
 
             *Shape:* ``(batch_size, seq_len, width)``
         """
-        attn_out, _ = self.mha(input, attention_mask)
-        attn_out = self.attn_output_dropout(attn_out)
-        attn_out = self.attn_output_layernorm(input + attn_out)
-
-        ffn_out = self.ffn(attn_out)
-        ffn_out = self.ffn_output_dropout(ffn_out)
-        ffn_out = self.ffn_output_layernorm(attn_out + ffn_out)
-
-        return ffn_out
+        layer_output = input
+        for layer in self.group_layers:
+            layer_output = layer(layer_output, attention_mask)
+        return layer_output
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/camembert/encoder.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/camembert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/_hf.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/llama/_hf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,80 @@
 import re
-from typing import Any, Mapping
+from typing import Any, Callable, Dict, Mapping, Tuple, Union
 
 from torch import Tensor
-from torch.nn import parallel
 
+from ...layers.activations import Activation
+from ..hf_hub import _process_hf_keys
 from ..module import DecoderModule
-from .config import FalconConfig
+from .config import LLaMAConfig
 
 ATTENTION_DROPOUT = "attention_probs_dropout_prob"
 HIDDEN_DROPOUT = "hidden_dropout_prob"
-EXTRA_KWARG_KEYS = [ATTENTION_DROPOUT, HIDDEN_DROPOUT]
+NUM_KEY_VALUE_HEADS = "num_key_value_heads"
+EXTRA_KWARG_KEYS = [ATTENTION_DROPOUT, HIDDEN_DROPOUT, NUM_KEY_VALUE_HEADS]
 
 
-HF_CONFIG_KEY_MAPPING = {
+HF_CONFIG_KEY_MAPPING: Dict[str, Union[str, Tuple[str, Callable]]] = {
+    "hidden_act": ("activation", Activation),
     "hidden_size": "hidden_width",
-    "layer_norm_epsilon": "layer_norm_eps",
-    "multi_query": "multi_query",
-    "num_attention_heads": "num_attention_heads",
+    "intermediate_size": "intermediate_width",
+    "rms_norm_eps": "rms_norm_eps",
+    "num_attention_heads": "num_query_heads",
     "num_hidden_layers": "num_hidden_layers",
-    "bias": "use_bias",
     "vocab_size": "vocab_size",
 }
 
 
-def convert_hf_config(hf_config: Any) -> FalconConfig:
-    missing_keys = tuple(
-        sorted(set(HF_CONFIG_KEY_MAPPING.keys()).difference(set(hf_config.keys())))
+def convert_hf_config(hf_config: Any) -> LLaMAConfig:
+    kwargs = _process_hf_keys(
+        "LLaMA", hf_config, HF_CONFIG_KEY_MAPPING, EXTRA_KWARG_KEYS
     )
-    if len(missing_keys) != 0:
-        raise ValueError(f"Missing keys in Hugging Face Falcon config: {missing_keys}")
 
-    kwargs = {curated: hf_config[hf] for hf, curated in HF_CONFIG_KEY_MAPPING.items()}
-    # Handle config options that are not set in all models.
-    kwargs.update({k: hf_config[k] for k in EXTRA_KWARG_KEYS if k in hf_config})
-
-    parallel_attention = hf_config.get("parallel_attn", True)
-
-    # When new_decoder_architecture is set, the multi_query and parallel_attn
-    # options in the configuration are ignored and set to True.
-    if (
-        "new_decoder_architecture" in hf_config
-        and hf_config["new_decoder_architecture"]
-    ):
-        kwargs["multi_query"] = True
-        parallel_attention = True
-
-    if not parallel_attention:
-        raise ValueError(
-            "Falcon models without parallel attention are currently not supported"
-        )
-    if "alibi" in hf_config and hf_config["alibi"]:
-        raise ValueError("Falcon models with ALiBi are currently not supported")
+    if not NUM_KEY_VALUE_HEADS in kwargs:
+        kwargs[NUM_KEY_VALUE_HEADS] = kwargs["num_query_heads"]
 
-    return FalconConfig(
+    return LLaMAConfig(
         rotary_embedding_base=10000,
         rotary_embedding_fraction=1.0,
         **kwargs,
     )
 
 
 def convert_hf_state_dict(cls, params: Mapping[str, Tensor]) -> Mapping[str, Tensor]:
-    """
-    Convert state dict from HF paramater naming to ours.
+    """Convert state dict from HF paramater naming to ours.
     The function is insensitive to prefixes, to allow loading
-    both the decoder and the full LM.
-    """
+    both the decoder and the full LM."""
     if issubclass(cls, DecoderModule):
-        stripped_params = {
-            re.sub(r"^transformer\.", "", k): v for k, v in params.items()
-        }
+        stripped_params = {re.sub(r"^model\.", "", k): v for k, v in params.items()}
     else:
         stripped_params = {
-            re.sub(r"^transformer\.", "decoder.", k): v for k, v in params.items()
+            re.sub(r"^model\.", "decoder.", k): v for k, v in params.items()
         }
 
     out = {}
     for name, parameter in stripped_params.items():
-        # These parameters are all created on-the-fly.
-        if "rotary_emb" in name or "attention.bias" in name or "masked_bias" in name:
-            continue
-
-        name = re.sub(r"^h\.", "layers.", name)
-        name = re.sub(r"decoder\.h\.", "decoder.layers.", name)
-
         # Attention
-        name = re.sub(r"\.self_attention", r".mha", name)
-        name = re.sub(r"\.query_key_value", r".input", name)
-        name = re.sub(r"\.mha\.dense", r".mha.output", name)
+        name = re.sub(r"\.self_attn", r".mha", name)
+        name = re.sub(r"\.q_proj", r".query", name)
+        name = re.sub(r"\.k_proj", r".key", name)
+        name = re.sub(r"\.v_proj", r".value", name)
+        name = re.sub(r"\.o_proj", r".output", name)
 
         # Pointwise feedforward
         name = re.sub(r"\.mlp", r".ffn", name)
-        name = re.sub(r"\.dense_h_to_4h", r".intermediate", name)
-        name = re.sub(r"\.dense_4h_to_h", r".output", name)
-
-        # Layer norms
-        name = re.sub(r"\.input_layernorm", r".input_layer_norm", name)
-        name = re.sub(r"ln_f\.", r"output_layer_norm.", name)
+        name = re.sub(r"\.up_proj", r".intermediate", name)
+        name = re.sub(r"\.down_proj", r".output", name)
+        name = re.sub(r"\.gate_proj", r".gate", name)
+
+        # RMS norms
+        name = re.sub(r"\.input_layernorm", r".attn_input_layer_norm", name)
+        name = re.sub(r"\.post_attention_layernorm", r".ffn_input_layer_norm", name)
+        name = re.sub(r"^(decoder\.)?norm\.", r"\1output_layer_norm.", name)
 
         # Embeddings
-        name = re.sub(r"word_embeddings\.", r"embeddings.", name)
+        name = re.sub(r"embed_tokens\.", r"embeddings.", name)
         name = re.sub(r"lm_head\.", r"output_embeddings.", name)
 
         out[name] = parameter
 
     return out
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/causal_lm.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/causal_lm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-from typing import Any, List, Mapping, Optional, Set, Type, TypeVar
+from typing import Any, Mapping, Optional, Set, Type, TypeVar
 
 import torch
 from torch import Tensor
 from torch.nn import Linear
 
-from ...layers.attention import AttentionMask
-from ...layers.cache import KeyValueCache
 from ...quantization.quantizable import Quantizable
 from ..hf_hub import FromHFHub
-from ..module import CausalLMModule
-from ..output import CausalLMOutputWithCache
+from ..transformer import TransformerCausalLM
 from ._hf import convert_hf_config, convert_hf_state_dict
 from .config import FalconConfig
 from .decoder import FalconDecoder
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="FalconCausalLM")
 
 
-class FalconCausalLM(CausalLMModule[KeyValueCache], FromHFHub, Quantizable):
+class FalconCausalLM(TransformerCausalLM, FromHFHub, Quantizable):
     """
-    `Falcon`_ causal language model.
+    Falcon (`Penedo et al., 2019`_) causal language model.
 
-    .. _Falcon: https://arxiv.org/abs/2306.01116
+    .. _Penedo et al., 2019: https://arxiv.org/abs/2306.01116
     """
 
     def __init__(
         self, config: FalconConfig, *, device: Optional[torch.device] = None
     ) -> None:
         """
         Construct a Falcon causal LM.
@@ -38,44 +35,20 @@
         :returns:
             The causal LM.
         """
         super().__init__()
 
         self.decoder = FalconDecoder(config, device=device)
         self.output_embeddings = Linear(
-            in_features=config.layer.hidden_width,
+            in_features=config.layer.feedforward.hidden_width,
             out_features=config.embedding.vocab_size,
             bias=False,
             device=device,
         )
 
-    def forward(
-        self,
-        input_ids: Tensor,
-        attention_mask: Optional[AttentionMask] = None,
-        cache: Optional[List[KeyValueCache]] = None,
-        positions: Optional[Tensor] = None,
-        store_cache: bool = False,
-    ) -> CausalLMOutputWithCache[KeyValueCache]:
-        decoder_output = self.decoder(
-            input_ids,
-            attention_mask,
-            cache=cache,
-            store_cache=store_cache,
-            positions=positions,
-        )
-        logits = self.output_embeddings(decoder_output.last_hidden_layer_state)
-
-        return CausalLMOutputWithCache(
-            cache=decoder_output.cache,
-            embedding_output=decoder_output.embedding_layer,
-            layer_hidden_states=decoder_output.all_hidden_layer_states,
-            logits=logits,
-        )
-
     @classmethod
     def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
         return convert_hf_state_dict(cls, params)
 
     @classmethod
     def from_hf_config(
         cls: Type[Self],
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/config.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/decoder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,214 +1,162 @@
-from dataclasses import dataclass
+from functools import partial
+from typing import Any, Mapping, Optional, Type, TypeVar
 
+import torch
+from torch import Tensor
+from torch.nn import Dropout, Embedding, LayerNorm, ModuleList
+
+from ...layers.attention import (
+    AttentionHeads,
+    AttentionLinearBiases,
+    QkvMode,
+    SelfAttention,
+)
+from ...layers.embeddings import QueryKeyRotaryEmbeddings
+from ...layers.feedforward import PointwiseFeedForward
+from ...layers.transformer import (
+    DecoderLayer,
+    TransformerDropouts,
+    TransformerLayerNorms,
+)
+from ..hf_hub import FromHFHub
+from ..transformer import TransformerDecoder
+from ._hf import convert_hf_config, convert_hf_state_dict
+from .config import FalconConfig
+from .layer import OldFalconDecoderLayer
+
+# Only provided as typing.Self in Python 3.11+.
+Self = TypeVar("Self", bound="FalconDecoder")
 
-@dataclass
-class FalconAttentionConfig:
-    """
-    `Falcon`_ attention configuration.
-
-    .. _Falcon: https://arxiv.org/abs/2306.01116
-    """
-
-    dropout_prob: float
-    hidden_width: int
-    multi_query: bool
-    num_attention_heads: int
-    rotary_fraction: float
-    rotary_base: int
-    use_bias: bool
-
-    def __init__(
-        self,
-        *,
-        dropout_prob: float = 0.1,
-        hidden_width: int = 2560,
-        multi_query: bool = True,
-        num_attention_heads: int = 71,
-        rotary_base=10000,
-        rotary_fraction=0.25,
-        use_bias: bool = False,
-    ):
-        """
-        :param dropout_prob:
-            Dropout to apply after attention.
-        :param hidden_width:
-            Hidden width of the transformer.
-        :param multi_query:
-            Use multiple query heads and single key and value heads.
-        :param num_attention_heads:
-            Number of attention heads.
-        :param rotary_base:
-            Base in signifying the rotary embedding period.
-        :param rotary_fraction:
-            Fraction of hidden width to apply rotary embeddings to.
-            Must be in ``[0,1]``.
-        :param use_bias:
-            Use bias in linear layers.
-        """
 
-        self.dropout_prob = dropout_prob
-        self.hidden_width = hidden_width
-        self.multi_query = multi_query
-        self.num_attention_heads = num_attention_heads
-        self.rotary_base = rotary_base
-        self.rotary_fraction = rotary_fraction
-        self.use_bias = use_bias
-
-
-@dataclass
-class FalconEmbeddingConfig:
+class FalconDecoder(TransformerDecoder, FromHFHub):
     """
-    `Falcon`_ embedding configuration.
+    Falcon (`Penedo et al., 2019`_) decoder.
 
-    .. _Falcon: https://arxiv.org/abs/2306.01116
+    .. _Penedo et al., 2019: https://arxiv.org/abs/2306.01116
     """
 
-    dropout_prob: float
-    embedding_width: int
-    layer_norm_eps: float
-    vocab_size: int
-
     def __init__(
-        self,
-        *,
-        dropout_prob: float = 0.1,
-        embedding_width: int = 2560,
-        layer_norm_eps: float = 1e-5,
-        vocab_size: int = 50432,
+        self, config: FalconConfig, *, device: Optional[torch.device] = None
     ) -> None:
         """
-        :param dropout_prob:
-            Dropout to apply after attention.
-        :param embedding_width:
-            Width of the embeddings.
-        :param layer_norm_eps:
-            Epsilon for layer normalization.
-        :param vocab_size:
-            Vocabulary size (number of embeddings).
-        """
-
-        self.dropout_prob = dropout_prob
-        self.embedding_width = embedding_width
-        self.vocab_size = vocab_size
-        self.layer_norm_eps = layer_norm_eps
-
-
-@dataclass
-class FalconLayerConfig:
-    """
-    `Falcon`_ layer configuration.
-
-    .. _Falcon: https://arxiv.org/abs/2306.01116
-    """
-
-    dropout_prob: float
-    hidden_width: int
-    layer_norm_eps: float
-    num_hidden_layers: int
-    use_bias: bool
+        Construct a Falcon decoder.
 
-    def __init__(
-        self,
-        *,
-        dropout_prob: float = 0.0,
-        hidden_width: int = 2560,
-        num_hidden_layers: int = 32,
-        layer_norm_eps: float = 1e-5,
-        use_bias: bool = False,
-    ) -> None:
-        """
-        :param dropout_prob:
-            Dropout to apply after hidden layers.
-        :param hidden_width:
-            Hidden width of the transformer.
-        :param layer_norm_eps:
-            Epsilon for layer normalization.
-        :param num_hidden_layers:
-            Number of hidden layers.
-        :param use_bias:
-            Use bias in linear layers.
+        :param config:
+            Decoder configuration.
+        :param device:
+            Device to which the module is to be moved.
+        :returns:
+            The decoder.
         """
+        super().__init__()
 
-        self.dropout_prob = dropout_prob
-        self.hidden_width = hidden_width
-        self.num_hidden_layers = num_hidden_layers
-        self.layer_norm_eps = layer_norm_eps
-        self.use_bias = use_bias
+        self.embeddings = Embedding(
+            config.embedding.vocab_size, config.embedding.embedding_width, device=device
+        )
+        self.dropout = Dropout(p=config.embedding.dropout_prob)
 
+        if config.new_decoder_architecture:
+            decoder_layer = partial(
+                self._create_new_decoder_architecture_layer, config, device
+            )
+        else:
+            decoder_layer = partial(
+                self._create_old_decoder_architecture_layer, config, device
+            )
 
-class FalconConfig:
-    """
-    `Falcon`_ model configuration.
-
-    .. _Falcon: https://arxiv.org/abs/2306.01116
-    """
+        self.layers = ModuleList(
+            [decoder_layer() for _ in range(config.layer.num_hidden_layers)]
+        )
 
-    attention: FalconAttentionConfig
-    embedding: FalconEmbeddingConfig
-    layer: FalconLayerConfig
+        self.output_layer_norm = LayerNorm(
+            config.layer.feedforward.hidden_width,
+            config.layer.layer_norm_eps,
+            device=device,
+        )
 
-    def __init__(
-        self,
+    @classmethod
+    def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
+        return convert_hf_state_dict(cls, params)
+
+    @classmethod
+    def from_hf_config(
+        cls: Type[Self],
         *,
-        attention_probs_dropout_prob: float = 0.0,
-        hidden_dropout_prob: float = 0.0,
-        hidden_width: int = 2560,
-        layer_norm_eps: float = 1e-5,
-        multi_query: bool = True,
-        num_attention_heads: int = 71,
-        num_hidden_layers: int = 32,
-        rotary_embedding_base: int = 10000,
-        rotary_embedding_fraction: float = 0.25,
-        use_bias: bool = False,
-        vocab_size: int = 50280,
+        hf_config: Any,
+        device: Optional[torch.device] = None,
+    ) -> Self:
+        config = convert_hf_config(hf_config)
+        return cls(config, device=device)
+
+    def _create_old_decoder_architecture_layer(
+        self, config: FalconConfig, device: Optional[torch.device]
     ):
-        """
-        :param attention_probs_dropout_prob:
-            Dropout to apply after attention.
-        :param hidden_dropout_prob:
-            Dropout to apply to the hidden and embedding layers.
-        :param hidden_width:
-            Hidden width of the transformer.
-        :param layer_norm_eps:
-            Epsilon for layer normalization.
-        :param multi_query:
-            Use multiple query heads and single key and value heads.
-        :param num_hidden_layers:
-            Number of hidden layers.
-        :param rotary_embedding_base:
-            Base in signifying the rotary embedding period.
-        :param rotary_embedding_fraction:
-            Fraction of hidden width to apply rotary embeddings to.
-            Must be in ``[0,1]``.
-        :param use_bias:
-            Use bias in linear layers.
-        :param vocab_size:
-            Vocabulary size (number of embeddings).
-        """
+        return OldFalconDecoderLayer(config.layer, device=device)
 
-        # TODO: max_position_embeddings and model_max_length are currently
-        #       not used. We may want to limit the rotary embeddings to these
-        #       values in the future. We should check empirically if the auto
-        #       resizing in rotary embeddings makes sense.
-
-        self.attention = FalconAttentionConfig(
-            dropout_prob=attention_probs_dropout_prob,
-            hidden_width=hidden_width,
-            multi_query=multi_query,
-            num_attention_heads=num_attention_heads,
-            rotary_fraction=rotary_embedding_fraction,
-            rotary_base=rotary_embedding_base,
-            use_bias=use_bias,
-        )
-        self.embedding = FalconEmbeddingConfig(
-            dropout_prob=hidden_dropout_prob,
-            embedding_width=hidden_width,
-            vocab_size=vocab_size,
-            layer_norm_eps=layer_norm_eps,
-        )
-        self.layer = FalconLayerConfig(
-            dropout_prob=hidden_dropout_prob,
-            hidden_width=hidden_width,
-            layer_norm_eps=layer_norm_eps,
-            num_hidden_layers=num_hidden_layers,
+    def _create_new_decoder_architecture_layer(
+        self, config: FalconConfig, device: Optional[torch.device]
+    ):
+        if config.layer.attention.rotary_embeddings is None:
+            raise ValueError(
+                "Falcon attention config does not contain rotary embedding parameters"
+            )
+
+        hidden_width = config.layer.feedforward.hidden_width
+        layer_norm = partial(
+            LayerNorm,
+            hidden_width,
+            config.layer.layer_norm_eps,
+            device=device,
+        )
+        num_attention_heads = config.layer.attention.num_query_heads
+        attention_biases = (
+            AttentionLinearBiases(
+                num_attention_heads=config.layer.attention.num_query_heads,
+                is_causal=True,
+                is_inverted=True,
+            )
+            if config.layer.attention.use_alibi
+            else None
+        )
+        # Rotary embeddings are disabled when using ALiBi.
+        rotary_embeds = (
+            QueryKeyRotaryEmbeddings(
+                fraction=config.layer.attention.rotary_embeddings.rotary_fraction,
+                base=config.layer.attention.rotary_embeddings.rotary_base,
+                dims_per_head=hidden_width // num_attention_heads,
+            )
+            if not config.layer.attention.use_alibi
+            else None
+        )
+        return DecoderLayer(
+            attention_layer=SelfAttention(
+                attention_biases=attention_biases,
+                attention_heads=AttentionHeads.key_value_broadcast(
+                    num_query_heads=num_attention_heads,
+                    num_key_value_heads=config.layer.attention.num_key_value_heads,
+                ),
+                dropout_prob=config.layer.attention.dropout_prob,
+                hidden_width=hidden_width,
+                qkv_mode=QkvMode.MERGED_SPLIT_AFTER,
+                rotary_embeds=rotary_embeds,
+                use_bias=config.layer.attention.use_bias,
+                device=device,
+            ),
+            feed_forward_layer=PointwiseFeedForward(
+                activation=config.layer.feedforward.activation.module(),
+                hidden_width=hidden_width,
+                intermediate_width=config.layer.feedforward.intermediate_width,
+                use_bias=config.layer.feedforward.use_bias,
+                use_gate=config.layer.feedforward.use_gate,
+                device=device,
+            ),
+            dropouts=TransformerDropouts.parallel_attention_dropout(
+                config.layer.dropout_prob
+            ),
+            layer_norms=TransformerLayerNorms(
+                attn_input_layer_norm=layer_norm(),
+                ffn_input_layer_norm=layer_norm(),
+            ),
+            # The new decoder uses parallel attention unconditionally.
+            parallel_attention=True,
         )
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/decoder.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/bert/encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,98 @@
-from typing import Any, List, Mapping, Optional, Type, TypeVar
+from functools import partial
+from typing import Any, Mapping, Optional, Type, TypeVar
 
 import torch
 from torch import Tensor
-from torch.nn import Dropout, Embedding, LayerNorm, ModuleList
+from torch.nn import LayerNorm
 
-from ...layers.attention import AttentionMask
-from ...layers.cache import KeyValueCache
+from ...layers.attention import AttentionHeads, QkvMode, SelfAttention
+from ...layers.feedforward import PointwiseFeedForward
+from ...layers.transformer import (
+    EncoderLayer,
+    TransformerDropouts,
+    TransformerLayerNorms,
+)
 from ..hf_hub import FromHFHub
-from ..module import DecoderModule
-from ..output import ModelOutputWithCache
+from ..transformer import TransformerEncoder
 from ._hf import convert_hf_config, convert_hf_state_dict
-from .config import FalconConfig
-from .layer import FalconDecoderLayer
+from .config import BERTConfig
+from .embeddings import BERTEmbeddings
 
 # Only provided as typing.Self in Python 3.11+.
-Self = TypeVar("Self", bound="FalconDecoder")
+Self = TypeVar("Self", bound="BERTEncoder")
 
 
-class FalconDecoder(DecoderModule, FromHFHub):
+class BERTEncoder(TransformerEncoder, FromHFHub):
     """
-    `Falcon`_ decoder.
+    BERT (`Devlin et al., 2018`_) encoder.
 
-    .. _Falcon: https://arxiv.org/abs/2306.01116
+    .. _Devlin et al., 2018 : https://arxiv.org/abs/1810.04805
     """
 
-    def __init__(
-        self, config: FalconConfig, *, device: Optional[torch.device] = None
-    ) -> None:
+    def __init__(self, config: BERTConfig, *, device: Optional[torch.device] = None):
         """
-        Construct a Falcon decoder.
+        Construct a BERT encoder.
 
         :param config:
-            Decoder configuration.
+            Encoder configuration.
         :param device:
             Device to which the module is to be moved.
         :returns:
-            The decoder.
+            The encoder.
         """
         super().__init__()
 
-        self.embeddings = Embedding(
-            config.embedding.vocab_size, config.embedding.embedding_width, device=device
-        )
-        self.dropout = Dropout(p=config.embedding.dropout_prob)
+        self.embeddings = BERTEmbeddings(config.embedding, config.layer, device=device)
+        self.max_seq_len = config.model_max_length
 
-        self.layers = ModuleList(
+        layer_norm = partial(
+            LayerNorm,
+            config.layer.feedforward.hidden_width,
+            config.layer.layer_norm_eps,
+            device=device,
+        )
+        self.layers = torch.nn.ModuleList(
             [
-                FalconDecoderLayer(config.layer, config.attention, device=device)
+                EncoderLayer(
+                    attention_layer=SelfAttention(
+                        attention_heads=AttentionHeads.uniform(
+                            config.layer.attention.num_query_heads
+                        ),
+                        dropout_prob=config.layer.attention.dropout_prob,
+                        hidden_width=config.layer.feedforward.hidden_width,
+                        qkv_mode=QkvMode.SEPARATE,
+                        rotary_embeds=None,
+                        use_bias=config.layer.attention.use_bias,
+                        device=device,
+                    ),
+                    feed_forward_layer=PointwiseFeedForward(
+                        activation=config.layer.feedforward.activation.module(),
+                        hidden_width=config.layer.feedforward.hidden_width,
+                        intermediate_width=config.layer.feedforward.intermediate_width,
+                        use_bias=config.layer.feedforward.use_bias,
+                        use_gate=config.layer.feedforward.use_gate,
+                        device=device,
+                    ),
+                    dropouts=TransformerDropouts.layer_output_dropouts(
+                        config.layer.dropout_prob
+                    ),
+                    layer_norms=TransformerLayerNorms(
+                        attn_residual_layer_norm=layer_norm(),
+                        ffn_residual_layer_norm=layer_norm(),
+                    ),
+                    parallel_attention=config.layer.attention.parallel_attention,
+                )
                 for _ in range(config.layer.num_hidden_layers)
             ]
         )
 
-        self.output_layer_norm = LayerNorm(
-            config.layer.hidden_width, config.layer.layer_norm_eps, device=device
-        )
-
-    def forward(
-        self,
-        input_ids: Tensor,
-        attention_mask: Optional[AttentionMask] = None,
-        cache: Optional[List[KeyValueCache]] = None,
-        positions: Optional[Tensor] = None,
-        store_cache: bool = False,
-    ) -> ModelOutputWithCache[KeyValueCache]:
-        embeddings = self.embeddings(input_ids)
-        embeddings = self.dropout(embeddings)
-        layer_output = embeddings
-
-        layer_outputs = []
-        new_cache = []
-        layer_cache = None
-        for layer in self.layers:
-            if cache is not None:
-                # The key-value cache is stored per layer, so peel off one
-                # layer at a time.
-                layer_cache = cache[0]
-                cache = cache[1:]
-            layer_output, new_layer_cache = layer(
-                layer_output,
-                attention_mask,
-                cache=layer_cache,
-                store_cache=store_cache,
-                positions=positions,
-            )
-            layer_outputs.append(layer_output)
-            if store_cache:
-                new_cache.append(new_layer_cache)
-
-        layer_outputs[-1] = self.output_layer_norm(layer_outputs[-1])
-
-        return ModelOutputWithCache(
-            embedding_output=embeddings,
-            layer_hidden_states=layer_outputs,
-            cache=new_cache if store_cache else None,
-        )
-
     @classmethod
     def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
-        return convert_hf_state_dict(cls, params)
+        return convert_hf_state_dict(params)
 
     @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/falcon/layer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/falcon/layer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,103 @@
 from typing import Optional, Tuple
 
 import torch
 from torch import Tensor
 from torch.nn import Module
 
 from ...layers.attention import (
+    AttentionHeads,
+    AttentionLinearBiases,
     AttentionMask,
     KeyValueCache,
-    QkvHeadSharing,
     QkvMode,
-    RotaryEmbeddingConfig,
     SelfAttention,
 )
+from ...layers.embeddings import QueryKeyRotaryEmbeddings
 from ...layers.feedforward import PointwiseFeedForward
-from .config import FalconAttentionConfig, FalconLayerConfig
+from ..config import TransformerLayerConfig
 
 
-class FalconDecoderLayer(Module):
+class OldFalconDecoderLayer(Module):
     """
-    `Falcon`_ layer.
+    Falcon (`Penedo et al., 2019`_) layer using the old decoder architecture.
 
-    .. _Falcon: https://arxiv.org/abs/2306.01116
+    .. _Penedo et al., 2019: https://arxiv.org/abs/2306.01116
     """
 
     def __init__(
         self,
-        layer_config: FalconLayerConfig,
-        attention_config: FalconAttentionConfig,
+        layer_config: TransformerLayerConfig,
         *,
         device: Optional[torch.device] = None
     ):
         super().__init__()
 
+        attention_config = layer_config.attention
+        if attention_config.rotary_embeddings is None:
+            raise ValueError(
+                "Falcon attention config does not contain rotary embedding parameters"
+            )
+
+        self.parallel_attention = attention_config.parallel_attention
+
+        hidden_width = layer_config.feedforward.hidden_width
+        num_attention_heads = attention_config.num_query_heads
+        attention_biases = (
+            AttentionLinearBiases(
+                num_attention_heads=attention_config.num_query_heads,
+                is_causal=True,
+                is_inverted=True,
+            )
+            if attention_config.use_alibi
+            else None
+        )
+        # Rotary embeddings are disabled when using ALiBi.
+        rotary_embeds = (
+            QueryKeyRotaryEmbeddings(
+                fraction=attention_config.rotary_embeddings.rotary_fraction,
+                base=attention_config.rotary_embeddings.rotary_base,
+                dims_per_head=hidden_width // num_attention_heads,
+            )
+            if not attention_config.use_alibi
+            else None
+        )
         self.mha = SelfAttention(
+            attention_biases=attention_biases,
             dropout_prob=attention_config.dropout_prob,
-            hidden_width=attention_config.hidden_width,
-            qkv_head_sharing=QkvHeadSharing.KEY_VALUE
-            if attention_config.multi_query
-            else QkvHeadSharing.NONE,
-            num_attention_heads=attention_config.num_attention_heads,
-            rotary_embeds=RotaryEmbeddingConfig(
-                base=attention_config.rotary_base,
-                fraction=attention_config.rotary_fraction,
+            hidden_width=hidden_width,
+            attention_heads=AttentionHeads.key_value_broadcast(
+                num_query_heads=attention_config.num_query_heads,
+                num_key_value_heads=attention_config.num_key_value_heads,
             ),
-            qkv_mode=QkvMode.MERGED_SPLIT_AFTER,
+            rotary_embeds=rotary_embeds,
+            qkv_mode=QkvMode.MERGED_SPLIT_AFTER
+            if attention_config.num_key_value_heads == 1
+            else QkvMode.MERGED_SPLIT_BEFORE,
             use_bias=attention_config.use_bias,
             device=device,
         )
         self.attn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
-        self.input_layer_norm = torch.nn.LayerNorm(
-            layer_config.hidden_width, eps=layer_config.layer_norm_eps, device=device
+        self.attn_layer_norm = torch.nn.LayerNorm(
+            hidden_width, eps=layer_config.layer_norm_eps, device=device
         )
 
+        if not self.parallel_attention:
+            self.ffn_layer_norm = torch.nn.LayerNorm(
+                hidden_width,
+                eps=layer_config.layer_norm_eps,
+                device=device,
+            )
+
         self.ffn = PointwiseFeedForward(
-            hidden_act="gelu",
-            hidden_width=layer_config.hidden_width,
-            intermediate_width=4 * layer_config.hidden_width,
-            use_bias=layer_config.use_bias,
-            use_gate=False,
+            activation=layer_config.feedforward.activation.module(),
+            hidden_width=hidden_width,
+            intermediate_width=layer_config.feedforward.intermediate_width,
+            use_bias=layer_config.feedforward.use_bias,
+            use_gate=layer_config.feedforward.use_gate,
             device=device,
         )
         self.ffn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
 
     def forward(
         self,
         input: Tensor,
@@ -77,37 +113,45 @@
             Hidden representations to apply the layer to.
 
             *Shape:* ``(batch_size, seq_len, width)``
         :param attention_mask:
             Attention mask. Sequence elements for which the
             corresponding mask element is set to ``False`` are ignored
             during attention calculation.
-
-            *Shape:* ``(batch_size, seq_len)``
         :param cache:
             Key/value cache to avoid recomputing key/value representations
             for tokens that were previously seen.
         :param positions:
             Input positions. Positions are needed to look up rotary embeddings.
             Normally, these positions are calculated automatically. But if the
             positions deviate for some reason, they can be provided through this
             argument.
         :param store_cache:
             Whether to cache the key/value representations for future reuse.
         :returns:
             Layer output and the key/value cache.
         """
-        # NOTE: we currently only support parallel attention.
-        input_layer_norm = self.input_layer_norm(input)
+        residual = input
+
+        attn_layer_norm = self.attn_layer_norm(input)
 
         attn_out, cache = self.mha(
-            input_layer_norm,
+            attn_layer_norm,
             attention_mask,
             cache=cache,
             store_cache=store_cache,
             positions=positions,
             use_causal_mask=True,
         )
-        attn_out = self.attn_output_dropout(attn_out)
 
-        ffn_out = self.ffn(input_layer_norm)
-        return self.ffn_output_dropout(ffn_out + attn_out) + input, cache
+        if self.parallel_attention:
+            ffn_layer_norm = attn_layer_norm
+        else:
+            residual = residual + self.attn_output_dropout(attn_out)
+            ffn_layer_norm = self.ffn_layer_norm(residual)
+
+        ffn_out = self.ffn(ffn_layer_norm)
+
+        if self.parallel_attention:
+            ffn_out += attn_out
+
+        return residual + self.ffn_output_dropout(ffn_out), cache
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/_hf.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/_hf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 import re
-from typing import Any, Mapping
+from typing import Any, Callable, Dict, Mapping, Tuple, Union
 
 from torch import Tensor
 
+from ...layers.activations import Activation
+from ..hf_hub import _process_hf_keys
 from ..module import DecoderModule
 from .config import GPTNeoXConfig
 
 ATTENTION_DROPOUT = "attention_probs_dropout_prob"
 HIDDEN_DROPOUT = "hidden_dropout_prob"
 EXTRA_KWARG_KEYS = [ATTENTION_DROPOUT, HIDDEN_DROPOUT]
 
-HF_CONFIG_KEY_MAPPING = {
-    "hidden_act": "hidden_act",
+HF_CONFIG_KEY_MAPPING: Dict[str, Union[str, Tuple[str, Callable]]] = {
+    "hidden_act": ("activation", Activation),
     "hidden_size": "hidden_width",
     "intermediate_size": "intermediate_width",
     "layer_norm_eps": "layer_norm_eps",
     "max_position_embeddings": "max_position_embeddings",
     "num_attention_heads": "num_attention_heads",
     "num_hidden_layers": "num_hidden_layers",
     "rotary_emb_base": "rotary_embedding_base",
     "rotary_pct": "rotary_embedding_fraction",
     "vocab_size": "vocab_size",
 }
 
 
 def convert_hf_config(hf_config: Any) -> GPTNeoXConfig:
-    missing_keys = tuple(
-        sorted(set(HF_CONFIG_KEY_MAPPING.keys()).difference(set(hf_config.keys())))
+    kwargs = _process_hf_keys(
+        "GPT-NeoX", hf_config, HF_CONFIG_KEY_MAPPING, EXTRA_KWARG_KEYS
     )
-    if len(missing_keys) != 0:
-        raise ValueError(
-            f"Missing keys in Hugging Face GPT-NeoX model config: {missing_keys}"
-        )
-
-    kwargs = {curated: hf_config[hf] for hf, curated in HF_CONFIG_KEY_MAPPING.items()}
-    # Handle config options that are not set in all models.
-    kwargs.update({k: hf_config[k] for k in EXTRA_KWARG_KEYS if k in hf_config})
     return GPTNeoXConfig(
         model_max_length=hf_config["max_position_embeddings"],
         **kwargs,
     )
 
 
 def convert_hf_state_dict(cls, params: Mapping[str, Tensor]) -> Mapping[str, Tensor]:
@@ -72,16 +66,16 @@
 
         # Pointwise feedforward
         name = re.sub(r"\.mlp", r".ffn", name)
         name = re.sub(r"\.dense_h_to_4h", r".intermediate", name)
         name = re.sub(r"\.dense_4h_to_h", r".output", name)
 
         # Layer norms
-        name = re.sub(r"\.input_layernorm", r".input_layer_norm", name)
-        name = re.sub(r"\.post_attention_layernorm", r".ffn_layer_norm", name)
+        name = re.sub(r"\.input_layernorm", r".attn_input_layer_norm", name)
+        name = re.sub(r"\.post_attention_layernorm", r".ffn_input_layer_norm", name)
         name = re.sub(r"final_layer_norm\.", r"output_layer_norm.", name)
 
         # Embeddings
         name = re.sub(r"embed_in\.", r"embeddings.", name)
         name = re.sub(r"embed_out\.", r"output_embeddings.", name)
 
         out[name] = parameter
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/causal_lm.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/causal_lm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-from typing import Any, List, Mapping, Optional, Set, Type, TypeVar
+from typing import Any, Mapping, Optional, Set, Type, TypeVar
 
 import torch
 from torch import Tensor
 from torch.nn import Linear
 
-from ...layers.attention import AttentionMask
-from ...layers.cache import KeyValueCache
 from ...quantization import Quantizable
 from ..hf_hub import FromHFHub
-from ..module import CausalLMModule
-from ..output import CausalLMOutputWithCache
+from ..transformer import TransformerCausalLM
 from ._hf import convert_hf_config, convert_hf_state_dict
 from .config import GPTNeoXConfig
 from .decoder import GPTNeoXDecoder
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="GPTNeoXCausalLM")
 
 
-class GPTNeoXCausalLM(CausalLMModule[KeyValueCache], FromHFHub, Quantizable):
+class GPTNeoXCausalLM(TransformerCausalLM, FromHFHub, Quantizable):
     """
     GPT-NeoX (`Black et al., 2022`_) causal language model.
 
     .. _Black et al., 2022: https://arxiv.org/abs/2204.06745
     """
 
     def __init__(
@@ -38,44 +35,20 @@
         :returns:
             The causal LM.
         """
         super().__init__()
 
         self.decoder = GPTNeoXDecoder(config, device=device)
         self.output_embeddings = Linear(
-            in_features=config.layer.hidden_width,
+            in_features=config.layer.feedforward.hidden_width,
             out_features=config.embedding.vocab_size,
             bias=False,
             device=device,
         )
 
-    def forward(
-        self,
-        input_ids: Tensor,
-        attention_mask: Optional[AttentionMask] = None,
-        cache: Optional[List[KeyValueCache]] = None,
-        positions: Optional[Tensor] = None,
-        store_cache: bool = False,
-    ) -> CausalLMOutputWithCache[KeyValueCache]:
-        decoder_output = self.decoder(
-            input_ids,
-            attention_mask,
-            cache=cache,
-            store_cache=store_cache,
-            positions=positions,
-        )
-        logits = self.output_embeddings(decoder_output.last_hidden_layer_state)
-
-        return CausalLMOutputWithCache(
-            cache=decoder_output.cache,
-            embedding_output=decoder_output.embedding_layer,
-            layer_hidden_states=decoder_output.all_hidden_layer_states,
-            logits=logits,
-        )
-
     @classmethod
     def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
         return convert_hf_state_dict(cls, params)
 
     @classmethod
     def from_hf_config(
         cls: Type[Self],
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/gpt_neox/layer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/decoder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,117 @@
-from typing import Optional, Tuple
+from functools import partial
+from typing import Any, Mapping, Optional, Type, TypeVar
 
 import torch
 from torch import Tensor
-from torch.nn import Module
+from torch.nn import Dropout, Embedding, LayerNorm, ModuleList
 
-from ...layers.attention import (
-    AttentionMask,
-    KeyValueCache,
-    QkvHeadSharing,
-    QkvMode,
-    RotaryEmbeddingConfig,
-    SelfAttention,
-)
+from ...layers.attention import AttentionHeads, QkvMode, SelfAttention
+from ...layers.embeddings import QueryKeyRotaryEmbeddings
 from ...layers.feedforward import PointwiseFeedForward
-from .config import GPTNeoXAttentionConfig, GPTNeoXLayerConfig
+from ...layers.transformer import (
+    DecoderLayer,
+    TransformerDropouts,
+    TransformerLayerNorms,
+)
+from ..hf_hub import FromHFHub
+from ..transformer import TransformerDecoder
+from ._hf import convert_hf_config, convert_hf_state_dict
+from .config import GPTNeoXConfig
+
+# Only provided as typing.Self in Python 3.11+.
+Self = TypeVar("Self", bound="GPTNeoXDecoder")
 
 
-class GPTNeoXDecoderLayer(Module):
+class GPTNeoXDecoder(TransformerDecoder, FromHFHub):
     """
-    GPT-NeoX (`Black et al., 2022`_) decoder layer.
+    GPT-NeoX (`Black et al., 2022`_) decoder.
 
     .. _Black et al., 2022: https://arxiv.org/abs/2204.06745
     """
 
     def __init__(
-        self,
-        layer_config: GPTNeoXLayerConfig,
-        attention_config: GPTNeoXAttentionConfig,
-        *,
-        device: Optional[torch.device] = None
-    ):
+        self, config: GPTNeoXConfig, *, device: Optional[torch.device] = None
+    ) -> None:
+        """
+        Construct a GPT-NeoX decoder.
+
+        :param config:
+            Decoder configuration.
+        :param device:
+            Device to which the module is to be moved.
+        :returns:
+            The decoder.
+        """
         super().__init__()
 
-        self.mha = SelfAttention(
-            dropout_prob=attention_config.dropout_prob,
-            qkv_head_sharing=QkvHeadSharing.NONE,
-            hidden_width=attention_config.hidden_width,
-            num_attention_heads=attention_config.num_attention_heads,
-            qkv_mode=QkvMode.MERGED_SPLIT_BEFORE,
-            rotary_embeds=RotaryEmbeddingConfig(
-                fraction=attention_config.rotary_fraction,
-                base=attention_config.rotary_base,
-            ),
-            use_bias=True,
-            device=device,
-        )
-        self.attn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
-        self.input_layer_norm = torch.nn.LayerNorm(
-            layer_config.hidden_width, eps=layer_config.layer_norm_eps, device=device
+        self.embeddings = Embedding(
+            config.embedding.vocab_size, config.embedding.embedding_width, device=device
         )
+        self.dropout = Dropout(p=config.embedding.dropout_prob)
 
-        self.ffn = PointwiseFeedForward(
-            hidden_act=layer_config.hidden_act,
-            hidden_width=layer_config.hidden_width,
-            intermediate_width=layer_config.intermediate_width,
-            use_bias=True,
-            use_gate=False,
+        hidden_width = config.layer.feedforward.hidden_width
+        num_attention_heads = config.layer.attention.num_query_heads
+        layer_norm = partial(
+            LayerNorm,
+            hidden_width,
+            config.layer.layer_norm_eps,
             device=device,
         )
-        self.ffn_layer_norm = torch.nn.LayerNorm(
-            layer_config.hidden_width, eps=layer_config.layer_norm_eps, device=device
+        if config.layer.attention.rotary_embeddings is None:
+            raise ValueError(
+                "GPT-NeoX attention config does not contain rotary embedding parameters"
+            )
+        self.layers = ModuleList(
+            [
+                DecoderLayer(
+                    attention_layer=SelfAttention(
+                        attention_heads=AttentionHeads.uniform(num_attention_heads),
+                        dropout_prob=config.layer.attention.dropout_prob,
+                        hidden_width=hidden_width,
+                        qkv_mode=QkvMode.MERGED_SPLIT_BEFORE,
+                        rotary_embeds=QueryKeyRotaryEmbeddings(
+                            fraction=config.layer.attention.rotary_embeddings.rotary_fraction,
+                            base=config.layer.attention.rotary_embeddings.rotary_base,
+                            dims_per_head=hidden_width // num_attention_heads,
+                        ),
+                        use_bias=config.layer.attention.use_bias,
+                        device=device,
+                    ),
+                    feed_forward_layer=PointwiseFeedForward(
+                        activation=config.layer.feedforward.activation.module(),
+                        hidden_width=hidden_width,
+                        intermediate_width=config.layer.feedforward.intermediate_width,
+                        use_bias=config.layer.feedforward.use_bias,
+                        use_gate=config.layer.feedforward.use_gate,
+                        device=device,
+                    ),
+                    dropouts=TransformerDropouts.layer_output_dropouts(
+                        config.layer.dropout_prob
+                    ),
+                    layer_norms=TransformerLayerNorms(
+                        attn_input_layer_norm=layer_norm(),
+                        ffn_input_layer_norm=layer_norm(),
+                    ),
+                    parallel_attention=config.layer.attention.parallel_attention,
+                )
+                for _ in range(config.layer.num_hidden_layers)
+            ]
         )
-        self.ffn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
-
-    def forward(
-        self,
-        input: Tensor,
-        attention_mask: Optional[AttentionMask],
-        cache: Optional[KeyValueCache] = None,
-        positions: Optional[Tensor] = None,
-        store_cache: bool = False,
-    ) -> Tuple[Tensor, Optional[KeyValueCache]]:
-        """
-        Apply the GPT-NeoX layer to the given piece hidden representations.
-
-        :param input:
-            Hidden representations to apply the layer to.
 
-            *Shape:* ``(batch_size, seq_len, width)``
-        :param attention_mask:
-            Attention mask. Sequence elements for which the
-            corresponding mask element is set to ``False`` are ignored
-            during attention calculation.
-
-            *Shape:* ``(batch_size, seq_len)``
-        :param cache:
-            Key/value cache to avoid recomputing
-            key/value representations for tokens that were previously seen.
-        :param positions:
-            Input positions. Positions are needed to look up rotary embeddings.
-            Normally, these positions are calculated automatically. But if the
-            positions deviate for some reason, they can be provided through this argument.
-        :param store_cache:
-            Whether to cache the key/value representations for future reuse.
-        :returns:
-            Layer output and the key/value cache.
-
-            *Shape:* ``(batch_size, seq_len, width)``
-        """
-        attn_out, cache = self.mha(
-            self.input_layer_norm(input),
-            attention_mask,
-            cache=cache,
-            store_cache=store_cache,
-            positions=positions,
-            use_causal_mask=True,
+        self.output_layer_norm = LayerNorm(
+            hidden_width, config.layer.layer_norm_eps, device=device
         )
-        attn_out = self.attn_output_dropout(attn_out)
-        ffn_out = self.ffn(self.ffn_layer_norm(input))
-        ffn_out = self.ffn_output_dropout(ffn_out)
 
-        # Parallel attention & feed-forward, Section 2.1.2
-        return input + attn_out + ffn_out, cache
+    @classmethod
+    def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
+        return convert_hf_state_dict(cls, params)
+
+    @classmethod
+    def from_hf_config(
+        cls: Type[Self],
+        *,
+        hf_config: Any,
+        device: Optional[torch.device] = None,
+    ) -> Self:
+        config = convert_hf_config(hf_config)
+        return cls(config, device=device)
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/_hf.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/_hf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,85 @@
 import re
-from typing import Any, Mapping
+from types import MappingProxyType
+from typing import Any, Callable, Dict, Mapping, Tuple, Union
 
 from torch import Tensor
 
-from ..module import DecoderModule
-from .config import LLaMAConfig
-
-ATTENTION_DROPOUT = "attention_probs_dropout_prob"
-HIDDEN_DROPOUT = "hidden_dropout_prob"
-EXTRA_KWARG_KEYS = [ATTENTION_DROPOUT, HIDDEN_DROPOUT]
-
-
-HF_CONFIG_KEY_MAPPING = {
-    "hidden_act": "hidden_act",
+from ...layers.activations import Activation
+from ..hf_hub import _process_hf_keys
+from .config import RoBERTaConfig
+
+HF_KEY_TO_CURATED_KEY = MappingProxyType(
+    {
+        "embeddings.word_embeddings.weight": "embeddings.inner.word_embeddings.weight",
+        "embeddings.token_type_embeddings.weight": "embeddings.inner.token_type_embeddings.weight",
+        "embeddings.position_embeddings.weight": "embeddings.inner.position_embeddings.weight",
+        "embeddings.LayerNorm.weight": "embeddings.inner.layer_norm.weight",
+        "embeddings.LayerNorm.bias": "embeddings.inner.layer_norm.bias",
+    }
+)
+
+
+HF_CONFIG_KEY_MAPPING: Dict[str, Union[str, Tuple[str, Callable]]] = {
+    "pad_token_id": "padding_id",
+    "attention_probs_dropout_prob": "attention_probs_dropout_prob",
+    "hidden_act": ("activation", Activation),
+    "hidden_dropout_prob": "hidden_dropout_prob",
     "hidden_size": "hidden_width",
     "intermediate_size": "intermediate_width",
-    "rms_norm_eps": "rms_norm_eps",
+    "layer_norm_eps": "layer_norm_eps",
+    "max_position_embeddings": "max_position_embeddings",
     "num_attention_heads": "num_attention_heads",
     "num_hidden_layers": "num_hidden_layers",
+    "type_vocab_size": "type_vocab_size",
     "vocab_size": "vocab_size",
 }
 
 
-def convert_hf_config(hf_config: Any) -> LLaMAConfig:
-    missing_keys = tuple(
-        sorted(set(HF_CONFIG_KEY_MAPPING.keys()).difference(set(hf_config.keys())))
-    )
-    if len(missing_keys) != 0:
-        raise ValueError(
-            f"Missing keys in Hugging Face LLaMA model config: {missing_keys}"
-        )
+def convert_hf_config(hf_config: Any) -> RoBERTaConfig:
+    kwargs = _process_hf_keys("RoBERTa", hf_config, HF_CONFIG_KEY_MAPPING)
 
-    kwargs = {curated: hf_config[hf] for hf, curated in HF_CONFIG_KEY_MAPPING.items()}
-    # Handle config options that are not set in all models.
-    kwargs.update({k: hf_config[k] for k in EXTRA_KWARG_KEYS if k in hf_config})
-    return LLaMAConfig(
-        rotary_embedding_base=10000,
-        rotary_embedding_fraction=1.0,
+    return RoBERTaConfig(
+        embedding_width=hf_config["hidden_size"],
+        # Positions embeddings for 0..padding_id are reserved.
+        model_max_length=hf_config["max_position_embeddings"]
+        - (kwargs["padding_id"] + 1),
         **kwargs,
     )
 
 
-def convert_hf_state_dict(cls, params: Mapping[str, Tensor]) -> Mapping[str, Tensor]:
-    """Convert state dict from HF paramater naming to ours.
-    The function is insensitive to prefixes, to allow loading
-    both the decoder and the full LM."""
-    if issubclass(cls, DecoderModule):
-        stripped_params = {re.sub(r"^model\.", "", k): v for k, v in params.items()}
-    else:
-        stripped_params = {
-            re.sub(r"^model\.", "decoder.", k): v for k, v in params.items()
-        }
-
+def convert_hf_state_dict(params: Mapping[str, Tensor]) -> Mapping[str, Tensor]:
     out = {}
+
+    # Strip the `roberta` prefix from XLM-RoBERTa model parameters.
+    stripped_params = {re.sub(r"^roberta\.", "", k): v for k, v in params.items()}
+
     for name, parameter in stripped_params.items():
-        # Attention
-        name = re.sub(r"\.self_attn", r".mha", name)
-        name = re.sub(r"\.q_proj", r".query", name)
-        name = re.sub(r"\.k_proj", r".key", name)
-        name = re.sub(r"\.v_proj", r".value", name)
-        name = re.sub(r"\.o_proj", r".output", name)
-
-        # Pointwise feedforward
-        name = re.sub(r"\.mlp", r".ffn", name)
-        name = re.sub(r"\.up_proj", r".intermediate", name)
-        name = re.sub(r"\.down_proj", r".output", name)
-        name = re.sub(r"\.gate_proj", r".gate", name)
-
-        # RMS norms
-        name = re.sub(r"\.input_layernorm", r".attn_rms_norm", name)
-        name = re.sub(r"\.post_attention_layernorm", r".ffn_rms_norm", name)
-        name = re.sub(r"^(decoder\.)?norm\.", r"\1output_rms_norm.", name)
-
-        # Embeddings
-        name = re.sub(r"embed_tokens\.", r"embeddings.", name)
-        name = re.sub(r"lm_head\.", r"output_embeddings.", name)
+        if "encoder.layer." not in name:
+            continue
+
+        # TODO: Make these substitutions less ugly.
+
+        # Remove the prefix and rename the internal 'layers' variable.
+        name = re.sub(r"^encoder\.", "", name)
+        name = re.sub(r"^layer", "layers", name)
+
+        # The HF model has one more level of indirection for the output layers in their
+        # attention heads and the feed-forward network layers.
+        name = re.sub(r"\.attention\.self\.(query|key|value)", r".mha.\1", name)
+        name = re.sub(r"\.attention\.(output)\.dense", r".mha.\1", name)
+        name = re.sub(
+            r"\.attention\.output\.LayerNorm", r".attn_residual_layer_norm", name
+        )
+        name = re.sub(r"\.(intermediate)\.dense", r".ffn.\1", name)
+        name = re.sub(
+            r"(\.\d+)\.output\.LayerNorm", r"\1.ffn_residual_layer_norm", name
+        )
+        name = re.sub(r"(\.\d+)\.(output)\.dense", r"\1.ffn.\2", name)
 
         out[name] = parameter
 
+    for hf_name, curated_name in HF_KEY_TO_CURATED_KEY.items():
+        if hf_name in stripped_params:
+            out[curated_name] = stripped_params[hf_name]
+
     return out
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/causal_lm.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/llama/causal_lm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import Any, List, Mapping, Optional, Set, Type, TypeVar
+from typing import Any, Mapping, Optional, Set, Type, TypeVar
 
 import torch
 from torch import Tensor
 from torch.nn import Linear
 
-from ...layers.attention import AttentionMask
-from ...layers.cache import KeyValueCache
 from ...quantization import Quantizable
 from ..hf_hub import FromHFHub
-from ..module import CausalLMModule
-from ..output import CausalLMOutputWithCache
+from ..transformer import TransformerCausalLM
 from ._hf import convert_hf_config, convert_hf_state_dict
 from .config import LLaMAConfig
 from .decoder import LLaMADecoder
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="LLaMACausalLM")
 
 
-class LLaMACausalLM(CausalLMModule[KeyValueCache], FromHFHub, Quantizable):
+class LLaMACausalLM(TransformerCausalLM, FromHFHub, Quantizable):
     """
-    LLaMa (`Touvron et al., 2023`_) causal language model.
+    LLaMa (`Touvron et al., 2023 [a]`_, `Touvron et al., 2023 [b]`_) causal language model.
 
-    .. _Touvron et al., 2023: https://arxiv.org/abs/2302.13971
+    .. _Touvron et al., 2023 [a]: https://arxiv.org/abs/2302.13971
+    .. _Touvron et al., 2023 [b]: https://arxiv.org/abs/2307.09288
     """
 
     def __init__(
         self, config: LLaMAConfig, *, device: Optional[torch.device] = None
     ) -> None:
         """
         Construct a LLaMA causal LM.
@@ -38,44 +36,20 @@
         :returns:
             The causal LM.
         """
         super().__init__()
 
         self.decoder = LLaMADecoder(config, device=device)
         self.output_embeddings = Linear(
-            in_features=config.layer.hidden_width,
+            in_features=config.layer.feedforward.hidden_width,
             out_features=config.embedding.vocab_size,
             bias=False,
             device=device,
         )
 
-    def forward(
-        self,
-        input_ids: Tensor,
-        attention_mask: Optional[AttentionMask] = None,
-        cache: Optional[List[KeyValueCache]] = None,
-        positions: Optional[Tensor] = None,
-        store_cache: bool = False,
-    ) -> CausalLMOutputWithCache[KeyValueCache]:
-        decoder_output = self.decoder(
-            input_ids,
-            attention_mask,
-            cache=cache,
-            store_cache=store_cache,
-            positions=positions,
-        )
-        logits = self.output_embeddings(decoder_output.last_hidden_layer_state)
-
-        return CausalLMOutputWithCache(
-            cache=decoder_output.cache,
-            embedding_output=decoder_output.embedding_layer,
-            layer_hidden_states=decoder_output.all_hidden_layer_states,
-            logits=logits,
-        )
-
     @classmethod
     def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
         return convert_hf_state_dict(cls, params)
 
     @classmethod
     def from_hf_config(
         cls: Type[Self],
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/decoder.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,33 @@
-from typing import Any, List, Mapping, Optional, Type, TypeVar
+from typing import List, Optional
 
 import torch
 from torch import Tensor
-from torch.nn import Dropout, Embedding, ModuleList
+from torch.nn import Module, ModuleList
 
-from ...layers.attention import AttentionMask
-from ...layers.cache import KeyValueCache
-from ...layers.normalization import RMSNorm
-from ..hf_hub import FromHFHub
-from ..module import DecoderModule
-from ..output import ModelOutputWithCache
-from ._hf import convert_hf_config, convert_hf_state_dict
-from .config import LLaMAConfig
-from .layer import LLaMADecoderLayer
-
-# Only provided as typing.Self in Python 3.11+.
-Self = TypeVar("Self", bound="LLaMADecoder")
-
-
-class LLaMADecoder(DecoderModule, FromHFHub):
-    """
-    LLaMa (`Touvron et al., 2023`_) decoder.
-
-    .. _Touvron et al., 2023: https://arxiv.org/abs/2302.13971
-    """
-
-    def __init__(
-        self, config: LLaMAConfig, *, device: Optional[torch.device] = None
-    ) -> None:
-        """
-        Construct a LLaMA decoder.
-
-        :param config:
-            Decoder configuration.
-        :param device:
-            Device to which the module is to be moved.
-        :returns:
-            The decoder.
-        """
-        super().__init__()
+from ..layers.attention import AttentionMask
+from ..layers.cache import KeyValueCache
+from .module import CausalLMModule, DecoderModule, EncoderModule
+from .output import CausalLMOutputWithCache, ModelOutput, ModelOutputWithCache
 
-        self.embeddings = Embedding(
-            config.embedding.vocab_size, config.embedding.embedding_width, device=device
-        )
-        self.dropout = Dropout(p=config.embedding.dropout_prob)
 
-        self.layers = ModuleList(
-            [
-                LLaMADecoderLayer(config.layer, config.attention, device=device)
-                for _ in range(config.layer.num_hidden_layers)
-            ]
-        )
+class TransformerDecoder(DecoderModule):
+    """
+    Transformer decoder (`Vaswani et al., 2017`_) base class.
 
-        self.output_rms_norm = RMSNorm(
-            config.layer.hidden_width, eps=config.layer.rms_norm_eps, device=device
-        )
+    This class provides an implementation of the ``forward`` method.
+    Subclasses must set the given member attributes.
+
+    .. _Vaswani et al., 2017: https://arxiv.org/abs/1706.03762
+    """
+
+    dropout: Module
+    embeddings: Module
+    layers: ModuleList
+    output_layer_norm: Module
 
     def forward(
         self,
         input_ids: Tensor,
         attention_mask: Optional[AttentionMask] = None,
         cache: Optional[List[KeyValueCache]] = None,
         positions: Optional[Tensor] = None,
@@ -84,28 +53,83 @@
                 store_cache=store_cache,
                 positions=positions,
             )
             layer_outputs.append(layer_output)
             if store_cache:
                 new_cache.append(new_layer_cache)
 
-        layer_outputs[-1] = self.output_rms_norm(layer_outputs[-1])
+        layer_outputs[-1] = self.output_layer_norm(layer_outputs[-1])
 
         return ModelOutputWithCache(
-            embedding_output=embeddings,
-            layer_hidden_states=layer_outputs,
+            all_outputs=[embeddings, *layer_outputs],
             cache=new_cache if store_cache else None,
         )
 
-    @classmethod
-    def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
-        return convert_hf_state_dict(cls, params)
-
-    @classmethod
-    def from_hf_config(
-        cls: Type[Self],
-        *,
-        hf_config: Any,
-        device: Optional[torch.device] = None,
-    ) -> Self:
-        config = convert_hf_config(hf_config)
-        return cls(config, device=device)
+
+class TransformerCausalLM(CausalLMModule[KeyValueCache]):
+    """
+    Transformer causal LM (`Vaswani et al., 2017`_) base class.
+
+    This class provides an implementation of the ``forward`` method.
+    Subclasses must set the given member attributes..
+
+    .. _Vaswani et al., 2017: https://arxiv.org/abs/1706.03762
+    """
+
+    decoder: TransformerDecoder
+    output_embeddings: Module
+
+    def forward(
+        self,
+        input_ids: Tensor,
+        attention_mask: Optional[AttentionMask] = None,
+        cache: Optional[List[KeyValueCache]] = None,
+        positions: Optional[Tensor] = None,
+        store_cache: bool = False,
+    ) -> CausalLMOutputWithCache[KeyValueCache]:
+        decoder_output = self.decoder(
+            input_ids,
+            attention_mask,
+            cache=cache,
+            store_cache=store_cache,
+            positions=positions,
+        )
+        if torch.jit.is_tracing():
+            logits = self.output_embeddings(decoder_output[0][-1])
+            return decoder_output + (logits,)  # type: ignore[return-value]
+        else:
+            logits = self.output_embeddings(decoder_output.last_hidden_layer_state)
+            return CausalLMOutputWithCache(
+                all_outputs=decoder_output.all_outputs,
+                cache=decoder_output.cache,
+                logits=logits,
+            )
+
+
+class TransformerEncoder(EncoderModule):
+    """
+    Transformer encoder (`Vaswani et al., 2017`_) base class.
+
+    This class provides an implementation of the ``forward`` method.
+    Subclasses must set the given member attributes.
+
+    .. _Vaswani et al., 2017: https://arxiv.org/abs/1706.03762
+    """
+
+    embeddings: Module
+    layers: ModuleList
+
+    def forward(
+        self,
+        input_ids: Tensor,
+        attention_mask: Optional[AttentionMask] = None,
+        token_type_ids: Optional[Tensor] = None,
+    ) -> ModelOutput:
+        embeddings = self.embeddings(input_ids, token_type_ids, None)
+        layer_output = embeddings
+
+        layer_outputs = []
+        for layer in self.layers:
+            layer_output, _ = layer(layer_output, attention_mask)
+            layer_outputs.append(layer_output)
+
+        return ModelOutput(all_outputs=[embeddings, *layer_outputs])
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/llama/layer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/gpt_neox/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,105 @@
-from typing import Optional, Tuple
+from dataclasses import dataclass
 
-import torch
-from torch import Tensor
-from torch.nn import Module
-
-from ...layers.attention import (
-    AttentionMask,
-    KeyValueCache,
-    QkvHeadSharing,
-    QkvMode,
+from ...layers.activations import Activation
+from ..config import (
     RotaryEmbeddingConfig,
-    SelfAttention,
+    TransformerAttentionLayerConfig,
+    TransformerEmbeddingLayerConfig,
+    TransformerFeedForwardLayerConfig,
+    TransformerLayerConfig,
 )
-from ...layers.feedforward import PointwiseFeedForward
-from ...layers.normalization import RMSNorm
-from .config import LLaMAAttentionConfig, LLaMALayerConfig
 
 
-class LLaMADecoderLayer(Module):
+@dataclass
+class GPTNeoXConfig:
     """
-    LLaMa (`Touvron et al., 2023`_) decoder layer.
+    GPT-NeoX (`Black et al., 2022`_) model configuration.
 
-    .. _Touvron et al., 2023: https://arxiv.org/abs/2302.13971
+    .. _Black et al., 2022: https://arxiv.org/abs/2204.06745
     """
 
+    embedding: TransformerEmbeddingLayerConfig
+    layer: TransformerLayerConfig
+
     def __init__(
         self,
-        layer_config: LLaMALayerConfig,
-        attention_config: LLaMAAttentionConfig,
         *,
-        device: Optional[torch.device] = None
+        attention_probs_dropout_prob: float = 0.0,
+        activation: Activation = Activation.GELU,
+        hidden_dropout_prob: float = 0.0,
+        hidden_width: int = 2560,
+        intermediate_width: int = 10240,
+        layer_norm_eps: float = 1e-5,
+        max_position_embeddings: int = 2048,
+        model_max_length: int = 2048,
+        num_attention_heads: int = 32,
+        num_hidden_layers: int = 32,
+        rotary_embedding_base: int = 10000,
+        rotary_embedding_fraction: float = 0.25,
+        vocab_size: int = 50280,
     ):
-        super().__init__()
-
-        self.mha = SelfAttention(
-            dropout_prob=attention_config.dropout_prob,
-            qkv_head_sharing=QkvHeadSharing.NONE,
-            hidden_width=attention_config.hidden_width,
-            num_attention_heads=attention_config.num_attention_heads,
-            qkv_mode=QkvMode.SEPARATE,
-            rotary_embeds=RotaryEmbeddingConfig(
-                fraction=attention_config.rotary_fraction,
-                base=attention_config.rotary_base,
-            ),
-            use_bias=False,
-            device=device,
-        )
-        self.attn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
-        self.attn_rms_norm = RMSNorm(
-            layer_config.hidden_width, eps=layer_config.rms_norm_eps, device=device
-        )
-
-        self.ffn = PointwiseFeedForward(
-            hidden_act=layer_config.hidden_act,
-            hidden_width=layer_config.hidden_width,
-            intermediate_width=layer_config.intermediate_width,
-            use_bias=False,
-            use_gate=True,
-            device=device,
-        )
-        self.ffn_rms_norm = RMSNorm(
-            layer_config.hidden_width, eps=layer_config.rms_norm_eps, device=device
-        )
-        self.ffn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
-
-    def forward(
-        self,
-        input: Tensor,
-        attention_mask: Optional[AttentionMask],
-        cache: Optional[KeyValueCache] = None,
-        positions: Optional[Tensor] = None,
-        store_cache: bool = False,
-    ) -> Tuple[Tensor, Optional[KeyValueCache]]:
         """
-        Apply the LLaMA layer to the given piece hidden representations.
-
-        :param input:
-            Hidden representations to apply the layer to.
-
-            *Shape:* ``(batch_size, seq_len, width)``
-        :param attention_mask:
-            Attention mask. Sequence elements for which the
-            corresponding mask element is set to ``False`` are ignored
-            during attention calculation.
-
-            *Shape:* ``(batch_size, seq_len)``
-        :param cache:
-            Key/value cache to avoid recomputing
-            key/value representations for tokens that were previously seen.
-        :param positions:
-            Input positions. Positions are needed to look up rotary embeddings.
-            Normally, these positions are calculated automatically. But if the
-            positions deviate for some reason, they can be provided through this argument.
-        :param store_cache:
-            Whether to cache the key/value representations for future reuse.
-        :returns:
-            Layer output and the key/value cache.
+        :param attention_probs_dropout_prob:
+            Dropout to apply after attention.
+        :param activation:
+            Activation used by the pointwise feed-forward layers.
+        :param hidden_dropout_prob:
+            Dropout to apply to the hidden and embedding layers.
+        :param hidden_width:
+            Hidden width of the transformer.
+        :param intermediate_width:
+            Intermediate width in the feed-forward layer. The non-linearity
+            is applied in this intermediate width.
+        :param layer_norm_eps:
+            Epsilon for layer normalization.
+        :param num_attention_heads:
+            Number of attention heads.
+        :param num_hidden_layers:
+            Number of hidden layers.
+        :param rotary_embedding_base:
+            Base in signifying the rotary embedding period.
+        :param rotary_embedding_fraction:
+            Fraction of hidden width to apply rotary embeddings to.
+            Must be in ``[0,1]``.
+        :param vocab_size:
+            Vocabulary size (number of embeddings).
         """
-        attn_out, cache = self.mha(
-            self.attn_rms_norm(input),
-            attention_mask,
-            cache=cache,
-            store_cache=store_cache,
-            positions=positions,
-            use_causal_mask=True,
-        )
-        attn_out = self.attn_output_dropout(attn_out)
-
-        input = input + attn_out
-
-        ffn_out = self.ffn(self.ffn_rms_norm(input))
-        ffn_out = self.ffn_output_dropout(ffn_out)
 
-        return input + ffn_out, cache
+        # TODO: max_position_embeddings and model_max_length are currently
+        #       not used. We may want to limit the rotary embeddings to these
+        #       values in the future. We should check empirically if the auto
+        #       resizing in rotary embeddings makes sense.
+
+        self.embedding = TransformerEmbeddingLayerConfig(
+            dropout_prob=hidden_dropout_prob,
+            embedding_width=hidden_width,
+            vocab_size=vocab_size,
+            layer_norm_eps=layer_norm_eps,
+            max_position_embeddings=None,
+            type_vocab_size=None,
+        )
+        self.layer = TransformerLayerConfig(
+            attention=TransformerAttentionLayerConfig(
+                dropout_prob=attention_probs_dropout_prob,
+                hidden_width=hidden_width,
+                num_query_heads=num_attention_heads,
+                num_key_value_heads=num_attention_heads,
+                parallel_attention=True,
+                rotary_embeddings=RotaryEmbeddingConfig(
+                    rotary_fraction=rotary_embedding_fraction,
+                    rotary_base=rotary_embedding_base,
+                ),
+                use_bias=True,
+                use_alibi=False,
+            ),
+            feedforward=TransformerFeedForwardLayerConfig(
+                hidden_width=hidden_width,
+                intermediate_width=intermediate_width,
+                activation=activation,
+                use_bias=True,
+                use_gate=False,
+            ),
+            dropout_prob=hidden_dropout_prob,
+            layer_norm_eps=layer_norm_eps,
+            num_hidden_layers=num_hidden_layers,
+        )
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/module.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import abstractmethod
 from typing import Generic, List, Optional
 
 from torch import Tensor
-from torch.nn import Module
+from torch.nn import Module, ModuleList
 
 from ..layers.attention import AttentionMask
+from ..layers.cache import KeyValueCache
 from .output import CacheT, CausalLMOutputWithCache, ModelOutput, ModelOutputWithCache
 
 
 class CausalLMModule(Generic[CacheT], Module):
     """
     Base class for causal language model modules.
     """
@@ -29,17 +30,14 @@
             Piece identifiers to apply the decoder to.
 
             *Shape:* ``(batch_size, seq_len)``
         :param attention_mask:
             Attention mask. Sequence elements for which the
             corresponding mask element is set to ``False`` are ignored
             during attention calculation.
-
-
-            *Shape:* ``(batch_size, seq_len)``
         :param cache:
             Key/value cache to avoid recomputing key/value representations
             for tokens that were previously seen.
         :param positions:
             Input positions. Positions are needed to look up rotary embeddings.
             Normally, these positions are calculated automatically. But if the
             positions deviate for some reason, they can be provided through this argument.
@@ -74,16 +72,14 @@
             Piece identifiers to apply the decoder to.
 
             *Shape:* ``(batch_size, seq_len)``
         :param attention_mask:
             Attention mask. Sequence elements for which the
             corresponding mask element is set to ``False`` are ignored
             during attention calculation.
-
-            *Shape:* ``(batch_size, seq_len)``
         :param cache:
             Key/value cache to avoid recomputing key/value representations
             for tokens that were previously seen.
         :param positions:
             Input positions. Positions are needed to look up rotary embeddings.
             Normally, these positions are calculated automatically. But if the
             positions deviate for some reason, they can be provided through this argument.
@@ -116,16 +112,14 @@
             Piece identifiers to apply the encoder to.
 
             *Shape:* ``(batch_size, seq_len)``
         :param attention_mask:
             Attention mask. Sequence elements for which the
             corresponding mask element is set to ``False`` are ignored
             during attention calculation.
-
-            *Shape:* ``(batch_size, seq_len)``
         :param token_type_ids:
             Token type identifiers to indicate the spans of different
             sequences in the input. Useful when performing tasks like
             sequence classification and question answering.
 
             *Shape:* ``(batch_size, seq_len)``
         :returns:
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/config.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         :param num_hidden_layers:
             Number of hidden layers.
         :param attention_probs_dropout_prob:
             Dropout probabilty of the self-attention layers.
         :param hidden_dropout_prob:
             Dropout probabilty of the point-wise feed-forward and
             embedding layers.
-        :param hidden_act:
-            Activation used by the point-wise feed-forward layers.
+        :param activation:
+            Activation used by the pointwise feed-forward layers.
         :param vocab_size:
             Size of main vocabulary.
         :param type_vocab_size:
             Size of token type vocabulary.
         :param max_position_embeddings:
             Maximum length of position embeddings.
         :param model_max_length:
@@ -53,12 +53,13 @@
         :param padding_id:
             Index of the padding meta-token.
         """
         super(RoBERTaConfig, self).__init__(
             *args,
             layer_norm_eps=layer_norm_eps,
             max_position_embeddings=max_position_embeddings,
-            padding_id=padding_id,
             type_vocab_size=type_vocab_size,
             vocab_size=vocab_size,
             **kwargs
         )
+
+        self.padding_id = padding_id
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/roberta/encoder.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/roberta/encoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+from functools import partial
 from typing import Any, Mapping, Optional, Type, TypeVar
 
 import torch
 from torch import Tensor
+from torch.nn import LayerNorm
 
-from ...layers.attention import AttentionMask
-from ..bert.layer import BERTEncoderLayer
+from ...layers.attention import AttentionHeads, QkvMode, SelfAttention
+from ...layers.feedforward import PointwiseFeedForward
+from ...layers.transformer import (
+    EncoderLayer,
+    TransformerDropouts,
+    TransformerLayerNorms,
+)
 from ..hf_hub import FromHFHub
-from ..module import EncoderModule
-from ..output import ModelOutput
+from ..transformer import TransformerEncoder
 from ._hf import convert_hf_config, convert_hf_state_dict
 from .config import RoBERTaConfig
 from .embeddings import RoBERTaEmbeddings
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="RoBERTaEncoder")
 
 
-class RoBERTaEncoder(EncoderModule, FromHFHub):
+class RoBERTaEncoder(TransformerEncoder, FromHFHub):
     """
     RoBERTa (`Liu et al., 2019`_) encoder.
 
     .. _Liu et al., 2019: https://arxiv.org/abs/1907.11692
     """
 
     def __init__(self, config: RoBERTaConfig, *, device: Optional[torch.device] = None):
@@ -35,47 +41,58 @@
             The encoder.
         """
         super().__init__()
 
         self.embeddings = RoBERTaEmbeddings(
             config.embedding, config.layer, padding_id=config.padding_id, device=device
         )
-        self.padding_id = config.padding_id
         self.max_seq_len = config.model_max_length
+
+        hidden_width = config.layer.feedforward.hidden_width
+        layer_norm = partial(
+            LayerNorm,
+            hidden_width,
+            config.layer.layer_norm_eps,
+            device=device,
+        )
         self.layers = torch.nn.ModuleList(
             [
-                BERTEncoderLayer(config.layer, config.attention, device=device)
+                EncoderLayer(
+                    attention_layer=SelfAttention(
+                        attention_heads=AttentionHeads.uniform(
+                            config.layer.attention.num_query_heads
+                        ),
+                        dropout_prob=config.layer.attention.dropout_prob,
+                        hidden_width=hidden_width,
+                        qkv_mode=QkvMode.SEPARATE,
+                        rotary_embeds=None,
+                        use_bias=config.layer.attention.use_bias,
+                        device=device,
+                    ),
+                    feed_forward_layer=PointwiseFeedForward(
+                        activation=config.layer.feedforward.activation.module(),
+                        hidden_width=hidden_width,
+                        intermediate_width=config.layer.feedforward.intermediate_width,
+                        use_bias=config.layer.feedforward.use_bias,
+                        use_gate=config.layer.feedforward.use_gate,
+                        device=device,
+                    ),
+                    dropouts=TransformerDropouts.layer_output_dropouts(
+                        config.layer.dropout_prob
+                    ),
+                    layer_norms=TransformerLayerNorms(
+                        attn_residual_layer_norm=layer_norm(),
+                        ffn_residual_layer_norm=layer_norm(),
+                    ),
+                    parallel_attention=config.layer.attention.parallel_attention,
+                )
                 for _ in range(config.layer.num_hidden_layers)
             ]
         )
 
-    def _create_attention_mask(self, x: Tensor) -> AttentionMask:
-        return AttentionMask(x.ne(self.padding_id))
-
-    def forward(
-        self,
-        input_ids: Tensor,
-        attention_mask: Optional[AttentionMask] = None,
-        token_type_ids: Optional[Tensor] = None,
-    ) -> ModelOutput:
-        if attention_mask is None:
-            attention_mask = self._create_attention_mask(input_ids)
-
-        embeddings = self.embeddings(input_ids, token_type_ids, None)
-        layer_output = embeddings
-
-        layer_outputs = []
-        for layer in self.layers:
-            layer_output = layer(layer_output, attention_mask)
-            layer_outputs.append(layer_output)
-
-        return ModelOutput(
-            embedding_output=embeddings, layer_hidden_states=layer_outputs
-        )
-
     @classmethod
     def convert_hf_state_dict(cls, params: Mapping[str, Tensor]):
         return convert_hf_state_dict(params)
 
     @classmethod
     def from_hf_config(
         cls: Type[Self],
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/models/xlm_roberta/encoder.py` & `curated-transformers-1.0.0.dev1/curated_transformers/models/xlm_roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/config.py` & `curated-transformers-1.0.0.dev1/curated_transformers/quantization/bnb/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,43 +16,44 @@
     #: ``NF4`` - NormalFloat 4-bit.
     NF4 = "nf4"
 
 
 @dataclass
 class _4BitConfig:
     """
-    Config for ``fp4``/``nf4`` quantization.
+    Configuration for ``fp4``/``nf4`` quantization.
     """
 
     quantization_dtype: Dtype4Bit
     compute_dtype: torch.dtype
     double_quantization: bool
 
 
 @dataclass
 class _8BitConfig:
     """
-    Config for ``int8`` quantization.
+    Configuration for ``int8`` quantization.
     """
 
     finetunable: bool
     outlier_threshold: float
 
 
 @dataclass
 class BitsAndBytesConfig:
     """
-    Config for quantization using the ``bitsandbytes`` library.
+    Configuration for quantization using the ``bitsandbytes`` library.
     """
 
     inner: Union[_4BitConfig, _8BitConfig]
 
     @staticmethod
     def for_8bit(outlier_threshold: float = 6.0, finetunable: bool = False):
-        """Construct a config for ``int8`` quantization.
+        """
+        Construct a configuration for ``int8`` quantization.
 
         :param outlier_threshold:
             Threshold for outlier detection during weight
             decomposition.
         :param finetunable:
             If the quantized model should support fine-tuning after
             quantization.
@@ -63,15 +64,16 @@
 
     @staticmethod
     def for_4bit(
         quantization_dtype: Dtype4Bit = Dtype4Bit.FP4,
         compute_dtype: torch.dtype = torch.bfloat16,
         double_quantization: bool = True,
     ):
-        """Construct a config for ``fp4``/``nf4`` quantization.
+        """
+        Construct a configuration for ``fp4``/``nf4`` quantization.
 
         :param quantization_dtype:
             Data type used for storing quantized weights.
         :param compute_dtype:
             Data type used for performing computations.
             Supported types: ``float16``, ``bfloat16``, ``float32``.
         :param double_quantization:
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/quantization/bnb/impl.py` & `curated-transformers-1.0.0.dev1/curated_transformers/quantization/bnb/impl.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/quantization/helpers.py` & `curated-transformers-1.0.0.dev1/curated_transformers/quantization/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from .bnb import prepare_for_quantization as bnb_prepare_for_quantization
 from .quantizable import Quantizable
 
 
 def prepare_module_for_quantization(
     module: Module, config: BitsAndBytesConfig
 ) -> Optional[TensorToParameterConverterT]:
-    """Prepares a module for quantiazation and returns an optional callback
+    """
+    Prepares a module for quantiazation and returns an optional callback
     to generate quantized parameter tensors.
 
     :param module:
         Top-level module to quantize. Should implement ``Quantizable``.
     :param config:
         Configuration for the quantizer.
     :returns:
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/quantization/quantizable.py` & `curated-transformers-1.0.0.dev1/curated_transformers/quantization/quantizable.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     module loading phase.
     """
 
     @classmethod
     @abstractmethod
     def modules_to_not_quantize(cls) -> Set[str]:
         """
-        Returns a set of prefixes that specify which
+        Return a set of prefixes that specify which
         modules are to be ignored during quantization.
 
         :returns:
             Set of module prefixes.
 
             If empty, all submodules will be quantized.
         """
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/conftest.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_auto_generator.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_dolly_v2.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_dolly_v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 @pytest.mark.skipif(not GPU_TESTS_ENABLED, reason="requires GPU")
 def test_generate_deterministic(dolly_generator):
     prompts = [
         "What is the Rust programming language?",
         "What is spaCy?",
     ]
     answers = [
-        "Rust is a multi-paradigm, high-level, general-purpose programming language. Rust is designed to have a small, stable, and fast implementation. Rust is also designed to be easy to learn. Rust is intended to be used for writing fast, reliable, and portable code.\n\n",
-        "SpaCy is an open-source natural language processing (NLP) library for Python. It is designed to be fast, scalable, and easy to use.\n\n",
+        "Rust is a multi-paradigm, high-level, general-purpose programming language. Rust is designed to have a small, consistent, and predictable language surface. Rust is also designed to be efficient, and to have a small memory footprint. Rust is designed to be safe, and to have a well-defined memory model. Rust is also designed to be concurrent, and to have a good support for concurrent programming. Rust is designed to be fast, and to have a good support for performance-critical code. Rust is also designed to be modular, and to have a good support for modular programming. Rust is designed to have a good support for internationalization and localization.\n\n",
+        "SpaCy is a natural language processing (NLP) library for Python that provides tokenization, part-of-speech (POS) tagging, named entity recognition (NER), and dependency parsing.\n\n",
     ]
     assert dolly_generator(prompts, config=GreedyGeneratorConfig()) == answers
 
     # Test in reverse order to verify that sequence identifiers are
     # handled correctly.
     assert (
         dolly_generator(prompts[::-1], config=GreedyGeneratorConfig()) == answers[::-1]
@@ -40,18 +40,16 @@
 @pytest.mark.slow
 @pytest.mark.skipif(not GPU_TESTS_ENABLED, reason="requires GPU")
 def test_generate_max_generated_pieces(dolly_generator):
     prompts = [
         "What is the Rust programming language?",
         "What is spaCy?",
     ]
-    answers = [
-        "Rust is a multi-paradigm,",
-        "SpaCy is an open-source natural language",
-    ]
+    answers = ["Rust is a multi-paradigm,", "SpaCy is a natural language processing (N"]
+
     assert (
         dolly_generator(prompts, config=GreedyGeneratorConfig(max_generated_pieces=10))
         == answers
     )
 
     # Test in reverse order to verify that sequence identifiers are
     # handled correctly.
@@ -69,18 +67,18 @@
     prompts = [
         "What is spaCy?",
         "What is spaCy?",
     ]
     # Fix the seed so that we are always randomly sampling in the same way.
     torch.manual_seed(0)
     assert dolly_generator(prompts, config=SampleGeneratorConfig(top_k=10)) == [
-        "SpaCy (short for Spanish-Portuguese-Chinese artificial intelligence language model) is an open-source language model (LLM) that uses a novel combination of deep learning, big-data, and semantic parsing to provide the best accuracy available with no human involvement. It is one of the most effective open-source language models.\n\n",
-        "SpaCy is an open-source package for Python that provides language model (LM) and automatic speech recognition (ASR) functionality.\n\n",
+        "SpaCy (short for spaCy Toolkit) is a Python library for Natural Language Processing (NLP) and machine translation based on the   spaCy research project. It has been open-source since June 2023 and has been used in production for NLP tasks like POS tag classification (part of OpenStax' TACL), question answering (QACQUEL), and semantic parsing (CoreNLP) as of October 2023.\n\n",
+        "SpaCy is an open-source package for Python that automates part of the process of building language models (LMs), or parsers for plain text, using a technique called graph-based learning. It supports English, French, German, Dutch, Italian, Spanish, Portuguese, Polish, and Dutch, all of which are official language groups of Europe.\n\n",
     ]
 
     torch.manual_seed(0)
     assert dolly_generator(
         prompts, config=SampleGeneratorConfig(top_k=5, temperature=2)
     ) == [
-        "SpaCy (short for spaCoN-based AI for Cyber-Security) is open source software that is used for automated language and named entity recognition (NER). SpaCy has been specifically developed for cybersecurity text processing and uses techniques that were developed for NLP over many years by the University of Pennsylvania's Named Entity Tagging (NetNesp) project, by Penn Tree Street Labs and other contributors, with a focus towards named- Entity Resolution (ner).\n\n",
-        "The spaCy library is an NLP package based on Stanford's SpanTweaked architecture for Stanford CoreNLP. SpaCy's main difference over Stanford CoreNLP is the usage of the PySpREnd language model, which was designed for Natural Language Processings, rather than just a simple parser, like the original SpanTweaked. This makes it possible to do much better NLP with the model than just the simple parsing of Stanford's ParserCore. However, spaCy is also a more general-purpose library, which also allows for more complex NLP tasks than just sentence parsing, such as part-of-speech taggers and dependency parsing, so it can be a good starting point for a NLTK-style library. In the field of machine learning and artificial intelligence, a spa file (spatial Pyramids file) describes a specific model trained on data, such as a part-of-speech tagged corpus, and it can be loaded and executed with spaCy's model or the Stanford CoreNLP's models (see Stanford CoreNLIps's API for loading a model from a spaCy spa file).\n\n",
+        "SpaCy (short for Spanish Language Model) is a natural language processor (NLP) for English based on the open source spaCy project. It supports sentence detection, part-of-speech tagging and coreference chains, among other things. spaCy was originally developed at the University of Cambridge's Machine Translation Lab. Since then, it has also developed a version optimized for Python that can be installed viapip.\n\n",
+        "The spaCy library is an NLP library based on Stanford's PoSpell architecture, that is designed to make NLP easy. spaCy supports all the standard NLTK pipeline stages and is able to outperform the NLTK on many Named Entity Tagging tasks, as well many others, both at test-level and at the system-wide average. It has a similar architecture to NLTK’s, but is designed from the ground up for the needs of a NLP research community rather than a production system: It has a smaller and less mature API, does away with its core tokenizer (which is notoriously hard to train), and is based on the Speller system from Stanford's CS-ADLDN program, which has been shown to significantly outperform the NLTK tokeniser in terms of both accuracy (93.7% on a test set of 20K tokens vs. NLTK's 76.3%) and efficiency.\n\n",
     ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_falcon.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_generic.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_generic.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import torch
 
 from curated_transformers.generation.config import (
     GreedyGeneratorConfig,
     SampleGeneratorConfig,
 )
 from curated_transformers.generation.default_generator import DefaultGenerator
+from curated_transformers.generation.logits import VocabMaskTransform
 
 from ..conftest import GPU_TESTS_ENABLED
 
 
 @pytest.fixture(scope="module")
 def falcon_generator():
     return DefaultGenerator.from_hf_hub(
@@ -80,7 +81,29 @@
     torch.manual_seed(0)
     assert falcon_generator(
         prompts, config=SampleGeneratorConfig(top_k=5, temperature=2)
     ) == [
         "spacy is a Natural Language Processing tool that can be used with many programming language to build NLP-based applications such as machine learning, sentiment analysis and chatbots, and to extract text from documents and other media. spacy uses the Stanford NLP model to learn from and generate text. This makes it one of the most popular and versatile NLP libraries available. The main features of spacy include text generation and manipulation, entity extraction, part-of-speech tagging and more.",
         "spaCy is a library for natural language processing in Scala. It's designed to be easy to use and provides a range of features including text analysis tools and pre-built models to analyze various text datasets.</s> \nCan spaCy be used to analyze text from different sources or does it only work with a specific type of text or data?</s> \nspaCy can analyze text from different sources and can be used to work with text in different languages such as German and Chinese.",
     ]
+
+
+@pytest.mark.slow
+@pytest.mark.skipif(not GPU_TESTS_ENABLED, reason="requires GPU")
+def test_generate_masked_output(falcon_generator):
+    prompt = [
+        "Repeat the following word: Madagascar\n",
+    ]
+    pieces_to_mask = [
+        58588,  # ĠMadagascar
+        18704,  # Mad
+        54453,  # agascar
+    ]
+
+    generated = falcon_generator(
+        prompt,
+        config=GreedyGeneratorConfig(
+            max_generated_pieces=50,
+            masked_pieces=pieces_to_mask,
+        ),
+    )
+    assert "Madagascar" not in generated
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/generation/test_stop.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/generation/test_stop.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import torch
 
 from curated_transformers.generation.state import GeneratorState
 from curated_transformers.generation.stop_conditions import (
     EndOfSequenceCondition,
     MaxGeneratedPiecesCondition,
 )
+from curated_transformers.layers.attention import AttentionMask
 
 
 def test_end_of_sequence_condition():
-    attention_mask = torch.ones((2, 2), dtype=torch.bool)
+    attention_mask = AttentionMask(torch.ones((2, 2), dtype=torch.bool))
     ids = torch.arange(0, 4).reshape(2, 2)
     state = GeneratorState(attention_mask=attention_mask, cache=None, prompt_ids=ids)
     state.generated_ids = torch.arange(4, 8).reshape(2, 2)
 
     completed_exclude = torch.zeros((2, 1), dtype=torch.bool)
     completed_include = torch.zeros((2, 1), dtype=torch.bool)
     EndOfSequenceCondition(4).update_completed(
@@ -46,15 +47,15 @@
         completed_include=completed_include,
     )
     assert completed_exclude.any()
     assert not completed_include.any()
 
 
 def test_max_generated_pieces_condition():
-    attention_mask = torch.ones((2, 3), dtype=torch.bool)
+    attention_mask = AttentionMask(torch.ones((2, 3), dtype=torch.bool))
     ids = torch.arange(0, 6).reshape(2, 3)
     state = GeneratorState(attention_mask=attention_mask, cache=None, prompt_ids=ids)
     state.generated_ids = torch.arange(4, 8).reshape(2, 2)
 
     completed_exclude = torch.zeros((2, 1), dtype=torch.bool)
     completed_include = torch.zeros((2, 1), dtype=torch.bool)
     MaxGeneratedPiecesCondition(3).update_completed(
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/camembert/test_encoder.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/models/test_hf_hub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
-from curated_transformers.models.camembert.encoder import CamemBERTEncoder
+from curated_transformers.models.bert.encoder import BERTEncoder
 
-from ...compat import has_hf_transformers
-from ...conftest import TORCH_DEVICES
-from ..util import assert_encoder_output_equals_hf
+from ..compat import has_hf_transformers
+from ..conftest import TORCH_DEVICES
+from .util import assert_encoder_output_equals_hf
 
 
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-def test_encoder(torch_device):
+def test_sharded_model_checkpoints(torch_device):
     assert_encoder_output_equals_hf(
-        CamemBERTEncoder, "explosion-testing/camembert-test", torch_device
+        BERTEncoder, "explosion-testing/bert-test-sharded", torch_device
     )
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/models/test_auto_models.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/models/test_auto_models.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/quantization/test_generation.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/quantization/test_generation.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from curated_transformers.tokenizers.legacy.bert_tokenizer import (
     BERTPreEncoder,
     BERTTokenizer,
 )
 from curated_transformers.tokenizers.legacy.legacy_tokenizer import DefaultNormalizer
 
 from ...compat import has_hf_transformers
-from ...util import torch_assertclose
+from ...utils import torch_assertclose
 from ..util import compare_tokenizer_outputs_with_hf_tokenizer
 
 
 @pytest.fixture
 def toy_tokenizer_from_files(test_dir):
     return BERTTokenizer.from_files(
         vocab_path=test_dir / "toy.wordpieces",
@@ -279,15 +279,15 @@
                     3,
                 ],
             ],
             dtype=torch.int32,
         ),
     )
     torch_assertclose(
-        pieces.attention_mask(),
+        pieces.attention_mask().bool_mask.squeeze(dim=(1, 2)),
         torch.tensor(
             [
                 [
                     True,
                     True,
                     True,
                     True,
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from curated_transformers.tokenizers import PiecesWithIds
 from curated_transformers.tokenizers.legacy.camembert_tokenizer import (
     CamemBERTTokenizer,
 )
 
 from ...compat import has_hf_transformers
-from ...util import torch_assertclose
+from ...utils import torch_assertclose
 from ..util import compare_tokenizer_outputs_with_hf_tokenizer
 
 
 @pytest.fixture
 def toy_tokenizer(test_dir):
     return CamemBERTTokenizer.from_files(
         model_path=test_dir / "toy.model",
@@ -330,15 +330,15 @@
                     6,
                 ],
             ],
             dtype=torch.int32,
         ),
     )
     torch_assertclose(
-        pieces.attention_mask(),
+        pieces.attention_mask().bool_mask.squeeze(dim=(1, 2)),
         torch.tensor(
             [
                 [
                     True,
                     True,
                     True,
                     True,
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import torch
 
 from curated_transformers.tokenizers import PiecesWithIds
 from curated_transformers.tokenizers.legacy import RoBERTaTokenizer
 
 from ...compat import has_hf_transformers
-from ...util import torch_assertclose
+from ...utils import torch_assertclose
 from ..util import compare_tokenizer_outputs_with_hf_tokenizer
 
 
 @pytest.fixture
 def toy_tokenizer_from_files(test_dir):
     return RoBERTaTokenizer.from_files(
         vocab_path=test_dir / "toy-vocab.json", merges_path=test_dir / "toy-merges.txt"
@@ -334,15 +334,15 @@
                     2,
                 ],
             ],
             dtype=torch.int32,
         ),
     )
     torch_assertclose(
-        pieces.attention_mask(),
+        pieces.attention_mask().bool_mask.squeeze(dim=(1, 2)),
         torch.tensor(
             [
                 [
                     True,
                     True,
                     True,
                     True,
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import torch
 
 from curated_transformers.tokenizers import PiecesWithIds
 from curated_transformers.tokenizers.legacy.xlmr_tokenizer import XLMRTokenizer
 
 from ...compat import has_hf_transformers
-from ...util import torch_assertclose
+from ...utils import torch_assertclose
 from ..util import compare_tokenizer_outputs_with_hf_tokenizer
 
 
 @pytest.fixture
 def toy_tokenizer(test_dir):
     return XLMRTokenizer.from_files(
         model_path=test_dir / "toy.model",
@@ -326,15 +326,15 @@
                 ],
             ],
             dtype=torch.int32,
         ),
     )
 
     torch_assertclose(
-        pieces.attention_mask(),
+        pieces.attention_mask().bool_mask.squeeze(dim=(1, 2)),
         torch.tensor(
             [
                 [
                     True,
                     True,
                     True,
                     True,
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-merges.txt` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-vocab.json` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.model` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.model`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.wordpieces` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_auto_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/test_auto_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_chunks.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/test_chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/test_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/test_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 
 from curated_transformers.tokenizers import Tokenizer
 from curated_transformers.tokenizers.chunks import InputChunks, TextChunk
 from curated_transformers.util.hf import TOKENIZER_JSON
 
 from ..compat import has_hf_transformers, transformers
-from ..util import torch_assertclose
+from ..utils import torch_assertclose
 from .util import compare_tokenizer_outputs_with_hf_tokenizer
 
 
 @dataclass
 class _TestModel:
     model: str
     pad_token: Optional[str] = None
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tests/tokenizers/util.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tests/tokenizers/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from ..compat import transformers
-from ..util import torch_assertclose
+from ..utils import torch_assertclose
 
 
 def compare_tokenizer_outputs_with_hf_tokenizer(
     sample_texts,
     hf_name,
     tokenizer_cls,
     pad_token: Optional[str] = None,
@@ -24,15 +24,18 @@
 
     # Test encoding with right-padding.
     hf_pieces = hf_tokenizer(sample_texts, padding=True, return_tensors="pt")
     torch_assertclose(
         pieces.padded_tensor(padding_id=hf_tokenizer.pad_token_id),
         hf_pieces["input_ids"].int(),
     )
-    torch_assertclose(pieces.attention_mask(), hf_pieces["attention_mask"].bool())
+    torch_assertclose(
+        pieces.attention_mask().bool_mask.squeeze(dim=(1, 2)),
+        hf_pieces["attention_mask"].bool(),
+    )
 
     # Test decoding
     decoded = tokenizer.decode(pieces.ids)
     hf_decoded = [
         hf_tokenizer.decode(ids, skip_special_tokens=True)
         for ids in hf_pieces["input_ids"]
     ]
@@ -43,9 +46,10 @@
     hf_tokenizer.padding_side = "left"
     hf_pieces = hf_tokenizer(sample_texts, padding=True, return_tensors="pt")
     torch_assertclose(
         pieces.padded_tensor(padding_id=hf_tokenizer.pad_token_id, pad_left=True),
         hf_pieces["input_ids"].int(),
     )
     torch_assertclose(
-        pieces.attention_mask(pad_left=True), hf_pieces["attention_mask"].bool()
+        pieces.attention_mask(pad_left=True).bool_mask.squeeze(dim=(1, 2)),
+        hf_pieces["attention_mask"].bool(),
     )
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/_hf_compat.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/_hf_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/auto_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/auto_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,16 @@
     """
     Infer the tokenizer class from the tokenizer configuration.
 
     :param name:
         Model name.
     :param revision:
         Model revision.
+    :returns:
+        Inferred class.
     """
 
     try:
         tokenizer_config = get_tokenizer_config(name=name, revision=revision)
     except EntryNotFoundError:
         return None
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/chunks.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/hf_hub.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/_fairseq.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/_fairseq.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/bert_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/bert_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         eos_piece: str = "[SEP]",
         unk_piece: str = "[UNK]",
         lowercase: bool = False,
         strip_accents: bool = False,
         tokenize_chinese_chars: bool = True,
     ):
         """
-        Construct a BERT tokenizer from a curated tokenizers WordPiece processor.
+        Construct a BERT tokenizer from a ``curated-tokenizers`` WordPiece processor.
 
         :param vocab:
             The word piece vocabulary.
         :param special_pieces:
             Special pieces.
         :param bos_piece:
             The piece used to mark the beginning of a sequence.
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/camembert_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/camembert_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self,
         *,
         processor: SentencePieceProcessor,
         bos_piece: str = "<s>",
         eos_piece: str = "</s>",
     ):
         """
-        Construct a CamemBERT tokenizer from a curated tokenizers SentencePiece processor.
+        Construct a CamemBERT tokenizer from a ``curated-tokenizers`` SentencePiece processor.
 
         :param processor:
             The processor to wrap.
         :param bos_piece:
             The piece to use to mark the beginning of a sequence.
         :param eos_piece:
             The piece to use to mark the end of a sequence.
@@ -114,19 +114,19 @@
         model_path: Path,
         bos_piece: str = "<s>",
         eos_piece: str = "</s>",
     ) -> Self:
         """
         Construct a tokenizer from vocabulary and merge files.
 
-        :params model_path:
+        :param model_path:
             Path to the SentencePiece model file.
-        :params bos_piece:
+        :param bos_piece:
             The piece to use to mark the beginning of a sequence.
-        :params eos_piece:
+        :param eos_piece:
             The piece to use to mark the end of a sequence.
         """
         processor = SentencePieceProcessor.from_file(str(model_path))
         return cls(
             processor=processor,
             bos_piece=bos_piece,
             eos_piece=eos_piece,
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/legacy_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/legacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/llama_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/llama_tokenizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 Self = TypeVar("Self", bound="LLaMATokenizer")
 
 DEFAULT_BOS_PIECE = "<s>"
 
 
 class LLaMATokenizer(SentencePieceTokenizer, LegacyFromHFHub):
     """
-    Legacy tokenizer for LLaMA (`Touvron et al., 2023`_) models.
+    Legacy tokenizer for LLaMA (`Touvron et al., 2023 [a]`_, `Touvron et al., 2023 [b]`_) models.
 
-    .. _Touvron et al., 2023: https://arxiv.org/abs/2302.13971
+    .. _Touvron et al., 2023 [a]: https://arxiv.org/abs/2302.13971
+    .. _Touvron et al., 2023 [b]: https://arxiv.org/abs/2307.09288
     """
 
     vocab_files: Dict[str, str] = {"model": "tokenizer.model"}
 
     def __init__(
         self,
         *,
         processor: SentencePieceProcessor,
         add_bos_piece: bool = True,
         add_eos_piece: bool = False,
     ):
         """
-        Construct a LLaMA tokenizer.
+        Construct a LLaMA tokenizer from a ``curated-tokenizers`` SentencePiece processor.
 
         :param processor:
             The processor to wrap.
         :param add_bos_piece:
             Add a begin-of-sequence piece.
         :param add_eos_piece:
             Add an end-of-sequence piece.
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/roberta_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
     def __init__(
         self,
         *,
         processor: SentencePieceProcessor,
     ):
         """
-        Construct a sentence piece tokenzier.
+        Construct a tokenizer from ``curated-tokenizers`` SentencePiece processor.
 
         :param processor:
             The processor to wrap.
         """
         self.processor = processor
-        self._eos_piece = processor.id_to_piece(processor.bos_id())
+        self._eos_piece = processor.id_to_piece(processor.eos_id())
 
     @property
     def eos_piece(self) -> Optional[str]:
         return self._eos_piece
 
     def piece_to_id(self, piece: str) -> Optional[int]:
         return self.processor.piece_to_id(piece)
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(
         self,
         *,
         vocab: Dict[str, int],
         special_pieces: Optional[Dict[str, int]],
     ):
         """
-        Construct a tokenizer from a curated tokenizers WordPiece processor.
+        Construct a tokenizer from a ``curated-tokenizers`` WordPiece processor.
 
         :param vocab:
             The word piece vocabulary.
         :param special_pieces:
             Special pieces.
         """
         # Special tokens are usually already in the wordpiece vocabs, but lets
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     def __init__(
         self,
         *,
         processor: SentencePieceProcessor,
     ):
         """
-        Construct a XLM-R tokenizer.
+        Construct a XLM-RoBERTa tokenizer from a ``curated-tokenizers`` SentencePiece processor.
 
         :param processor:
             The processor to wrap.
         """
         super().__init__(processor=processor)
 
         self.processor = processor
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/tokenizers/tokenizer.py` & `curated-transformers-1.0.0.dev1/curated_transformers/tokenizers/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,26 @@
 from typing import Any, Dict, Iterable, List, Optional, Type, TypeVar, Union, cast
 
 import torch
 from huggingface_hub.utils import EntryNotFoundError
 from tokenizers import Tokenizer as HFTokenizer
 from torch import Tensor
 
+from ..layers.attention import AttentionMask
 from ..util.hf import (
     HF_TOKENIZER_CONFIG,
     SPECIAL_TOKENS_MAP,
     TOKENIZER_JSON,
     get_special_piece,
     get_special_tokens_map,
     get_tokenizer_config,
+    hf_hub_download,
 )
 from ._hf_compat import clean_up_decoded_string_like_hf
-from .chunks import (
-    InputChunks,
-    MergedInputChunks,
-    MergedSpecialPieceChunk,
-    SpecialPieceChunk,
-    TextChunk,
-)
+from .chunks import InputChunks, MergedSpecialPieceChunk
 from .hf_hub import FromHFHub
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="Tokenizer")
 
 
 @dataclass
@@ -41,52 +37,70 @@
     :param pieces:
         Piece strings of each input sequence.
     """
 
     ids: List[List[int]]
     pieces: List[List[str]]
 
-    def attention_mask(self, *, pad_left: bool = False) -> Tensor:
+    def attention_mask(
+        self, *, pad_left: bool = False, device: Optional[torch.device] = None
+    ) -> AttentionMask:
         """
-        CPU tensor with attention masks. The mask is equivalent to:
+        Generate the attention masks. The mask is equivalent to:
         ``ids.padded_tensor(padding_id) != padding_id``
 
         :param pad_left:
             By default sequences shorter than the longest sequence are
             right-padded. Use left-padding when set to ``True``.
+        :param device:
+            Device on which the attention mask is created.
         :returns:
             The attention mask.
 
             *Shape:* ``(batch_size, max_seq_len)``
         """
         n_seqs = len(self.ids)
         max_len = max(len(seq_ids) for seq_ids in self.ids)
-        mask = torch.full((n_seqs, max_len), False)
+        mask = torch.full((n_seqs, max_len), False, device=device)
         for idx, seq_ids in enumerate(self.ids):
             if pad_left:
                 mask[idx, -len(seq_ids) :] = True
             else:
                 mask[idx, : len(seq_ids)] = True
-        return mask
-
-    def padded_tensor(self, *, padding_id: int, pad_left: bool = False):
-        """
-        Padded CPU tensor of the piece identifiers.
+        return AttentionMask(mask)
 
+    def padded_tensor(
+        self,
+        *,
+        padding_id: int = 0,
+        pad_left: bool = False,
+        device: Optional[torch.device] = None,
+    ) -> Tensor:
+        """
+        Generate a padded tensor of the piece identifiers.
+
+        :param padding_id:
+            Piece identifier of the padding piece. The actual identifier
+            generally doesn't matter when an attention mask is used (and
+            as long as it is a valid vocabulary index).
         :param pad_left:
             By default sequences shorter than the longest sequence are
             right-padded. Use left-padding when set to ``True``.
+        :param device:
+            Device on which the padded tensor is created.
         :returns:
             The padded piece ids.
 
             *Shape:* ``(batch_size, max_seq_len)``
         """
         n_seqs = len(self.ids)
         max_len = max(len(seq_ids) for seq_ids in self.ids)
-        padded = torch.full((n_seqs, max_len), padding_id, dtype=torch.int32)
+        padded = torch.full(
+            (n_seqs, max_len), padding_id, dtype=torch.int32, device=device
+        )
         for idx, seq_ids in enumerate(self.ids):
             if pad_left:
                 padded[idx, -len(seq_ids) :] = torch.tensor(seq_ids)
             else:
                 padded[idx, : len(seq_ids)] = torch.tensor(seq_ids)
         return padded
 
@@ -221,15 +235,15 @@
             The special piece, if defined in the special tokens mapping or
             the tokenizer configuration.
         """
         piece = None
         if special_tokens_map is not None:
             piece = get_special_piece(special_tokens_map, piece_name)
         if piece is None and tokenizer_config is not None:
-            get_special_piece(tokenizer_config, piece_name)
+            piece = get_special_piece(tokenizer_config, piece_name)
         return piece
 
     def decode(
         self,
         input: Iterable[Iterable[int]],
         *,
         skip_special_pieces: bool = True,
@@ -321,15 +335,22 @@
             tokenizer=hf_tokenizer,
             config=config,
             special_tokens_map=special_tokens_map,
         )
 
     @classmethod
     def from_hf_hub(cls: Type[Self], *, name: str, revision: str = "main") -> Self:
-        hf_tokenizer = HFTokenizer.from_pretrained(name, revision)
+        # We cannot directly use `HFTokenizer.from_pretrained`` to instantiate the HF
+        # tokenizer as it doesn't fetch the serialized files using the `huggingface_hub`
+        # library, which prevents us from being able to download models that require
+        # authentication.
+        tokenizer_path = hf_hub_download(
+            repo_id=name, filename=TOKENIZER_JSON, revision=revision
+        )
+        hf_tokenizer = HFTokenizer.from_file(tokenizer_path)
 
         try:
             config = get_tokenizer_config(name=name, revision=revision)
         except EntryNotFoundError:
             config = None
         try:
             special_tokens_map = get_special_tokens_map(name=name, revision=revision)
@@ -345,18 +366,22 @@
     def from_json(
         cls: Type[Self],
         tokenizer_json: str,
         config_json: Optional[str] = None,
         special_tokens_map_json: Optional[str] = None,
     ) -> Self:
         """
-        Load the tokenizer from a serialized JSON string..
+        Load the tokenizer from serialized JSON strings.
 
-        :param json:
-            The JSON string.
+        :param tokenizer_json:
+            The JSON string of the serialized tokenizer.
+        :param config_json:
+            The JSON string of the tokenizer config.
+        :param special_tokens_map_json:
+            The JSON string of the special tokens map.
         """
         hf_tokenizer = HFTokenizer.from_str(tokenizer_json)
         config = json.loads(config_json) if config_json is not None else None
         special_tokens_map = (
             json.loads(special_tokens_map_json)
             if special_tokens_map_json is not None
             else None
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/util/hf.py` & `curated-transformers-1.0.0.dev1/curated_transformers/util/hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
-import re
 import warnings
-from typing import Any, Dict, List, Mapping, Optional
+from typing import Any, Dict, List, Optional
 
 import huggingface_hub
-import torch
 from requests import HTTPError, ReadTimeout  # type: ignore
 
 HF_MODEL_CONFIG = "config.json"
 HF_MODEL_CHECKPOINT = "pytorch_model.bin"
 HF_MODEL_SHARDED_CHECKPOINT_INDEX = "pytorch_model.bin.index.json"
 HF_MODEL_SHARDED_CHECKPOINT_INDEX_WEIGHTS_KEY = "weight_map"
 HF_TOKENIZER_CONFIG = "tokenizer_config.json"
@@ -49,15 +47,15 @@
         if model_type is None:
             raise ValueError("Model type not found in Hugging Face model config")
         return model_type
 
 
 def get_model_config_filepath(name: str, revision: str) -> str:
     """
-    Returns the local file path of the Hugging Face model's config.
+    Return the local file path of the Hugging Face model's config.
     If the config is not found in the cache, it is downloaded from
     Hugging Face Hub.
 
     :param name:
         Model name.
     :param revision:
         Model revision.
@@ -73,15 +71,15 @@
             f"Couldn't find a valid config for model `{name}` "
             f"(revision `{revision}`) on HuggingFace Model Hub"
         )
 
 
 def get_model_checkpoint_filepaths(name: str, revision: str) -> List[str]:
     """
-    Returns a list of local file paths to PyTorch checkpoints that belong
+    Return a list of local file paths to PyTorch checkpoints that belong
     to the Hugging Face model. In case of non-sharded models, a single file path
     is returned. In case of sharded models, multiple file paths are returned.
 
     If the checkpoints are not found in the cache, they are downloaded from
     Hugging Face Hub.
 
     :param name:
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/util/pytorch.py` & `curated-transformers-1.0.0.dev1/curated_transformers/util/pytorch.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers/util/serde.py` & `curated-transformers-1.0.0.dev1/curated_transformers/util/serde.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     module_prefix: str,
     tensor_name: str,
     replacement_tensor: torch.Tensor,
     tensor_to_param_converter: TensorToParameterConverterT,
     device: Optional[torch.device] = None,
 ):
     """
-    Replaces a module's parameter or (persistent) buffer with the
+    Replace a module's parameter or (persistent) buffer with the
     passed tensor and moves it to the given device.
 
     This is a zero-copy operation (excluding D2H/H2D transfers) where
     the input tensor is directly associated with the module. Unexpected
     behaviour can occur if the same tensor is associated with multiple modules.
     """
     is_parameter = tensor_name in module._parameters
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers.egg-info/PKG-INFO` & `curated-transformers-1.0.0.dev1/curated_transformers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 1.0.0.dev0
-Summary: Curated transformer models
+Version: 1.0.0.dev1
+Summary: A PyTorch library of transformer models and components
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: quantization
 License-File: LICENSE
 
-# 🤖 Curated Transformers
+<img src="docs/source/logo.png" width="100" align="right"/>
+
+# Curated Transformers
 
 [![Documentation Status](https://readthedocs.org/projects/button/badge/?version=latest)](https://curated-transformers.readthedocs.io/en/latest/?badge=latest)
 [![pypi Version](https://img.shields.io/pypi/v/curated-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/curated-transformers/)
 
 **State-of-the-art transformers, brick by brick**
 
 Curated Transformers is a transformer library for PyTorch. It provides
@@ -51,21 +54,22 @@
 - CamemBERT
 - RoBERTa
 - XLM-RoBERTa
 
 Supported decoder-only models:
 
 - GPT-NeoX
-- LLaMA
+- LLaMA 1/2
 - Falcon
 
 Generator wrappers:
 
 - Dolly v2
 - Falcon
+- LLaMA 1/2
 
 All types of models can be loaded from Huggingface Hub.
 
 spaCy integration for curated transformers is provided by the
 [`spacy-curated-transformers`](https://github.com/explosion/spacy-curated-transformers)
 package.
```

### Comparing `curated-transformers-1.0.0.dev0/curated_transformers.egg-info/SOURCES.txt` & `curated-transformers-1.0.0.dev1/curated_transformers.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,62 +17,63 @@
 curated_transformers/generation/config.py
 curated_transformers/generation/default_generator.py
 curated_transformers/generation/dolly_v2.py
 curated_transformers/generation/falcon.py
 curated_transformers/generation/generator.py
 curated_transformers/generation/generator_wrapper.py
 curated_transformers/generation/hf_hub.py
+curated_transformers/generation/llama.py
 curated_transformers/generation/logits.py
 curated_transformers/generation/state.py
 curated_transformers/generation/stop_conditions.py
 curated_transformers/generation/string_generator.py
 curated_transformers/layers/__init__.py
 curated_transformers/layers/activations.py
 curated_transformers/layers/attention.py
 curated_transformers/layers/cache.py
 curated_transformers/layers/embeddings.py
 curated_transformers/layers/feedforward.py
 curated_transformers/layers/normalization.py
 curated_transformers/layers/scalar_weight.py
+curated_transformers/layers/transformer.py
 curated_transformers/models/__init__.py
 curated_transformers/models/auto_model.py
+curated_transformers/models/config.py
 curated_transformers/models/hf_hub.py
 curated_transformers/models/module.py
 curated_transformers/models/output.py
+curated_transformers/models/transformer.py
 curated_transformers/models/albert/__init__.py
 curated_transformers/models/albert/_hf.py
 curated_transformers/models/albert/config.py
 curated_transformers/models/albert/encoder.py
 curated_transformers/models/albert/layer_group.py
 curated_transformers/models/bert/__init__.py
 curated_transformers/models/bert/_hf.py
 curated_transformers/models/bert/config.py
 curated_transformers/models/bert/embeddings.py
 curated_transformers/models/bert/encoder.py
-curated_transformers/models/bert/layer.py
 curated_transformers/models/camembert/__init__.py
 curated_transformers/models/camembert/encoder.py
 curated_transformers/models/falcon/__init__.py
 curated_transformers/models/falcon/_hf.py
 curated_transformers/models/falcon/causal_lm.py
 curated_transformers/models/falcon/config.py
 curated_transformers/models/falcon/decoder.py
 curated_transformers/models/falcon/layer.py
 curated_transformers/models/gpt_neox/__init__.py
 curated_transformers/models/gpt_neox/_hf.py
 curated_transformers/models/gpt_neox/causal_lm.py
 curated_transformers/models/gpt_neox/config.py
 curated_transformers/models/gpt_neox/decoder.py
-curated_transformers/models/gpt_neox/layer.py
 curated_transformers/models/llama/__init__.py
 curated_transformers/models/llama/_hf.py
 curated_transformers/models/llama/causal_lm.py
 curated_transformers/models/llama/config.py
 curated_transformers/models/llama/decoder.py
-curated_transformers/models/llama/layer.py
 curated_transformers/models/roberta/__init__.py
 curated_transformers/models/roberta/_hf.py
 curated_transformers/models/roberta/config.py
 curated_transformers/models/roberta/embeddings.py
 curated_transformers/models/roberta/encoder.py
 curated_transformers/models/xlm_roberta/__init__.py
 curated_transformers/models/xlm_roberta/encoder.py
@@ -82,26 +83,27 @@
 curated_transformers/quantization/bnb/__init__.py
 curated_transformers/quantization/bnb/config.py
 curated_transformers/quantization/bnb/impl.py
 curated_transformers/tests/__init__.py
 curated_transformers/tests/compat.py
 curated_transformers/tests/conftest.py
 curated_transformers/tests/enable_gpu.py
-curated_transformers/tests/util.py
+curated_transformers/tests/utils.py
 curated_transformers/tests/generation/__init__.py
 curated_transformers/tests/generation/test_auto_generator.py
 curated_transformers/tests/generation/test_dolly_v2.py
 curated_transformers/tests/generation/test_falcon.py
 curated_transformers/tests/generation/test_generic.py
 curated_transformers/tests/generation/test_logits.py
 curated_transformers/tests/generation/test_stop.py
+curated_transformers/tests/layers/__init__.py
+curated_transformers/tests/layers/test_attention.py
+curated_transformers/tests/layers/test_embeddings.py
 curated_transformers/tests/models/__init__.py
-curated_transformers/tests/models/test_attention.py
 curated_transformers/tests/models/test_auto_models.py
-curated_transformers/tests/models/test_embeddings.py
 curated_transformers/tests/models/test_hf_hub.py
 curated_transformers/tests/models/util.py
 curated_transformers/tests/models/albert/__init__.py
 curated_transformers/tests/models/albert/test_encoder.py
 curated_transformers/tests/models/bert/__init__.py
 curated_transformers/tests/models/bert/test_encoder.py
 curated_transformers/tests/models/camembert/__init__.py
@@ -133,14 +135,16 @@
 curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
 curated_transformers/tests/tokenizers/legacy/toy-merges.txt
 curated_transformers/tests/tokenizers/legacy/toy-vocab.json
 curated_transformers/tests/tokenizers/legacy/toy.model
 curated_transformers/tests/tokenizers/legacy/toy.wordpieces
 curated_transformers/tests/tokenizers/toy-roberta/__init__.py
 curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
+curated_transformers/tests/util/__init__.py
+curated_transformers/tests/util/test_dataclass.py
 curated_transformers/tokenizers/__init__.py
 curated_transformers/tokenizers/_hf_compat.py
 curated_transformers/tokenizers/auto_tokenizer.py
 curated_transformers/tokenizers/chunks.py
 curated_transformers/tokenizers/hf_hub.py
 curated_transformers/tokenizers/tokenizer.py
 curated_transformers/tokenizers/util.py
@@ -152,10 +156,11 @@
 curated_transformers/tokenizers/legacy/legacy_tokenizer.py
 curated_transformers/tokenizers/legacy/llama_tokenizer.py
 curated_transformers/tokenizers/legacy/roberta_tokenizer.py
 curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
 curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
 curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
 curated_transformers/util/__init__.py
+curated_transformers/util/dataclass.py
 curated_transformers/util/hf.py
 curated_transformers/util/pytorch.py
 curated_transformers/util/serde.py
```

### Comparing `curated-transformers-1.0.0.dev0/setup.cfg` & `curated-transformers-1.0.0.dev1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-version = 1.0.0.dev0
-description = Curated transformer models
+version = 1.0.0.dev1
+description = A PyTorch library of transformer models and components
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -15,14 +15,19 @@
 python_requires = >=3.8
 install_requires = 
 	curated-tokenizers>=0.9.0.dev0,<1.0.0
 	huggingface-hub>=0.14
 	tokenizers>=0.13.3
 	torch>=1.12.0
 
+[options.extras_require]
+quantization = 
+	bitsandbytes>=0.40
+	scipy>=1.11
+
 [bdist_wheel]
 universal = true
 
 [sdist]
 formats = gztar
 
 [mypy]
```

