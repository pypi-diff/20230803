# Comparing `tmp/batdetect2-1.0.5.tar.gz` & `tmp/batdetect2-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batdetect2-1.0.5.tar", last modified: Thu May 11 13:13:14 2023, max compression
+gzip compressed data, was "batdetect2-1.0.6.tar", last modified: Thu Aug  3 11:49:55 2023, max compression
```

## Comparing `batdetect2-1.0.5.tar` & `batdetect2-1.0.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0    17694 2023-05-11 13:13:04.611105 batdetect2-1.0.5/LICENSE.md
--rw-r--r--   0        0        0     5584 2023-05-11 13:13:04.611105 batdetect2-1.0.5/README.md
--rw-r--r--   0        0        0       22 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/__init__.py
--rw-r--r--   0        0        0    12537 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/api.py
--rw-r--r--   0        0        0     4117 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/cli.py
--rw-r--r--   0        0        0        0 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/__init__.py
--rw-r--r--   0        0        0     4225 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/compute_features.py
--rw-r--r--   0        0        0     4970 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/model_helpers.py
--rw-r--r--   0        0        0    10568 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/models.py
--rw-r--r--   0        0        0     7481 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/parameters.py
--rw-r--r--   0        0        0     5873 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/post_process.py
--rw-r--r--   0        0        0        0 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/evaluate/__init__.py
--rw-r--r--   0        0        0    25540 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/evaluate/evaluate_models.py
--rw-r--r--   0        0        0     2244 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/evaluate/readme.md
--rw-r--r--   0        0        0        0 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/finetune/__init__.py
--rw-r--r--   0        0        0     9902 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/finetune/finetune_model.py
--rw-r--r--   0        0        0     6324 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/finetune/prep_data_finetune.py
--rw-r--r--   0        0        0     3158 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/finetune/readme.md
--rw-r--r--   0        0        0  7600690 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/models/Net2DFast_UK_same.pth.tar
--rw-r--r--   0        0        0       25 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/models/readme.md
--rw-r--r--   0        0        0     9832 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/plot.py
--rw-r--r--   0        0        0        0 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/__init__.py
--rw-r--r--   0        0        0    20543 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/audio_dataloader.py
--rwxr-xr-x   0        0        0    13217 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/evaluate.py
--rw-r--r--   0        0        0     1580 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/losses.py
--rw-r--r--   0        0        0     1186 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/readme.md
--rw-r--r--   0        0        0    17515 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/train_model.py
--rw-r--r--   0        0        0    12533 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/train_split.py
--rw-r--r--   0        0        0     5961 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/train_utils.py
--rw-r--r--   0        0        0    11150 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/types.py
--rw-r--r--   0        0        0        0 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/__init__.py
--rw-r--r--   0        0        0     8455 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/audio_utils.py
--rw-r--r--   0        0        0    23712 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/detector_utils.py
--rw-r--r--   0        0        0    16322 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/plot_utils.py
--rw-r--r--   0        0        0     7940 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/visualize.py
--rw-r--r--   0        0        0     8059 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/wavfile.py
--rw-r--r--   0        0        0     1749 2023-05-11 13:13:04.675105 batdetect2-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 13:13:04.675105 batdetect2-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0     9321 2023-05-11 13:13:04.675105 batdetect2-1.0.5/tests/test_api.py
--rw-r--r--   0        0        0     1853 2023-05-11 13:13:04.675105 batdetect2-1.0.5/tests/test_cli.py
--rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 batdetect2-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    17694 2023-08-03 11:49:45.767939 batdetect2-1.0.6/LICENSE.md
+-rw-r--r--   0        0        0     5587 2023-08-03 11:49:45.767939 batdetect2-1.0.6/README.md
+-rw-r--r--   0        0        0       22 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/__init__.py
+-rw-r--r--   0        0        0    12537 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/api.py
+-rw-r--r--   0        0        0     4117 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/cli.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/detector/__init__.py
+-rw-r--r--   0        0        0     9261 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/detector/compute_features.py
+-rw-r--r--   0        0        0     4970 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/detector/model_helpers.py
+-rw-r--r--   0        0        0    10568 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/detector/models.py
+-rw-r--r--   0        0        0     7481 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/detector/parameters.py
+-rw-r--r--   0        0        0     5873 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/detector/post_process.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/evaluate/__init__.py
+-rw-r--r--   0        0        0    25540 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/evaluate/evaluate_models.py
+-rw-r--r--   0        0        0     2244 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/evaluate/readme.md
+-rw-r--r--   0        0        0        0 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/finetune/__init__.py
+-rw-r--r--   0        0        0     9902 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/finetune/finetune_model.py
+-rw-r--r--   0        0        0     6324 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/finetune/prep_data_finetune.py
+-rw-r--r--   0        0        0     3158 2023-08-03 11:49:45.767939 batdetect2-1.0.6/batdetect2/finetune/readme.md
+-rw-r--r--   0        0        0  7600690 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/models/Net2DFast_UK_same.pth.tar
+-rw-r--r--   0        0        0       25 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/models/readme.md
+-rw-r--r--   0        0        0     9832 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/plot.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/train/__init__.py
+-rw-r--r--   0        0        0    20543 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/train/audio_dataloader.py
+-rwxr-xr-x   0        0        0    13217 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/train/evaluate.py
+-rw-r--r--   0        0        0     1580 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/train/losses.py
+-rw-r--r--   0        0        0     1186 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/train/readme.md
+-rw-r--r--   0        0        0    17515 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/train/train_model.py
+-rw-r--r--   0        0        0    12533 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/train/train_split.py
+-rw-r--r--   0        0        0     5961 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/train/train_utils.py
+-rw-r--r--   0        0        0    12439 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/types.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/utils/__init__.py
+-rw-r--r--   0        0        0     8455 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/utils/audio_utils.py
+-rw-r--r--   0        0        0    23714 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/utils/detector_utils.py
+-rw-r--r--   0        0        0    16322 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/utils/plot_utils.py
+-rw-r--r--   0        0        0     7940 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/utils/visualize.py
+-rw-r--r--   0        0        0     8059 2023-08-03 11:49:45.819941 batdetect2-1.0.6/batdetect2/utils/wavfile.py
+-rw-r--r--   0        0        0     1749 2023-08-03 11:49:45.835941 batdetect2-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-03 11:49:45.835941 batdetect2-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     9321 2023-08-03 11:49:45.835941 batdetect2-1.0.6/tests/test_api.py
+-rw-r--r--   0        0        0     2941 2023-08-03 11:49:45.835941 batdetect2-1.0.6/tests/test_cli.py
+-rw-r--r--   0        0        0     7262 2023-08-03 11:49:45.835941 batdetect2-1.0.6/tests/test_features.py
+-rw-r--r--   0        0        0     6540 1970-01-01 00:00:00.000000 batdetect2-1.0.6/PKG-INFO
```

### Comparing `batdetect2-1.0.5/LICENSE.md` & `batdetect2-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/README.md` & `batdetect2-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 You can use pip to install `batdetect2`:
 
 ```bash
 pip install batdetect2
 ```
 
 Alternatively, download this code from the repository (by clicking on the green button on top right) and unzip it.
