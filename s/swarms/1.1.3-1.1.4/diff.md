# Comparing `tmp/swarms-1.1.3.tar.gz` & `tmp/swarms-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-1.1.3.tar", last modified: Sat Jul 29 14:56:55 2023, max compression
+gzip compressed data, was "swarms-1.1.4.tar", last modified: Thu Aug  3 18:31:46 2023, max compression
```

## Comparing `swarms-1.1.3.tar` & `swarms-1.1.4.tar`

### file list

```diff
@@ -1,160 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.770467 swarms-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 14:56:45.000000 swarms-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-29 14:56:55.770467 swarms-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-07-29 14:56:45.000000 swarms-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.746467 swarms-1.1.3/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-29 14:56:45.000000 swarms-1.1.3/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:56:55.770467 swarms-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-29 14:56:45.000000 swarms-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.746467 swarms-1.1.3/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.746467 swarms-1.1.3/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory/ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/models/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/models/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/models/petals_hf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/agent_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/prompts/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/chains/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/agents/tools/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/agents/tools/core/code_interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/core/code_interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/core/code_interpreter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    73260 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/Calback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/ChatOpenAI.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/ConversationalChatAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/agent_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/agent_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/boss/boss_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/hivemind.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/orchestrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/utils/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/embeddings/pegasus.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/utils/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/character_generative.py
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/generative_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.762467 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.762467 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.766467 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.766467 swarms-1.1.3/swarms/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.766467 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.766467 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.770467 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.770467 swarms-1.1.3/swarms/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.770467 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/worker_agent_ultra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/worker_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/worker_ultra_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.746467 swarms-1.1.3/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 18:31:34.000000 swarms-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 18:31:46.296811 swarms-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-08-03 18:31:34.000000 swarms-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-03 18:31:34.000000 swarms-1.1.4/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 18:31:46.296811 swarms-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-03 18:31:34.000000 swarms-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/swarms/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.280810 swarms-1.1.4/swarms/agents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/petals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.280810 swarms-1.1.4/swarms/agents/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/agent_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/agent_prompt_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.280810 swarms-1.1.4/swarms/agents/prompts/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/chains/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/chat_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.280810 swarms-1.1.4/swarms/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/autogpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/code_intepretor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/developer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/exit_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/file_mangagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/Calback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/ChatOpenAI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/ConversationalChatAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/agent_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/agent_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/agents/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/human_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/boss/boss_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/orchestrator/orchestrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/swarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/swarms/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/embeddings/pegasus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/character_generative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/generative_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.292811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.292811 swarms-1.1.4/swarms/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.292811 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/swarms/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/omni_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/worker_agent_ultra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/worker_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/worker_ultra_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/top_level.txt
```

### Comparing `swarms-1.1.3/LICENSE` & `swarms-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/PKG-INFO` & `swarms-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.1.3
+Version: 1.1.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.1.3/README.md` & `swarms-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/api/app.py` & `swarms-1.1.4/api/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from fastapi_cache.coder import JsonCoder
 
 from fastapi_cache import FastAPICache
 from fastapi_cache.backends.redis import RedisBackend
 from aioredis import Redis
 
 from pydantic import BaseModel
-from swarms.swarms import swarm
+from swarms.swarms.swarms import swarm
 from fastapi_limiter import FastAPILimiter
 
 from fastapi_limiter.depends import RateLimiter
 from dotenv import load_dotenv
 
 load_dotenv()
```

### Comparing `swarms-1.1.3/setup.py` & `swarms-1.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 ##
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '1.1.3',
+  version = '1.1.4',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -25,14 +25,15 @@
         'torchvision',
         'torchaudio',
         'asyncio',
         'nest_asyncio',
         'bs4',
         'pegasusx',
         'oceandb',
+        'codeinterpreterapi[all]',
         'playwright',
         'duckduckgo_search',
         'faiss-cpu',
         'wget==3.2',
         'accelerate',
         'sphinx_rtd_theme',
         'addict',
```

### Comparing `swarms-1.1.3/swarms/agents/agent.py` & `swarms-1.1.4/swarms/workers/worker_node.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,144 +1,168 @@
-#base toolset
-from swarms.agents.tools.agent_tools import *
-from swarms.utils.logger import logger
-
-from langchain.tools import BaseTool
+import logging
+from typing import List, Optional, Union
 
