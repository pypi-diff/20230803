# Comparing `tmp/llm_atc-0.1.1.tar.gz` & `tmp/llm_atc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_atc-0.1.1.tar", max compression
+gzip compressed data, was "llm_atc-0.1.2.tar", max compression
```

## Comparing `llm_atc-0.1.1.tar` & `llm_atc-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3190 2023-08-01 22:09:36.921078 llm_atc-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-08-01 22:09:36.927039 llm_atc-0.1.1/llm_atc/__init__.py
--rw-r--r--   0        0        0     5859 2023-08-01 21:43:53.652173 llm_atc-0.1.1/llm_atc/cli.py
--rw-r--r--   0        0        0     2037 2023-08-01 11:00:40.450414 llm_atc-0.1.1/llm_atc/config/serve/serve.yml
--rw-r--r--   0        0        0     3310 2023-08-01 22:05:13.864460 llm_atc-0.1.1/llm_atc/config/train/vicuna.yml
--rw-r--r--   0        0        0      260 2023-07-31 02:19:45.084926 llm_atc-0.1.1/llm_atc/constants.py
--rw-r--r--   0        0        0     2452 2023-08-01 22:09:36.921583 llm_atc-0.1.1/llm_atc/launch.py
--rw-r--r--   0        0        0     3759 2023-08-01 21:40:08.369934 llm_atc-0.1.1/llm_atc/run.py
--rw-r--r--   0        0        0     2446 2023-08-01 01:49:11.981818 llm_atc-0.1.1/llm_atc/serve.py
--rw-r--r--   0        0        0      414 2023-08-01 22:09:36.927527 llm_atc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 llm_atc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4338 2023-08-03 11:17:53.028125 llm_atc-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 22:09:36.927039 llm_atc-0.1.2/llm_atc/__init__.py
+-rw-r--r--   0        0        0     5859 2023-08-01 21:43:53.652173 llm_atc-0.1.2/llm_atc/cli.py
+-rw-r--r--   0        0        0     2044 2023-08-03 11:17:53.034566 llm_atc-0.1.2/llm_atc/config/serve/serve.yml
+-rw-r--r--   0        0        0     3310 2023-08-01 22:05:13.864460 llm_atc-0.1.2/llm_atc/config/train/vicuna.yml
+-rw-r--r--   0        0        0      260 2023-07-31 02:19:45.084926 llm_atc-0.1.2/llm_atc/constants.py
+-rw-r--r--   0        0        0     2452 2023-08-01 22:09:36.921583 llm_atc-0.1.2/llm_atc/launch.py
+-rw-r--r--   0        0        0     3759 2023-08-01 21:40:08.369934 llm_atc-0.1.2/llm_atc/run.py
+-rw-r--r--   0        0        0     2389 2023-08-03 11:17:53.034816 llm_atc-0.1.2/llm_atc/serve.py
+-rw-r--r--   0        0        0      414 2023-08-03 11:17:53.034996 llm_atc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 llm_atc-0.1.2/PKG-INFO
```

### Comparing `llm_atc-0.1.1/llm_atc/cli.py` & `llm_atc-0.1.2/llm_atc/cli.py`

 * *Files identical despite different names*

### Comparing `llm_atc-0.1.1/llm_atc/config/serve/serve.yml` & `llm_atc-0.1.2/llm_atc/config/serve/serve.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 resources:
   accelerators: A100:1
   disk_size: 1024
-  disk_tier: high
 
 file_mounts:
   /llm-atc:
     name: llm-atc # Make sure it is unique or you own this bucket name
     mode: MOUNT  # MOUNT or COPY. Defaults to MOUNT if not specified
 
 setup: |
@@ -15,14 +14,15 @@
     conda activate chatbot
   fi
 
   # Install dependencies
   pip install vllm
   pip install git+https://github.com/lm-sys/FastChat.git
   pip install --upgrade openai
+  pip install ray==2.5.1
   sudo apt update
   sudo apt install -y rclone
 
 
 run: |
 
   master_addr=`echo "$SKYPILOT_NODE_IPS" | head -n1`
```

### Comparing `llm_atc-0.1.1/llm_atc/config/train/vicuna.yml` & `llm_atc-0.1.2/llm_atc/config/train/vicuna.yml`

 * *Files identical despite different names*

### Comparing `llm_atc-0.1.1/llm_atc/launch.py` & `llm_atc-0.1.2/llm_atc/launch.py`

 * *Files identical despite different names*

### Comparing `llm_atc-0.1.1/llm_atc/run.py` & `llm_atc-0.1.2/llm_atc/run.py`

 * *Files identical despite different names*

### Comparing `llm_atc-0.1.1/llm_atc/serve.py` & `llm_atc-0.1.2/llm_atc/serve.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import os
 import sky
 import sys
 
 from llm_atc.launch import SUPPORTED_MODELS
 from llm_atc.run import RunTracker
