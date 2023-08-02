# Comparing `tmp/spice_agent-0.1.8.tar.gz` & `tmp/spice_agent-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_agent-0.1.8.tar", max compression
+gzip compressed data, was "spice_agent-0.1.9.tar", max compression
```

## Comparing `spice_agent-0.1.8.tar` & `spice_agent-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1921 2023-07-27 00:18:38.620121 spice_agent-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/__init__.py
--rw-r--r--   0        0        0       22 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/__version__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/auth/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/auth/actions.py
--rw-r--r--   0        0        0     2976 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/auth/commands.py
--rw-r--r--   0        0        0     1869 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/cli.py
--rw-r--r--   0        0        0     5039 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/client.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/__init__.py
--rw-r--r--   0        0        0     2500 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/actions.py
--rw-r--r--   0        0        0     1508 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/commands.py
--rw-r--r--   0        0        0     4302 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/launch_agents.py
--rw-r--r--   0        0        0     4982 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/daemons/launch_service.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/graphql/documents/__init__.py
--rw-r--r--   0        0        0     1196 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/graphql/documents/authentication.gql
--rw-r--r--   0        0        0     1504 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/graphql/sdk.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/hardware/__init__.py
--rw-r--r--   0        0        0     7954 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/hardware/actions.py
--rw-r--r--   0        0        0     1070 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/hardware/commands.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/inference/__init__.py
--rw-r--r--   0        0        0     6884 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/inference/actions.py
--rw-r--r--   0        0        0     1055 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/inference/commands.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/tests/__init__.py
--rw-r--r--   0        0        0      555 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/tests/test_version.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/training/__init__.py
--rw-r--r--   0        0        0    41859 2023-07-27 00:18:38.620121 spice_agent-0.1.8/spice_agent/training/actions.py
--rw-r--r--   0        0        0       97 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/training/commands.py
--rw-r--r--   0        0        0     7269 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/uploader/actions.py
--rw-r--r--   0        0        0     1907 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/utils/config.py
--rw-r--r--   0        0        0      252 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/utils/printer.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/utils/updates.py
--rw-r--r--   0        0        0     1788 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/utils/version.py
--rw-r--r--   0        0        0        0 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/worker/__init__.py
--rw-r--r--   0        0        0     9500 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/worker/actions.py
--rw-r--r--   0        0        0      397 2023-07-27 00:18:38.624121 spice_agent-0.1.8/spice_agent/worker/commands.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1952 2023-07-29 01:53:03.594931 spice_agent-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/auth/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/auth/actions.py
+-rw-r--r--   0        0        0     2976 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/auth/commands.py
+-rw-r--r--   0        0        0     1869 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/cli.py
+-rw-r--r--   0        0        0     5039 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/client.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/daemons/__init__.py
+-rw-r--r--   0        0        0     2500 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/daemons/actions.py
+-rw-r--r--   0        0        0     1508 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/daemons/commands.py
+-rw-r--r--   0        0        0     4302 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/daemons/launch_agents.py
+-rw-r--r--   0        0        0     4982 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/daemons/launch_service.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/graphql/documents/__init__.py
+-rw-r--r--   0        0        0     1196 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/graphql/documents/authentication.gql
+-rw-r--r--   0        0        0     1504 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/graphql/sdk.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/hardware/__init__.py
+-rw-r--r--   0        0        0     7954 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/hardware/actions.py
+-rw-r--r--   0        0        0     1070 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/hardware/commands.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/inference/__init__.py
+-rw-r--r--   0        0        0     9002 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/inference/actions.py
+-rw-r--r--   0        0        0     1055 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/inference/commands.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/tests/__init__.py
+-rw-r--r--   0        0        0      555 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/tests/test_version.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/training/__init__.py
+-rw-r--r--   0        0        0    41859 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/training/actions.py
+-rw-r--r--   0        0        0       97 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/training/commands.py
+-rw-r--r--   0        0        0     7269 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/uploader/actions.py
+-rw-r--r--   0        0        0     1907 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/utils/config.py
+-rw-r--r--   0        0        0      252 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/utils/printer.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/utils/updates.py
+-rw-r--r--   0        0        0     1788 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/utils/version.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/worker/__init__.py
+-rw-r--r--   0        0        0     9500 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/worker/actions.py
+-rw-r--r--   0        0        0      397 2023-07-29 01:53:03.594931 spice_agent-0.1.9/spice_agent/worker/commands.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 spice_agent-0.1.9/PKG-INFO
```

### Comparing `spice_agent-0.1.8/pyproject.toml` & `spice_agent-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_agent"
-version = "0.1.8"
+version = "0.1.9"
 description = "spice agent"
 authors = ["Dylan Stein <dylan@spice.cloud>", "Ankush Patel <ankush@spice.cloud>"]
 license = ""
 
 [tool.poetry.dependencies]
 python = "^3.11.3"
 gql = "^3.4.1"