-from typing import List, Any, Optional
-from langchain.memory.chat_message_histories import FileChatMessageHistory
+import faiss
+from langchain.agents import Tool
+from langchain.chat_models import ChatOpenAI
+from langchain.docstore import InMemoryDocstore
+from langchain.embeddings import OpenAIEmbeddings
+# TODO: refactor to Agent class
+from langchain.experimental.autonomous_agents.autogpt.agent import AutoGPT
+from langchain.vectorstores import FAISS
+
+from swarms.agents.tools.autogpt import (
+    FileChatMessageHistory,
+    ReadFileTool,
+    WebpageQATool,
+    WriteFileTool,
+    DuckDuckGoSearchRun,
+    load_qa_with_sources_chain,
+    process_csv,
+    web_search,
+)
 
-import logging
-from swarms.agents.models.hf import HuggingFaceLLM
+ROOT_DIR = "./data/"
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
-class AgentNodeInitializer:
-    """Useful for spawning autonomous agent instances to accomplish complex tasks."""
 
+class WorkerNodeInitializer:
+    """Useful for when you need to spawn an autonomous agent instance as a worker to accomplish complex tasks, it can search the internet or spawn child multi-modality models to process and generate images and text or audio and so on"""
     def __init__(self, 
-                 llm: Optional[Any] = None, 
-                 tools: Optional[List[BaseTool]] = None, 
-                 vectorstore: Optional[List[Any]] = None, 
-                 temperature: float = 0.5,
-                 model_type: Optional[str] = None, 
-                 human_in_the_loop: bool = True,
-                 model_id: Optional[str] = None,
-                 embedding_size: int = 8192,
-                 system_prompt: Optional[str] = None,
-                 max_iterations: Optional[int] = None,
-                 agent_name: Optional[str] = None,
-                 agent_role: Optional[str] = None,
-                 verbose: bool = False,
-                 openai_api_key: Optional[str] = None):
-
-        if not openai_api_key and (model_type is None or model_type.lower() == 'openai'):
-            raise ValueError("OpenAI API key cannot be None when model_type is 'openai'")
-
-        self.llm = llm or self.initialize_llm(model_type, model_id, openai_api_key, temperature)
-        self.tools = tools or []
-        self.vectorstore = vectorstore or []
-
-        self.temperature = temperature
-        self.model_type = model_type
+                 openai_api_key: str,
+                 llm: Optional[Union[InMemoryDocstore, ChatOpenAI]] = None, 
+                 tools: Optional[List[Tool]] = None, 
+                #  vectorstore: Optional[FAISS] = None,
+                #  embedding_size: Optional[int] = 1926,
+                 worker_name: Optional[str] = "Swarm Worker AI Assistant", 
+                 worker_role: Optional[str] = "Assistant", 
+                 human_in_the_loop: Optional[bool] = False, 
+                 search_kwargs: dict = {}, 
+                 verbose: Optional[bool] = False,
+                 chat_history_file: str = "chat_history.txt"):
+        self.openai_api_key = openai_api_key
+        self.llm = llm if llm is not None else ChatOpenAI()
+        self.tools = tools if tools is not None else [ReadFileTool(), WriteFileTool()]
+        # self.vectorstore = vectorstore
+
+        # Initializing agent in the constructor
+        self.worker_name = worker_name
+        self.worker_role = worker_role
+        # self.embedding_size = embedding_size
         self.human_in_the_loop = human_in_the_loop
-
-        self.model_id = model_id
-        self.embedding_size = embedding_size
-        self.system_prompt = system_prompt
-
-        self.agent_name = agent_name
-        self.agent_role = agent_role
+        self.search_kwargs = search_kwargs
         self.verbose = verbose
+        self.chat_history_file = chat_history_file
 
-        self.openai_api_key = openai_api_key
-        self.agent = None
-        
-        self.initialize_agent()
+        self.create_agent()
 
-    def initialize_llm(self, model_type: str, model_id: str, openai_api_key: str, temperature: float):
-        try:
-            if model_type.lower() == 'openai':
-                return ChatOpenAI(openai_api_key=openai_api_key, temperature=temperature)
-            elif model_type.lower() == 'huggingface':
-                return HuggingFaceLLM(model_id=model_id, temperature=temperature)
-            else:
-                raise ValueError("Invalid model_type. It should be either 'openai' or 'huggingface'")
-        except Exception as e:
-            logger.error(f"Failed to initialize language model: {e}")
-            raise e
-
-    def initialize_agent(self):
+    def create_agent(self):
+        
+        logging.info("Creating agent in WorkerNode")
         try:
+            # if self.vectorstore is None:
+            #     raise ValueError("Vectorstore is not initialized in WorkerNodeInitializer")
+            vectorstore = self.initialize_vectorstore()
+            
             self.agent = AutoGPT.from_llm_and_tools(
-                ai_name=self.agent_name,
-                ai_role=self.agent_role,
+                ai_name=self.worker_name,
+                ai_role=self.worker_role,
                 tools=self.tools,
                 llm=self.llm,
-                memory=self.vectorstore.as_retriever(search_kwargs={}),
+                memory=vectorstore,
                 human_in_the_loop=self.human_in_the_loop,
-                chat_history_memory=FileChatMessageHistory("chat_history.txt"),
-                verbose=self.verbose,
+                chat_history_memory=FileChatMessageHistory(self.chat_history_file),
             )
