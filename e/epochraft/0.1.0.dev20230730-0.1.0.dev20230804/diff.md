# Comparing `tmp/epochraft-0.1.0.dev20230730.tar.gz` & `tmp/epochraft-0.1.0.dev20230804.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epochraft-0.1.0.dev20230730.tar", last modified: Sun Jul 30 13:07:36 2023, max compression
+gzip compressed data, was "epochraft-0.1.0.dev20230804.tar", last modified: Thu Aug  3 15:09:56 2023, max compression
```

## Comparing `epochraft-0.1.0.dev20230730.tar` & `epochraft-0.1.0.dev20230804.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-07-30 13:07:36.651943 epochraft-0.1.0.dev20230730/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1069 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/LICENSE
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3263 2023-07-30 13:07:36.651943 epochraft-0.1.0.dev20230730/PKG-INFO
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      801 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/README.md
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-07-30 13:07:36.647942 epochraft-0.1.0.dev20230730/epochraft/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      335 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/__init__.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3461 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/base.py
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-07-30 13:07:36.651943 epochraft-0.1.0.dev20230730/epochraft/sources/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      203 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/sources/__init__.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     2930 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/sources/mosaicml.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1951 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/sources/sequence.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3404 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/testing.py
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-07-30 13:07:36.651943 epochraft-0.1.0.dev20230730/epochraft/transforms/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      396 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/transforms/__init__.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1260 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/transforms/batch.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3138 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/transforms/concat_chunk.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1696 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/transforms/count.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      998 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/transforms/filter_map.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3271 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/epochraft/transforms/interleave.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)       33 2023-07-30 13:07:34.000000 epochraft-0.1.0.dev20230730/epochraft/version.py
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-07-30 13:07:36.651943 epochraft-0.1.0.dev20230730/epochraft.egg-info/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3263 2023-07-30 13:07:36.000000 epochraft-0.1.0.dev20230730/epochraft.egg-info/PKG-INFO
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      568 2023-07-30 13:07:36.000000 epochraft-0.1.0.dev20230730/epochraft.egg-info/SOURCES.txt
--rw-rw-r--   0 takiba    (1000) takiba    (1000)        1 2023-07-30 13:07:36.000000 epochraft-0.1.0.dev20230730/epochraft.egg-info/dependency_links.txt
--rw-rw-r--   0 takiba    (1000) takiba    (1000)       86 2023-07-30 13:07:36.000000 epochraft-0.1.0.dev20230730/epochraft.egg-info/requires.txt
--rw-rw-r--   0 takiba    (1000) takiba    (1000)       10 2023-07-30 13:07:36.000000 epochraft-0.1.0.dev20230730/epochraft.egg-info/top_level.txt
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     2066 2023-07-30 13:07:29.000000 epochraft-0.1.0.dev20230730/pyproject.toml
--rw-rw-r--   0 takiba    (1000) takiba    (1000)       38 2023-07-30 13:07:36.651943 epochraft-0.1.0.dev20230730/setup.cfg
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1069 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/LICENSE
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     3642 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/PKG-INFO
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1180 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/README.md
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      463 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     7615 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/base.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft/combinations/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      135 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/combinations/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     2202 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/combinations/concat.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     3280 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/combinations/interleave.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft/sources/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      325 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/sources/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1904 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/sources/iterable.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     2930 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/sources/mosaicml.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1951 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/sources/sequence.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     3481 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/testing.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft/transforms/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      589 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1266 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/batch.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     3435 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/concat_chunk.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1724 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/count.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      955 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/filter_map.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     7242 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/parallel_filter_map.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)       33 2023-08-03 15:09:53.000000 epochraft-0.1.0.dev20230804/epochraft/version.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft.egg-info/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     3642 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/PKG-INFO
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      712 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/SOURCES.txt
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)        1 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/dependency_links.txt
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)       99 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/requires.txt
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)       10 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/top_level.txt
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     2086 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/pyproject.toml
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)       38 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/setup.cfg
```

### Comparing `epochraft-0.1.0.dev20230730/LICENSE` & `epochraft-0.1.0.dev20230804/LICENSE`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230730/PKG-INFO` & `epochraft-0.1.0.dev20230804/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epochraft
-Version: 0.1.0.dev20230730
+Version: 0.1.0.dev20230804
 Summary: Supercharge Your LLM Training with Checkpointable Data Loading
 Author: Takuya Akiba
 Author-email: takuya.akiba@stability.ai
 License: MIT License
         
         Copyright (c) 2023 Takuya Akiba
         
@@ -47,22 +47,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: development
 License-File: LICENSE
 
 # Epochraft
 
 [![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org)
-[![pypi](https://img.shields.io/pypi/v/epochraft.svg)](https://pypi.python.org/pypi/epochraft)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/optuna/optuna)
 [![Checks status](https://github.com/iwiwi/epochraft/actions/workflows/checks.yml/badge.svg?branch=main)](https://github.com/iwiwi/epochraft/actions)
 [![Tests status](https://github.com/iwiwi/epochraft/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/iwiwi/epochraft/actions)
+[![pypi](https://img.shields.io/pypi/v/epochraft.svg)](https://pypi.python.org/pypi/epochraft)
 
 
 Supercharge your LLM training with checkpointable data loading.
 
+## Key Features
+
+* **Checkpointing** - Epochraft operates completely deterministically, and allows for a full restoration of state through checkpointing.
+* **Simple** - It's a minimally readable implementation that makes it easy for users to add sources and transforms.
+* **LLM-Ready** - It is equipped out of the box with features necessary for pre-training and SFT of LLMs.
+
+
+
 ## Development
 
 
 ```
 pip install -e .[development]
 mypy .; black .; flake8 .; isort .
 pytest tests