-Once unziped, run this from extracted folder.
+Once unzipped, run this from extracted folder.
 
 ```bash
 pip install .
 ```
 
 Make sure you have the environment activated before installing `batdetect2`.
 
@@ -94,15 +94,15 @@
 # Do something else ...
 ```
 
 You can integrate the detections or the extracted features to your custom analysis pipeline.
 
 
 ## Training the model on your own data
-Take a look at the steps outlined in fintuning readme [here](bat_detect/finetune/readme.md) for a description of how to train your own model.
+Take a look at the steps outlined in fine tuning readme [here](bat_detect/finetune/readme.md) for a description of how to train your own model.
 
 
 ## Data and annotations
 The raw audio data and annotations used to train the models in the paper will be added soon.
 The audio interface used to annotate audio data for training and evaluation is available [here](https://github.com/macaodha/batdetect2_GUI).
```

### Comparing `batdetect2-1.0.5/batdetect2/api.py` & `batdetect2-1.0.6/batdetect2/api.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/cli.py` & `batdetect2-1.0.6/batdetect2/cli.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/detector/model_helpers.py` & `batdetect2-1.0.6/batdetect2/detector/model_helpers.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/detector/models.py` & `batdetect2-1.0.6/batdetect2/detector/models.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/detector/parameters.py` & `batdetect2-1.0.6/batdetect2/detector/parameters.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/detector/post_process.py` & `batdetect2-1.0.6/batdetect2/detector/post_process.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/evaluate/evaluate_models.py` & `batdetect2-1.0.6/batdetect2/evaluate/evaluate_models.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/evaluate/readme.md` & `batdetect2-1.0.6/batdetect2/evaluate/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/finetune/finetune_model.py` & `batdetect2-1.0.6/batdetect2/finetune/finetune_model.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/finetune/prep_data_finetune.py` & `batdetect2-1.0.6/batdetect2/finetune/prep_data_finetune.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/finetune/readme.md` & `batdetect2-1.0.6/batdetect2/finetune/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/models/Net2DFast_UK_same.pth.tar` & `batdetect2-1.0.6/batdetect2/models/Net2DFast_UK_same.pth.tar`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/plot.py` & `batdetect2-1.0.6/batdetect2/plot.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/train/audio_dataloader.py` & `batdetect2-1.0.6/batdetect2/train/audio_dataloader.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/train/evaluate.py` & `batdetect2-1.0.6/batdetect2/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/train/losses.py` & `batdetect2-1.0.6/batdetect2/train/losses.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/train/readme.md` & `batdetect2-1.0.6/batdetect2/train/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/train/train_model.py` & `batdetect2-1.0.6/batdetect2/train/train_model.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/train/train_split.py` & `batdetect2-1.0.6/batdetect2/train/train_split.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/train/train_utils.py` & `batdetect2-1.0.6/batdetect2/train/train_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/types.py` & `batdetect2-1.0.6/batdetect2/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Types used in the code base."""
-from typing import List, NamedTuple, Optional
+from typing import List, NamedTuple, Optional, Union
 
 import numpy as np
 import torch
 
 try:
     from typing import TypedDict
 except ImportError:
