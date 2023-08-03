# Comparing `tmp/factool-0.1.0.tar.gz` & `tmp/factool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factool-0.1.0.tar", last modified: Sun Jul 23 04:42:24 2023, max compression
+gzip compressed data, was "factool-0.1.2.tar", last modified: Thu Aug  3 01:43:06 2023, max compression
```

## Comparing `factool-0.1.0.tar` & `factool-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.141682 factool-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-23 04:41:39.000000 factool-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    31412 2023-07-23 04:42:24.141682 factool-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30781 2023-07-23 04:41:39.000000 factool-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.137682 factool-0.1.0/factool/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-23 04:41:39.000000 factool-0.1.0/factool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.137682 factool-0.1.0/factool/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 04:41:39.000000 factool-0.1.0/factool/code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.137682 factool-0.1.0/factool/code/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 04:41:39.000000 factool-0.1.0/factool/code/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-23 04:41:39.000000 factool-0.1.0/factool/code/helper/_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-23 04:41:39.000000 factool-0.1.0/factool/code/helper/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-23 04:41:39.000000 factool-0.1.0/factool/code/helper/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-23 04:41:39.000000 factool-0.1.0/factool/code/helper/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-07-23 04:41:39.000000 factool-0.1.0/factool/code/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 04:41:39.000000 factool-0.1.0/factool/code/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-23 04:41:39.000000 factool-0.1.0/factool/env_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-23 04:41:39.000000 factool-0.1.0/factool/factool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.137682 factool-0.1.0/factool/knowledge_qa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 04:41:39.000000 factool-0.1.0/factool/knowledge_qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-23 04:41:39.000000 factool-0.1.0/factool/knowledge_qa/google_serper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-23 04:41:39.000000 factool-0.1.0/factool/knowledge_qa/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-23 04:41:39.000000 factool-0.1.0/factool/knowledge_qa/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.137682 factool-0.1.0/factool/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 04:41:39.000000 factool-0.1.0/factool/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-23 04:41:39.000000 factool-0.1.0/factool/math/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-23 04:41:39.000000 factool-0.1.0/factool/math/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.141682 factool-0.1.0/factool/scientific/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 04:41:39.000000 factool-0.1.0/factool/scientific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-23 04:41:39.000000 factool-0.1.0/factool/scientific/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-23 04:41:39.000000 factool-0.1.0/factool/scientific/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-23 04:41:39.000000 factool-0.1.0/factool/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.141682 factool-0.1.0/factool/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/__init_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.141682 factool-0.1.0/factool/utils/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/claim_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/openai_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.141682 factool-0.1.0/factool/utils/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/prompts/agreement_verification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/prompts/claim_extraction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/prompts/query_generation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/prompts/self_check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-23 04:41:39.000000 factool-0.1.0/factool/utils/utils_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 04:42:24.137682 factool-0.1.0/factool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31412 2023-07-23 04:42:24.000000 factool-0.1.0/factool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-23 04:42:24.000000 factool-0.1.0/factool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 04:42:24.000000 factool-0.1.0/factool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-23 04:42:24.000000 factool-0.1.0/factool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-23 04:42:24.000000 factool-0.1.0/factool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-23 04:42:24.141682 factool-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-23 04:41:39.000000 factool-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-03 01:42:28.000000 factool-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33550 2023-08-03 01:43:06.493901 factool-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32919 2023-08-03 01:42:28.000000 factool-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.489900 factool-0.1.2/factool/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 01:42:28.000000 factool-0.1.2/factool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/factool/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:28.000000 factool-0.1.2/factool/code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/factool/code/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:28.000000 factool-0.1.2/factool/code/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-03 01:42:28.000000 factool-0.1.2/factool/code/helper/_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-03 01:42:28.000000 factool-0.1.2/factool/code/helper/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-03 01:42:28.000000 factool-0.1.2/factool/code/helper/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-03 01:42:28.000000 factool-0.1.2/factool/code/helper/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-08-03 01:42:28.000000 factool-0.1.2/factool/code/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:28.000000 factool-0.1.2/factool/code/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-03 01:42:28.000000 factool-0.1.2/factool/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-08-03 01:42:28.000000 factool-0.1.2/factool/factool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/factool/knowledge_qa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:28.000000 factool-0.1.2/factool/knowledge_qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-03 01:42:28.000000 factool-0.1.2/factool/knowledge_qa/google_serper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-08-03 01:42:28.000000 factool-0.1.2/factool/knowledge_qa/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-03 01:42:28.000000 factool-0.1.2/factool/knowledge_qa/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/factool/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:28.000000 factool-0.1.2/factool/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-08-03 01:42:28.000000 factool-0.1.2/factool/math/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 01:42:28.000000 factool-0.1.2/factool/math/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/factool/scientific/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:28.000000 factool-0.1.2/factool/scientific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-08-03 01:42:28.000000 factool-0.1.2/factool/scientific/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-03 01:42:28.000000 factool-0.1.2/factool/scientific/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-03 01:42:28.000000 factool-0.1.2/factool/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/factool/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/__init_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/factool/utils/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/claim_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/openai_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.493901 factool-0.1.2/factool/utils/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/prompts/agreement_verification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/prompts/claim_extraction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/prompts/query_generation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/prompts/self_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 01:42:28.000000 factool-0.1.2/factool/utils/utils_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:43:06.489900 factool-0.1.2/factool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33550 2023-08-03 01:43:06.000000 factool-0.1.2/factool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-03 01:43:06.000000 factool-0.1.2/factool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:43:06.000000 factool-0.1.2/factool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 01:43:06.000000 factool-0.1.2/factool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 01:43:06.000000 factool-0.1.2/factool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-03 01:43:06.493901 factool-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 01:42:28.000000 factool-0.1.2/setup.py
```

### Comparing `factool-0.1.0/PKG-INFO` & `factool-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factool
-Version: 0.1.0
+Version: 0.1.2
 Summary: Factuality Detection for Generative AI
 Home-page: https://github.com/GAIR-NLP/factool
 Author: GAIR Research Group
 License: Apache License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing
@@ -12,16 +12,21 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 
 ## FacTool: Factuality Detection in Generative AI