```

### Comparing `epochraft-0.1.0.dev20230730/epochraft/sources/mosaicml.py` & `epochraft-0.1.0.dev20230804/epochraft/sources/mosaicml.py`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230730/epochraft/sources/sequence.py` & `epochraft-0.1.0.dev20230804/epochraft/sources/sequence.py`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230730/epochraft/testing.py` & `epochraft-0.1.0.dev20230804/epochraft/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,8 +96,10 @@
     state_dict = it.state_dict()
     subsequent_samples_original = list(itertools.islice(it, n_subsequent_samples))
 
     # Resume from the state dict
     it = resuming_dataset.iter(state_dict=state_dict)
     subsequent_samples_resumed = list(itertools.islice(it, n_subsequent_samples))
 
+    print(subsequent_samples_original)
+    print(subsequent_samples_resumed)
     assert_sample_lists_equal(subsequent_samples_original, subsequent_samples_resumed)
```

### Comparing `epochraft-0.1.0.dev20230730/epochraft/transforms/batch.py` & `epochraft-0.1.0.dev20230804/epochraft/transforms/batch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Optional
 
-from ..base import CheckpointableDataset, CheckpointableIterator, CollateFnType, Sample, StateDict
+from ..base import CheckpointableDataset, CheckpointableIterator, CollateFn, Sample, StateDict
 
 
 class BatchIterator(CheckpointableIterator):
-    def __init__(self, dataset: Batch, source: CheckpointableIterator) -> None:
+    def __init__(self, dataset: BatchDataset, source: CheckpointableIterator) -> None:
         self.dataset = dataset
         self.source = source
 
     def __next__(self) -> Sample:
         batch = []
         try:
             for _ in range(self.dataset.batch_size):
@@ -21,20 +21,20 @@
 
         return self.dataset.collate_fn(batch)
 
     def state_dict(self) -> StateDict:
         return self.source.state_dict()
 
 