@@ -21,18 +21,21 @@
 except ImportError:
     from typing_extensions import NotRequired
 
 
 __all__ = [
     "Annotation",
     "DetectionModel",
+    "FeatureExtractionParameters",
+    "FeatureExtractor",
     "FileAnnotations",
     "ModelOutput",
     "ModelParameters",
     "NonMaximumSuppressionConfig",
+    "Prediction",
     "PredictionResults",
     "ProcessingConfiguration",
     "ResultParams",
     "RunResults",
     "SpectrogramParameters",
 ]
 
@@ -308,14 +311,48 @@
     pred_class_un_norm: torch.Tensor
     """Tensor with predicted class probabilities before softmax."""
 
     features: torch.Tensor
     """Tensor with intermediate features."""
 
 
+class Prediction(TypedDict):
+    """Singe prediction."""
+
+    det_prob: float
+    """Detection probability."""
+
+    x_pos: int
+    """X position of the detection in pixels."""
+
+    y_pos: int
+    """Y position of the detection in pixels."""
+
+    bb_width: int
+    """Width of the detection in pixels."""
+
+    bb_height: int
+    """Height of the detection in pixels."""
+
+    start_time: float
+    """Start time of the detection in seconds."""
+
+    end_time: float
+    """End time of the detection in seconds."""
+
+    low_freq: float
+    """Low frequency of the detection in Hz."""
+
+    high_freq: float
+    """High frequency of the detection in Hz."""
+
+    class_prob: np.ndarray
+    """Vector holding the probability of each class."""
+
+
 class PredictionResults(TypedDict):
     """Results of the prediction.
 
     Each key is a list of length `num_detections` containing the
     corresponding values for each detection.
     """
 
@@ -414,14 +451,24 @@
     nms_top_k_per_sec: float
     """Number of top detections to keep per second."""
 
     detection_threshold: float
     """Threshold for detection probability."""
 
 
+class FeatureExtractionParameters(TypedDict):
+    """Parameters that control the feature extraction function."""
+
+    min_freq: int
+    """Minimum frequency to consider in Hz."""
+
+    max_freq: int
+    """Maximum frequency to consider in Hz."""
+
+
 class HeatmapParameters(TypedDict):
     """Parameters that control the heatmap generation function."""
 
     class_names: List[str]
 
     fft_win_length: float
     """Length of the FFT window in seconds."""
@@ -469,7 +516,15 @@
     """Individual IDs of the annotations."""
 
     x_inds: NotRequired[np.ndarray]
     """X coordinate of the annotations in the spectrogram."""
 
     y_inds: NotRequired[np.ndarray]
     """Y coordinate of the annotations in the spectrogram."""