+            # self.agent.chain.verbose = verbose
         except Exception as e:
-            logger.error(f"Error while creating agent: {str(e)}")
+            logging.error(f"Error while creating agent: {str(e)}")
             raise e
 
-    def add_tool(self, tool: BaseTool):
-        if not isinstance(tool, BaseTool):
-            logger.error("Tool must be an instance of BaseTool.")
-            raise TypeError("Tool must be an instance of BaseTool.")
+    def add_tool(self, tool: Optional[Tool] = None):
+        if tool is None:
+            tool = DuckDuckGoSearchRun()
+        
+        if not isinstance(tool, Tool):
+            logging.error("Tool must be an instance of Tool.")
+            raise TypeError("Tool must be an instance of Tool.")
+        
         self.tools.append(tool)
 
-    def run(self, prompt: str) -> str:
+    def initialize_vectorstore(self):
+        try:
+            embeddings_model = OpenAIEmbeddings(openai_api_key=self.openai_api_key)
+            embedding_size = 8192
+            index = faiss.IndexFlatL2(embedding_size=embedding_size)
+            return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
+        
+        except Exception as e:
+            logging.error(f"Failed to initialize vector store: {e}")
+            return None
+
+    def run(self, prompt) -> str:
+        if not isinstance(prompt, str):
+            logging.error("Prompt must be a string.")
+            raise TypeError("Prompt must be a string.")
+        
         if not prompt:
-            logger.error("Prompt is empty.")
+            logging.error("Prompt is empty.")
             raise ValueError("Prompt is empty.")
+        
         try:
             self.agent.run([f"{prompt}"])
-            return "Task completed by AgentNode"
+            return "Task completed by WorkerNode"
         except Exception as e:
-            logger.error(f"While running the agent: {str(e)}")
+            logging.error(f"While running the agent: {str(e)}")
             raise e
 
-
-class AgentNode:
-    def __init__(self, openai_api_key):
+class WorkerNode:
+    def __init__(self, 
+            openai_api_key: str,
+            temperature: int, 
+            llm: Optional[Union[InMemoryDocstore, ChatOpenAI]] = None, 
+            tools: Optional[List[Tool]] = None, 
+            # vectorstore: Optional[FAISS] = None,
+            # embedding_size: Optional[int] = 4026,
+            worker_name: Optional[str] = "Swarm Worker AI Assistant", 
+            worker_role: Optional[str] = "Assistant", 
+            human_in_the_loop: Optional[bool] = False, 
+            search_kwargs: dict = {}, 
+            verbose: Optional[bool] = False,
+            chat_history_file: str = "chat_history.txt"):       
+    
         if not openai_api_key:
-            logging.error("OpenAI API key is not provided")
             raise ValueError("openai_api_key cannot be None")
         
         self.openai_api_key = openai_api_key
+        self.worker_node_initializer = WorkerNodeInitializer(openai_api_key)
+        self.name = worker_name  # Added a name attribute
+        self.description = "A worker node that executes tasks"  # Added a description attribute
+        # self.embedding_size = embedding_size
 
-    def initialize_llm(self, llm_class):
-        """
-        Init LLM 
-
-        Params:
-            llm_class(class): The Language model class. Default is OpenAI.
-            temperature (float): The Temperature for the language model. Default is 0.5
-        """
-        try: 
-            # Initialize language model
-            if self.llm_class == 'openai' or OpenAI:
-                return llm_class(openai_api_key=self.openai_api_key, temperature=self.temperature)
-            elif self.model_type == "huggingface":
-                return HuggingFaceLLM(model_id=self.model_id, temperature=self.temperature)
+
+    def initialize_llm(self, llm_class, temperature):
+        if not llm_class:
+            logging.error("llm_class cannot be none")
+            raise ValueError("llm_class cannot be None")
+        
+        try:
+            return llm_class(openai_api_key=self.openai_api_key, temperature=temperature)
         except Exception as e:
             logging.error(f"Failed to initialize language model: {e}")
+            raise
+
 
     def initialize_tools(self, llm_class):
         if not llm_class:
             logging.error("llm_class not cannot be none")
             raise ValueError("llm_class cannot be none")
         try:
-                
-            logging.info('Creating AgentNode')
+            logging.info('Creating WorkerNode')
             llm = self.initialize_llm(llm_class)
