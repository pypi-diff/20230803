# Comparing `tmp/grouped_query_attention_pytorch-0.1.0rc2.tar.gz` & `tmp/grouped_query_attention_pytorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grouped_query_attention_pytorch-0.1.0rc2.tar", last modified: Tue Aug  1 01:57:57 2023, max compression
+gzip compressed data, was "grouped_query_attention_pytorch-0.2.0.tar", last modified: Thu Aug  3 00:46:07 2023, max compression
```

## Comparing `grouped_query_attention_pytorch-0.1.0rc2.tar` & `grouped_query_attention_pytorch-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.172505 grouped_query_attention_pytorch-0.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.164504 grouped_query_attention_pytorch-0.1.0rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-08-01 01:57:57.172505 grouped_query_attention_pytorch-0.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   335190 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/doc/attention.png
--rw-r--r--   0 runner    (1001) docker     (123)    37835 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_attention.png
--rw-r--r--   0 runner    (1001) docker     (123)    37657 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_t5.png
--rw-r--r--   0 runner    (1001) docker     (123)   118342 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_t5_original.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/utils/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/scripts/benchmark_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/scripts/benchmark_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:57:57.172505 grouped_query_attention_pytorch-0.1.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.172505 grouped_query_attention_pytorch-0.1.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/test_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.959612 grouped_query_attention_pytorch-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-03 00:46:07.959612 grouped_query_attention_pytorch-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)   335190 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/doc/attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37835 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/doc/benchmark_attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37657 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/doc/benchmark_t5.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118342 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/doc/benchmark_t5_original.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/utils/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/scripts/benchmark_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/scripts/benchmark_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:46:07.959612 grouped_query_attention_pytorch-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.959612 grouped_query_attention_pytorch-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/test_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/test_transformer.py
```

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/publish.yaml` & `grouped_query_attention_pytorch-0.2.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/test.yaml` & `grouped_query_attention_pytorch-0.2.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/.gitignore` & `grouped_query_attention_pytorch-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/LICENSE` & `grouped_query_attention_pytorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/PKG-INFO` & `grouped_query_attention_pytorch-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grouped_query_attention_pytorch
-Version: 0.1.0rc2
+Version: 0.2.0
 Summary: grouped-query-attention-pytorch
 Author-email: Frank Odom <frank.odom.iii@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/README.md` & `grouped_query_attention_pytorch-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/doc/attention.png` & `grouped_query_attention_pytorch-0.2.0/doc/attention.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_attention.png` & `grouped_query_attention_pytorch-0.2.0/doc/benchmark_attention.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_t5.png` & `grouped_query_attention_pytorch-0.2.0/doc/benchmark_t5.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_t5_original.png` & `grouped_query_attention_pytorch-0.2.0/doc/benchmark_t5_original.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/attention.py` & `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/t5.py` & `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/transformer.py` & `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from enum import Enum
 from math import log
 from typing import Callable, Optional, Union
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
 from torch.nn.modules.transformer import _get_activation_fn
@@ -71,30 +70,33 @@
         # The 'MultiheadGQA' module uses ths same initialization,
         # so we just need to worry about the 'Linear' modules here.
         nn.init.xavier_normal_(self.linear1.weight, gain=self.gamma_init)
         nn.init.constant_(self.linear1.bias, 0)
         nn.init.xavier_normal_(self.linear2.weight, gain=self.gamma_init)
         nn.init.constant_(self.linear2.bias, 0)
 
-    def forward(self, src: Tensor, is_causal: bool = False) -> Tensor:
-        x = src
-
-        # Self-attention block
+    def _self_attention_block(self, x: Tensor, is_causal: bool = False) -> Tensor:
         x = self.norm1(x)
         x, _ = self.self_attn(x, x, x, is_causal=is_causal)
         x = self.dropout(x)
+        return x
 
-        # Feedforward block
+    def _feedforward_block(self, x: Tensor) -> Tensor:
         x = self.norm2(x)
         x = self.activation(self.linear1(x))
         x = self.dropout(x)
         x = self.norm3(x)
         x = self.linear2(x)
         x = self.dropout(x)
+        return x
 
+    def forward(self, src: Tensor, is_causal: bool = False) -> Tensor:
+        x = src
+        x = x + self._self_attention_block(x, is_causal=is_causal)
+        x = x + self._feedforward_block(x)
         return x
 
 
 class GQATransformerDecoderLayer(nn.Module):
     # NOTE: Mostly pulled from 'nn.TransformerDecoderLayer', but with changes:
     #   - use sub-LayerNorm like in MAGNETO. See: https://arxiv.org/abs/2210.06423
     #   - use MultiheadGQA instead of MultiheadAttention
@@ -167,41 +169,48 @@
         # The 'MultiheadGQA' module uses ths same initialization,
         # so we just need to worry about the 'Linear' modules here.
         nn.init.xavier_normal_(self.linear1.weight, gain=self.gamma_init)
         nn.init.constant_(self.linear1.bias, 0)
         nn.init.xavier_normal_(self.linear2.weight, gain=self.gamma_init)
         nn.init.constant_(self.linear2.bias, 0)
 
-    def forward(
-        self,
-        tgt: Tensor,
-        memory: Tensor,
-        tgt_is_causal: bool = False,
-        memory_is_causal: bool = False,
-    ) -> Tensor:
-        x = tgt
-
-        # Self-attention block
+    def _self_attention_block(self, x: Tensor, is_causal: bool = False) -> Tensor:
         x = self.norm1(x)
-        x, _ = self.self_attn(x, x, x, is_causal=tgt_is_causal)
+        x, _ = self.self_attn(x, x, x, is_causal=is_causal)
         x = self.dropout(x)
+        return x
 
-        # Multihead attention block
+    def _multihead_attention_block(
+        self, x: Tensor, memory: Tensor, is_causal: bool = False
+    ) -> Tensor:
         x = self.norm2(x)
-        x, _ = self.multihead_attn(x, memory, memory, is_causal=memory_is_causal)
+        x, _ = self.multihead_attn(x, memory, memory, is_causal=is_causal)
         x = self.dropout(x)
+        return x
 
-        # Feedforward block
+    def _feedforward_block(self, x: Tensor) -> Tensor:
         x = self.norm3(x)
         x = self.activation(self.linear1(x))
         x = self.dropout(x)
         x = self.norm4(x)
         x = self.linear2(x)
         x = self.dropout(x)
+        return x
 
+    def forward(
+        self,
+        tgt: Tensor,
+        memory: Tensor,
+        tgt_is_causal: bool = False,
+        memory_is_causal: bool = False,
+    ) -> Tensor:
+        x = tgt
+        x = x + self._self_attention_block(x, is_causal=tgt_is_causal)
+        x = x + self._multihead_attention_block(x, memory, is_causal=memory_is_causal)
+        x = x + self._feedforward_block(x)
         return x
 
 
 class GQATransformer(nn.Module):
     def __init__(
         self,
         d_model: int = 512,
@@ -277,18 +286,14 @@
             tgt = layer(tgt, mem, memory_is_causal=is_causal, tgt_is_causal=is_causal)
         if self.decoder.norm is not None:
             tgt = self.decoder.norm(tgt)
 
         return tgt
 
 
-class PositionalEncoding(str, Enum):
-    XPOS = "xpos"
-
-
 class GQATransformerLM(nn.Module):
     def __init__(
         self,
         num_tokens: int,  # (required) usually obtained from the tokenizer
         d_model: int = 512,
         nhead: int = 8,
         kv_heads: int = 4,
```

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/utils/benchmark.py` & `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/PKG-INFO` & `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grouped-query-attention-pytorch
-Version: 0.1.0rc2
+Version: 0.2.0
 Summary: grouped-query-attention-pytorch
 Author-email: Frank Odom <frank.odom.iii@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/SOURCES.txt` & `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .coveragerc
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
+.github/FUNDING.yml
 .github/workflows/publish.yaml
 .github/workflows/test.yaml
 doc/attention.png
 doc/benchmark_attention.png
 doc/benchmark_t5.png
 doc/benchmark_t5_original.png
 grouped_query_attention_pytorch/__init__.py
```

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/pyproject.toml` & `grouped_query_attention_pytorch-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/scripts/README.md` & `grouped_query_attention_pytorch-0.2.0/scripts/README.md`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/scripts/benchmark_attention.py` & `grouped_query_attention_pytorch-0.2.0/scripts/benchmark_attention.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/scripts/benchmark_t5.py` & `grouped_query_attention_pytorch-0.2.0/scripts/benchmark_t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/tests/conftest.py` & `grouped_query_attention_pytorch-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/tests/test_attention.py` & `grouped_query_attention_pytorch-0.2.0/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/tests/test_t5.py` & `grouped_query_attention_pytorch-0.2.0/tests/test_t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0rc2/tests/test_transformer.py` & `grouped_query_attention_pytorch-0.2.0/tests/test_transformer.py`

 * *Files identical despite different names*

