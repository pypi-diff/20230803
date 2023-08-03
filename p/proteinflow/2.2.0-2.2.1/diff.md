# Comparing `tmp/proteinflow-2.2.0.tar.gz` & `tmp/proteinflow-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-2.2.0.tar", last modified: Wed Aug  2 14:26:43 2023, max compression
+gzip compressed data, was "proteinflow-2.2.1.tar", last modified: Thu Aug  3 16:32:24 2023, max compression
```

## Comparing `proteinflow-2.2.0.tar` & `proteinflow-2.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-02 14:26:29.000000 proteinflow-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-02 14:26:43.440483 proteinflow-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-08-02 14:26:29.000000 proteinflow-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.436483 proteinflow-2.2.0/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 14:26:29.000000 proteinflow-2.2.0/dev/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:26:29.000000 proteinflow-2.2.0/dev/update_init_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    28157 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)    74235 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41886 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/data/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/download/
--rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/download/boto.py
--rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/ligand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/split/
--rw-r--r--   0 runner    (1001) docker     (123)    50801 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/split/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-02 14:26:29.000000 proteinflow-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 14:26:43.444483 proteinflow-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_ligands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 16:32:10.000000 proteinflow-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-03 16:32:24.854595 proteinflow-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-08-03 16:32:10.000000 proteinflow-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 16:32:10.000000 proteinflow-2.2.1/dev/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 16:32:10.000000 proteinflow-2.2.1/dev/update_init_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    28157 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/proteinflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    74235 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43477 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/data/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/proteinflow/download/
+-rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/download/boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/ligand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/proteinflow/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/proteinflow/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/proteinflow/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/proteinflow/split/
+-rw-r--r--   0 runner    (1001) docker     (123)    50805 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/split/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-03 16:32:10.000000 proteinflow-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-03 16:32:24.854595 proteinflow-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_ligands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_sabdab.py
```

### Comparing `proteinflow-2.2.0/LICENSE` & `proteinflow-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/PKG-INFO` & `proteinflow-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.2.0
+Version: 2.2.1
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.2.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.2.1 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.2.0/README.md` & `proteinflow-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/dev/bump_version.py` & `proteinflow-2.2.1/dev/bump_version.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/dev/update_init_docs.py` & `proteinflow-2.2.1/dev/update_init_docs.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/__init__.py` & `proteinflow-2.2.1/proteinflow/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/cli.py` & `proteinflow-2.2.1/proteinflow/cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/constants.py` & `proteinflow-2.2.1/proteinflow/constants.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/data/__init__.py` & `proteinflow-2.2.1/proteinflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/data/torch.py` & `proteinflow-2.2.1/proteinflow/data/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Subclasses of `torch.utils.data.Dataset` and `torch.utils.data.DataLoader` that are tuned for loading proteinflow data."""
 import os
 import pickle
 import random
 from collections import defaultdict
 from copy import deepcopy
-from itertools import combinations
+from itertools import combinations, groupby
+from operator import itemgetter
 
 import numpy as np
 import torch
 from p_tqdm import p_map
 from torch.utils.data import DataLoader, Dataset
 from tqdm import tqdm
 
@@ -354,14 +355,21 @@
             from a polymer is sampled, the center of the masked region will be forced to be in a binding site (in PDB datasets)
         mask_all_cdrs : bool, default False
             if `True`, all CDRs will be masked (in SAbDab datasets)
         load_ligands : bool, default False
             if `True`, the ligands will be loaded as well
         pyg_graph : bool, default False
             if `True`, the output will be a `torch_geometric.data.Data` object instead of a dictionary
+        patch_around_mask : bool, default False
+            if `True`, the data entries will be cut around the masked region
+        initial_patch_size : int, default 128
+            the size of the initial patch (used if `patch_around_mask` is `True`)
+        antigen_patch_size : int, default 128
+            the size of the antigen patch (used if `patch_around_mask` is `True` and the dataset is SAbDab)
+
         """
         alphabet = ALPHABET
         self.alphabet_dict = defaultdict(lambda: 0)
         for i, letter in enumerate(alphabet):
             self.alphabet_dict[letter] = i
         self.alphabet_dict["X"] = 0
         self.files = defaultdict(lambda: defaultdict(list))  # file path by biounit id
@@ -606,15 +614,14 @@
                     non_zero = torch.where(data["mask"][chain_bool])[0]
                     res_i = non_zero[random.randint(0, len(non_zero) - 1)]
                 res_coords = data["X"][res_i, 2, :]
                 neighbor_indices = torch.where(data["mask"][chain_bool])[0]
                 if self.mask_frac is not None:
                     assert self.mask_frac > 0 and self.mask_frac < 1
                     k = int(len(neighbor_indices) * self.mask_frac)