-            web_search = DuckDuckGoSearchRun()
 
             tools = [
                 web_search,
                 WriteFileTool(root_dir=ROOT_DIR),
                 ReadFileTool(root_dir=ROOT_DIR),
                 process_csv,
                 WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
@@ -146,46 +170,43 @@
             if not tools:
                 logging.error("Tools are not initialized")
                 raise ValueError("Tools are not initialized")
             return tools
         except Exception as e:
             logging.error(f"Failed to initialize tools: {e}")
 
-    def initialize_vectorstore(self):
-        try:
-            embeddings_model = OpenAIEmbeddings(openai_api_key=self.openai_api_key)
-            index = faiss.IndexFlatL2(self.embedding_size)
-            return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
-        except Exception as e:
-            logging.error(f"Failed to initialize vector store: {e}")
-            raise
-
-    def create_agent(self, llm_class=ChatOpenAI, ai_name="Swarm Agent AI Assistant", ai_role="Assistant", human_in_the_loop=False, search_kwargs={}, verbose=False):
+    def create_worker_node(self, worker_name, worker_role, human_in_the_loop, llm_class=ChatOpenAI, search_kwargs={}, **kwargs):
         if not llm_class:
             logging.error("llm_class cannot be None.")
             raise ValueError("llm_class cannot be None.")
         try:
-            agent_tools = self.initialize_tools(llm_class)
-            vectorstore = self.initialize_vectorstore()
-            agent = AgentNode(llm=self.initialize_llm(llm_class), tools=agent_tools, vectorstore=vectorstore)
-            agent.create_agent(ai_name=ai_name, ai_role=ai_role, human_in_the_loop=human_in_the_loop, search_kwargs=search_kwargs, verbose=verbose)
-            return agent
+            worker_tools = self.initialize_tools(llm_class)
+            vectorstore = self.worker_node_initializer.initialize_vectorstore()
+            worker_node = WorkerNodeInitializer(
+                openai_api_key=self.openai_api_key, # pass the openai_api_key
+                llm=self.initialize_llm(llm_class), 
+                tools=worker_tools, 
+                vectorstore=vectorstore,
+                ai_name=worker_name, 
+                ai_role=worker_role, 
+                human_in_the_loop=human_in_the_loop, 
+                search_kwargs=search_kwargs,
+            )
+            worker_node.name = worker_name  # Setting the name here
+            return worker_node
         except Exception as e:
-            logging.error(f"Failed to create agent node: {e}")
+            logging.error(f"Failed to create worker node: {e}")
             raise
 
-def agent(openai_api_key, objective):
-    if not objective or not isinstance(objective, str):
-        logging.error("Invalid objective")
-        raise ValueError("A valid objective is required")
 
+
+def worker_node(openai_api_key):
     if not openai_api_key:
         logging.error("OpenAI API key is not provided")
         raise ValueError("OpenAI API key is required")
+    
     try:
-        initializer = AgentNodeInitializer(openai_api_key)
-        agent = initializer.create_agent()
-        agent = agent.run(objective)
-        return agent
+        worker_node = WorkerNode(openai_api_key)
+        return worker_node.create_worker_node()
     except Exception as e:
-        logging.error(f"An error occured in agent: {e}")
-        raise
+        logging.error(f"An error occured in worker_node: {e}")
+        raise
```

### Comparing `swarms-1.1.3/swarms/agents/base.py` & `swarms-1.1.4/swarms/agents/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,67 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 from langchain.chains.llm import LLMChain
-from langchain.chat_models.base import BaseChatModel
 from langchain.memory import ChatMessageHistory
-from langchain.schema import (
-    BaseChatMessageHistory,
-    Document,
-)
-from langchain.schema.messages import AIMessage, HumanMessage, SystemMessage
-from langchain.tools.base import BaseTool
-from langchain.tools.human.tool import HumanInputRun
+from langchain.schema import BaseChatMessageHistory, Document
 from langchain.vectorstores.base import VectorStoreRetriever
-from langchain_experimental.autonomous_agents.autogpt.prompt_generator import (
-    FINISH_NAME,
-)
 from pydantic import ValidationError
 
+from swarms.agents.models.base import AbstractModel
+from swarms.agents.prompts.agent_output_parser import AgentOutputParser
+from swarms.agents.prompts.agent_prompt import AIMessage, HumanMessage, SystemMessage
+from swarms.agents.prompts.agent_prompt_auto import MessageFormatter, PromptConstructor
+from swarms.agents.prompts.prompt_generator import FINISH_NAME
+from swarms.agents.tools.base import BaseTool
 from swarms.agents.utils.Agent import AgentOutputParser
+from swarms.agents.utils.human_input import HumanInputRun
 
 
 class Agent:
     """Base Agent class"""
 
     def __init__(
         self,
         ai_name: str,
-        memory: VectorStoreRetriever,
         chain: LLMChain,
-        output_parser: BaseAgentOutputParser,
+        memory: VectorStoreRetriever,
+        output_parser: AgentOutputParser,
         tools: List[BaseTool],
         feedback_tool: Optional[HumanInputRun] = None,
         chat_history_memory: Optional[BaseChatMessageHistory] = None,
     ):
         self.ai_name = ai_name
+        self.chain = chain
         self.memory = memory
         self.next_action_count = 0
-        self.chain = chain
         self.output_parser = output_parser
         self.tools = tools
         self.feedback_tool = feedback_tool
         self.chat_history_memory = chat_history_memory or ChatMessageHistory()
 
     @classmethod
     def from_llm_and_tools(
         cls,
         ai_name: str,
         ai_role: str,
         memory: VectorStoreRetriever,
         tools: List[BaseTool],
-        llm: BaseChatModel,
+        llm: AbstractModel,
         human_in_the_loop: bool = False,
-        output_parser: Optional[BaseAgentOutputParser] = None,
+        output_parser: Optional[AgentOutputParser] = None,
         chat_history_memory: Optional[BaseChatMessageHistory] = None,
     ) -> Agent:
-        prompt = AgentPrompt(
-            ai_name=ai_name,
-            ai_role=ai_role,
-            tools=tools,
-            input_variables=["memory", "messages", "goals", "user_input"],
-            token_counter=llm.get_num_tokens,
-        )
+        prompt_constructor = PromptConstructor(ai_name=ai_name,
+                                               ai_role=ai_role,
+                                               tools=tools)
+        message_formatter = MessageFormatter()
         human_feedback_tool = HumanInputRun() if human_in_the_loop else None
-        chain = LLMChain(llm=llm, prompt=prompt)
+        chain = LLMChain(llm=llm, prompt_constructor=prompt_constructor, message_formatter=message_formatter)
         return cls(
             ai_name,
             memory,
             chain,
             output_parser or AgentOutputParser(),
             tools,
             feedback_tool=human_feedback_tool,
@@ -132,8 +126,10 @@
                 feedback = f"\n{self.feedback_tool.run('Input: ')}"
                 if feedback in {"q", "stop"}:
                     print("EXITING")
                     return "EXITING"
                 memory_to_add += feedback
 
             self.memory.add_documents([Document(page_content=memory_to_add)])
-            self.chat_history_memory.add_message(SystemMessage(content=result))
+            self.chat_history_memory.add_message(SystemMessage(content=result))
+
+
```

### Comparing `swarms-1.1.3/swarms/agents/memory/base.py` & `swarms-1.1.4/swarms/agents/memory/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/memory/chroma.py` & `swarms-1.1.4/swarms/agents/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/memory/ocean.py` & `swarms-1.1.4/swarms/agents/memory/ocean.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/memory.py` & `swarms-1.1.4/swarms/agents/memory.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List
+from pydantic import Field
 
 from langchain.memory.chat_memory import BaseChatMemory, get_prompt_input_key
 from langchain.vectorstores.base import VectorStoreRetriever
 
-from pydantic import Field
 
 
 class AutoGPTMemory(BaseChatMemory):
     retriever: VectorStoreRetriever = Field(exclude=True)
     """VectorStoreRetriever object to connect to."""
 
     @property
```

### Comparing `swarms-1.1.3/swarms/agents/models/hf.py` & `swarms-1.1.4/swarms/agents/models/huggingface.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         try:
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_id)
             self.model = AutoModelForCausalLM.from_pretrained(self.model_id, quantization_config=bnb_config)
             self.model.to(self.device)
         except Exception as e:
             self.logger.error(f"Failed to load the model or the tokenizer: {e}")
             raise
-    def generate_text(self, prompt_text: str, max_length: int = None):
+    def generate(self, prompt_text: str, max_length: int = None):
         max_length = max_length if max_length else self.max_length
         try:
             inputs = self.tokenizer.encode(prompt_text, return_tensors="pt").to(self.device)
             with torch.no_grad():
                 outputs = self.model.generate(inputs, max_length=max_length, do_sample=True)
             return self.tokenizer.decode(outputs[0], skip_special_tokens=True)
         except Exception as e:
```

### Comparing `swarms-1.1.3/swarms/agents/prompts/agent_prompt.py` & `swarms-1.1.4/swarms/agents/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/prompts/chains/llm.py` & `swarms-1.1.4/swarms/agents/prompts/chains/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/prompts/prompts.py` & `swarms-1.1.4/swarms/agents/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/utils/Agent.py` & `swarms-1.1.4/swarms/agents/utils/Agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/utils/Calback.py` & `swarms-1.1.4/swarms/agents/utils/Calback.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/utils/ChatOpenAI.py` & `swarms-1.1.4/swarms/agents/utils/ChatOpenAI.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/utils/ConversationalChatAgent.py` & `swarms-1.1.4/swarms/agents/utils/ConversationalChatAgent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/utils/agent_creator.py` & `swarms-1.1.4/swarms/agents/utils/agent_creator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/utils/agent_setup.py` & `swarms-1.1.4/swarms/agents/utils/agent_setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/utils/output_parser.py` & `swarms-1.1.4/swarms/agents/utils/output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/agents/utils/prompts.py` & `swarms-1.1.4/swarms/agents/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/boss/boss_node.py` & `swarms-1.1.4/swarms/boss/boss_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+from typing import Optional
 
 import faiss
 from langchain import LLMChain, OpenAI, PromptTemplate
 from langchain.agents import AgentExecutor, Tool, ZeroShotAgent
 from langchain.docstore import InMemoryDocstore
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.experimental import BabyAGI
@@ -16,45 +17,46 @@
 
 # ---------- Boss Node ----------
 class BossNodeInitializer:
     """
     The BossNode class is responsible for creating and executing tasks using the BabyAGI model.
     It takes a language model (llm), a vectorstore for memory, an agent_executor for task execution, and a maximum number of iterations for the BabyAGI model.
     """
-    def __init__(self, llm, vectorstore, agent_executor, max_iterations):
+    def __init__(self, llm, vectorstore, agent_executor, max_iterations, human_in_the_loop):
         if not llm or not vectorstore or not agent_executor or not max_iterations:
             logging.error("llm, vectorstore, agent_executor, and max_iterations cannot be None.")
             raise ValueError("llm, vectorstore, agent_executor, and max_iterations cannot be None.")
         self.llm = llm
         self.vectorstore = vectorstore
         self.agent_executor = agent_executor
         self.max_iterations = max_iterations
+        self.human_in_the_loop = human_in_the_loop
 
         try:
             self.baby_agi = BabyAGI.from_llm(
                 llm=self.llm,
                 vectorstore=self.vectorstore,
                 task_execution_chain=self.agent_executor,
                 max_iterations=self.max_iterations,
-                human_in_the_loop=True
+                human_in_the_loop=self.human_in_the_loop
             )
         except ValidationError as e:
             logging.error(f"Validation Error while initializing BabyAGI: {e}")
             raise
         except Exception as e:
             logging.error(f"Unexpected Error while initializing BabyAGI: {e}")
             raise
 
     def initialize_vectorstore(self):
         """
         Init vector store
         """
         try:     
             embeddings_model = OpenAIEmbeddings(openai_api_key=self.openai_api_key)
-            embedding_size = 1536
+            embedding_size = 8192
             index = faiss.IndexFlatL2(embedding_size)
             return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
         except Exception as e:
             logging.error(f"Failed to initialize vector store: {e}")
             return None
         
     def initialize_llm(self, llm_class, temperature=0.5):
@@ -93,40 +95,80 @@
             self.baby_agi(task)
         except Exception as e:
             logging.error(f"Error while executing task: {e}")
             raise
 
 
 
-# from swarms import BossNode, OpenAI, LLMChain, Tool, ZeroShotAgent, AgentExecutor, PromptTemplate
 
-def BossNode(objective, api_key=None, vectorstore=None, worker_node=None, llm_class=OpenAI, max_iterations=5, verbose=False):
-    """
-    Wrapper function to initialize and use BossNode with given parameters.
-    API key can be passed as argument or set as an environment variable.
-    """
-    api_key = api_key or os.getenv('API_KEY')
+class BossNode:
+    def __init__(self,
+                #  vectorstore,
+                 objective: Optional[str] = None,
+                 boss_system_prompt: Optional[str] = "You are a boss planner in a swarm...",
+                 api_key=None,
+                 worker_node=None,
+                 llm_class=OpenAI,
+                 max_iterations=5,
+                 verbose=False,
+                 ):
+        
+        self.api_key = api_key or os.getenv("OPENAI_API_KEY")
+        # self.vectorstore = vectorstore
+        self.worker_node = worker_node
+        self.boss_system_prompt = boss_system_prompt
+        self.llm_class = llm_class
+        self.max_iterations = max_iterations
+        self.verbose = verbose
+
+        if not self.api_key:
+            raise ValueError("[BossNode][ValueError][API KEY must be provided either as an argument or as an environment variable API_KEY]")
+        
+        self.llm = self.initialize_llm(self.llm_class)
 
-    if not api_key:
-        raise ValueError("API key must be provided either as argument or as an environment variable named 'API_KEY'.")
+        todo_prompt = PromptTemplate.from_template(boss_system_prompt)
+        todo_chain = LLMChain(llm=self.llm, prompt=todo_prompt)
+
+        tools = [
+            Tool(name="TODO", func=todo_chain.run, description="useful for when you need to come up with todo lists..."),
+            self.worker_node
+        ]
+        suffix = """Question: {task}\n{agent_scratchpad}"""
+        prefix = """You are a Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n """
+        
+        prompt = ZeroShotAgent.create_prompt(tools, prefix=prefix, suffix=suffix, input_variables=["objective", "task", "context", "agent_scratchpad"],)
+        llm_chain = LLMChain(llm=self.llm, prompt=prompt)
+        agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=[tool.name for tool in tools])
+
+        self.agent_executor = AgentExecutor.from_agent_and_tools(agent=agent, tools=tools, verbose=self.verbose)
+
+        vectorstore = self.initialize_vectorstore()
+
+        self.boss_initializer = BossNodeInitializer(
+            llm=self.llm, 
+            vectorstore=vectorstore, 
+            agent_executor=self.agent_executor, 
+            max_iterations=self.max_iterations, 
+        )
+        self.task = self.boss_initializer.create_task(objective)
+
+    def initialize_llm(self, llm_class, temperature=0.5):
+        try:
+            return llm_class(openai_api_key=self.api_key, temperature=temperature)
+        except Exception as e:
+            logging.error(f"Failed to initialize language model: {e}")
+            raise e
+        
+    def initialize_vectorstore(self):
+        try:     
+            embeddings_model = OpenAIEmbeddings(openai_api_key=self.openai_api_key)
+            embedding_size = 8192
+            index = faiss.IndexFlatL2(embedding_size)
+            return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
+        except Exception as e:
+            logging.error(f"Failed to initialize vector store: {e}")
+            return None
+        
 