-class Batch(CheckpointableDataset):
+class BatchDataset(CheckpointableDataset):
     def __init__(
         self,
         source: CheckpointableDataset,
         batch_size: int,
-        collate_fn: CollateFnType,
+        collate_fn: CollateFn,
         drop_last: bool,
     ) -> None:
         self.source = source
         self.batch_size = batch_size
         self.collate_fn = collate_fn
         self.drop_last = drop_last
```

### Comparing `epochraft-0.1.0.dev20230730/epochraft/transforms/concat_chunk.py` & `epochraft-0.1.0.dev20230804/epochraft/transforms/concat_chunk.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,30 @@
         else:
             raise ValueError(f"Expected integer ndarray, got ndarray of {data.dtype}")
     else:
         tensor = torch.tensor(data, dtype=torch.long)
 
     if tensor.dtype != torch.long:
         raise ValueError(f"Expected long tensor, got {tensor.dtype}")
-    if tensor.dim() != 1:
+
+    if tensor.dim() == 2:
+        if tensor.shape[0] != 1:
+            raise ValueError(
+                "input_ids must be 1-dimensional tensor or 2-dimensional tensor with batch size 1"
+            )
+        tensor = tensor[0]
+    elif tensor.dim() != 1:
         raise ValueError("input_ids must be 1-dimensional tensor")
     return tensor
 
 
 class ConcatChunkIterator(CheckpointableIterator):
     def __init__(
         self,
-        dataset: ConcatChunk,
+        dataset: ConcatChunkDataset,
         source: CheckpointableIterator,
         buffer: Optional[torch.LongTensor],
     ) -> None:
         self.dataset = dataset
         self.source = source
         self.buffer = torch.empty((0,), dtype=torch.long) if buffer is None else buffer
 
@@ -50,27 +57,28 @@
                 [
                     self.buffer,
                     self.dataset.bos_tokens,
                     tokens,
                     self.dataset.eos_tokens,
                 ]
             )
+            print(tokens.shape, self.buffer.shape)
 
         y = self.buffer[: self.dataset.chunk_length]
         self.buffer = self.buffer[self.dataset.chunk_length :]
         return {self.dataset.column: y}
 
     def state_dict(self) -> StateDict:
         return {
             "source": self.source.state_dict(),
             "buffer": self.buffer,
         }
 
 