-from sky.data.storage import StoreType, get_store_prefix
 from typing import Any, Dict, List, Optional, Union
 
 
 def serve_route(model_names: List[str], **serve_kwargs):
     """Routes model serve requests to the corresponding model serve config
 
     Args:
```

### Comparing `llm_atc-0.1.1/PKG-INFO` & `llm_atc-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,27 @@
-Metadata-Version: 2.1
-Name: llm-atc
-Version: 0.1.1
-Summary: 
-Author: Andrew Aikawa
-Author-email: asai@berkeley.edu
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.6,<9.0.0)
-Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
-Requires-Dist: posthog (>=3.0.1,<4.0.0)
-Requires-Dist: prettytable (>=3.8.0,<4.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Description-Content-Type: text/markdown
-
 <p align="center">
   <img height='100px' src="https://www.ocf.berkeley.edu/~asai/static/images/trainy.png">
 </p>
 
 ![GitHub Repo stars](https://img.shields.io/github/stars/Trainy-ai/llm-atc?style=social)
 [![](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/TrainyAI)
 [![](https://dcbadge.vercel.app/api/server/d67CMuKY5V)](https://discord.gg/d67CMuKY5V)
 
-LLM-ATC (**A**ir **T**raffic **C**ontroller) is a CLI for fine tuning and serving open source models using your own cloud credentials. We hope that this project can lower the cognitive overhead orchestration for fine tuning and model serving.
+LLM-ATC (**A**ir **T**raffic **C**ontroller) is a CLI for fine tuning and serving open source models using your own cloud credentials. We hope that this project can lower the cognitive overhead of orchestration for fine tuning and model serving.
 
 ## Installation
 
-Follow the instructions here (to install Skypilot and provide cloud credentials)[https://skypilot.readthedocs.io/en/latest/getting-started/installation.html]. We use Skypilot for cloud orchestration. Steps to create an environment from source is shown below.
+Follow the instructions here [to install Skypilot and provide cloud credentials](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html). We use Skypilot for cloud orchestration. Steps to setup an environment is shown below.
 
 ```
 # create a fresh environment
 conda create -n "llm-atc" python=3.10
+conda activate sky
 
-# For Macs, macOS >= 10.15 is required to install SkyPilot. Apple Silicon-based devices (e.g. Apple M1)
+# For Macs, macOS >= 10.15 is required to install SkyPilot. For Apple Silicon-based devices (e.g. Apple M1)
 pip uninstall grpcio; conda install -c conda-forge grpcio=1.43.0
 
 # install the skypilot cli and dependency, for the clouds you want, e.g. GCP
 pip install skypilot[gcp] # for aws, skypilot[aws]
 
 
 # Configure your cloud credentials. This is a GCP example. See https://skypilot.readthedocs.io/en/latest/getting-started/ installation.html for examples with other cloud providers.
@@ -73,23 +57,43 @@
 
 If your client disconnects from the train, the train run will continue. You can check it's status with `sky queue mycluster`
 
 When training completes, by default, your model, will be saved to an object store corresponding to the cloud provider which launched the training instance. For instance,
 
 ```
 # s3 location
-s3://llm-atc/vicuna_test
+s3://llm-atc/myvicuna
 # gcp location
-g3://llm-atc/vicuna_test
+g3://llm-atc/myvicuna
 ```
 
 ## Serving
 
-`llm-atc` can serve both models from HuggingFace or that you've trained through `llm-atc` 
+`llm-atc` can serve both models from HuggingFace or that you've trained through `llm-atc serve`. For example
+
+```
+# serve an llm-atc finetuned model, requires `llm-atc/` prefix and grabs model checkpoint from object store
+llm-atc serve --name llm-atc/myvicuna --accelerator A100:1 -c serveCluster --cloud gcp --region asia-southeast1
+
+# serve a HuggingFace model, e.g. `lmsys/vicuna-13b-v1.3`
+llm-atc serve --name lmsys/vicuna-13b-v1.3 --accelerator A100:1 -c serveCluster --cloud gcp --region asia-southeast1
+```
+
+This creates a OpenAI API server on port 8000 on the cluster head and one model worker.
+Forward this port to your laptop with 
+```
+# Forward port 8000 to your localhost
+ssh -N -L 8000:localhost:8000 serveCluster
+
+# test which models are available
+curl http://localhost:8000/v1/models
+```
+and you can connect to this server and
+develop your using your finetuned models with your favorite LLM frameworks like [LangChain](https://python.langchain.com/docs/get_started/introduction.html). An example of how integrate Langchain (through Fastchat) is linked [here](https://github.com/lm-sys/FastChat/blob/main/docs/langchain_integration.md). **Example with ATC coming soon**
+
 
 ## How does it work?
 
-Training, serving, and orchestration are powered by [SkyPilot](https://github.com/skypilot-org/skypilot) and [FastChat](https://github.com/lm-sys/FastChat/). We've made this decision since we believe this will allow people to train and deploy custom LLMs without cloud-lockin.
+Training, serving, and orchestration are powered by [SkyPilot](https://github.com/skypilot-org/skypilot), [FastChat](https://github.com/lm-sys/FastChat/), and [vLLM](https://github.com/vllm-project/vllm). We've made this decision since we believe this will allow people to train and deploy custom LLMs without cloud-lockin.
 
 We currently rely on default hyperparameters from other training code repositories, but we will add options to overwrite these so that users have more control over training, but for now, we think the defaults should suffice for most use cases. 
 
-
```

