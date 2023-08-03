# Comparing `tmp/neuroimager-0.0.8.tar.gz` & `tmp/neuroimager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroimager-0.0.8.tar", last modified: Sun Jul 30 13:45:59 2023, max compression
+gzip compressed data, was "neuroimager-0.0.9.tar", last modified: Thu Aug  3 14:53:56 2023, max compression
```

## Comparing `neuroimager-0.0.8.tar` & `neuroimager-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.181077 neuroimager-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 13:45:44.000000 neuroimager-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-30 13:45:59.177077 neuroimager-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-30 13:45:44.000000 neuroimager-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.169077 neuroimager-0.0.8/neuroimager/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.173077 neuroimager-0.0.8/neuroimager/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/brainage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/pipes/task_fmri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.173077 neuroimager-0.0.8/neuroimager/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/plotting/styler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.177077 neuroimager-0.0.8/neuroimager/preproc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/preproc/decompose.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/preproc/prep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.177077 neuroimager-0.0.8/neuroimager/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/stats/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/stats/perm_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.177077 neuroimager-0.0.8/neuroimager/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/fc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-30 13:45:44.000000 neuroimager-0.0.8/neuroimager/utils/rbload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:45:59.169077 neuroimager-0.0.8/neuroimager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 13:45:59.000000 neuroimager-0.0.8/neuroimager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 13:45:59.181077 neuroimager-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-30 13:45:44.000000 neuroimager-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.322424 neuroimager-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 14:53:46.000000 neuroimager-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-03 14:53:56.322424 neuroimager-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-03 14:53:46.000000 neuroimager-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.310424 neuroimager-0.0.9/neuroimager/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.318424 neuroimager-0.0.9/neuroimager/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/brainage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30640 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/task_fmri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.318424 neuroimager-0.0.9/neuroimager/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/plotting/styler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.318424 neuroimager-0.0.9/neuroimager/preproc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/preproc/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/preproc/prep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.318424 neuroimager-0.0.9/neuroimager/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/stats/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/stats/perm_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.322424 neuroimager-0.0.9/neuroimager/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/rbload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.314424 neuroimager-0.0.9/neuroimager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:53:56.322424 neuroimager-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-03 14:53:46.000000 neuroimager-0.0.9/setup.py
```

### Comparing `neuroimager-0.0.8/LICENSE` & `neuroimager-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/PKG-INFO` & `neuroimager-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroimager
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of utilities used for MRI data analysis
 Home-page: https://github.com/Wetiqe/neuroimager
 Author: Wetiqe
 Author-email: jzni132134@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -24,17 +24,34 @@
 Build a package can keep the analysis scripts short and concise.
 
 This package provides some utilities used for MRI data analysis. And some of them also supports SKLearn Pipeline.
 Note this package is mainly warppers of other packages, intended to optimize for neuroimaging analysis 
 (That's why I can this warppers locally). The tools, especially the pipelines are build based on my personal projects,
 so it may not be very general and suits your need. But I will try to make it more general if I am able to do.
 
+# NOTE!!! This package is still under development and heavily tested, expected to be unstable when used in your analysis.
+# Aims
+This package aims to make 'standard' neuroimaging analysis more easier. 
+In most cases, it is not suitable for developing new analysis pipeline, but some handy small functions may 
+still be helpful to you. Such as atalas operation, permutation based statistics, matrix transformation etc.
+
+## Main Functions
+* Build warpper classes for some common analysis used in MRI analysis (Actually, in my own analysis)
+* Permutation based statistics for neuroimaging
+* Matrix data ML preprocessing and analysis 
+* Nice plotting functions 
+## Styles
+* Preprocess and analyze data using SKLearn transformer style API (Ideally)
+* Statistical analysis aims to be pingouin style
+* Plotting aims to be seaborn style
+
 ![meme](./assets/images/readme1.jpeg)
 
-# A Highly Warpped Pipeline for Task-fMRI analysis
+# Gallery
+## A Highly Warpped Pipeline for Task-fMRI analysis
 This is built on top of nilearn pipeline, doing 1st level and 3rd level analysis as defined by FSL.
 Only a few parameters needs to be set, and the pipeline will do the rest. See example scripts for more details.
 ```python
 task_pipe = Pipeline(
     [
         (
             "first_level",
@@ -61,16 +78,16 @@
 )
 
 results = task_pipe.fit(
     (all_img, confounds, confounds_items, events),
 )
 ```
 
-# Automatic Analysis of HMM model estimated by HMM-MAR
-## Get all model selection metrics and generate a HTML report
+## Automatic Analysis of HMM model estimated by HMM-MAR
+### Get all model selection metrics and generate a HTML report
 
 ```python
 from neuroimager.pipes.hmm import HmmModelSelector
 
 selector = HmmModelSelector(
     models_dir=models_dir,
     krange=krange,
@@ -78,15 +95,15 @@
     volumes=volumes,
     subj_num=sub_num,
     sessions=session_num,
 )
 selector.auto_parse()
 ```
 
-## Get the features of the selected models
+### Get the features of the selected models
 
 ```python
 from neuroimager.pipes.hmm import HmmParser
 
 hmm = HmmParser(
     hmm_file,
     volumes=volumes,
@@ -97,15 +114,15 @@
     auto_parse=True,
     generate_report=False,
 )
 hmm.generate_report(threshold=0.15, plot_vpath=True)
 print(hmm.chronnectome)
 ```
 
-# Atlas Operation
+## Atlas Operation
 
 Suggest you have two probability atlas:
 
 ```python
 from nilearn import plotting
 import nibabel as nib
 import os
@@ -125,30 +142,30 @@
 ```
 
 ![harvard](./assets/images/harvardoxford.png) 
 ![jhu](./assets/images/JHU-tracts.png)
 
 Then you can use the atlas_operation to do some operations on the atlases:
 
-## Remove selected regions
+### Remove selected regions
 ```python
 from neuroimager.utils import filter_rois
 from nilearn import plotting
 import nibabel as nib
 harvard_sub = nib.load("./assets/masks/HarvardOxford-sub-prob-1mm.nii.gz")
 rois_to_remove = [0, 1, 11, 12]  # remove the cortical regions in this atlas
 output_path = "./assets/output/filtered_harvard_sub.nii.gz"
 filtered_atlas = filter_rois(harvard_sub, rois_to_remove, output_path)
 plotting.plot_prob_atlas(filtered_atlas, draw_cross=False, threshold="auto")
 plotting.show()
 ```
 
 ![filtered_harvard](./assets/images/subregions.png)
 
-## Merge two atlases
+### Merge two atlases
 
 ```python
 from neuroimager.utils import combine_probabilistic_atlases
 
 atlas_paths = [
     "./assets/output/filtered_harvard_sub.nii.gz",
     "./assets/masks/JHU-ICBM-tracts-prob-1mm.nii.gz",
```

### Comparing `neuroimager-0.0.8/README.md` & `neuroimager-0.0.9/neuroimager.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,57 @@
+Metadata-Version: 2.1
+Name: neuroimager
+Version: 0.0.9
+Summary: A collection of utilities used for MRI data analysis
+Home-page: https://github.com/Wetiqe/neuroimager
+Author: Wetiqe
+Author-email: jzni132134@gmail.com
+Classifier: Development Status :: 1 - Planning
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Provides-Extra: torch
+License-File: LICENSE
+
 # Neuroimager
 
 The intetion of this pacakge is to make the crossplatform coding and computing much easier. 
 I am using Linux and the remote HPC systems together and sometimes I may use windows or colab.
 It's not very pleasent to keep things synced. Plus different system may have compatibility issues. 
 Build a package can keep the analysis scripts short and concise.
 
 This package provides some utilities used for MRI data analysis. And some of them also supports SKLearn Pipeline.
 Note this package is mainly warppers of other packages, intended to optimize for neuroimaging analysis 
 (That's why I can this warppers locally). The tools, especially the pipelines are build based on my personal projects,
 so it may not be very general and suits your need. But I will try to make it more general if I am able to do.
 
+# NOTE!!! This package is still under development and heavily tested, expected to be unstable when used in your analysis.
+# Aims
+This package aims to make 'standard' neuroimaging analysis more easier. 
+In most cases, it is not suitable for developing new analysis pipeline, but some handy small functions may 
+still be helpful to you. Such as atalas operation, permutation based statistics, matrix transformation etc.
+
+## Main Functions
+* Build warpper classes for some common analysis used in MRI analysis (Actually, in my own analysis)
+* Permutation based statistics for neuroimaging
+* Matrix data ML preprocessing and analysis 
+* Nice plotting functions 
+## Styles
+* Preprocess and analyze data using SKLearn transformer style API (Ideally)
+* Statistical analysis aims to be pingouin style
+* Plotting aims to be seaborn style
+
 ![meme](./assets/images/readme1.jpeg)
 
-# A Highly Warpped Pipeline for Task-fMRI analysis
+# Gallery
+## A Highly Warpped Pipeline for Task-fMRI analysis
 This is built on top of nilearn pipeline, doing 1st level and 3rd level analysis as defined by FSL.
 Only a few parameters needs to be set, and the pipeline will do the rest. See example scripts for more details.
 ```python
 task_pipe = Pipeline(
     [
         (
             "first_level",
@@ -43,16 +78,16 @@
 )
 
 results = task_pipe.fit(
     (all_img, confounds, confounds_items, events),
 )
 ```
 
-# Automatic Analysis of HMM model estimated by HMM-MAR
-## Get all model selection metrics and generate a HTML report
+## Automatic Analysis of HMM model estimated by HMM-MAR
+### Get all model selection metrics and generate a HTML report
 
 ```python
 from neuroimager.pipes.hmm import HmmModelSelector
 
 selector = HmmModelSelector(
     models_dir=models_dir,
     krange=krange,
@@ -60,15 +95,15 @@
     volumes=volumes,
     subj_num=sub_num,
     sessions=session_num,
 )
 selector.auto_parse()
 ```
 
-## Get the features of the selected models
+### Get the features of the selected models
 
 ```python
 from neuroimager.pipes.hmm import HmmParser
 
 hmm = HmmParser(
     hmm_file,
     volumes=volumes,
@@ -79,15 +114,15 @@
     auto_parse=True,
     generate_report=False,
 )
 hmm.generate_report(threshold=0.15, plot_vpath=True)
 print(hmm.chronnectome)
 ```
 
-# Atlas Operation
+## Atlas Operation
 
 Suggest you have two probability atlas:
 
 ```python
 from nilearn import plotting
 import nibabel as nib
 import os
@@ -107,30 +142,30 @@
 ```
 
 ![harvard](./assets/images/harvardoxford.png) 
 ![jhu](./assets/images/JHU-tracts.png)
 
 Then you can use the atlas_operation to do some operations on the atlases:
 
-## Remove selected regions
+### Remove selected regions
 ```python
 from neuroimager.utils import filter_rois
 from nilearn import plotting
 import nibabel as nib
 harvard_sub = nib.load("./assets/masks/HarvardOxford-sub-prob-1mm.nii.gz")
 rois_to_remove = [0, 1, 11, 12]  # remove the cortical regions in this atlas
 output_path = "./assets/output/filtered_harvard_sub.nii.gz"
 filtered_atlas = filter_rois(harvard_sub, rois_to_remove, output_path)
 plotting.plot_prob_atlas(filtered_atlas, draw_cross=False, threshold="auto")
 plotting.show()
 ```
 
 ![filtered_harvard](./assets/images/subregions.png)
 
-## Merge two atlases
+### Merge two atlases
 
 ```python
 from neuroimager.utils import combine_probabilistic_atlases
 
 atlas_paths = [
     "./assets/output/filtered_harvard_sub.nii.gz",
     "./assets/masks/JHU-ICBM-tracts-prob-1mm.nii.gz",
@@ -138,8 +173,8 @@
 combined_atlas = combine_probabilistic_atlases(
     atlas_paths, "./assets/output/combined_prob_atlas.nii.gz"
 )
 plotting.plot_roi(combined_atlas, title="3D Atlas")
 plotting.show()
 
 ```
-![combined_atlas](./assets/images/combined.png)
+![combined_atlas](./assets/images/combined.png)
```

### Comparing `neuroimager-0.0.8/neuroimager/pipes/brainage.py` & `neuroimager-0.0.9/neuroimager/pipes/brainage.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/pipes/cca.py` & `neuroimager-0.0.9/neuroimager/pipes/cca.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/pipes/explore.py` & `neuroimager-0.0.9/neuroimager/pipes/explore.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/pipes/graph.py` & `neuroimager-0.0.9/neuroimager/pipes/graph.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/pipes/hmm.py` & `neuroimager-0.0.9/neuroimager/pipes/hmm.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/pipes/task_fmri.py` & `neuroimager-0.0.9/neuroimager/pipes/task_fmri.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,16 +235,16 @@
         os.makedirs(self.out_dir, exist_ok=True)
         if self.imgs is not None:
             if self.subj_ids is not None:
                 if len(self.imgs) != len(self.subj_ids):
                     raise ValueError(
                         "The number of images and subject ids must be equal"
                     )
-            if confounds is None:
-                self.confounds = [None] * len(imgs)
+            if self.confounds is None:
+                self.confounds = [None] * len(self.imgs)
         if self.confounds is not None:
             if self.confound_items is None:
                 self.confound_items = [
                     "white_matter",
                     "framewise_displacement",
                     "trans_x",
                     "trans_y",
```

### Comparing `neuroimager-0.0.8/neuroimager/plotting/plot.py` & `neuroimager-0.0.9/neuroimager/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/plotting/styler.py` & `neuroimager-0.0.9/neuroimager/plotting/styler.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/preproc/decompose.py` & `neuroimager-0.0.9/neuroimager/preproc/decompose.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/preproc/prep.py` & `neuroimager-0.0.9/neuroimager/preproc/prep.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/stats/correlation.py` & `neuroimager-0.0.9/neuroimager/stats/correlation.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/stats/perm_ttest.py` & `neuroimager-0.0.9/neuroimager/stats/perm_ttest.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/utils/__init__.py` & `neuroimager-0.0.9/neuroimager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/utils/atlas.py` & `neuroimager-0.0.9/neuroimager/utils/atlas.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/utils/fc.py` & `neuroimager-0.0.9/neuroimager/utils/fc.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/utils/ml.py` & `neuroimager-0.0.9/neuroimager/utils/ml.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager/utils/rbload.py` & `neuroimager-0.0.9/neuroimager/utils/rbload.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/neuroimager.egg-info/PKG-INFO` & `neuroimager-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 2.1
-Name: neuroimager
-Version: 0.0.8
-Summary: A collection of utilities used for MRI data analysis
-Home-page: https://github.com/Wetiqe/neuroimager
-Author: Wetiqe
-Author-email: jzni132134@gmail.com
-Classifier: Development Status :: 1 - Planning
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: torch
-License-File: LICENSE
-
 # Neuroimager
 
 The intetion of this pacakge is to make the crossplatform coding and computing much easier. 
 I am using Linux and the remote HPC systems together and sometimes I may use windows or colab.
 It's not very pleasent to keep things synced. Plus different system may have compatibility issues. 
 Build a package can keep the analysis scripts short and concise.
 
 This package provides some utilities used for MRI data analysis. And some of them also supports SKLearn Pipeline.
 Note this package is mainly warppers of other packages, intended to optimize for neuroimaging analysis 
 (That's why I can this warppers locally). The tools, especially the pipelines are build based on my personal projects,
 so it may not be very general and suits your need. But I will try to make it more general if I am able to do.
 
+# NOTE!!! This package is still under development and heavily tested, expected to be unstable when used in your analysis.
+# Aims
+This package aims to make 'standard' neuroimaging analysis more easier. 
+In most cases, it is not suitable for developing new analysis pipeline, but some handy small functions may 
+still be helpful to you. Such as atalas operation, permutation based statistics, matrix transformation etc.
+
+## Main Functions
+* Build warpper classes for some common analysis used in MRI analysis (Actually, in my own analysis)
+* Permutation based statistics for neuroimaging
+* Matrix data ML preprocessing and analysis 
+* Nice plotting functions 
+## Styles
+* Preprocess and analyze data using SKLearn transformer style API (Ideally)
+* Statistical analysis aims to be pingouin style
+* Plotting aims to be seaborn style
+
 ![meme](./assets/images/readme1.jpeg)
 
-# A Highly Warpped Pipeline for Task-fMRI analysis
+# Gallery
+## A Highly Warpped Pipeline for Task-fMRI analysis
 This is built on top of nilearn pipeline, doing 1st level and 3rd level analysis as defined by FSL.
 Only a few parameters needs to be set, and the pipeline will do the rest. See example scripts for more details.
 ```python
 task_pipe = Pipeline(
     [
         (
             "first_level",
@@ -61,16 +60,16 @@
 )
 
 results = task_pipe.fit(
     (all_img, confounds, confounds_items, events),
 )
 ```
 
-# Automatic Analysis of HMM model estimated by HMM-MAR
-## Get all model selection metrics and generate a HTML report
+## Automatic Analysis of HMM model estimated by HMM-MAR
+### Get all model selection metrics and generate a HTML report
 
 ```python
 from neuroimager.pipes.hmm import HmmModelSelector
 
 selector = HmmModelSelector(
     models_dir=models_dir,
     krange=krange,
@@ -78,15 +77,15 @@
     volumes=volumes,
     subj_num=sub_num,
     sessions=session_num,
 )
 selector.auto_parse()
 ```
 
-## Get the features of the selected models
+### Get the features of the selected models
 
 ```python
 from neuroimager.pipes.hmm import HmmParser
 
 hmm = HmmParser(
     hmm_file,
     volumes=volumes,
@@ -97,15 +96,15 @@
     auto_parse=True,
     generate_report=False,
 )
 hmm.generate_report(threshold=0.15, plot_vpath=True)
 print(hmm.chronnectome)
 ```
 
-# Atlas Operation
+## Atlas Operation
 
 Suggest you have two probability atlas:
 
 ```python
 from nilearn import plotting
 import nibabel as nib
 import os
@@ -125,30 +124,30 @@
 ```
 
 ![harvard](./assets/images/harvardoxford.png) 
 ![jhu](./assets/images/JHU-tracts.png)
 
 Then you can use the atlas_operation to do some operations on the atlases:
 
-## Remove selected regions
+### Remove selected regions
 ```python
 from neuroimager.utils import filter_rois
 from nilearn import plotting
 import nibabel as nib
 harvard_sub = nib.load("./assets/masks/HarvardOxford-sub-prob-1mm.nii.gz")
 rois_to_remove = [0, 1, 11, 12]  # remove the cortical regions in this atlas
 output_path = "./assets/output/filtered_harvard_sub.nii.gz"
 filtered_atlas = filter_rois(harvard_sub, rois_to_remove, output_path)
 plotting.plot_prob_atlas(filtered_atlas, draw_cross=False, threshold="auto")
 plotting.show()
 ```
 
 ![filtered_harvard](./assets/images/subregions.png)
 
-## Merge two atlases
+### Merge two atlases
 
 ```python
 from neuroimager.utils import combine_probabilistic_atlases
 
 atlas_paths = [
     "./assets/output/filtered_harvard_sub.nii.gz",
     "./assets/masks/JHU-ICBM-tracts-prob-1mm.nii.gz",
@@ -156,8 +155,8 @@
 combined_atlas = combine_probabilistic_atlases(
     atlas_paths, "./assets/output/combined_prob_atlas.nii.gz"
 )
 plotting.plot_roi(combined_atlas, title="3D Atlas")
 plotting.show()
 
 ```
-![combined_atlas](./assets/images/combined.png)
+![combined_atlas](./assets/images/combined.png)
```

### Comparing `neuroimager-0.0.8/neuroimager.egg-info/SOURCES.txt` & `neuroimager-0.0.9/neuroimager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.8/setup.py` & `neuroimager-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 current_dir = os.path.abspath(os.path.dirname(__file__))
 # Read the contents of your README file
 with open(os.path.join(current_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="neuroimager",
-    version="0.0.8",
+    version="0.0.9",
     description="A collection of utilities used for MRI data analysis",
     author="Wetiqe",
     author_email="jzni132134@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Wetiqe/neuroimager",
     packages=find_packages(),
@@ -24,14 +24,16 @@
         "pingouin",
         "seaborn",
         "sklearn",
         "nilearn",
         "networkx",
         "munkres",
         "scikit-network",
+        "pybids",
+        "tqdm",
     ],
     extras_require={"torch": ["torch>=1.0.0"]},
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