-    llm = BossNode.initialize_llm(llm_class)  # This function should be defined elsewhere
+    def run(self):
+        self.boss_initializer.run(self.task)
 
-    todo_prompt = PromptTemplate.from_template("You are a boss planer in a swarm who is an expert at coming up with a todo list for a given objective and then creating a worker to help you accomplish your task. Rate every task on the importance of it's probability to complete the main objective on a scale from 0 to 1, an integer. Come up with a todo list for this objective: {objective} and then spawn a worker agent to complete the task for you. Always spawn a worker agent after creating a plan and pass the objective and plan to the worker agent.")
-    todo_chain = LLMChain(llm=llm, prompt=todo_prompt)
-
-    tools = [
-        Tool(name="TODO", func=todo_chain.run, description="useful for when you need to come up with todo lists. Input: an objective to create a todo list for your objective. Note create a todo list then assign a ranking from 0.0 to 1.0 to each task, then sort the tasks based on the tasks most likely to achieve the objective. The Output: a todo list for that objective with rankings for each step from 0.1 Please be very clear what the objective is!"),
-        worker_node
-    ]
-    suffix = """Question: {task}\n{agent_scratchpad}"""
-    prefix = """You are an Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n """
-    
-    prompt = ZeroShotAgent.create_prompt(tools, prefix=prefix, suffix=suffix, input_variables=["objective", "task", "context", "agent_scratchpad"],)
-    llm_chain = LLMChain(llm=llm, prompt=prompt)
-    agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=[tool.name for tool in tools])
-
-    agent_executor = AgentExecutor.from_agent_and_tools(agent=agent, tools=tools, verbose=verbose)
-
-    boss = BossNode(llm, vectorstore, agent_executor, max_iterations)
-    task = boss.create_task(objective)
-    boss.run(task)
```

### Comparing `swarms-1.1.3/swarms/hivemind.py` & `swarms-1.1.4/swarms/swarms/hivemind.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #kye gomez jul 13 4:01pm, can scale up the number of swarms working on a probkem with `hivemind(swarms=4, or swarms=auto which will scale the agents depending on the complexity)`
 
 import concurrent.futures
 import logging
 
 #this needs to change, we need to specify exactly what needs to be imported
 from swarms.agents.tools.agent_tools import *
