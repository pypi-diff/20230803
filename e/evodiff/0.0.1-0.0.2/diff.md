# Comparing `tmp/evodiff-0.0.1.tar.gz` & `tmp/evodiff-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodiff-0.0.1.tar", last modified: Thu Jul 20 14:22:53 2023, max compression
+gzip compressed data, was "evodiff-0.0.2.tar", last modified: Thu Aug  3 01:39:12 2023, max compression
```

## Comparing `evodiff-0.0.1.tar` & `evodiff-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-07-20 14:22:53.190587 evodiff-0.0.1/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-20 14:08:00.000000 evodiff-0.0.1/LICENSE
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6471 2023-07-20 14:22:53.190137 evodiff-0.0.1/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6021 2023-07-20 14:08:00.000000 evodiff-0.0.1/README.md
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-07-20 14:22:53.185526 evodiff-0.0.1/evodiff/
--rw-r--r--   0 nityathakkar   (501) staff       (20)      196 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/__init__.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    16981 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/collaters.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/constants.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    21609 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/data.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/losses.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/metrics.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/model.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    11816 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/pretrained.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    14390 2023-07-20 14:08:00.000000 evodiff-0.0.1/evodiff/utils.py
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-07-20 14:22:53.189545 evodiff-0.0.1/evodiff.egg-info/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6471 2023-07-20 14:22:53.000000 evodiff-0.0.1/evodiff.egg-info/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)      336 2023-07-20 14:22:53.000000 evodiff-0.0.1/evodiff.egg-info/SOURCES.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-07-20 14:22:53.000000 evodiff-0.0.1/evodiff.egg-info/dependency_links.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-07-20 14:22:53.000000 evodiff-0.0.1/evodiff.egg-info/top_level.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-07-20 14:20:32.000000 evodiff-0.0.1/pyproject.toml
--rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-07-20 14:22:53.190738 evodiff-0.0.1/setup.cfg
--rw-r--r--   0 nityathakkar   (501) staff       (20)      614 2023-07-20 14:08:00.000000 evodiff-0.0.1/setup.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 01:39:12.627252 evodiff-0.0.2/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.2/LICENSE
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       22 2023-08-03 01:37:06.000000 evodiff-0.0.2/MANIFEST.in
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6885 2023-08-03 01:39:12.626569 evodiff-0.0.2/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6433 2023-08-03 01:27:58.000000 evodiff-0.0.2/README.md
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 01:39:12.567304 evodiff-0.0.2/config/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      417 2023-07-27 13:33:47.000000 evodiff-0.0.2/config/config38M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      398 2023-07-27 13:33:47.000000 evodiff-0.0.2/config/config640M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      352 2023-07-27 13:33:47.000000 evodiff-0.0.2/config/configMSA-600M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      348 2023-07-27 13:33:47.000000 evodiff-0.0.2/config/configMSA.json
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 01:39:12.579373 evodiff-0.0.2/evodiff/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      215 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/__init__.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    14694 2023-08-03 01:27:58.000000 evodiff-0.0.2/evodiff/collaters.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/constants.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    22358 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/data.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/losses.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/metrics.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/model.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    25379 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/plot.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    11836 2023-08-03 01:27:58.000000 evodiff-0.0.2/evodiff/pretrained.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    16217 2023-08-03 01:27:58.000000 evodiff-0.0.2/evodiff/utils.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 01:39:12.625509 evodiff-0.0.2/evodiff.egg-info/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6885 2023-08-03 01:39:12.000000 evodiff-0.0.2/evodiff.egg-info/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      458 2023-08-03 01:39:12.000000 evodiff-0.0.2/evodiff.egg-info/SOURCES.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-03 01:39:12.000000 evodiff-0.0.2/evodiff.egg-info/dependency_links.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-08-03 01:39:12.000000 evodiff-0.0.2/evodiff.egg-info/top_level.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-03 01:38:51.000000 evodiff-0.0.2/pyproject.toml
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-03 01:39:12.627491 evodiff-0.0.2/setup.cfg
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      733 2023-08-03 01:38:22.000000 evodiff-0.0.2/setup.py
```

### Comparing `evodiff-0.0.1/LICENSE` & `evodiff-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.1/PKG-INFO` & `evodiff-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
 Home-page: https://github.com/pypa/sampleproject
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EvoDiff: Generation of protein sequences and evolutionary alignments via discrete diffusion models
 
 In this work, we train and evaluate a series of discrete diffusion models for both unconditional and conditional generation of single protein sequences as well as multiple sequence alignments (MSAs). We test both order-agnostic autoregressive diffusion and discrete denoising diffusion probabilistic models for protein sequence generation; formulate unique, bio-inspired corruption schemes for both classes of models; and evaluate the quality of generated samples for fidelity, diversity, and structural plausibility.
 
 ### Installation
