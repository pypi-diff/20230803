# Comparing `tmp/hot-fair-utilities-1.1.1.tar.gz` & `tmp/hot-fair-utilities-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hot-fair-utilities-1.1.1.tar", last modified: Mon Jul 24 06:43:34 2023, max compression
+gzip compressed data, was "hot-fair-utilities-1.1.2.tar", last modified: Thu Aug  3 09:21:17 2023, max compression
```

## Comparing `hot-fair-utilities-1.1.1.tar` & `hot-fair-utilities-1.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.060154 hot-fair-utilities-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    42190 2023-07-24 06:43:34.060154 hot-fair-utilities-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.052154 hot-fair-utilities-1.1.1/hot_fair_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/georeferencing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.056154 hot-fair-utilities-1.1.1/hot_fair_utilities/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/inference/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.056154 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/building_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/get_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/merge_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/polygonize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/vectorize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.056154 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/clip_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/fix_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/reproject_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.060154 hot-fair-utilities-1.1.1/hot_fair_utilities/training/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/ramp_config_base.json
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/run_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.056154 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42190 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:43:34.060154 hot-fair-utilities-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:21:17.134488 hot-fair-utilities-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-03 09:21:05.000000 hot-fair-utilities-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 09:21:05.000000 hot-fair-utilities-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    42190 2023-08-03 09:21:17.134488 hot-fair-utilities-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-03 09:21:05.000000 hot-fair-utilities-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:21:17.130488 hot-fair-utilities-1.1.2/hot_fair_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/georeferencing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:21:17.130488 hot-fair-utilities-1.1.2/hot_fair_utilities/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/inference/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:21:17.130488 hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/building_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/get_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/merge_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/polygonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/vectorize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:21:17.130488 hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/clip_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/fix_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/reproject_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:21:17.134488 hot-fair-utilities-1.1.2/hot_fair_utilities/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/training/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/training/prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/training/ramp_config_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/training/run_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/hot_fair_utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:21:17.130488 hot-fair-utilities-1.1.2/hot_fair_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42190 2023-08-03 09:21:17.000000 hot-fair-utilities-1.1.2/hot_fair_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-03 09:21:17.000000 hot-fair-utilities-1.1.2/hot_fair_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:21:17.000000 hot-fair-utilities-1.1.2/hot_fair_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-03 09:21:17.000000 hot-fair-utilities-1.1.2/hot_fair_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 09:21:17.000000 hot-fair-utilities-1.1.2/hot_fair_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:21:17.134488 hot-fair-utilities-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:21:06.000000 hot-fair-utilities-1.1.2/setup.py
```

### Comparing `hot-fair-utilities-1.1.1/LICENSE` & `hot-fair-utilities-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/PKG-INFO` & `hot-fair-utilities-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utilities for AI - Assisted Mapping fAIr
 Author-email: Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hot-fair-utilities-1.1.1/README.md` & `hot-fair-utilities-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/georeferencing.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/georeferencing.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/inference/predict.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/inference/predict.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/inference/utils.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/inference/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/building_footprint.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/building_footprint.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/get_polygons.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/get_polygons.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/merge_polygons.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/merge_polygons.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/polygonize.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/polygonize.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/utils.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/vectorize.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/postprocessing/vectorize.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/clip_labels.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/clip_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/fix_labels.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/fix_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/preprocess.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/reproject_labels.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/preprocessing/reproject_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/training/cleanup.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/training/cleanup.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/training/prepare_data.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/training/prepare_data.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/training/ramp_config_base.json` & `hot-fair-utilities-1.1.2/hot_fair_utilities/training/ramp_config_base.json`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/training/run_training.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/training/run_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,21 +318,24 @@
     loss = history.history["loss"]
     # val_loss = history.history["val_loss"]
     epochs = range(1, len(loss) + 1)
 
     acc = history.history["sparse_categorical_accuracy"]
     val_acc = history.history["val_sparse_categorical_accuracy"]
 
+    plt.figure()
+
     # Plot training and validation accuracy
     plt.plot(epochs, acc, "y", label="Training Accuracy")
     plt.plot(epochs, val_acc, "r", label="Validation Accuracy")
 
     # Set labels and title
     plt.xlabel("Epochs")
     plt.ylabel("Accuracy")
     plt.title("Training and Validation Accuracy")
 
     plt.legend()
     plt.savefig(
         f"{cfg['graph_location']}/training_validation_sparse_categorical_accuracy.png"
     )
+    plt.clf()
     print(f"Graph generated at : {cfg['graph_location']}")
```

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/training/train.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/training/train.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities/utils.py` & `hot-fair-utilities-1.1.2/hot_fair_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/PKG-INFO` & `hot-fair-utilities-1.1.2/hot_fair_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utilities for AI - Assisted Mapping fAIr
 Author-email: Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/SOURCES.txt` & `hot-fair-utilities-1.1.2/hot_fair_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.1.1/pyproject.toml` & `hot-fair-utilities-1.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hot-fair-utilities"
-version = "1.1.1"
+version = "1.1.2"
 description = "Utilities for AI - Assisted Mapping fAIr"
 readme = "README.md"
 authors = [{ name = "Hot Tech Team", email = "sysadmin@hotosm.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
```