-from swarms.swarms import HierarchicalSwarm
+from swarms.swarms.swarms import HierarchicalSwarm
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 # add typechecking, documentation, and deeper error handling 
 # TODO: MANY WORKERS
 class HiveMind:
     def __init__(self, openai_api_key="", num_swarms=1, max_workers=None):
```

### Comparing `swarms-1.1.3/swarms/orchestrate.py` & `swarms-1.1.4/swarms/orchestrator/orchestrate.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/utils/embeddings/base.py` & `swarms-1.1.4/swarms/utils/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/utils/embeddings/pegasus.py` & `swarms-1.1.4/swarms/utils/embeddings/pegasus.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/utils/main.py` & `swarms-1.1.4/swarms/utils/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/utils/static.py` & `swarms-1.1.4/swarms/utils/static.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/character_generative.py` & `swarms-1.1.4/swarms/workers/character_generative.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/generative_worker.py` & `swarms-1.1.4/swarms/workers/generative_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/GroundingDINO/setup.py` & `swarms-1.1.4/swarms/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/models/segment_anything/setup.py` & `swarms-1.1.4/swarms/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/multi_modal_worker.py` & `swarms-1.1.4/swarms/workers/multi_modal_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-1.1.4/swarms/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/omni_worker.py` & `swarms-1.1.4/swarms/workers/omni_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/worker_agent_ultra.py` & `swarms-1.1.4/swarms/workers/worker_agent_ultra.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms/workers/worker_ultra_node.py` & `swarms-1.1.4/swarms/workers/worker_ultra_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.3/swarms.egg-info/PKG-INFO` & `swarms-1.1.4/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.1.3
+Version: 1.1.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.1.3/swarms.egg-info/SOURCES.txt` & `swarms-1.1.4/swarms.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 LICENSE
 README.md
 setup.py
 api/__init__.py
 api/app.py
 swarms/__init__.py