@@ -19,16 +19,17 @@
 sentry-sdk = "^1.24.0"
 datasets = "^2.13.1"
 boto3 = "^1.26.165"
 evaluate = "^0.4.0"
 scikit-learn = "^1.2.2"
 accelerate = "^0.20.3"
 torchvision = "^0.15.2"
-diffusers = "^0.17.1"
+diffusers = "^0.18.0"
 outdated = "^0.2.2"
+invisible-watermark = "^0.2.0"
 
 [tool.poetry.dev-dependencies]
 ruff = "^0.0.275"
 black = "^23.3.0"
 prospector = "^1.10.2"
 ipython = "^8.9.0"
 ipdb = "^0.13.11"
```

### Comparing `spice_agent-0.1.8/spice_agent/auth/actions.py` & `spice_agent-0.1.9/spice_agent/auth/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/auth/commands.py` & `spice_agent-0.1.9/spice_agent/auth/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/cli.py` & `spice_agent-0.1.9/spice_agent/cli.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/client.py` & `spice_agent-0.1.9/spice_agent/client.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/daemons/actions.py` & `spice_agent-0.1.9/spice_agent/daemons/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/daemons/commands.py` & `spice_agent-0.1.9/spice_agent/daemons/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/daemons/launch_agents.py` & `spice_agent-0.1.9/spice_agent/daemons/launch_agents.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/daemons/launch_service.py` & `spice_agent-0.1.9/spice_agent/daemons/launch_service.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/graphql/documents/authentication.gql` & `spice_agent-0.1.9/spice_agent/graphql/documents/authentication.gql`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/graphql/sdk.py` & `spice_agent-0.1.9/spice_agent/graphql/sdk.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/hardware/actions.py` & `spice_agent-0.1.9/spice_agent/hardware/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/hardware/commands.py` & `spice_agent-0.1.9/spice_agent/hardware/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/inference/actions.py` & `spice_agent-0.1.9/spice_agent/inference/actions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import json
 import logging
 import os
 from pathlib import Path
 from typing import Dict, Optional
 
-from diffusers import StableDiffusionPipeline
+from diffusers import (
+    DiffusionPipeline,
+    StableDiffusionXLPipeline,
+    StableDiffusionXLImg2ImgPipeline,
+)
 from gql import gql
 from gql.transport.exceptions import TransportQueryError
 from torch.mps import empty_cache as mps_empty_cache
 
 from spice_agent.utils.config import SPICE_INFERENCE_DIRECTORY
 
 os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
@@ -142,23 +146,66 @@
                     text_output=json.dumps(result),
                 )
             elif is_text_input and is_file_output:
                 SPICE_INFERENCE_DIRECTORY.mkdir(parents=True, exist_ok=True)
                 save_at = Path(SPICE_INFERENCE_DIRECTORY / f"{inference_job_id}.png")
                 was_guarded = False
                 if not save_at.exists():
-                    pipe = StableDiffusionPipeline.from_pretrained(
-                        model_repo_id, torch_dtype=torch.float32
+                    pipe = DiffusionPipeline.from_pretrained(
+                        model_repo_id,
+                        torch_dtype=torch.float16,
+                        variant="fp16",
+                        use_safetensors=True,
                     )
                     pipe = pipe.to(self.device)  # type: ignore
-                    pipe_result = pipe(text_input, return_dict=True)  # type: ignore
-                    result = pipe_result.images[0]  # type: ignore
-                    if pipe_result.nsfw_content_detected:  # type: ignore
-                        was_guarded = pipe_result.nsfw_content_detected[0]  # type: ignore # noqa
-                    result.save(save_at)
+
+                    # Configure MOE for xl diffusion base + refinement
+                    if (
+                        isinstance(pipe, StableDiffusionXLPipeline)
+                        and "stabilityai/stable-diffusion-xl-base-1.0"
+                    ):
+                        # arguments
+                        refiner = StableDiffusionXLImg2ImgPipeline.from_pretrained(
+                            "stabilityai/stable-diffusion-xl-refiner-1.0",
+                            text_encoder_2=pipe.text_encoder_2,
+                            vae=pipe.vae,
+                            torch_dtype=torch.float16,
+                            variant="fp16",
+                            use_safetensors=True,
+                        )
+
+                        refiner = refiner.to(self.device)
+
+                        latents = pipe(
+                            prompt=text_input,
+                            # negative_prompt=negative_prompt,
+                            # num_images_per_prompt=num_images_per_prompt,
+                            # num_inference_steps=n_steps,
+                            output_type="latent",
+                        ).images  # type: ignore
+
+                        pipe_result = refiner(
+                            prompt=text_input,
+                            # negative_prompt=negative_prompt,
+                            # num_images_per_prompt=num_images_per_prompt,
+                            # num_inference_steps=n_steps,
+                            image=latents,  # type: ignore
+                        )  # type: ignore
+                    else:
+                        pipe_result = pipe(text_input, return_dict=False)  # type:ignore
+
+                    # pipe returns a tuple in the form the first element is a list with
+                    # the generated images, and the second element is a list of `bool`s
+                    # denoting whether the corresponding generated image likely
+                    # represents "not-safe-for-work" (nsfw) content, according to the
+                    # `safety_checker`.
+                    result = pipe_result[0][0]  # type: ignore
+                    if len(pipe_result) > 1:
+                        was_guarded = pipe_result[1][0]  # type: ignore
+                    result.save(save_at)  # type: ignore
                 else:
                     LOGGER.info(f""" [*] File already exists at: {save_at}""")
 
                 upload_file_response = self.spice.uploader.upload_file_via_api(
                     path=save_at
                 )
                 file_id = upload_file_response.json()["data"]["uploadFile"]["id"]
```