+
+
+class FeatureExtractor(Protocol):
+    """Protocol for feature extractors."""
+
+    def __call__(self, prediction: Prediction, **kwargs) -> Union[float, int]:
+        """Extract features from a prediction."""
+        ...
```

### Comparing `batdetect2-1.0.5/batdetect2/utils/audio_utils.py` & `batdetect2-1.0.6/batdetect2/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/utils/detector_utils.py` & `batdetect2-1.0.6/batdetect2/utils/detector_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,15 +769,15 @@
             sampling_rate,
             model,
             config,
             device,
         )
 
         # convert to numpy
-        spec_np = spec.detach().cpu().numpy()
+        spec_np = spec.detach().cpu().numpy().squeeze()
 
         # add chunk time to start and end times
         pred_nms["start_times"] += chunk_time
         pred_nms["end_times"] += chunk_time
 
         predictions.append(pred_nms)
 
@@ -790,15 +790,15 @@
 
         if config["cnn_features"]:
             cnn_feats.append(features[0])
 
         if config["spec_slices"]:
             # FIX: This is not currently working. Returns empty slices
             spec_slices.extend(
-                feats.extract_spec_slices(spec_np, pred_nms, config)
+                feats.extract_spec_slices(spec_np, pred_nms)
             )
 
     # Merge results from chunks
     predictions, spec_feats, cnn_feats, spec_slices = _merge_results(
         predictions,
         spec_feats,
         cnn_feats,
```

### Comparing `batdetect2-1.0.5/batdetect2/utils/plot_utils.py` & `batdetect2-1.0.6/batdetect2/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/utils/visualize.py` & `batdetect2-1.0.6/batdetect2/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/batdetect2/utils/wavfile.py` & `batdetect2-1.0.6/batdetect2/utils/wavfile.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/pyproject.toml` & `batdetect2-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.2.2",
 ]
 
 [tool.black]
-line-length = 80
+line-length = 79
 
 [[tool.mypy.overrides]]
 module = [
     "librosa",
     "pandas",
 ]
 ignore_missing_imports = true
@@ -27,15 +27,15 @@
     "tests",
 ]
 venvPath = "."
 venv = ".venv"
 
 [project]
 name = "batdetect2"
-version = "1.0.5"
+version = "1.0.6"
 description = "Deep learning model for detecting and classifying bat echolocation calls in high frequency audio recordings."
 authors = [
     { name = "Oisin Mac Aodha", email = "oisin.macaodha@ed.ac.uk" },
     { name = "Santiago Martinez Balvanera", email = "santiago.balvanera.20@ucl.ac.uk" },
 ]
 dependencies = [
     "librosa",
```

### Comparing `batdetect2-1.0.5/tests/test_api.py` & `batdetect2-1.0.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.5/PKG-INFO` & `batdetect2-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batdetect2
-Version: 1.0.5
+Version: 1.0.6
 Summary: Deep learning model for detecting and classifying bat echolocation calls in high frequency audio recordings.
 License: CC-by-nc-4
 Keywords: bat,echolocation,deep learning,audio,machine learning,classification,detection
 Author-email: Oisin Mac Aodha <oisin.macaodha@ed.ac.uk>,Santiago Martinez Balvanera <santiago.balvanera.20@ucl.ac.uk>
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -44,15 +44,15 @@
 You can use pip to install `batdetect2`:
 
 ```bash
 pip install batdetect2
 ```
 
 Alternatively, download this code from the repository (by clicking on the green button on top right) and unzip it.
-Once unziped, run this from extracted folder.
+Once unzipped, run this from extracted folder.
 
 ```bash
 pip install .
 ```
 
 Make sure you have the environment activated before installing `batdetect2`.
 
@@ -113,15 +113,15 @@
 # Do something else ...
 ```
 
 You can integrate the detections or the extracted features to your custom analysis pipeline.
 
 
 ## Training the model on your own data
-Take a look at the steps outlined in fintuning readme [here](bat_detect/finetune/readme.md) for a description of how to train your own model.
+Take a look at the steps outlined in fine tuning readme [here](bat_detect/finetune/readme.md) for a description of how to train your own model.
 
 
 ## Data and annotations
 The raw audio data and annotations used to train the models in the paper will be added soon.
 The audio interface used to annotate audio data for training and evaluation is available [here](https://github.com/macaodha/batdetect2_GUI).
```