-swarms/hivemind.py
-swarms/orchestrate.py
-swarms/swarms.py
 swarms.egg-info/PKG-INFO
 swarms.egg-info/SOURCES.txt
 swarms.egg-info/dependency_links.txt
 swarms.egg-info/requires.txt
 swarms.egg-info/top_level.txt
 swarms/agents/__init__.py
-swarms/agents/agent.py
 swarms/agents/base.py
 swarms/agents/memory.py
 swarms/agents/memory/__init__.py
 swarms/agents/memory/base.py
 swarms/agents/memory/chroma.py
 swarms/agents/memory/ocean.py
 swarms/agents/models/__init__.py
-swarms/agents/models/hf.py
-swarms/agents/models/llm.py
-swarms/agents/models/petals_hf.py
+swarms/agents/models/anthropic.py
+swarms/agents/models/base.py
+swarms/agents/models/huggingface.py
+swarms/agents/models/openai.py
+swarms/agents/models/palm.py
+swarms/agents/models/petals.py
 swarms/agents/prompts/__init__.py
+swarms/agents/prompts/agent_output_parser.py
 swarms/agents/prompts/agent_prompt.py
+swarms/agents/prompts/agent_prompt_auto.py
+swarms/agents/prompts/chat_prompt.py
+swarms/agents/prompts/prompt_generator.py
 swarms/agents/prompts/prompts.py
 swarms/agents/prompts/chains/__init__.py
 swarms/agents/prompts/chains/llm.py
 swarms/agents/tools/__init__.py