-                    k = max(k, 10)
                 else:
                     up = min(
                         self.upper_limit, int(len(neighbor_indices) * 0.5)
                     )  # do not mask more than half of the sequence
                     low = min(up - 1, self.lower_limit)
                     k = random.choice(range(low, up))
                 dist = torch.norm(
@@ -801,60 +808,92 @@
                         if chain.split("__")[1] == cdr:
                             add = True
                             break
                     if add:
                         self.indices.append(i)
 
     def _to_pyg_graph(self, data):
+        """Convert a dictionary of data to a PyTorch Geometric graph."""
         from torch_geometric.data import Data
 
         pyg_data = Data(x=data["X"])
         for key, value in data.items():
             pyg_data[key] = value.unsqueeze(0)
         return pyg_data
 
-    def _get_anchor_ind(self, data):
-        masked_ind = torch.where(data["masked_res"].bool())[0]
-        known_ind = torch.where(data["mask"].bool())[0]
-        start, end = masked_ind[0], masked_ind[-1]
-        start = known_ind[known_ind < start][-1]
-        end = known_ind[known_ind > end][0]
-        return start, end
+    @staticmethod
+    def get_anchor_ind(masked_res, mask):
+        """Get the indices of the anchor residues.
+
+        Anchor residues are defined as the first and last known residues before and
+        after each continuous masked region.
+
+        Parameters
+        ----------
+        masked_res : torch.Tensor
+            A boolean tensor indicating which residues should be predicted
+        mask : torch.Tensor
+            A boolean tensor indicating which residues are known
+
+        Returns
+        -------
+        list
+            A list of indices of the anchor residues
+
+        """
+        anchor_ind = []
+        masked_ind = torch.where(masked_res.bool())[0]
+        known_ind = torch.where(mask.bool())[0]
+        for _, g in groupby(enumerate(masked_ind), lambda x: x[0] - x[1]):
+            group = map(itemgetter(1), g)
+            group = list(map(int, group))
+            start, end = group[0], group[-1]
+            start = (
+                known_ind[known_ind < start][-1]
+                if (known_ind < start).sum() > 0
+                else known_ind[0]
+            )
+            end = (
+                known_ind[known_ind > end][0]
+                if (known_ind > end).sum() > 0
+                else known_ind[-1]
+            )
+            anchor_ind += [start, end]
+        return anchor_ind
 
     def _get_antibody_mask(self, data):
+        """Get a mask for the antibody residues."""
         mask = torch.zeros_like(data["mask"]).bool()
         cdrs = data["cdr"]
         chain_enc = data["chain_encoding_all"]
         for chain_ind in data["chain_dict"].values():
             chain_mask = chain_enc == chain_ind
             chain_cdrs = cdrs[chain_mask]
             if len(torch.unique(chain_cdrs)) > 1:
                 mask[chain_mask] = True
         return mask
 
     def _patch(self, data):
+        """Cut the data around the anchor residues."""
         # adapted from diffab
         pos_alpha = data["X"][:, 2]
-        start, end = self._get_anchor_ind(data)
-        anchor_points = torch.stack([pos_alpha[start], pos_alpha[end]], dim=0)
-        dist_anchor = torch.cdist(pos_alpha, anchor_points[[0]], p=2).min(dim=1)[
-            0
-        ]  # (L, )
+        anchor_ind = self.get_anchor_ind(data["masked_res"], data["mask"])
+        anchor_points = torch.stack([pos_alpha[ind] for ind in anchor_ind], dim=0)
+        dist_anchor = torch.cdist(pos_alpha, anchor_points, p=2).min(dim=1)[0]  # (L, )
         dist_anchor[~data["mask"].bool()] = float("+inf")
         initial_patch_idx = torch.topk(
             dist_anchor,
             k=min(self.initial_patch_size, dist_anchor.size(0)),
             largest=False,
             sorted=True,
         )[
             1
         ]  # (initial_patch_size, )
-        patch_mask = data["masked_res"].clone()
-        patch_mask[start] = True
-        patch_mask[end] = True
+        patch_mask = data["masked_res"].bool().clone()
+        patch_mask[[int(x) for x in anchor_ind]] = True
         patch_mask[initial_patch_idx] = True
 
         if self.sabdab:
             antibody_mask = self._get_antibody_mask(data)
             antigen_mask = ~antibody_mask
             dist_anchor_antigen = dist_anchor.masked_fill(
                 mask=antibody_mask, value=float("+inf")  # Fill antibody with +inf
```

### Comparing `proteinflow-2.2.0/proteinflow/data/utils.py` & `proteinflow-2.2.1/proteinflow/data/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/download/__init__.py` & `proteinflow-2.2.1/proteinflow/download/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/download/boto.py` & `proteinflow-2.2.1/proteinflow/download/boto.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/ligand.py` & `proteinflow-2.2.1/proteinflow/ligand.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/logging/__init__.py` & `proteinflow-2.2.1/proteinflow/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/metrics/__init__.py` & `proteinflow-2.2.1/proteinflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/processing/__init__.py` & `proteinflow-2.2.1/proteinflow/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/split/__init__.py` & `proteinflow-2.2.1/proteinflow/split/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     homomers = []
     single_chains = []
     all_files = np.array(list(os.listdir(dataset_dir)))
     all_pdb_files = np.array([f[:4] for f in all_files])
 
     for pdb in tqdm(pdb_seqs_dict.keys()):
         file_names = all_files[all_pdb_files == pdb]
-        if type(file_names) == str:
+        if isinstance(file_names, str):
             file_names = [file_names]
         seqs = pdb_seqs_dict[pdb]
         if len(seqs) == 1 and len(seqs[0].split("-")) == 1:
             for file_name in file_names:
                 single_chains.append((file_name, seqs[0]))
 
         elif len(seqs) == 1 and len(file_names) == 1:
```

### Comparing `proteinflow-2.2.0/proteinflow/split/utils.py` & `proteinflow-2.2.1/proteinflow/split/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow/visualize.py` & `proteinflow-2.2.1/proteinflow/visualize.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/proteinflow.egg-info/PKG-INFO` & `proteinflow-2.2.1/proteinflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.2.0
+Version: 2.2.1
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.2.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.2.1 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.2.0/proteinflow.egg-info/SOURCES.txt` & `proteinflow-2.2.1/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/pyproject.toml` & `proteinflow-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-2.2.0/tests/test_download.py` & `proteinflow-2.2.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/tests/test_entry.py` & `proteinflow-2.2.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/tests/test_generate.py` & `proteinflow-2.2.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/tests/test_ligands.py` & `proteinflow-2.2.1/tests/test_ligands.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.0/tests/test_sabdab.py` & `proteinflow-2.2.1/tests/test_sabdab.py`

 * *Files identical despite different names*