### Comparing `spice_agent-0.1.8/spice_agent/inference/commands.py` & `spice_agent-0.1.9/spice_agent/inference/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/tests/test_version.py` & `spice_agent-0.1.9/spice_agent/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/training/actions.py` & `spice_agent-0.1.9/spice_agent/training/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/uploader/actions.py` & `spice_agent-0.1.9/spice_agent/uploader/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/utils/config.py` & `spice_agent-0.1.9/spice_agent/utils/config.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/utils/version.py` & `spice_agent-0.1.9/spice_agent/utils/version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/spice_agent/worker/actions.py` & `spice_agent-0.1.9/spice_agent/worker/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.8/PKG-INFO` & `spice_agent-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: spice-agent
-Version: 0.1.8
+Version: 0.1.9
 Summary: spice agent
 Author: Dylan Stein
 Author-email: dylan@spice.cloud
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: boto3 (>=1.26.165,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: datasets (>=2.13.1,<3.0.0)
-Requires-Dist: diffusers (>=0.17.1,<0.18.0)
+Requires-Dist: diffusers (>=0.18.0,<0.19.0)
 Requires-Dist: evaluate (>=0.4.0,<0.5.0)
 Requires-Dist: gql (>=3.4.1,<4.0.0)
+Requires-Dist: invisible-watermark (>=0.2.0,<0.3.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: outdated (>=0.2.2,<0.3.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: sentry-sdk (>=1.24.0,<2.0.0)
```