+To download our code, 
+```
+pip install evodiff
+pip install git+https://github.com/microsoft/protein-sequence-models.git # bleeding edge, current repo main branch
+```
+
+To set up a working environment, run:
 ```
 cd evodiff
 conda env create -f environment.yml
 conda activate evodiff
 pip install -e .
 ```
+
+You will also need to install PyTorch. We tested our models on ` v2.0.1 `.
+
 We obtain sequences from the [Uniref50 dataset](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4375400/), which contains approximately 45 million protein sequences. The Multiple Sequence Alignments (MSAs) are from the [OpenFold dataset](https://www.biorxiv.org/content/10.1101/2022.11.20.517210v2), containing MSAs for 132,000 unique Protein Data Bank (PDB) chains.
 
 ### Loading pretrained models
 To load a model:
 ```
 from evodiff.pretrained import OA_AR_640M
 
@@ -71,22 +81,25 @@
 ```
 test_data = UniRefDataset('data/uniref50/', 'rtest', structure=False)
 ```
 To access the generated sequences: 
 ```
 TODO: function to download gen seqs from Zenodo
 ```
-To analyze the quality of the generations, we look at the amino acid KL divergence ([aa_reconstruction_parity_plot](https://github.com/microsoft/evodiff/blob/main/analysis/plot.py), the secondary structure KL divergence ([evodiff/analysis/calc_kl_ss.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_kl_ss.py)), the model perplexity ([evodiff/analysis/model_perp.py](https://github.com/microsoft/evodiff/blob/main/analysis/model_perp.py)), the Fréchet inception distance ([evodiff/analysis/calc_fid.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_fid.py)), and the hamming distance ([evodiff/analysis/calc_nearestseq_hamming.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_nearestseq_hamming.py)).
+To analyze the quality of the generations, we look at the amino acid KL divergence ([aa_reconstruction_parity_plot](https://github.com/microsoft/evodiff/blob/main/analysis/plot.py)), the secondary structure KL divergence ([evodiff/analysis/calc_kl_ss.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_kl_ss.py)), the model perplexity ([evodiff/analysis/model_perp.py](https://github.com/microsoft/evodiff/blob/main/analysis/model_perp.py)), the Fréchet inception distance ([evodiff/analysis/calc_fid.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_fid.py)), and the hamming distance ([evodiff/analysis/calc_nearestseq_hamming.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_nearestseq_hamming.py)).
 
 We also compute the self-consistency perplexity to evaluate the foldability of generated sequences. To do so, we make use of various tools:
 * [TM score](https://zhanggroup.org/TM-score/)
 * [Omegafold](https://github.com/HeliXonProtein/OmegaFold)
 * [ProteinMPNN](https://github.com/dauparas/ProteinMPNN)
 * [ESM-IF1](https://github.com/facebookresearch/esm/tree/main/esm/inverse_folding); see this [Jupyter notebook](https://colab.research.google.com/github/facebookresearch/esm/blob/main/examples/inverse_folding/notebook.ipynb) for setup details.
 * [PGP](https://github.com/hefeda/PGP)
+* [DISOPRED3](https://github.com/psipred/disopred)
+
+Please follow the setup instructions outlined by the authors of those tools.
 
 Our analysis scripts for iterating over these tools are in the [evodiff/analysis/downstream_scripts](https://github.com/microsoft/evodiff/tree/main/analysis/downstream_bash_scripts) folder. Once we run the scripts in this folder, we analyze the results in [self_consistency_analysis.py](https://github.com/microsoft/evodiff/blob/main/analysis/self_consistency_analysis.py).
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
```

### Comparing `evodiff-0.0.1/README.md` & `evodiff-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 # EvoDiff: Generation of protein sequences and evolutionary alignments via discrete diffusion models
 
 In this work, we train and evaluate a series of discrete diffusion models for both unconditional and conditional generation of single protein sequences as well as multiple sequence alignments (MSAs). We test both order-agnostic autoregressive diffusion and discrete denoising diffusion probabilistic models for protein sequence generation; formulate unique, bio-inspired corruption schemes for both classes of models; and evaluate the quality of generated samples for fidelity, diversity, and structural plausibility.
 
 ### Installation
+To download our code, 
+```
+pip install evodiff
+pip install git+https://github.com/microsoft/protein-sequence-models.git # bleeding edge, current repo main branch
+```
+
+To set up a working environment, run:
 ```
 cd evodiff
 conda env create -f environment.yml
 conda activate evodiff
 pip install -e .
 ```
+
+You will also need to install PyTorch. We tested our models on ` v2.0.1 `.
+
 We obtain sequences from the [Uniref50 dataset](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4375400/), which contains approximately 45 million protein sequences. The Multiple Sequence Alignments (MSAs) are from the [OpenFold dataset](https://www.biorxiv.org/content/10.1101/2022.11.20.517210v2), containing MSAs for 132,000 unique Protein Data Bank (PDB) chains.
 
 ### Loading pretrained models
 To load a model:
 ```
 from evodiff.pretrained import OA_AR_640M
 
@@ -59,22 +69,25 @@
 ```
 test_data = UniRefDataset('data/uniref50/', 'rtest', structure=False)
 ```
 To access the generated sequences: 
 ```
 TODO: function to download gen seqs from Zenodo
 ```
-To analyze the quality of the generations, we look at the amino acid KL divergence ([aa_reconstruction_parity_plot](https://github.com/microsoft/evodiff/blob/main/analysis/plot.py), the secondary structure KL divergence ([evodiff/analysis/calc_kl_ss.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_kl_ss.py)), the model perplexity ([evodiff/analysis/model_perp.py](https://github.com/microsoft/evodiff/blob/main/analysis/model_perp.py)), the Fréchet inception distance ([evodiff/analysis/calc_fid.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_fid.py)), and the hamming distance ([evodiff/analysis/calc_nearestseq_hamming.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_nearestseq_hamming.py)).
+To analyze the quality of the generations, we look at the amino acid KL divergence ([aa_reconstruction_parity_plot](https://github.com/microsoft/evodiff/blob/main/analysis/plot.py)), the secondary structure KL divergence ([evodiff/analysis/calc_kl_ss.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_kl_ss.py)), the model perplexity ([evodiff/analysis/model_perp.py](https://github.com/microsoft/evodiff/blob/main/analysis/model_perp.py)), the Fréchet inception distance ([evodiff/analysis/calc_fid.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_fid.py)), and the hamming distance ([evodiff/analysis/calc_nearestseq_hamming.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_nearestseq_hamming.py)).
 
 We also compute the self-consistency perplexity to evaluate the foldability of generated sequences. To do so, we make use of various tools:
 * [TM score](https://zhanggroup.org/TM-score/)
 * [Omegafold](https://github.com/HeliXonProtein/OmegaFold)
 * [ProteinMPNN](https://github.com/dauparas/ProteinMPNN)
 * [ESM-IF1](https://github.com/facebookresearch/esm/tree/main/esm/inverse_folding); see this [Jupyter notebook](https://colab.research.google.com/github/facebookresearch/esm/blob/main/examples/inverse_folding/notebook.ipynb) for setup details.
 * [PGP](https://github.com/hefeda/PGP)
+* [DISOPRED3](https://github.com/psipred/disopred)
+
+Please follow the setup instructions outlined by the authors of those tools.
 
 Our analysis scripts for iterating over these tools are in the [evodiff/analysis/downstream_scripts](https://github.com/microsoft/evodiff/tree/main/analysis/downstream_bash_scripts) folder. Once we run the scripts in this folder, we analyze the results in [self_consistency_analysis.py](https://github.com/microsoft/evodiff/blob/main/analysis/self_consistency_analysis.py).
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
```

### Comparing `evodiff-0.0.1/evodiff/collaters.py` & `evodiff-0.0.2/evodiff/collaters.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,67 +102,14 @@
             src.append(x_t)
         # PAD out
         src = _pad(src, self.tokenizer.pad_id)
         masks = _pad(masks*1,0) #, self.seq_length, 0)
         tokenized = _pad(tokenized, self.tokenizer.pad_id)
         return (src.to(torch.long), torch.tensor(timesteps), tokenized.to(torch.long), masks)
 
-class LRMaskCollater(object):
-    """
-    Mask Collater for masking batch data in a L->R Autoregressive fashion (used only for downstream)
-    inputs:
-        sequences : list of sequences
-        inputs_padded: if inputs are padded (due to truncation in Simple_Collater) set True (default False)
-
-    OA-ARM variables:
-        D : possible permutations from 0.. max length
-        t : randomly selected timestep
-
-    outputs:
-        src : source  masked sequences (model input)
-        timesteps: (D-t+1) term
-        tokenized: tokenized sequences (target seq)
-        masks: masks used to generate src
-    """
-    def __init__(self, tokenizer=Tokenizer()):
-        self.tokenizer = tokenizer
-
-    def __call__(self, sequences):
-        tokenized = [torch.tensor(self.tokenizer.tokenize(s)) for s in sequences]
-        max_len = max(len(t) for t in tokenized)
-        src=[]
-        timesteps = []
-        masks=[]
-        mask_id = torch.tensor(self.tokenizer.mask_id, dtype=torch.int64)
-        for i,x in enumerate(tokenized):
-            # Randomly generate timestep and indices to mask
-            D = len(x) # D should have the same dimensions as each sequence length
-            if D <= 1:  # for sequence length = 1 in dataset
-                t = 1
-            else:
-                t = np.random.randint(1, D) # randomly sample timestep
-            num_mask = (D-t+1)
-            # Append timestep
-            timesteps.append(num_mask)
-            # Generate mask
-            mask_arr = np.arange(t,D) # Generates array of len num_mask # TODO if this is the only diff line merge with collater above)
-            index_arr = np.arange(0, max_len) #index array [1...seq_len]
-            mask = np.isin(index_arr, mask_arr, invert=False).reshape(index_arr.shape) # mask bools indices specified by mask_arr
-            # Mask inputs
-            mask = torch.tensor(mask, dtype=torch.bool)
-            masks.append(mask)
-            x_t = ~mask[0:D] * x + mask[0:D] * mask_id
-            src.append(x_t)
-        # PAD out
-        src = _pad(src, self.tokenizer.pad_id)
-        masks = _pad(masks*1,0) #, self.seq_length, 0)
-        tokenized = _pad(tokenized, self.tokenizer.pad_id)
-        return (src.to(torch.long), torch.tensor(timesteps), tokenized.to(torch.long), masks)
-
-
 class D3PMCollater(object):
     """
     D3PM Collater for generating batch data according to markov process according to Austin et al.
     inputs:
         sequences : list of sequences
         tokenizer: Tokenizer()
         masking scheme: 'BLOSUM' uses blosum matrix, 'RANDOM' uses uniform transition matrix
```

### Comparing `evodiff-0.0.1/evodiff/data.py` & `evodiff-0.0.2/evodiff/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from torch.utils.data import Dataset
 import pandas as pd
 
 from evodiff.utils import Tokenizer
 from sequence_models.utils import parse_fasta
 from sequence_models.constants import PROTEIN_ALPHABET, trR_ALPHABET, PAD, GAP
 from collections import Counter
+import torch
+import os
+from torch.utils.data import Subset
+
 
 def read_openfold_files(data_dir, filename):
     """
     Helper function to read the openfold files
 
     inputs:
         data_dir : path to directory with data
@@ -66,14 +70,31 @@
             path = read_openfold_files(data_dir, filename)
         parsed_msa = parse_fasta(path)
         msa_depth.append(len(parsed_msa))
         msa_lengths.append(len(parsed_msa[0]))  # all seq in MSA are same length
     np.savez_compressed(data_dir+save_depth_file, np.asarray(msa_depth))
     np.savez_compressed(data_dir + save_length_file, np.asarray(msa_lengths))
 
+
+def get_valid_msas(data_top_dir, data_dir='openfold/', selection_type='MaxHamming', n_sequences=64, max_seq_len=512,
+                   out_path='../DMs/ref/'):
+    assert data_dir=='openfold', "get_valid_msas only works on OPENFOLD"
+    _ = torch.manual_seed(1) # same seeds used for training
+    np.random.seed(1)
+
+    dataset = A3MMSADataset(selection_type, n_sequences, max_seq_len, data_dir=os.path.join(data_top_dir,data_dir), min_depth=64)
+
+    train_size = len(dataset)
+    random_ind = np.random.choice(train_size, size=(train_size - 10000), replace=False)
+    val_ind = np.delete(np.arange(train_size), random_ind)
+    ds_valid = Subset(dataset, val_ind)
+
+    return ds_valid
+
+
 def get_idr_query_index(data_dir, all_files, save_file):
     """
     Function to get IDR query index
 
     inputs:
         data_dir : path to directory with data
         all_files: all filenames
```

### Comparing `evodiff-0.0.1/evodiff/losses.py` & `evodiff-0.0.2/evodiff/losses.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.1/evodiff/metrics.py` & `evodiff-0.0.2/evodiff/metrics.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.1/evodiff/model.py` & `evodiff-0.0.2/evodiff/model.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.1/evodiff/pretrained.py` & `evodiff-0.0.2/evodiff/pretrained.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     tie_weights=False
     final_norm=True
     model = ByteNetLMTime(n_tokens, d_embed, d_model, n_layers, kernel_size, r,
                           causal=causal, padding_idx=masking_idx, rank=weight_rank, dropout=dropout,
                           tie_weights=tie_weights, final_ln=final_norm, slim=slim, activation=activation,
                           timesteps=diffusion_timesteps)
     state_dict = download_model(model_name)
-    sd = torch.load(state_dict, map_location=torch.device('cpu'))
-    msd = sd['model_state_dict']
+    # sd = torch.load(state_dict, map_location=torch.device('cpu'))
+    msd = state_dict['model_state_dict']
     msd = {k.split('module.')[1]: v for k, v in msd.items()}
     model.load_state_dict(msd)
 
     return model, tokenizer
 
 def load_msa_checkpoint(model_name, config_path, diffusion_timesteps, tokenizer=Tokenizer()):
     with open(config_path, 'r') as f:
@@ -59,16 +59,16 @@
                                padding_idx=MSA_ALPHABET.index(MSA_PAD), mask_idx=MSA_ALPHABET.index(MASK))
     else:
         padding_idx = tokenizer.pad_id
         masking_idx = tokenizer.mask_id
         model = MSATransformerTime(d_embed, d_hidden, n_layers, n_heads, timesteps=diffusion_timesteps, use_ckpt=True,
                                n_tokens=len(MSA_ALPHABET), padding_idx=padding_idx, mask_idx=masking_idx)
     state_dict = download_model(model_name)
-    sd = torch.load(state_dict, map_location=torch.device('cpu'))
-    msd = sd['model_state_dict']
+    # sd = torch.load(state_dict, map_location=torch.device('cpu'))
+    msd = state_dict['model_state_dict']
     msd = {k.split('module.')[1]: v for k, v in msd.items()}
     model.load_state_dict(msd)
     return model, tokenizer
 
 def D3PM_BLOSUM_640M(return_all=False):
     dt=500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=True)
```

### Comparing `evodiff-0.0.1/evodiff.egg-info/PKG-INFO` & `evodiff-0.0.2/evodiff.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
 Home-page: https://github.com/pypa/sampleproject
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EvoDiff: Generation of protein sequences and evolutionary alignments via discrete diffusion models
 
 In this work, we train and evaluate a series of discrete diffusion models for both unconditional and conditional generation of single protein sequences as well as multiple sequence alignments (MSAs). We test both order-agnostic autoregressive diffusion and discrete denoising diffusion probabilistic models for protein sequence generation; formulate unique, bio-inspired corruption schemes for both classes of models; and evaluate the quality of generated samples for fidelity, diversity, and structural plausibility.
 
 ### Installation
+To download our code, 
+```
+pip install evodiff
+pip install git+https://github.com/microsoft/protein-sequence-models.git # bleeding edge, current repo main branch
+```
+
+To set up a working environment, run:
 ```
 cd evodiff
 conda env create -f environment.yml
 conda activate evodiff
 pip install -e .
 ```
+
+You will also need to install PyTorch. We tested our models on ` v2.0.1 `.
+
 We obtain sequences from the [Uniref50 dataset](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4375400/), which contains approximately 45 million protein sequences. The Multiple Sequence Alignments (MSAs) are from the [OpenFold dataset](https://www.biorxiv.org/content/10.1101/2022.11.20.517210v2), containing MSAs for 132,000 unique Protein Data Bank (PDB) chains.
 
 ### Loading pretrained models
 To load a model:
 ```
 from evodiff.pretrained import OA_AR_640M
 
@@ -71,22 +81,25 @@
 ```
 test_data = UniRefDataset('data/uniref50/', 'rtest', structure=False)
 ```
 To access the generated sequences: 
 ```
 TODO: function to download gen seqs from Zenodo
 ```
-To analyze the quality of the generations, we look at the amino acid KL divergence ([aa_reconstruction_parity_plot](https://github.com/microsoft/evodiff/blob/main/analysis/plot.py), the secondary structure KL divergence ([evodiff/analysis/calc_kl_ss.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_kl_ss.py)), the model perplexity ([evodiff/analysis/model_perp.py](https://github.com/microsoft/evodiff/blob/main/analysis/model_perp.py)), the Fréchet inception distance ([evodiff/analysis/calc_fid.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_fid.py)), and the hamming distance ([evodiff/analysis/calc_nearestseq_hamming.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_nearestseq_hamming.py)).
+To analyze the quality of the generations, we look at the amino acid KL divergence ([aa_reconstruction_parity_plot](https://github.com/microsoft/evodiff/blob/main/analysis/plot.py)), the secondary structure KL divergence ([evodiff/analysis/calc_kl_ss.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_kl_ss.py)), the model perplexity ([evodiff/analysis/model_perp.py](https://github.com/microsoft/evodiff/blob/main/analysis/model_perp.py)), the Fréchet inception distance ([evodiff/analysis/calc_fid.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_fid.py)), and the hamming distance ([evodiff/analysis/calc_nearestseq_hamming.py](https://github.com/microsoft/evodiff/blob/main/analysis/calc_nearestseq_hamming.py)).
 
 We also compute the self-consistency perplexity to evaluate the foldability of generated sequences. To do so, we make use of various tools:
 * [TM score](https://zhanggroup.org/TM-score/)
 * [Omegafold](https://github.com/HeliXonProtein/OmegaFold)
 * [ProteinMPNN](https://github.com/dauparas/ProteinMPNN)
 * [ESM-IF1](https://github.com/facebookresearch/esm/tree/main/esm/inverse_folding); see this [Jupyter notebook](https://colab.research.google.com/github/facebookresearch/esm/blob/main/examples/inverse_folding/notebook.ipynb) for setup details.
 * [PGP](https://github.com/hefeda/PGP)
+* [DISOPRED3](https://github.com/psipred/disopred)
+
+Please follow the setup instructions outlined by the authors of those tools.
 
 Our analysis scripts for iterating over these tools are in the [evodiff/analysis/downstream_scripts](https://github.com/microsoft/evodiff/tree/main/analysis/downstream_bash_scripts) folder. Once we run the scripts in this folder, we analyze the results in [self_consistency_analysis.py](https://github.com/microsoft/evodiff/blob/main/analysis/self_consistency_analysis.py).
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
```