+[**Factuality Leaderboard**](https://github.com/GAIR-NLP/factool#factuality-leaderboard) | 
+[**Installation**](https://github.com/GAIR-NLP/factool#installation) | 
+[**Quick Start**](https://github.com/GAIR-NLP/factool#quick-start) |
+[**ChatGPT Plugin with FacTool**](https://github.com/GAIR-NLP/factool#chatgpt-plugin-with-factool) |
+[**Citation**](https://github.com/GAIR-NLP/factool#citation) |
 
-This repository contains the source code and plugin configuration for our [paper]():
+This repository contains the source code and plugin configuration for our [paper](https://arxiv.org/abs/2307.13528):
 
 Factool is a tool augmented framework for detecting factual errors of texts generated by large language models (e.g., ChatGPT). 
 Factool now supports 4 tasks: 
 * **knowledge-based QA**: Factool detects factual errors in knowledge-based QA.
 * **code generation**: Factool detects execution errors in code generation.
 * **mathematical reasoning**: Factool detects calculation errors in mathematical reasoning.
 * **scientific literature review**: Factool detects hallucinated scientific literatures.
@@ -31,14 +36,30 @@
  </p>
  
 
 Demo of Knowledge-based QA: 
 
 ![Alt Text](./figs/factool_plugin_kbqa.gif)
 
+![Alt Text](./figs/factool_chinese.gif)
+
+![Alt Text](./figs/factool_japanese.gif)
+
+## Factuality Leaderboard
+
+Our factuality leaderboard shows the factual accuracy of different chatbots evaluated by FacTool.
+
+| LLMs | Weighted Claim-Level Accuracy | Response-Level Accuracy |
+| -------- | -------- | -------- |
+| GPT-4  | **75.60**  | **43.33**  |
+| ChatGPT  | 68.63  | 36.67  |
+| Claude-v1  | 63.95  | 26.67 |
+| Bard  | 61.15  | 33.33 |
+| Vicuna-13B  | 50.35 | 21.67 |
+
 
 ## Installation
 
 * #### For General User
 
 ```bash
 pip install factool
@@ -59,15 +80,15 @@
 ### API Key Preparation
 * get your OpenAI API key from [here](https://beta.openai.com/). This is used in all scenarios (Knowledge-based QA, Code, Math, Scientific Literature Review). 
 * get your Serper API key from [here](https://serper.dev/). This is only used in Knowledge-based QA. 
 * get your Scraper API key from [here](https://www.scraperapi.com/). This is only used in Scientific Literature Review. 
 
 ### General Usage
 
-You could also directly refer to [example.py](https://github.com/GAIR-NLP/factool/blob/main/example.py) and [example_inputs.jsonl](https://github.com/GAIR-NLP/factool/blob/main/example_inputs.jsonl) for general usage.
+You could also directly refer to [./example/example.py](https://github.com/GAIR-NLP/factool/blob/main/example/example.py) and [example_inputs.jsonl](https://github.com/GAIR-NLP/factool/blob/main/example/example_inputs.jsonl) for general usage.
 
 <details>
 <summary>General Usage (click to toggle the content)</summary>
 
 ```python
 export OPENAI_API_KEY=... # this is required in all tasks
 export SERPER_API_KEY=... # this is required only in knowledge-based QA
@@ -155,53 +176,60 @@
   "detailed_information": [
     {
       'prompt': prompt_1, 
       'response': response_1, 
       'category': 'kbqa', 
       'claims': [claim_11, claim_12, ..., claims_1n], 
       'queries': [[query_111, query_112], [query_121, query_122], ..[query_1n1, query_1n2]], 
-      'evidences': [[evidences_11], [evidences_12], ..., [evidences_1n]], 
+      'evidences': [[evidences_with_source_11], [evidences_with_source_12], ..., [evidences_with_source_1n]], 
       'claim_level_factuality': [{claim_11, reasoning_11, error_11, correction_11, factuality_11}, {claim_12, reasoning_12, error_12, correction_12, factuality_12}, ..., {claim_1n, reasoning_1n, error_1n, correction_1n, factuality_1n}], 
       'response_level_factuality': factuality_1
     },
     {
       'prompt': prompt_2, 
       'response': response_2, 
       'category': 'kbqa',
       'claims': [claim_21, claim_22, ..., claims_2n], 
       'queries': [[query_211, query_212], [query_221, query_222], ..., [query_2n1, query_2n2]], 
-      'evidences': [[evidences_21], [evidences_22], ..., [evidences_2n]], 
+      'evidences': [[evidences_with_source_21], [evidences_with_source_22], ..., [evidences_with_source_2n]], 
       'claim_level_factuality': [{claim_21, reasoning_21, error_21, correction_21, factuality_21}, {claim_22, reasoning_22, error_22, correction_22, factuality_22}, ..., {claim_2n, reasoning_2n, error_2n, correction_2n, factuality_2n}],
       'response_level_factuality': factuality_2,
     },
     ...
   ]
 }
 ```
 
 In this case, you will get:
 
 
-```json
+```python
 {
-  "average_claim_level_factuality": avg_claim_level_factuality,
-  "average_response_level_factuality": avg_response_level_factuality,
-  "detailed_information": [
-    {
-      'prompt': 'Introduce Graham Neubig',
-      'response': 'Graham Neubig is a professor at MIT',
-      'category': 'kbqa',
-      'entry_point': 'answer_question',
-      'claims': [{'claim': 'Graham Neubig is a professor at MIT'}],
-      'queries': [['Is Graham Neubig a professor at MIT?', 'Graham Neubig MIT']],
-      'evidences': [['I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'Graham Neubig. I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with ...', 'Missing: MIT? | Must include:MIT?.', 'Associate Professor, Language Technology Institute, Carnegie Mellon University Affiliated Faculty, Machine Learning Department, Carnegie Mellon University', 'Missing: MIT? | Must include:MIT?.', 'I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with a bunch of great ...', 'Missing: MIT | Must include:MIT.', 'I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'was heavily inspired by an MIT PhD thesis finished 16 years earlier in 1996! ... Episode 22 of The Thesis Review: Graham Neubig (@gneubig), ...', 'Graham Neubig,. Graham Neubig. Graduate School of Information Science Nara Institute of Science and Technology. Search for other works by this author on:.']],
-      'claim_level_factuality': [{'reasoning': 'The given text states that Graham Neubig is a professor at MIT. However, the provided evidences consistently mention that Graham Neubig is an Associate Professor at Carnegie Mellon University. There is no mention of Graham Neubig being affiliated with MIT in any of the provided evidences.', 'error': 'The given text Falsely states that Graham Neubig is a professor at MIT.', 'correction': 'Graham Neubig is an Associate Professor at Carnegie Mellon University.', 'factuality': False, 'claim': 'Graham Neubig is a professor at MIT'}],
-      'response_level_factuality': False
-    }
-  ]
+    'average_claim_level_factuality': 0.0,  
+    'average_response_level_factuality': 0.0, 
+    'detailed_information': [
+        {
+          'prompt': 'Introduce Graham Neubig',
+          'response': 'Graham Neubig is a professor at MIT', 
+          'category': 'kbqa', 'search_type': 'online', 
+          'claims': [{'claim': 'Graham Neubig is a professor at MIT'}], 
+          'queries': [['Graham Neubig current position', 'Is Graham Neubig a professor at MIT?']], 
+          'evidences': [{'evidence': 'I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'source': 'https://www.linkedin.com/in/graham-neubig-10b41616b'}, {'evidence': 'Missing: position | Show results with:position', 'source': 'https://www.linkedin.com/in/graham-neubig-10b41616b'}, {'evidence': 'My research is concerned with language and its role in human communication. In particular, my long-term research goal is to break down barriers in ...', 'source': 'https://miis.cs.cmu.edu/people/222215657/graham-neubig'}, {'evidence': 'My research focuses on handling human languages (like English or Japanese) with computers -- natural language processing. In particular, I am interested in ...', 'source': 'http://www.phontron.com/'}, {'evidence': 'Missing: current | Show results with:current', 'source': 'http://www.phontron.com/'}, {'evidence': 'Graham Neubig. I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with ...', 'source': 'http://www.phontron.com/'}, {'evidence': 'Missing: MIT? | Show results with:MIT?', 'source': 'http://www.phontron.com/'}, {'evidence': 'Associate Professor, Language Technology Institute, Carnegie Mellon University Affiliated Faculty, Machine Learning Department, Carnegie Mellon University', 'source': 'https://www.phontron.com/research.php'}, {'evidence': 'Missing: MIT? | Show results with:MIT?', 'source': 'https://www.phontron.com/research.php'}, {'evidence': 'MIT Embodied Intelligence ... About the speaker: Graham ...', 'source': 'https://youtube.com/watch?v=CtcP5bvODzY'}],
+          'claim_level_factuality': [
+              {
+                'reasoning': 'The given text is non-factual. The evidence provided clearly states that Graham Neubig is an Associate Professor of Computer Science at Carnegie Mellon University, not at MIT.', 
+                'error': 'The error in the text is the incorrect affiliation of Graham Neubig. He is not a professor at MIT.', 
+                'correction': 'Graham Neubig is a professor at Carnegie Mellon University.', 
+                'factuality': False, 
+                'claim': 'Graham Neubig is a professor at MIT'
+              }
+          ], 
+          'response_level_factuality': False
+       }
+    ]
 }
 ```
 </details>
 
 
 
 
@@ -280,15 +308,15 @@
 }
 ```
 
 
 
 In this case, you will get:
 
-```json
+```python
 {
   "average_claim_level_factuality": 1.0,
   "average_response_level_factuality": 1.0,
   "detailed_information": [
     {
       'prompt': 'def get_max_triples(n): """ You are given a positive integer n. You have to create an integer array a of length n. For each i (1 ≤ i ≤ n), the value of a[i] = i * i - i + 1. Return the number of triples (a[i], a[j], a[k]) of a where i < j < k, and a[i] + a[j] + a[k] is a multiple of 3. Example : Input: n = 5 Output: 1 Explanation: a = [1, 3, 7, 13, 21] The only valid triple is (1, 7, 13). """ Now implement the function get_max_triples using Python',
       'response': 'def get_max_triples(n):\n    a = [i * i - i + 1 for i in range(1, n+1)]\n    count = 0\n    for i in range(n-2):\n        for j in range(i+1, n-1):\n            for k in range(j+1, n):\n                if (a[i] + a[j] + a[k]) % 3 == 0:\n                    count += 1\n    return count\n\nprint(get_max_triples(5)) # Output: 1', 
@@ -377,15 +405,15 @@
     ]
 }
 ```
 
 
 In this case, you will get:
 
-```json
+```python
 {
   "average_claim_level_factuality": 0.5,
   "average_response_level_factuality": 0.0,
   "detailed_information": [
     {
       'prompt': "Stephen placed an online order for groceries.  His final bill came to $7023116.  Because this was through a delivery vendor, they tacked on a 25% fee to his final total and charged him $3.00 in delivery fees.  Stephen also added a $4.00 tip.  After the extra fees, what was the final price of Stephen's groceries?",
       'category': 'math',
@@ -483,15 +511,15 @@
     ...
   ]
 }
 ```
 
 In this case, you will get:
 
-```json
+```python
 {
     "average_claim_level_factuality": 0.0, 
     "average_response_level_factuality": 0.0, 
     "detailed_information": [
       {
         'prompt': "Detail how machine learning algorithms are applied in data analytics and the processes involved in training these algorithms. Please cite relevant research papers or textbooks to support your points, including the author's name, the title of the work, and the year of publication.", 'response': 'Machine learning algorithms play a crucial role in data analytics. They are used to extract insights and knowledge from large datasets, which can be used to make informed decisions and predictions. The following are the processes involved in training machine learning algorithms:\n\n1. Data Preprocessing: The first step in training a machine learning algorithm is to preprocess the data. This involves cleaning the data, handling missing values, encoding categorical variables, and scaling the data. The aim of preprocessing is to ensure that the data is in a format that can be used by the machine learning algorithm.\n2. Feature Selection: Once the data has been preprocessed, the next step is to select the relevant features that will be used to train the machine learning algorithm. This involves identifying the features that are most important for predicting the target variable. Feature selection can be done using various techniques, such as filter methods, wrapper methods, and embedded methods.\n3. Model Selection: After feature selection, the next step is to select the appropriate machine learning algorithm to use. There are various types of machine learning algorithms, such as supervised learning, unsupervised learning, and reinforcement learning. The choice of algorithm depends on the nature of the problem and the type of data available.\n4. Training the Model: Once the model has been selected, the next step is to train the machine learning algorithm using the preprocessed data. This involves using a training set of data to optimize the parameters of the model so that it can accurately predict the target variable.\n5. Model Evaluation: After the model has been trained, the next step is to evaluate its performance. This involves testing the model on a separate test set of data and measuring its accuracy, precision, recall, and other performance metrics.\n6. Model Deployment: Once the model has been evaluated and fine-tuned, it can be deployed in a production environment. This involves integrating the model into a larger system or workflow, and monitoring its performance over time.\n\nResearch papers and textbooks that support the above points include:\n\n* "An Introduction to Machine Learning" by Alpaydin, B., (2010) which provides a comprehensive overview of machine learning algorithms and their applications.\n* "Data Mining: Concepts and Techniques" by Han, J., Kamber, B., & Pei, J., (2011) which provides a detailed introduction to data mining and its applications.\n* "Machine Learning: Trends, Perspectives, and Prospects" by Kamber, B., & Pei, J., (2012) which provides an overview of the current trends and future prospects of machine learning.\n* "Machine Learning for Data Mining" by He, C., & Wang, Y., (2015) which provides an in-depth introduction to machine learning algorithms and their applications in data mining.', 
         'category': 'scientific', 
@@ -521,15 +549,21 @@
 * Run the API locally: `uvicorn main:app --host 0.0.0.0 --port ${PORT:-5003}`
 * Enter plugin store of [ChatGPT Website](https://chat.openai.com/?model=gpt-4-plugins)
 * Click 'develop your own plugin' then enter the website domain `localhost:5003` under 'domain'.
 
 ### Demo
 
 <details>
-<summary>Videos</summary>
+<summary>Videos (click to toggle the content)</summary>
+
+Knowledge-based QA: 
+
+![Alt Text](./figs/factool_plugin_kbqa2.gif)
+
+![Alt Text](./figs/factool_plugin_kbqa3.gif)
 
 Code: 
 
 ![Alt Text](./figs/factool_plugin_code.gif)
 
 Math: 
 
@@ -537,8 +571,19 @@
 
 Scientific Literature Review: 
 
 ![Alt Text](./figs/factool_plugin_scientific.gif)
 
 </details>
 
+## Citation
+Please cite our [paper](https://arxiv.org/abs/2307.13528) if you find the repository helpful.
+```
+@article{chern2023factool,
+  title={FacTool: Factuality Detection in Generative AI--A Tool Augmented Framework for Multi-Task and Multi-Domain Scenarios},
+  author={Chern, I-Chun and Chern, Steffi and Chen, Shiqi and Yuan, Weizhe and Feng, Kehua and Zhou, Chunting and He, Junxian and Neubig, Graham and Liu, Pengfei},
+  journal={arXiv preprint arXiv:2307.13528},
+  year={2023}
+}
+```
+
```

### Comparing `factool-0.1.0/README.md` & `factool-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 ## FacTool: Factuality Detection in Generative AI
+[**Factuality Leaderboard**](https://github.com/GAIR-NLP/factool#factuality-leaderboard) | 
+[**Installation**](https://github.com/GAIR-NLP/factool#installation) | 
+[**Quick Start**](https://github.com/GAIR-NLP/factool#quick-start) |
+[**ChatGPT Plugin with FacTool**](https://github.com/GAIR-NLP/factool#chatgpt-plugin-with-factool) |
+[**Citation**](https://github.com/GAIR-NLP/factool#citation) |
 
-This repository contains the source code and plugin configuration for our [paper]():
+This repository contains the source code and plugin configuration for our [paper](https://arxiv.org/abs/2307.13528):
 
 Factool is a tool augmented framework for detecting factual errors of texts generated by large language models (e.g., ChatGPT). 
 Factool now supports 4 tasks: 
 * **knowledge-based QA**: Factool detects factual errors in knowledge-based QA.
 * **code generation**: Factool detects execution errors in code generation.
 * **mathematical reasoning**: Factool detects calculation errors in mathematical reasoning.
 * **scientific literature review**: Factool detects hallucinated scientific literatures.
@@ -14,14 +19,30 @@
  </p>
  
 
 Demo of Knowledge-based QA: 
 
 ![Alt Text](./figs/factool_plugin_kbqa.gif)
 
+![Alt Text](./figs/factool_chinese.gif)
+
+![Alt Text](./figs/factool_japanese.gif)
+
+## Factuality Leaderboard
+
+Our factuality leaderboard shows the factual accuracy of different chatbots evaluated by FacTool.
+
+| LLMs | Weighted Claim-Level Accuracy | Response-Level Accuracy |
+| -------- | -------- | -------- |
+| GPT-4  | **75.60**  | **43.33**  |
+| ChatGPT  | 68.63  | 36.67  |
+| Claude-v1  | 63.95  | 26.67 |
+| Bard  | 61.15  | 33.33 |
+| Vicuna-13B  | 50.35 | 21.67 |
+
 
 ## Installation
 
 * #### For General User
 
 ```bash
 pip install factool
@@ -42,15 +63,15 @@
 ### API Key Preparation
 * get your OpenAI API key from [here](https://beta.openai.com/). This is used in all scenarios (Knowledge-based QA, Code, Math, Scientific Literature Review). 
 * get your Serper API key from [here](https://serper.dev/). This is only used in Knowledge-based QA. 
 * get your Scraper API key from [here](https://www.scraperapi.com/). This is only used in Scientific Literature Review. 
 
 ### General Usage
 
-You could also directly refer to [example.py](https://github.com/GAIR-NLP/factool/blob/main/example.py) and [example_inputs.jsonl](https://github.com/GAIR-NLP/factool/blob/main/example_inputs.jsonl) for general usage.
+You could also directly refer to [./example/example.py](https://github.com/GAIR-NLP/factool/blob/main/example/example.py) and [example_inputs.jsonl](https://github.com/GAIR-NLP/factool/blob/main/example/example_inputs.jsonl) for general usage.
 
 <details>
 <summary>General Usage (click to toggle the content)</summary>
 
 ```python
 export OPENAI_API_KEY=... # this is required in all tasks
 export SERPER_API_KEY=... # this is required only in knowledge-based QA
@@ -138,53 +159,60 @@
   "detailed_information": [
     {
       'prompt': prompt_1, 
       'response': response_1, 
       'category': 'kbqa', 
       'claims': [claim_11, claim_12, ..., claims_1n], 
       'queries': [[query_111, query_112], [query_121, query_122], ..[query_1n1, query_1n2]], 
-      'evidences': [[evidences_11], [evidences_12], ..., [evidences_1n]], 
+      'evidences': [[evidences_with_source_11], [evidences_with_source_12], ..., [evidences_with_source_1n]], 
       'claim_level_factuality': [{claim_11, reasoning_11, error_11, correction_11, factuality_11}, {claim_12, reasoning_12, error_12, correction_12, factuality_12}, ..., {claim_1n, reasoning_1n, error_1n, correction_1n, factuality_1n}], 
       'response_level_factuality': factuality_1
     },
     {
       'prompt': prompt_2, 
       'response': response_2, 
       'category': 'kbqa',
       'claims': [claim_21, claim_22, ..., claims_2n], 
       'queries': [[query_211, query_212], [query_221, query_222], ..., [query_2n1, query_2n2]], 
-      'evidences': [[evidences_21], [evidences_22], ..., [evidences_2n]], 
+      'evidences': [[evidences_with_source_21], [evidences_with_source_22], ..., [evidences_with_source_2n]], 
       'claim_level_factuality': [{claim_21, reasoning_21, error_21, correction_21, factuality_21}, {claim_22, reasoning_22, error_22, correction_22, factuality_22}, ..., {claim_2n, reasoning_2n, error_2n, correction_2n, factuality_2n}],
       'response_level_factuality': factuality_2,
     },
     ...
   ]
 }
 ```
 
 In this case, you will get:
 
 
-```json
+```python
 {
-  "average_claim_level_factuality": avg_claim_level_factuality,
-  "average_response_level_factuality": avg_response_level_factuality,
-  "detailed_information": [
-    {
-      'prompt': 'Introduce Graham Neubig',
-      'response': 'Graham Neubig is a professor at MIT',
-      'category': 'kbqa',
-      'entry_point': 'answer_question',
-      'claims': [{'claim': 'Graham Neubig is a professor at MIT'}],
-      'queries': [['Is Graham Neubig a professor at MIT?', 'Graham Neubig MIT']],
-      'evidences': [['I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'Graham Neubig. I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with ...', 'Missing: MIT? | Must include:MIT?.', 'Associate Professor, Language Technology Institute, Carnegie Mellon University Affiliated Faculty, Machine Learning Department, Carnegie Mellon University', 'Missing: MIT? | Must include:MIT?.', 'I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with a bunch of great ...', 'Missing: MIT | Must include:MIT.', 'I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'was heavily inspired by an MIT PhD thesis finished 16 years earlier in 1996! ... Episode 22 of The Thesis Review: Graham Neubig (@gneubig), ...', 'Graham Neubig,. Graham Neubig. Graduate School of Information Science Nara Institute of Science and Technology. Search for other works by this author on:.']],
-      'claim_level_factuality': [{'reasoning': 'The given text states that Graham Neubig is a professor at MIT. However, the provided evidences consistently mention that Graham Neubig is an Associate Professor at Carnegie Mellon University. There is no mention of Graham Neubig being affiliated with MIT in any of the provided evidences.', 'error': 'The given text Falsely states that Graham Neubig is a professor at MIT.', 'correction': 'Graham Neubig is an Associate Professor at Carnegie Mellon University.', 'factuality': False, 'claim': 'Graham Neubig is a professor at MIT'}],
-      'response_level_factuality': False
-    }
-  ]
+    'average_claim_level_factuality': 0.0,  
+    'average_response_level_factuality': 0.0, 
+    'detailed_information': [
+        {
+          'prompt': 'Introduce Graham Neubig',
+          'response': 'Graham Neubig is a professor at MIT', 
+          'category': 'kbqa', 'search_type': 'online', 
+          'claims': [{'claim': 'Graham Neubig is a professor at MIT'}], 
+          'queries': [['Graham Neubig current position', 'Is Graham Neubig a professor at MIT?']], 
+          'evidences': [{'evidence': 'I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'source': 'https://www.linkedin.com/in/graham-neubig-10b41616b'}, {'evidence': 'Missing: position | Show results with:position', 'source': 'https://www.linkedin.com/in/graham-neubig-10b41616b'}, {'evidence': 'My research is concerned with language and its role in human communication. In particular, my long-term research goal is to break down barriers in ...', 'source': 'https://miis.cs.cmu.edu/people/222215657/graham-neubig'}, {'evidence': 'My research focuses on handling human languages (like English or Japanese) with computers -- natural language processing. In particular, I am interested in ...', 'source': 'http://www.phontron.com/'}, {'evidence': 'Missing: current | Show results with:current', 'source': 'http://www.phontron.com/'}, {'evidence': 'Graham Neubig. I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with ...', 'source': 'http://www.phontron.com/'}, {'evidence': 'Missing: MIT? | Show results with:MIT?', 'source': 'http://www.phontron.com/'}, {'evidence': 'Associate Professor, Language Technology Institute, Carnegie Mellon University Affiliated Faculty, Machine Learning Department, Carnegie Mellon University', 'source': 'https://www.phontron.com/research.php'}, {'evidence': 'Missing: MIT? | Show results with:MIT?', 'source': 'https://www.phontron.com/research.php'}, {'evidence': 'MIT Embodied Intelligence ... About the speaker: Graham ...', 'source': 'https://youtube.com/watch?v=CtcP5bvODzY'}],
+          'claim_level_factuality': [
+              {
+                'reasoning': 'The given text is non-factual. The evidence provided clearly states that Graham Neubig is an Associate Professor of Computer Science at Carnegie Mellon University, not at MIT.', 
+                'error': 'The error in the text is the incorrect affiliation of Graham Neubig. He is not a professor at MIT.', 
+                'correction': 'Graham Neubig is a professor at Carnegie Mellon University.', 
+                'factuality': False, 
+                'claim': 'Graham Neubig is a professor at MIT'
+              }
+          ], 
+          'response_level_factuality': False
+       }
+    ]
 }
 ```
 </details>
 
 
 
 
@@ -263,15 +291,15 @@
 }
 ```
 
 
 
 In this case, you will get:
 
-```json
+```python
 {
   "average_claim_level_factuality": 1.0,
   "average_response_level_factuality": 1.0,
   "detailed_information": [
     {
       'prompt': 'def get_max_triples(n): """ You are given a positive integer n. You have to create an integer array a of length n. For each i (1 ≤ i ≤ n), the value of a[i] = i * i - i + 1. Return the number of triples (a[i], a[j], a[k]) of a where i < j < k, and a[i] + a[j] + a[k] is a multiple of 3. Example : Input: n = 5 Output: 1 Explanation: a = [1, 3, 7, 13, 21] The only valid triple is (1, 7, 13). """ Now implement the function get_max_triples using Python',
       'response': 'def get_max_triples(n):\n    a = [i * i - i + 1 for i in range(1, n+1)]\n    count = 0\n    for i in range(n-2):\n        for j in range(i+1, n-1):\n            for k in range(j+1, n):\n                if (a[i] + a[j] + a[k]) % 3 == 0:\n                    count += 1\n    return count\n\nprint(get_max_triples(5)) # Output: 1', 
@@ -360,15 +388,15 @@
     ]
 }
 ```
 
 
 In this case, you will get:
 
-```json
+```python
 {
   "average_claim_level_factuality": 0.5,
   "average_response_level_factuality": 0.0,
   "detailed_information": [
     {
       'prompt': "Stephen placed an online order for groceries.  His final bill came to $7023116.  Because this was through a delivery vendor, they tacked on a 25% fee to his final total and charged him $3.00 in delivery fees.  Stephen also added a $4.00 tip.  After the extra fees, what was the final price of Stephen's groceries?",
       'category': 'math',
@@ -466,15 +494,15 @@
     ...
   ]
 }
 ```
 
 In this case, you will get:
 
-```json
+```python
 {
     "average_claim_level_factuality": 0.0, 
     "average_response_level_factuality": 0.0, 
     "detailed_information": [
       {
         'prompt': "Detail how machine learning algorithms are applied in data analytics and the processes involved in training these algorithms. Please cite relevant research papers or textbooks to support your points, including the author's name, the title of the work, and the year of publication.", 'response': 'Machine learning algorithms play a crucial role in data analytics. They are used to extract insights and knowledge from large datasets, which can be used to make informed decisions and predictions. The following are the processes involved in training machine learning algorithms:\n\n1. Data Preprocessing: The first step in training a machine learning algorithm is to preprocess the data. This involves cleaning the data, handling missing values, encoding categorical variables, and scaling the data. The aim of preprocessing is to ensure that the data is in a format that can be used by the machine learning algorithm.\n2. Feature Selection: Once the data has been preprocessed, the next step is to select the relevant features that will be used to train the machine learning algorithm. This involves identifying the features that are most important for predicting the target variable. Feature selection can be done using various techniques, such as filter methods, wrapper methods, and embedded methods.\n3. Model Selection: After feature selection, the next step is to select the appropriate machine learning algorithm to use. There are various types of machine learning algorithms, such as supervised learning, unsupervised learning, and reinforcement learning. The choice of algorithm depends on the nature of the problem and the type of data available.\n4. Training the Model: Once the model has been selected, the next step is to train the machine learning algorithm using the preprocessed data. This involves using a training set of data to optimize the parameters of the model so that it can accurately predict the target variable.\n5. Model Evaluation: After the model has been trained, the next step is to evaluate its performance. This involves testing the model on a separate test set of data and measuring its accuracy, precision, recall, and other performance metrics.\n6. Model Deployment: Once the model has been evaluated and fine-tuned, it can be deployed in a production environment. This involves integrating the model into a larger system or workflow, and monitoring its performance over time.\n\nResearch papers and textbooks that support the above points include:\n\n* "An Introduction to Machine Learning" by Alpaydin, B., (2010) which provides a comprehensive overview of machine learning algorithms and their applications.\n* "Data Mining: Concepts and Techniques" by Han, J., Kamber, B., & Pei, J., (2011) which provides a detailed introduction to data mining and its applications.\n* "Machine Learning: Trends, Perspectives, and Prospects" by Kamber, B., & Pei, J., (2012) which provides an overview of the current trends and future prospects of machine learning.\n* "Machine Learning for Data Mining" by He, C., & Wang, Y., (2015) which provides an in-depth introduction to machine learning algorithms and their applications in data mining.', 
         'category': 'scientific', 
@@ -504,22 +532,39 @@
 * Run the API locally: `uvicorn main:app --host 0.0.0.0 --port ${PORT:-5003}`
 * Enter plugin store of [ChatGPT Website](https://chat.openai.com/?model=gpt-4-plugins)
 * Click 'develop your own plugin' then enter the website domain `localhost:5003` under 'domain'.
 
 ### Demo
 
 <details>
-<summary>Videos</summary>
+<summary>Videos (click to toggle the content)</summary>
+
+Knowledge-based QA: 
+
+![Alt Text](./figs/factool_plugin_kbqa2.gif)
+
+![Alt Text](./figs/factool_plugin_kbqa3.gif)
 
 Code: 
 
 ![Alt Text](./figs/factool_plugin_code.gif)
 
 Math: 
 
 ![Alt Text](./figs/factool_plugin_math.gif)
 
 Scientific Literature Review: 
 
 ![Alt Text](./figs/factool_plugin_scientific.gif)
 
 </details>
+
+## Citation
+Please cite our [paper](https://arxiv.org/abs/2307.13528) if you find the repository helpful.
+```
+@article{chern2023factool,
+  title={FacTool: Factuality Detection in Generative AI--A Tool Augmented Framework for Multi-Task and Multi-Domain Scenarios},
+  author={Chern, I-Chun and Chern, Steffi and Chen, Shiqi and Yuan, Weizhe and Feng, Kehua and Zhou, Chunting and He, Junxian and Neubig, Graham and Liu, Pengfei},
+  journal={arXiv preprint arXiv:2307.13528},
+  year={2023}
+}
+```
```

### Comparing `factool-0.1.0/factool/code/helper/_execution.py` & `factool-0.1.2/factool/code/helper/_execution.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/code/helper/execution.py` & `factool-0.1.2/factool/code/helper/execution.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/code/helper/io_utils.py` & `factool-0.1.2/factool/code/helper/io_utils.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/code/helper/postprocess.py` & `factool-0.1.2/factool/code/helper/postprocess.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/code/pipeline.py` & `factool-0.1.2/factool/code/pipeline.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/env_config.py` & `factool-0.1.2/factool/env_config.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/knowledge_qa/google_serper.py` & `factool-0.1.2/factool/knowledge_qa/google_serper.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,40 +43,49 @@
     
     def _parse_results(self, results):
         snippets = []
 
         if results.get("answerBox"):
             answer_box = results.get("answerBox", {})
             if answer_box.get("answer"):
-                return [answer_box.get("answer")]
+                element = {"content":answer_box.get("answer"),"source":"None"}
+                return [element]
             elif answer_box.get("snippet"):
-                return [answer_box.get("snippet").replace("\n", " ")]
+                element = {"content":answer_box.get("snippet").replace("\n", " "),"source":"None"}
+                return [element]
             elif answer_box.get("snippetHighlighted"):
-                return answer_box.get("snippetHighlighted")
+                element = {"content":answer_box.get("snippetHighlighted"),"source":"None"}
+                return [element]
             
         if results.get("knowledgeGraph"):
             kg = results.get("knowledgeGraph", {})
             title = kg.get("title")
             entity_type = kg.get("type")
             if entity_type:
-                snippets.append(f"{title}: {entity_type}.")
+                element = {"content":f"{title}: {entity_type}","source":"None"}
+                snippets.append(element)
             description = kg.get("description")
             if description:
-                snippets.append(description)
+                element = {"content":description,"source":"None"}
+                snippets.append(element)
             for attribute, value in kg.get("attributes", {}).items():
-                snippets.append(f"{title} {attribute}: {value}.")
+                element = {"content":f"{attribute}: {value}","source":"None"}
+                snippets.append(element)
 
         for result in results["organic"][: self.k]:
             if "snippet" in result:
-                snippets.append(result["snippet"])
+                element = {"content":result["snippet"],"source":result["link"]}
+                snippets.append(element)
             for attribute, value in result.get("attributes", {}).items():
-                snippets.append(f"{attribute}: {value}.")
+                element = {"content":f"{attribute}: {value}","source":result["link"]}
+                snippets.append(element)
 
         if len(snippets) == 0:
-            return ["No good Google Search Result was found"]
+            element = {"content":"No good Google Search Result was found","source":"None"}
+            return [element]
         
         # keep only the first k snippets
         snippets = snippets[:int(self.k / 2)]
 
         return snippets
     
     async def parallel_searches(self, search_queries, gl, hl):
@@ -92,16 +101,16 @@
         for sublist in queries:
             if sublist is None:
                 sublist = ['None', 'None']
             for item in sublist:
                 flattened_queries.append(item)
 
         results = await self.parallel_searches(flattened_queries, gl=self.gl, hl=self.hl)
-        snippets = []
+        snippets_list = []
         for i in range(len(results)):
-            snippets.append(self._parse_results(results[i]))
-        snippets_split = [snippets[i] + snippets[i+1] for i in range(0, len(snippets), 2)]
+            snippets_list.append(self._parse_results(results[i]))
+        snippets_split = [snippets_list[i] + snippets_list[i+1] for i in range(0, len(snippets_list), 2)]
         return snippets_split
     
 if __name__ == "__main__":
     search = GoogleSerperAPIWrapper()
-    print(search.run("What is the capital of the United States?"))
+    print(asyncio.run(search.run("What is the capital of the United States?")))
```

### Comparing `factool-0.1.0/factool/knowledge_qa/pipeline.py` & `factool-0.1.2/factool/knowledge_qa/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 import os
 import time
 import math
 import pdb
 from typing import List, Dict
 
 from factool.knowledge_qa.tool import google_search
+from factool.knowledge_qa.tool import local_search
 from factool.utils.base.pipeline import pipeline
 
 class knowledge_qa_pipeline(pipeline):
-    def __init__(self, foundation_model, snippet_cnt):
+    def __init__(self, foundation_model, snippet_cnt, search_type, data_link=None, Embed_link=None):
         super().__init__('knowledge_qa', foundation_model)
-
-        self.tool = google_search(snippet_cnt = snippet_cnt)
-
+        if(search_type == 'online'):
+            self.tool = google_search(snippet_cnt = snippet_cnt)
+        elif(search_type == 'local'):
+            self.tool = local_search(snippet_cnt = snippet_cnt, data_link=data_link, embedding_link=Embed_link)
         with open(os.path.join(self.prompts_path, "claim_extraction.yaml"), 'r') as file:
             data = yaml.load(file, Loader=yaml.FullLoader)
         self.claim_prompt = data['knowledge_qa']
 
         with open(os.path.join(self.prompts_path, 'query_generation.yaml'), 'r') as file:
             data = yaml.load(file, Loader=yaml.FullLoader)
         self.query_prompt = data['knowledge_qa']
@@ -59,24 +61,29 @@
         ]
         return await self.chat.async_run(messages_list, Dict)
     
     async def run_with_tool_live(self, responses):
         claims_in_responses = await self._claim_extraction(responses)
         queries_in_responses = []
         evidences_in_responses = []
+        sources_in_responses = []
         verifications_in_responses = []
+        #pdb.set_trace()
         for claims_in_response in claims_in_responses:
             queries = await self._query_generation(claims_in_response)
             queries_in_responses.append(queries)
-            evidences = await self.tool.run(queries)
+            search_outputs_for_claims = await self.tool.run(queries)
+            evidences = [output["content"] for search_outputs_for_claim in search_outputs_for_claims for output in search_outputs_for_claim]
             evidences_in_responses.append(evidences)
+            sources = [output["source"] for search_outputs_for_claim in search_outputs_for_claims for output in search_outputs_for_claim]
+            sources_in_responses.append(sources)
             verifications = await self._verification(claims_in_response, evidences)
             verifications_in_responses.append(verifications)
 
-        return claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses
+        return claims_in_responses, queries_in_responses, evidences_in_responses, sources_in_responses, verifications_in_responses
     
     async def run_with_tool_live_without_claim_extraction(self, claims):
         queries = await self._query_generation(claims)
         evidences = await self.tool.run(queries)
 
         final_response = await self._verification(claims, evidences)
         for i in range(len(final_response)):
@@ -93,31 +100,36 @@
         self.sample_list = [{"prompt": prompt, "response": response, "category": 'kbqa'} for prompt, response in zip(prompts, responses)]
 
         for i in range(num_batches):
             print(i)
             batch_start = i * batch_size
             batch_end = min((i + 1) * batch_size, len(responses))
 
-            claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses = await self.run_with_tool_live(responses[batch_start:batch_end])
+            claims_in_responses, queries_in_responses, evidences_in_responses, sources_in_responses, verifications_in_responses = await self.run_with_tool_live(responses[batch_start:batch_end])
 
-            for j, (claims_in_response, queries_in_response, evidences_in_response, verifications_in_response) in enumerate(zip(claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses)):
+            for j, (claims_in_response, queries_in_response, evidences_in_response, sources_in_response, verifications_in_response) in enumerate(zip(claims_in_responses, queries_in_responses, evidences_in_responses, sources_in_responses, verifications_in_responses)):
                 index = batch_start + j
                 
                 if claims_in_response != None:
                     for k, claim in enumerate(claims_in_response):
                         if verifications_in_response[k] != None:
                             if claim != None:
                                 verifications_in_response[k].update({'claim': claim['claim']})
                             else:
                                 verifications_in_response[k].update({'claim': 'None'})
 
+                evidences_with_source = []
+                for evidence, source in zip(evidences_in_response, sources_in_response):
+                    evidences_with_source.append({'evidence': evidence, 'source': source})
                 self.sample_list[index].update({
                     'claims': claims_in_response,
                     'queries': queries_in_response,
-                    'evidences': evidences_in_response,
+                    # 'evidences': evidences_in_response,
+                    # 'sources': sources_in_response,
+                    'evidences': evidences_with_source,
                     'claim_level_factuality': verifications_in_response,
                     'response_level_factuality': all([verification['factuality'] if verification != None else True for verification in verifications_in_response])
                 })
 
         return self.sample_list
     
     async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
@@ -201,8 +213,8 @@
                         'self_check_reasoning': response.get('reasoning', 'None')
                     })
 
             # save everything after each batch to prevent data loss
             with open(self_check_classified_dataset_path, 'w') as f:
                 for item in self.sample_list:
                     json_str = json.dumps(item)
-                    f.write(json_str + '\n')
+                    f.write(json_str + '\n')
```

### Comparing `factool-0.1.0/factool/math/pipeline.py` & `factool-0.1.2/factool/math/pipeline.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/math/tool.py` & `factool-0.1.2/factool/math/tool.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/scientific/pipeline.py` & `factool-0.1.2/factool/scientific/pipeline.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/scientific/tool.py` & `factool-0.1.2/factool/scientific/tool.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/utils/base/pipeline.py` & `factool-0.1.2/factool/utils/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/utils/claim_extractor.py` & `factool-0.1.2/factool/utils/claim_extractor.py`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/utils/openai_wrapper.py` & `factool-0.1.2/factool/utils/openai_wrapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,14 +23,16 @@
             self,
             model_name='gpt-3.5-turbo',
             max_tokens=2500,
             temperature=0,
             top_p=1,
             request_timeout=60,
     ):
+        if 'gpt' not in model_name:
+            openai.api_base = "http://localhost:8000/v1"
         self.config = {
             'model_name': model_name,
             'max_tokens': max_tokens,
             'temperature': temperature,
             'top_p': top_p,
             'request_timeout': request_timeout,
         }
@@ -79,14 +81,18 @@
                     await asyncio.sleep(1)
                 except openai.error.Timeout:
                     print('Timeout error, waiting for 1 second...')
                     await asyncio.sleep(1)
                 except openai.error.ServiceUnavailableError:
                     print('Service unavailable error, waiting for 3 second...')
                     await asyncio.sleep(3)
+                except openai.error.APIConnectionError:
+                    print('API Connection error, waiting for 3 second...')
+                    await asyncio.sleep(3)
+
             return None
 
         async_responses = [
             _request_with_retry(messages)
             for messages in messages_list
         ]
 
@@ -115,16 +121,44 @@
             
             messages_list_cur_index = [i for i in messages_list_cur_index if i not in finised_index]
             
             retry -= 1
         
         return responses
 
+class OpenAIEmbed():
+    async def create_embedding(self, text, retry=3):
+        for _ in range(retry):
+            try:
+                response = await openai.Embedding.acreate(input=text, model="text-embedding-ada-002")
+                return response
+            except openai.error.RateLimitError:
+                print('Rate limit error, waiting for 1 second...')
+                await asyncio.sleep(1)
+            except openai.error.APIError:
+                print('API error, waiting for 1 second...')
+                await asyncio.sleep(1)
+            except openai.error.Timeout:
+                print('Timeout error, waiting for 1 second...')
+                await asyncio.sleep(1)
+        return None
+
+    async def process_batch(self, batch, retry=3):
+        tasks = [self.create_embedding(text, retry=retry) for text in batch]
+        return await asyncio.gather(*tasks)
+
 if __name__ == "__main__":
     chat = OpenAIChat()
 
     predictions = chat.async_run(
         messages_list=[
             [{"role": "user", "content": "show either 'ab' or '['a']'. Do not do anything else."}],
         ] * 20,
         expected_type=List,
-    )
+    )
+
+    # Usage
+    embed = OpenAIEmbed()
+    batch = ["string1", "string2", "string3", "string4", "string5", "string6", "string7", "string8", "string9", "string10"]  # Your batch of strings
+    embeddings = asyncio.run(embed.process_batch(batch, retry=3))
+    for embedding in embeddings:
+        print(embedding["data"][0]["embedding"])
```

### Comparing `factool-0.1.0/factool/utils/prompts/agreement_verification.yaml` & `factool-0.1.2/factool/utils/prompts/agreement_verification.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     The following is the given text
     [text]: {claim}
     The following is the provided evidences
     [evidences]: {evidence}
     You should only respond in format as described below. DO NOT RETURN ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
     [response format]: 
     {{
-      "reasoning": "Why is the given text factual or non-factual? Be careful when you said something is non-factual. When you said something is non-factual, you must provide mulitple evidences to support your decision.",
+      "reasoning": "Why is the given text factual or non-factual? Be careful when you said something is non-factual. When you said something is non-factual, you must provide multiple evidences to support your decision.",
       "error": "None if the text is factual; otherwise, describe the error.",
       "correction": "The corrected text if there is an error.",
       "factuality": True if the given text is factual, False otherwise.
     }}
 
 scientific:
   system: |-
@@ -41,8 +41,8 @@
     [string1]: "Tom Brown et. al"
     [list1]: ["Y. Lecun", "G. Hinton"]
     [response]: {{"reasoning": "string 1 contains 1 last name 'Brown'. Brown is not present in list1.", "factuality": False}}
 
     Complete the following:
     [string1]: {string1}
     [list1]: {list2}
-    [response]: 
+    [response]:
```

### Comparing `factool-0.1.0/factool/utils/prompts/claim_extraction.yaml` & `factool-0.1.2/factool/utils/prompts/claim_extraction.yaml`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/utils/prompts/query_generation.yaml` & `factool-0.1.2/factool/utils/prompts/query_generation.yaml`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool/utils/prompts/self_check.yaml` & `factool-0.1.2/factool/utils/prompts/self_check.yaml`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/factool.egg-info/PKG-INFO` & `factool-0.1.2/factool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factool
-Version: 0.1.0
+Version: 0.1.2
 Summary: Factuality Detection for Generative AI
 Home-page: https://github.com/GAIR-NLP/factool
 Author: GAIR Research Group
 License: Apache License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing
@@ -12,16 +12,21 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 
 ## FacTool: Factuality Detection in Generative AI
+[**Factuality Leaderboard**](https://github.com/GAIR-NLP/factool#factuality-leaderboard) | 
+[**Installation**](https://github.com/GAIR-NLP/factool#installation) | 
+[**Quick Start**](https://github.com/GAIR-NLP/factool#quick-start) |
+[**ChatGPT Plugin with FacTool**](https://github.com/GAIR-NLP/factool#chatgpt-plugin-with-factool) |
+[**Citation**](https://github.com/GAIR-NLP/factool#citation) |
 
-This repository contains the source code and plugin configuration for our [paper]():
+This repository contains the source code and plugin configuration for our [paper](https://arxiv.org/abs/2307.13528):
 
 Factool is a tool augmented framework for detecting factual errors of texts generated by large language models (e.g., ChatGPT). 
 Factool now supports 4 tasks: 
 * **knowledge-based QA**: Factool detects factual errors in knowledge-based QA.
 * **code generation**: Factool detects execution errors in code generation.
 * **mathematical reasoning**: Factool detects calculation errors in mathematical reasoning.
 * **scientific literature review**: Factool detects hallucinated scientific literatures.
@@ -31,14 +36,30 @@
  </p>
  
 
 Demo of Knowledge-based QA: 
 
 ![Alt Text](./figs/factool_plugin_kbqa.gif)
 
+![Alt Text](./figs/factool_chinese.gif)
+
+![Alt Text](./figs/factool_japanese.gif)
+
+## Factuality Leaderboard
+
+Our factuality leaderboard shows the factual accuracy of different chatbots evaluated by FacTool.
+
+| LLMs | Weighted Claim-Level Accuracy | Response-Level Accuracy |
+| -------- | -------- | -------- |
+| GPT-4  | **75.60**  | **43.33**  |
+| ChatGPT  | 68.63  | 36.67  |
+| Claude-v1  | 63.95  | 26.67 |
+| Bard  | 61.15  | 33.33 |
+| Vicuna-13B  | 50.35 | 21.67 |
+
 
 ## Installation
 
 * #### For General User
 
 ```bash
 pip install factool
@@ -59,15 +80,15 @@
 ### API Key Preparation
 * get your OpenAI API key from [here](https://beta.openai.com/). This is used in all scenarios (Knowledge-based QA, Code, Math, Scientific Literature Review). 
 * get your Serper API key from [here](https://serper.dev/). This is only used in Knowledge-based QA. 
 * get your Scraper API key from [here](https://www.scraperapi.com/). This is only used in Scientific Literature Review. 
 
 ### General Usage
 
-You could also directly refer to [example.py](https://github.com/GAIR-NLP/factool/blob/main/example.py) and [example_inputs.jsonl](https://github.com/GAIR-NLP/factool/blob/main/example_inputs.jsonl) for general usage.
+You could also directly refer to [./example/example.py](https://github.com/GAIR-NLP/factool/blob/main/example/example.py) and [example_inputs.jsonl](https://github.com/GAIR-NLP/factool/blob/main/example/example_inputs.jsonl) for general usage.
 
 <details>
 <summary>General Usage (click to toggle the content)</summary>
 
 ```python
 export OPENAI_API_KEY=... # this is required in all tasks
 export SERPER_API_KEY=... # this is required only in knowledge-based QA
@@ -155,53 +176,60 @@
   "detailed_information": [
     {
       'prompt': prompt_1, 
       'response': response_1, 
       'category': 'kbqa', 
       'claims': [claim_11, claim_12, ..., claims_1n], 
       'queries': [[query_111, query_112], [query_121, query_122], ..[query_1n1, query_1n2]], 
-      'evidences': [[evidences_11], [evidences_12], ..., [evidences_1n]], 
+      'evidences': [[evidences_with_source_11], [evidences_with_source_12], ..., [evidences_with_source_1n]], 
       'claim_level_factuality': [{claim_11, reasoning_11, error_11, correction_11, factuality_11}, {claim_12, reasoning_12, error_12, correction_12, factuality_12}, ..., {claim_1n, reasoning_1n, error_1n, correction_1n, factuality_1n}], 
       'response_level_factuality': factuality_1
     },
     {
       'prompt': prompt_2, 
       'response': response_2, 
       'category': 'kbqa',
       'claims': [claim_21, claim_22, ..., claims_2n], 
       'queries': [[query_211, query_212], [query_221, query_222], ..., [query_2n1, query_2n2]], 
-      'evidences': [[evidences_21], [evidences_22], ..., [evidences_2n]], 
+      'evidences': [[evidences_with_source_21], [evidences_with_source_22], ..., [evidences_with_source_2n]], 
       'claim_level_factuality': [{claim_21, reasoning_21, error_21, correction_21, factuality_21}, {claim_22, reasoning_22, error_22, correction_22, factuality_22}, ..., {claim_2n, reasoning_2n, error_2n, correction_2n, factuality_2n}],
       'response_level_factuality': factuality_2,
     },
     ...
   ]
 }
 ```
 
 In this case, you will get:
 
 
-```json
+```python
 {
-  "average_claim_level_factuality": avg_claim_level_factuality,
-  "average_response_level_factuality": avg_response_level_factuality,
-  "detailed_information": [
-    {
-      'prompt': 'Introduce Graham Neubig',
-      'response': 'Graham Neubig is a professor at MIT',
-      'category': 'kbqa',
-      'entry_point': 'answer_question',
-      'claims': [{'claim': 'Graham Neubig is a professor at MIT'}],
-      'queries': [['Is Graham Neubig a professor at MIT?', 'Graham Neubig MIT']],
-      'evidences': [['I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'Graham Neubig. I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with ...', 'Missing: MIT? | Must include:MIT?.', 'Associate Professor, Language Technology Institute, Carnegie Mellon University Affiliated Faculty, Machine Learning Department, Carnegie Mellon University', 'Missing: MIT? | Must include:MIT?.', 'I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with a bunch of great ...', 'Missing: MIT | Must include:MIT.', 'I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'was heavily inspired by an MIT PhD thesis finished 16 years earlier in 1996! ... Episode 22 of The Thesis Review: Graham Neubig (@gneubig), ...', 'Graham Neubig,. Graham Neubig. Graduate School of Information Science Nara Institute of Science and Technology. Search for other works by this author on:.']],
-      'claim_level_factuality': [{'reasoning': 'The given text states that Graham Neubig is a professor at MIT. However, the provided evidences consistently mention that Graham Neubig is an Associate Professor at Carnegie Mellon University. There is no mention of Graham Neubig being affiliated with MIT in any of the provided evidences.', 'error': 'The given text Falsely states that Graham Neubig is a professor at MIT.', 'correction': 'Graham Neubig is an Associate Professor at Carnegie Mellon University.', 'factuality': False, 'claim': 'Graham Neubig is a professor at MIT'}],
-      'response_level_factuality': False
-    }
-  ]
+    'average_claim_level_factuality': 0.0,  
+    'average_response_level_factuality': 0.0, 
+    'detailed_information': [
+        {
+          'prompt': 'Introduce Graham Neubig',
+          'response': 'Graham Neubig is a professor at MIT', 
+          'category': 'kbqa', 'search_type': 'online', 
+          'claims': [{'claim': 'Graham Neubig is a professor at MIT'}], 
+          'queries': [['Graham Neubig current position', 'Is Graham Neubig a professor at MIT?']], 
+          'evidences': [{'evidence': 'I am an Associate Professor of Computer Science at Carnegie Mellon University and CEO of Inspired Cognition. My research and development focuses on AI and ...', 'source': 'https://www.linkedin.com/in/graham-neubig-10b41616b'}, {'evidence': 'Missing: position | Show results with:position', 'source': 'https://www.linkedin.com/in/graham-neubig-10b41616b'}, {'evidence': 'My research is concerned with language and its role in human communication. In particular, my long-term research goal is to break down barriers in ...', 'source': 'https://miis.cs.cmu.edu/people/222215657/graham-neubig'}, {'evidence': 'My research focuses on handling human languages (like English or Japanese) with computers -- natural language processing. In particular, I am interested in ...', 'source': 'http://www.phontron.com/'}, {'evidence': 'Missing: current | Show results with:current', 'source': 'http://www.phontron.com/'}, {'evidence': 'Graham Neubig. I am an Associate Professor at the Carnegie Mellon University Language Technology Institute in the School of Computer Science, and work with ...', 'source': 'http://www.phontron.com/'}, {'evidence': 'Missing: MIT? | Show results with:MIT?', 'source': 'http://www.phontron.com/'}, {'evidence': 'Associate Professor, Language Technology Institute, Carnegie Mellon University Affiliated Faculty, Machine Learning Department, Carnegie Mellon University', 'source': 'https://www.phontron.com/research.php'}, {'evidence': 'Missing: MIT? | Show results with:MIT?', 'source': 'https://www.phontron.com/research.php'}, {'evidence': 'MIT Embodied Intelligence ... About the speaker: Graham ...', 'source': 'https://youtube.com/watch?v=CtcP5bvODzY'}],
+          'claim_level_factuality': [
+              {
+                'reasoning': 'The given text is non-factual. The evidence provided clearly states that Graham Neubig is an Associate Professor of Computer Science at Carnegie Mellon University, not at MIT.', 
+                'error': 'The error in the text is the incorrect affiliation of Graham Neubig. He is not a professor at MIT.', 
+                'correction': 'Graham Neubig is a professor at Carnegie Mellon University.', 
+                'factuality': False, 
+                'claim': 'Graham Neubig is a professor at MIT'
+              }
+          ], 
+          'response_level_factuality': False
+       }
+    ]
 }
 ```
 </details>
 
 
 
 
@@ -280,15 +308,15 @@
 }
 ```
 
 
 
 In this case, you will get:
 
-```json
+```python
 {
   "average_claim_level_factuality": 1.0,
   "average_response_level_factuality": 1.0,
   "detailed_information": [
     {
       'prompt': 'def get_max_triples(n): """ You are given a positive integer n. You have to create an integer array a of length n. For each i (1 ≤ i ≤ n), the value of a[i] = i * i - i + 1. Return the number of triples (a[i], a[j], a[k]) of a where i < j < k, and a[i] + a[j] + a[k] is a multiple of 3. Example : Input: n = 5 Output: 1 Explanation: a = [1, 3, 7, 13, 21] The only valid triple is (1, 7, 13). """ Now implement the function get_max_triples using Python',
       'response': 'def get_max_triples(n):\n    a = [i * i - i + 1 for i in range(1, n+1)]\n    count = 0\n    for i in range(n-2):\n        for j in range(i+1, n-1):\n            for k in range(j+1, n):\n                if (a[i] + a[j] + a[k]) % 3 == 0:\n                    count += 1\n    return count\n\nprint(get_max_triples(5)) # Output: 1', 
@@ -377,15 +405,15 @@
     ]
 }
 ```
 
 
 In this case, you will get:
 
-```json
+```python
 {
   "average_claim_level_factuality": 0.5,
   "average_response_level_factuality": 0.0,
   "detailed_information": [
     {
       'prompt': "Stephen placed an online order for groceries.  His final bill came to $7023116.  Because this was through a delivery vendor, they tacked on a 25% fee to his final total and charged him $3.00 in delivery fees.  Stephen also added a $4.00 tip.  After the extra fees, what was the final price of Stephen's groceries?",
       'category': 'math',
@@ -483,15 +511,15 @@
     ...
   ]
 }
 ```
 
 In this case, you will get:
 
-```json
+```python
 {
     "average_claim_level_factuality": 0.0, 
     "average_response_level_factuality": 0.0, 
     "detailed_information": [
       {
         'prompt': "Detail how machine learning algorithms are applied in data analytics and the processes involved in training these algorithms. Please cite relevant research papers or textbooks to support your points, including the author's name, the title of the work, and the year of publication.", 'response': 'Machine learning algorithms play a crucial role in data analytics. They are used to extract insights and knowledge from large datasets, which can be used to make informed decisions and predictions. The following are the processes involved in training machine learning algorithms:\n\n1. Data Preprocessing: The first step in training a machine learning algorithm is to preprocess the data. This involves cleaning the data, handling missing values, encoding categorical variables, and scaling the data. The aim of preprocessing is to ensure that the data is in a format that can be used by the machine learning algorithm.\n2. Feature Selection: Once the data has been preprocessed, the next step is to select the relevant features that will be used to train the machine learning algorithm. This involves identifying the features that are most important for predicting the target variable. Feature selection can be done using various techniques, such as filter methods, wrapper methods, and embedded methods.\n3. Model Selection: After feature selection, the next step is to select the appropriate machine learning algorithm to use. There are various types of machine learning algorithms, such as supervised learning, unsupervised learning, and reinforcement learning. The choice of algorithm depends on the nature of the problem and the type of data available.\n4. Training the Model: Once the model has been selected, the next step is to train the machine learning algorithm using the preprocessed data. This involves using a training set of data to optimize the parameters of the model so that it can accurately predict the target variable.\n5. Model Evaluation: After the model has been trained, the next step is to evaluate its performance. This involves testing the model on a separate test set of data and measuring its accuracy, precision, recall, and other performance metrics.\n6. Model Deployment: Once the model has been evaluated and fine-tuned, it can be deployed in a production environment. This involves integrating the model into a larger system or workflow, and monitoring its performance over time.\n\nResearch papers and textbooks that support the above points include:\n\n* "An Introduction to Machine Learning" by Alpaydin, B., (2010) which provides a comprehensive overview of machine learning algorithms and their applications.\n* "Data Mining: Concepts and Techniques" by Han, J., Kamber, B., & Pei, J., (2011) which provides a detailed introduction to data mining and its applications.\n* "Machine Learning: Trends, Perspectives, and Prospects" by Kamber, B., & Pei, J., (2012) which provides an overview of the current trends and future prospects of machine learning.\n* "Machine Learning for Data Mining" by He, C., & Wang, Y., (2015) which provides an in-depth introduction to machine learning algorithms and their applications in data mining.', 
         'category': 'scientific', 
@@ -521,15 +549,21 @@
 * Run the API locally: `uvicorn main:app --host 0.0.0.0 --port ${PORT:-5003}`
 * Enter plugin store of [ChatGPT Website](https://chat.openai.com/?model=gpt-4-plugins)
 * Click 'develop your own plugin' then enter the website domain `localhost:5003` under 'domain'.
 
 ### Demo
 
 <details>
-<summary>Videos</summary>
+<summary>Videos (click to toggle the content)</summary>
+
+Knowledge-based QA: 
+
+![Alt Text](./figs/factool_plugin_kbqa2.gif)
+
+![Alt Text](./figs/factool_plugin_kbqa3.gif)
 
 Code: 
 
 ![Alt Text](./figs/factool_plugin_code.gif)
 
 Math: 
 
@@ -537,8 +571,19 @@
 
 Scientific Literature Review: 
 
 ![Alt Text](./figs/factool_plugin_scientific.gif)
 
 </details>
 
+## Citation
+Please cite our [paper](https://arxiv.org/abs/2307.13528) if you find the repository helpful.
+```
+@article{chern2023factool,
+  title={FacTool: Factuality Detection in Generative AI--A Tool Augmented Framework for Multi-Task and Multi-Domain Scenarios},
+  author={Chern, I-Chun and Chern, Steffi and Chen, Shiqi and Yuan, Weizhe and Feng, Kehua and Zhou, Chunting and He, Junxian and Neubig, Graham and Liu, Pengfei},
+  journal={arXiv preprint arXiv:2307.13528},
+  year={2023}
+}
+```
+
```

### Comparing `factool-0.1.0/factool.egg-info/SOURCES.txt` & `factool-0.1.2/factool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `factool-0.1.0/setup.cfg` & `factool-0.1.2/setup.cfg`

 * *Files identical despite different names*