-class ConcatChunk(CheckpointableDataset):
+class ConcatChunkDataset(CheckpointableDataset):
     def __init__(
         self,
         source: CheckpointableDataset,
         chunk_length: int,
         column: str,
         bos_tokens: Optional[Union[int, TokenArray]],
         eos_tokens: Optional[Union[int, TokenArray]],
```

### Comparing `epochraft-0.1.0.dev20230730/epochraft/transforms/count.py` & `epochraft-0.1.0.dev20230804/epochraft/transforms/count.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from typing import Optional
 
 from ..base import CheckpointableDataset, CheckpointableIterator, Sample, StateDict
 
 
 class CountIterator(CheckpointableIterator):
-    def __init__(self, dataset: Count, source: CheckpointableIterator, start_count: int) -> None:
+    def __init__(
+        self, dataset: CountDataset, source: CheckpointableIterator, start_count: int
+    ) -> None:
         self.count = start_count
         self.dataset = dataset
         self.source = source
 
     def __next__(self) -> Sample:
         count = self.count
         self.count += 1
@@ -27,15 +29,15 @@
     def state_dict(self) -> StateDict:
         return {
             "source": self.source.state_dict(),
             "count": self.count,
         }
 
 
-class Count(CheckpointableDataset):
+class CountDataset(CheckpointableDataset):
     def __init__(
         self,
         source: CheckpointableDataset,
         count_column: Optional[str] = None,
         max_count: Optional[int] = None,
     ) -> None:
         self.source = source
```

### Comparing `epochraft-0.1.0.dev20230730/epochraft/transforms/filter_map.py` & `epochraft-0.1.0.dev20230804/epochraft/transforms/filter_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Optional
+from typing import Any, Optional
 
-from ..base import CheckpointableDataset, CheckpointableIterator, Sample, StateDict
-
-
-FilterMapFn = Callable[[Sample], Optional[Sample]]
+from ..base import CheckpointableDataset, CheckpointableIterator, FilterMapFn, Sample, StateDict
 
 
 class FilterMapIterator(CheckpointableIterator):
     def __init__(self, source: CheckpointableIterator, fn: FilterMapFn):
         self.source = source
         self.fn = fn
 
@@ -19,15 +16,15 @@
             if sample is not None:
                 return sample
 
     def state_dict(self) -> StateDict:
         return self.source.state_dict()
 
 
-class FilterMap(CheckpointableDataset):
+class FilterMapDataset(CheckpointableDataset):
     def __init__(self, source: CheckpointableDataset, fn: FilterMapFn):
         self.source = source
         self.fn = fn
 
     def iter(self, state_dict: Optional[dict[str, Any]] = None) -> CheckpointableIterator:
         iter = self.source.iter(state_dict=state_dict)
         return FilterMapIterator(iter, self.fn)
```

### Comparing `epochraft-0.1.0.dev20230730/epochraft/transforms/interleave.py` & `epochraft-0.1.0.dev20230804/epochraft/combinations/interleave.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,13 +85,13 @@
         iters = [
             source.iter(state_dict=state_dict)
             for source, state_dict in zip(self.sources, source_state_dicts)
         ]
         return InterleaveIterator(self, iters, start_index=index)
 
 
-def interleave(
+def interleave_datasets(
     sources: list[CheckpointableDataset],
     weights: Optional[list[float]] = None,
     chunk_size: int = 1024,
 ) -> CheckpointableDataset:
     return Interleave(sources, weights, chunk_size=chunk_size)
```

### Comparing `epochraft-0.1.0.dev20230730/epochraft.egg-info/PKG-INFO` & `epochraft-0.1.0.dev20230804/epochraft.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epochraft
-Version: 0.1.0.dev20230730
+Version: 0.1.0.dev20230804
 Summary: Supercharge Your LLM Training with Checkpointable Data Loading
 Author: Takuya Akiba
 Author-email: takuya.akiba@stability.ai
 License: MIT License
         
         Copyright (c) 2023 Takuya Akiba
         
@@ -47,22 +47,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: development
 License-File: LICENSE
 
 # Epochraft
 
 [![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org)
-[![pypi](https://img.shields.io/pypi/v/epochraft.svg)](https://pypi.python.org/pypi/epochraft)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/optuna/optuna)
 [![Checks status](https://github.com/iwiwi/epochraft/actions/workflows/checks.yml/badge.svg?branch=main)](https://github.com/iwiwi/epochraft/actions)
 [![Tests status](https://github.com/iwiwi/epochraft/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/iwiwi/epochraft/actions)
+[![pypi](https://img.shields.io/pypi/v/epochraft.svg)](https://pypi.python.org/pypi/epochraft)
 
 
 Supercharge your LLM training with checkpointable data loading.
 
+## Key Features
+
+* **Checkpointing** - Epochraft operates completely deterministically, and allows for a full restoration of state through checkpointing.
+* **Simple** - It's a minimally readable implementation that makes it easy for users to add sources and transforms.
+* **LLM-Ready** - It is equipped out of the box with features necessary for pre-training and SFT of LLMs.
+
+
+
 ## Development
 
 
 ```
 pip install -e .[development]
 mypy .; black .; flake8 .; isort .
 pytest tests
```

### Comparing `epochraft-0.1.0.dev20230730/pyproject.toml` & `epochraft-0.1.0.dev20230804/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "black",
     "blackdoc",
     "flake8",
     "isort",
     "mypy",
     "pytest",
     "mosaicml-streaming",
+    "transformers",
 ]
 
 [project.urls]
 repository = "https://github.com/iwiwi/epochraft"
 
 [tool.setuptools.packages.find]
 include = ["epochraft*"]
```