+swarms/agents/tools/autogpt.py
 swarms/agents/tools/base.py
-swarms/agents/tools/main.py
-swarms/agents/tools/core/__init__.py
-swarms/agents/tools/core/code_interpreter/__init__.py
-swarms/agents/tools/core/code_interpreter/main.py
+swarms/agents/tools/code_intepretor.py
+swarms/agents/tools/developer.py
+swarms/agents/tools/exit_conversation.py
+swarms/agents/tools/file_mangagement.py
+swarms/agents/tools/models.py
+swarms/agents/tools/requests.py
 swarms/agents/utils/Agent.py
 swarms/agents/utils/Calback.py
 swarms/agents/utils/ChatOpenAI.py
 swarms/agents/utils/ConversationalChatAgent.py
 swarms/agents/utils/__init__.py
 swarms/agents/utils/agent_creator.py
 swarms/agents/utils/agent_setup.py
+swarms/agents/utils/human_input.py
 swarms/agents/utils/output_parser.py
 swarms/agents/utils/prompts.py
+swarms/agents/utils/callbacks/__init__.py
 swarms/boss/__init__.py
 swarms/boss/boss_node.py
+swarms/orchestrator/__init__.py
+swarms/orchestrator/orchestrate.py
+swarms/swarms/__init__.py
+swarms/swarms/hivemind.py
+swarms/swarms/swarms.py
 swarms/utils/__init__.py
 swarms/utils/logger.py
 swarms/utils/main.py
 swarms/utils/static.py
 swarms/utils/task.py
 swarms/utils/embeddings/__init__.py
 swarms/utils/embeddings/base.py
```

### Comparing `swarms-1.1.3/swarms.egg-info/requires.txt` & `swarms-1.1.4/swarms.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 torchvision
 torchaudio
 asyncio
 nest_asyncio
 bs4
 pegasusx
 oceandb
+codeinterpreterapi[all]
 playwright
 duckduckgo_search
 faiss-cpu
 wget==3.2
 accelerate
 sphinx_rtd_theme
 addict
```

