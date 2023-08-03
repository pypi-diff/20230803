# Comparing `tmp/yoyodyne-0.2.4.tar.gz` & `tmp/yoyodyne-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoyodyne-0.2.4.tar", last modified: Wed Jul 19 18:17:37 2023, max compression
+gzip compressed data, was "yoyodyne-0.2.5.tar", last modified: Thu Aug  3 18:41:09 2023, max compression
```

## Comparing `yoyodyne-0.2.4.tar` & `yoyodyne-0.2.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2023-07-19 18:17:37.831990 yoyodyne-0.2.4/
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    10814 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/LICENSE.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    13616 2023-07-19 18:17:37.831990 yoyodyne-0.2.4/PKG-INFO
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    12856 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/README.md
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     1277 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/pyproject.toml
--rw-rw-r--   0 kbg       (1000) kbg       (1000)       38 2023-07-19 18:17:37.831990 yoyodyne-0.2.4/setup.cfg
-drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2023-07-19 18:17:37.827990 yoyodyne-0.2.4/yoyodyne/
--rw-rw-r--   0 kbg       (1000) kbg       (1000)      289 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/__init__.py
-drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2023-07-19 18:17:37.831990 yoyodyne-0.2.4/yoyodyne/data/
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     2783 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/data/__init__.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     3495 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/data/batches.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     5329 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/data/collators.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     6982 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/data/datamodules.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     6192 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/data/datasets.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     4486 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/data/indexes.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     4958 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/data/tsv.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)      943 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/defaults.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     3974 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/evaluators.py
-drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2023-07-19 18:17:37.831990 yoyodyne-0.2.4/yoyodyne/models/
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     1891 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/__init__.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    18548 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/base.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    17097 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/expert.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    13365 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/lstm.py
-drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2023-07-19 18:17:37.831990 yoyodyne-0.2.4/yoyodyne/models/modules/
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     3017 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/modules/__init__.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     3305 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/modules/attention.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     4502 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/modules/base.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     1442 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/modules/linear.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     7322 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/modules/lstm.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    10275 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/modules/transformer.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    14654 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/pointer_generator.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    21503 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/transducer.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     6461 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/models/transformer.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     4376 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/predict.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     7644 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/schedulers.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)      169 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/special.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    10519 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/train.py
--rw-rw-r--   0 kbg       (1000) kbg       (1000)      599 2023-07-19 18:15:31.000000 yoyodyne-0.2.4/yoyodyne/util.py
-drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2023-07-19 18:17:37.827990 yoyodyne-0.2.4/yoyodyne.egg-info/
--rw-rw-r--   0 kbg       (1000) kbg       (1000)    13616 2023-07-19 18:17:37.000000 yoyodyne-0.2.4/yoyodyne.egg-info/PKG-INFO
--rw-rw-r--   0 kbg       (1000) kbg       (1000)      982 2023-07-19 18:17:37.000000 yoyodyne-0.2.4/yoyodyne.egg-info/SOURCES.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)        1 2023-07-19 18:17:37.000000 yoyodyne-0.2.4/yoyodyne.egg-info/dependency_links.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)       96 2023-07-19 18:17:37.000000 yoyodyne-0.2.4/yoyodyne.egg-info/entry_points.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)       82 2023-07-19 18:17:37.000000 yoyodyne-0.2.4/yoyodyne.egg-info/requires.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)        9 2023-07-19 18:17:37.000000 yoyodyne-0.2.4/yoyodyne.egg-info/top_level.txt
+drwxr-xr-x   0 kbg      (304185) primarygroup (89939)        0 2023-08-03 18:41:09.885669 yoyodyne-0.2.5/
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    10814 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/LICENSE.txt
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    13864 2023-08-03 18:41:09.885669 yoyodyne-0.2.5/PKG-INFO
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    13104 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/README.md
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     1277 2023-08-03 18:34:34.000000 yoyodyne-0.2.5/pyproject.toml
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)       38 2023-08-03 18:41:09.885669 yoyodyne-0.2.5/setup.cfg
+drwxr-xr-x   0 kbg      (304185) primarygroup (89939)        0 2023-08-03 18:41:09.881669 yoyodyne-0.2.5/yoyodyne/
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)      289 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/__init__.py
+drwxr-xr-x   0 kbg      (304185) primarygroup (89939)        0 2023-08-03 18:41:09.881669 yoyodyne-0.2.5/yoyodyne/data/
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     2431 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/data/__init__.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     3495 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/data/batches.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     5329 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/data/collators.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     6604 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/data/datamodules.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     6215 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/data/datasets.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     4486 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/data/indexes.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     4846 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/data/tsv.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)      943 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/defaults.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     5056 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/evaluators.py
+drwxr-xr-x   0 kbg      (304185) primarygroup (89939)        0 2023-08-03 18:41:09.881669 yoyodyne-0.2.5/yoyodyne/models/
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     1891 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/__init__.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    18644 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/base.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    17097 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/expert.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    13365 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/lstm.py
+drwxr-xr-x   0 kbg      (304185) primarygroup (89939)        0 2023-08-03 18:41:09.885669 yoyodyne-0.2.5/yoyodyne/models/modules/
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     3017 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/modules/__init__.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     3305 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/modules/attention.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     4502 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/modules/base.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     1442 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/modules/linear.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     7322 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/modules/lstm.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    10275 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/modules/transformer.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    14657 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/pointer_generator.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    21504 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/transducer.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     6461 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/models/transformer.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     4330 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/predict.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)     7644 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/schedulers.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)      169 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/special.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    10412 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/train.py
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)      599 2023-08-03 18:34:26.000000 yoyodyne-0.2.5/yoyodyne/util.py
+drwxr-xr-x   0 kbg      (304185) primarygroup (89939)        0 2023-08-03 18:41:09.881669 yoyodyne-0.2.5/yoyodyne.egg-info/
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)    13864 2023-08-03 18:41:09.000000 yoyodyne-0.2.5/yoyodyne.egg-info/PKG-INFO
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)      982 2023-08-03 18:41:09.000000 yoyodyne-0.2.5/yoyodyne.egg-info/SOURCES.txt
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)        1 2023-08-03 18:41:09.000000 yoyodyne-0.2.5/yoyodyne.egg-info/dependency_links.txt
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)       96 2023-08-03 18:41:09.000000 yoyodyne-0.2.5/yoyodyne.egg-info/entry_points.txt
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)       82 2023-08-03 18:41:09.000000 yoyodyne-0.2.5/yoyodyne.egg-info/requires.txt
+-rw-r--r--   0 kbg      (304185) primarygroup (89939)        9 2023-08-03 18:41:09.000000 yoyodyne-0.2.5/yoyodyne.egg-info/top_level.txt
```

### Comparing `yoyodyne-0.2.4/LICENSE.txt` & `yoyodyne-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/PKG-INFO` & `yoyodyne-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoyodyne
-Version: 0.2.4
+Version: 0.2.5
 Summary: Small-vocabulary neural sequence-to-sequence models
 Author: Adam Wiemerslage, Kyle Gorman, Travis Bartley
 License: Apache 2.0
 Project-URL: homepage, https://github.com/CUNY-CL/yoyodyne
 Keywords: computational linguistics,morphology,natural language processing,language
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -79,46 +79,48 @@
 must specify the following required arguments:
 
 -   `--model_dir`: path for model metadata and checkpoints
 -   `--experiment`: name of experiment (pick something unique)
 -   `--train`: path to TSV file containing training data
 -   `--val`: path to TSV file containing validation data
 
-The user can also specify various optional training and architectural
-arguments. See below or run [`yoyodyne-train --help`](yoyodyne/train.py) for
-more information.
+The user can also specify various optional training and architectural arguments.
+See below or run [`yoyodyne-train --help`](yoyodyne/train.py) for more
+information.
 
 ### Prediction
 
-Prediction is performed by the [`yoyodyne-predict`](yoyodyne/predict.py)
-script. One must specify the following required arguments:
+Prediction is performed by the [`yoyodyne-predict`](yoyodyne/predict.py) script.
+One must specify the following required arguments:
 
 -   `--model_dir`: path for model metadata
 -   `--experiment`: name of experiment
 -   `--checkpoint`: path to checkpoint
--   `--predict`: path to TSV file containing data to be predicted
+-   `--predict`: path to file containing data to be predicted
 -   `--output`: path for predictions
 
-Run [`yoyodyne-predict --help`](yoyodyne/predict.py) for more information.
+The `--predict` file can either be a TSV file or an ordinary TXT file with one
+source string per line; in the latter case, specify `--target_col 0`. Run
+[`yoyodyne-predict --help`](yoyodyne/predict.py) for more information.
 
 ## Data format
 
 The default data format is a two-column TSV file in which the first column is
 the source string and the second the target string.
 
     source   target
 
 To enable the use of a feature column, one specifies a (non-zero) argument to
-`--features-col`. For instance in the SIGMORPHON 2017 shared task, the first
+`--features_col`. For instance in the SIGMORPHON 2017 shared task, the first-
 column is the source (a lemma), the second is the target (the inflection), and
 the third contains semi-colon delimited feature strings:
 
     source   target    feat1;feat2;...
 
-this format is specified by `--features-col 3`.
+this format is specified by `--features_col 3`.
 
 Alternatively, for the [SIGMORPHON 2016 shared
 task](https://sigmorphon.github.io/sharedtasks/2016/) data:
 
     source   feat1,feat2,...    target
 
 this format is specified by `--features_col 2 --features_sep , --target_col 3`.
@@ -168,15 +170,16 @@
     parameter.
 -   `"lstm"`: This is an LSTM decoder with LSTM encoders (by default); in lieu
     of an attention mechanism, the last non-padding hidden state of the encoder
     is concatenated with the decoder hidden state.
 -   `pointer_generator_lstm`: This is an LSTM decoder with LSTM encoders (by
     default) and a pointer-generator mechanism. Since this model contains a copy
     mechanism, it may be superior to the `lstm` when the input and output
-    vocabularies overlap significantly.
+    vocabularies overlap significantly. Note that this model requires that the
+    number of `--encoder_layers` and `--decoder_layers` match.
 -   `"transducer"`: This is an LSTM decoder with LSTM encoders (by default) and
     a neural transducer mechanism. On model creation, expectation maximization
     is used to learn a sequence of edit operations, and imitation learning is
     used to train the model to implement the oracle policy, with roll-in
     controlled by the `--oracle_factor` flag (default: `1`). Since this model
     assumes monotonic alignment, it may be superior to attentive models when the
     alignment between input and output is roughly monotonic and when input and
```

### Comparing `yoyodyne-0.2.4/README.md` & `yoyodyne-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,46 +60,48 @@
 must specify the following required arguments:
 
 -   `--model_dir`: path for model metadata and checkpoints
 -   `--experiment`: name of experiment (pick something unique)
 -   `--train`: path to TSV file containing training data
 -   `--val`: path to TSV file containing validation data
 
-The user can also specify various optional training and architectural
-arguments. See below or run [`yoyodyne-train --help`](yoyodyne/train.py) for
-more information.
+The user can also specify various optional training and architectural arguments.
+See below or run [`yoyodyne-train --help`](yoyodyne/train.py) for more
+information.
 
 ### Prediction
 
-Prediction is performed by the [`yoyodyne-predict`](yoyodyne/predict.py)
-script. One must specify the following required arguments:
+Prediction is performed by the [`yoyodyne-predict`](yoyodyne/predict.py) script.
+One must specify the following required arguments:
 
 -   `--model_dir`: path for model metadata
 -   `--experiment`: name of experiment
 -   `--checkpoint`: path to checkpoint
--   `--predict`: path to TSV file containing data to be predicted
+-   `--predict`: path to file containing data to be predicted
 -   `--output`: path for predictions
 
-Run [`yoyodyne-predict --help`](yoyodyne/predict.py) for more information.
+The `--predict` file can either be a TSV file or an ordinary TXT file with one
+source string per line; in the latter case, specify `--target_col 0`. Run
+[`yoyodyne-predict --help`](yoyodyne/predict.py) for more information.
 
 ## Data format
 
 The default data format is a two-column TSV file in which the first column is
 the source string and the second the target string.
 
     source   target
 
 To enable the use of a feature column, one specifies a (non-zero) argument to
-`--features-col`. For instance in the SIGMORPHON 2017 shared task, the first
+`--features_col`. For instance in the SIGMORPHON 2017 shared task, the first-
 column is the source (a lemma), the second is the target (the inflection), and
 the third contains semi-colon delimited feature strings:
 
     source   target    feat1;feat2;...
 
-this format is specified by `--features-col 3`.
+this format is specified by `--features_col 3`.
 
 Alternatively, for the [SIGMORPHON 2016 shared
 task](https://sigmorphon.github.io/sharedtasks/2016/) data:
 
     source   feat1,feat2,...    target
 
 this format is specified by `--features_col 2 --features_sep , --target_col 3`.
@@ -149,15 +151,16 @@
     parameter.
 -   `"lstm"`: This is an LSTM decoder with LSTM encoders (by default); in lieu
     of an attention mechanism, the last non-padding hidden state of the encoder
     is concatenated with the decoder hidden state.
 -   `pointer_generator_lstm`: This is an LSTM decoder with LSTM encoders (by
     default) and a pointer-generator mechanism. Since this model contains a copy
     mechanism, it may be superior to the `lstm` when the input and output
-    vocabularies overlap significantly.
+    vocabularies overlap significantly. Note that this model requires that the
+    number of `--encoder_layers` and `--decoder_layers` match.
 -   `"transducer"`: This is an LSTM decoder with LSTM encoders (by default) and
     a neural transducer mechanism. On model creation, expectation maximization
     is used to learn a sequence of edit operations, and imitation learning is
     used to train the model to implement the oracle policy, with roll-in
     controlled by the `--oracle_factor` flag (default: `1`). Since this model
     assumes monotonic alignment, it may be superior to attentive models when the
     alignment between input and output is roughly monotonic and when input and
```

### Comparing `yoyodyne-0.2.4/pyproject.toml` & `yoyodyne-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.packages.find]
 include = ["yoyodyne*"]
 exclude = ["examples*"]
 
 [project]
 name = "yoyodyne"
-version = "0.2.4"
+version = "0.2.5"
 description = "Small-vocabulary neural sequence-to-sequence models"
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { text = "Apache 2.0" }
 authors = [
     {name = "Adam Wiemerslage"},
     {name = "Kyle Gorman"},
```

### Comparing `yoyodyne-0.2.4/yoyodyne/data/__init__.py` & `yoyodyne-0.2.5/yoyodyne/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,26 +54,14 @@
         type=str,
         default=defaults.FEATURES_SEP,
         help="String used to split features string into symbols; "
         "an empty string indicates that each Unicode codepoint "
         "is its own symbol. Default: %(default)r.",
     )
     parser.add_argument(
-        "--tied_vocabulary",
-        action="store_true",
-        default=defaults.TIED_VOCABULARY,
-        help="Share source and target embeddings. Default: %(default)s.",
-    )
-    parser.add_argument(
-        "--no_tied_vocabulary",
-        action="store_false",
-        dest="tied_vocabulary",
-        default=True,
-    )
-    parser.add_argument(
         "--batch_size",
         type=int,
         default=defaults.BATCH_SIZE,
         help="Batch size. Default: %(default)s.",
     )
     parser.add_argument(
         "--max_source_length",
```

### Comparing `yoyodyne-0.2.4/yoyodyne/data/batches.py` & `yoyodyne-0.2.5/yoyodyne/data/batches.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/data/collators.py` & `yoyodyne-0.2.5/yoyodyne/data/collators.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/data/datamodules.py` & `yoyodyne-0.2.5/yoyodyne/data/datamodules.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,16 +30,14 @@
         source_col: int = defaults.SOURCE_COL,
         features_col: int = defaults.FEATURES_COL,
         target_col: int = defaults.TARGET_COL,
         # String parsing arguments.
         source_sep: str = defaults.SOURCE_SEP,
         features_sep: str = defaults.FEATURES_SEP,
         target_sep: str = defaults.TARGET_SEP,
-        # Vocabulary options.
-        tied_vocabulary: bool = defaults.TIED_VOCABULARY,
         # Collator options.
         batch_size=defaults.BATCH_SIZE,
         separate_features: bool = False,
         max_source_length: int = defaults.MAX_SOURCE_LENGTH,
         max_target_length: int = defaults.MAX_TARGET_LENGTH,
         # Indexing.
         index: Optional[indexes.Index] = None,
@@ -55,55 +53,50 @@
         )
         self.train = train
         self.val = val
         self.predict = predict
         self.test = test
         self.batch_size = batch_size
         self.separate_features = separate_features
-        self.index = (
-            index if index is not None else self._make_index(tied_vocabulary)
-        )
+        self.index = index if index is not None else self._make_index()
         self.collator = collators.Collator(
             pad_idx=self.index.pad_idx,
-            has_features=self.index.has_features,
-            has_target=self.index.has_target,
+            has_features=self.has_features,
+            has_target=self.has_target,
             separate_features=separate_features,
             features_offset=self.index.source_vocab_size
-            if self.index.has_features
+            if self.has_features
             else 0,
             max_source_length=max_source_length,
             max_target_length=max_target_length,
         )
 
-    def _make_index(self, tied_vocabulary: bool) -> indexes.Index:
+    def _make_index(self) -> indexes.Index:
         # Computes index.
         source_vocabulary: Set[str] = set()
         features_vocabulary: Set[str] = set()
         target_vocabulary: Set[str] = set()
         for path in self.paths:
-            if self.parser.has_features:
-                if self.parser.has_target:
+            if self.has_features:
+                if self.has_target:
                     for source, features, target in self.parser.samples(path):
                         source_vocabulary.update(source)
                         features_vocabulary.update(features)
                         target_vocabulary.update(target)
                 else:
                     for source, features in self.parser.samples(path):
                         source_vocabulary.update(source)
                         features_vocabulary.update(features)
-            elif self.parser.has_target:
+            elif self.has_target:
                 for source, target in self.parser.samples(path):
                     source_vocabulary.update(source)
                     target_vocabulary.update(target)
             else:
                 for source in self.parser.samples(path):
                     source_vocabulary.update(source)
-            if self.parser.has_target and tied_vocabulary:
-                source_vocabulary.update(target_vocabulary)
-                target_vocabulary.update(source_vocabulary)
         return indexes.Index(
             source_vocabulary=sorted(source_vocabulary),
             features_vocabulary=sorted(features_vocabulary)
             if features_vocabulary
             else None,
             target_vocabulary=sorted(target_vocabulary)
             if target_vocabulary
@@ -122,34 +115,34 @@
             yield self.predict
         if self.test is not None:
             yield self.test
 
     def log_vocabularies(self) -> None:
         """Logs this module's vocabularies."""
         util.log_info(f"Source vocabulary: {self.index.source_map.pprint()}")
-        if self.index.has_features:
+        if self.has_features:
             util.log_info(
                 f"Features vocabulary: {self.index.features_map.pprint()}"
             )
-        if self.index.has_target:
+        if self.has_target:
             util.log_info(
                 f"Target vocabulary: {self.index.target_map.pprint()}"
             )
 
     def write_index(self, model_dir: str, experiment: str) -> None:
         """Writes the index."""
         self.index.write(model_dir, experiment)
 
     @property
     def has_features(self) -> int:
-        return self.index.has_features
+        return self.parser.has_features
 
     @property
     def has_target(self) -> int:
-        return self.index.has_target
+        return self.parser.has_target
 
     @property
     def source_vocab_size(self) -> int:
         if self.separate_features:
             return self.index.source_vocab_size
         else:
             return (
```

### Comparing `yoyodyne-0.2.4/yoyodyne/data/datasets.py` & `yoyodyne-0.2.5/yoyodyne/data/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,19 @@
 
     samples: List[List[str]]
     index: indexes.Index  # Usually copied from the DataModule.
     parser: tsv.TsvParser  # Ditto.
 
     @property
     def has_features(self) -> bool:
-        return self.index.has_features
+        return self.parser.has_features
 
     @property
     def has_target(self) -> bool:
-        return self.index.has_target
+        return self.parser.has_target
 
     def _encode(
         self,
         symbols: List[str],
         symbol_map: indexes.SymbolMap,
     ) -> torch.Tensor:
         """Encodes a sequence as a tensor of indices with string boundary IDs.
@@ -202,29 +202,30 @@
 
         Args:
             idx (int).
 
         Returns:
             Item.
         """
-        if self.index.has_features:
-            if self.index.has_target:
+        if self.has_features:
+            if self.has_target:
                 source, features, target = self.samples[idx]
                 return Item(
                     source=self.encode_source(source),
                     features=self.encode_features(features),
                     target=self.encode_target(target),
                 )
             else:
                 source, features = self.samples[idx]
                 return Item(
                     source=self.encode_source(source),
                     features=self.encode_features(features),
                 )
-        elif self.index.has_target:
+        elif self.has_target:
             source, target = self.samples[idx]
             return Item(
                 source=self.encode_source(source),
                 target=self.encode_target(target),
             )
         else:
+            source = self.samples[idx]
             return Item(source=self.encode_source(source))
```

### Comparing `yoyodyne-0.2.4/yoyodyne/data/indexes.py` & `yoyodyne-0.2.5/yoyodyne/data/indexes.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         """
         super().__init__()
         self.source_map = SymbolMap(source_vocabulary)
         self.features_map = (
             SymbolMap(features_vocabulary) if features_vocabulary else None
         )
         self.target_map = (
-            SymbolMap(target_vocabulary) if source_vocabulary else None
+            SymbolMap(target_vocabulary) if target_vocabulary else None
         )
 
     # Serialization support.
 
     @classmethod
     def read(cls, model_dir: str, experiment: str) -> "Index":
         """Loads index.
```

### Comparing `yoyodyne-0.2.4/yoyodyne/data/tsv.py` & `yoyodyne-0.2.5/yoyodyne/data/tsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,14 @@
 
     def __post_init__(self) -> None:
         # This is automatically called after initialization.
         if self.source_col < 1:
             raise Error(f"Out of range source column: {self.source_col}")
         if self.features_col < 0:
             raise Error(f"Out of range features column: {self.features_col}")
-        if self.features_col < 0:
-            raise Error(f"Out of range features column: {self.features_col}")
         if self.target_col < 0:
             raise Error(f"Out of range target column: {self.target_col}")
 
     @staticmethod
     def _tsv_reader(path: str) -> Iterator[str]:
         with open(path, "r") as tsv:
             yield from csv.reader(tsv, delimiter="\t")
```

### Comparing `yoyodyne-0.2.4/yoyodyne/defaults.py` & `yoyodyne-0.2.5/yoyodyne/defaults.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/evaluators.py` & `yoyodyne-0.2.5/yoyodyne/evaluators.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,69 @@
 """Evaluators."""
 
+from __future__ import annotations
+import dataclasses
+
 import torch
 from torch.nn import functional
 
 
 class Error(Exception):
     pass
 
 
+@dataclasses.dataclass
+class EvalItem:
+    num_correct: int
+    num_predicted: int
+
+    @property
+    def accuracy(self) -> float:
+        """Computes the accuracy."""
+        return self.num_correct / self.num_predicted
+
+    def __add__(self, other_eval: EvalItem) -> EvalItem:
+        """Adds two EvalItems by summing along both attributes.
+
+        Args:
+            other_eval (EvalItem): The other eval item to add to self.
+
+        Returns:
+            EvalItem.
+        """
+        return EvalItem(
+            self.num_correct + other_eval.num_correct,
+            self.num_predicted + other_eval.num_predicted,
+        )
+
+    def __radd__(self, start_val: int) -> EvalItem:
+        """Reverse add. Expects a zero-valued integer.
+
+        Args:
+            start_val (int): An initial value for calling the first add in an
+                iterable. Expected to be 0.
+
+        Returns:
+            EvalItem.
+        """
+        return EvalItem(
+            self.num_correct + start_val, self.num_predicted + start_val
+        )
+
+
 class Evaluator:
     """Evaluates predictions."""
 
-    def val_accuracy(
+    def evaluate(
         self,
         predictions: torch.Tensor,
         golds: torch.Tensor,
         end_idx: int,
         pad_idx: int,
-    ) -> float:
+    ) -> EvalItem:
         """Computes the exact word match accuracy.
 
         Args:
             predictions (torch.Tensor): B x vocab_size x seq_len.
             golds (torch.Tensor): B x seq_len x 1.
             end_idx (int): end of sequence index.
             pad_idx (int): padding index.
@@ -34,37 +76,37 @@
                 f"Preds batch size ({predictions.size(0)}) and "
                 f"golds batch size ({golds.size(0)} do not match"
             )
         # Gets the max value at each dim2 in predictions.
         _, predictions = torch.max(predictions, dim=2)
         # Finalizes the predictions.
         predictions = self.finalize_predictions(predictions, end_idx, pad_idx)
-        return self.accuracy(predictions, golds, pad_idx)
+        return self.get_eval_item(predictions, golds, pad_idx)
 
     @staticmethod
-    def accuracy(
+    def get_eval_item(
         predictions: torch.Tensor,
         golds: torch.Tensor,
         pad_idx: int,
-    ) -> float:
+    ) -> EvalItem:
         if predictions.size(1) > golds.size(1):
             predictions = predictions[:, : golds.size(1)]
         elif predictions.size(1) < golds.size(1):
             num_pads = (0, golds.size(1) - predictions.size(1))
             predictions = functional.pad(
                 predictions, num_pads, "constant", pad_idx
             )
         # Gets the count of exactly matching tensors in the batch.
         # -> B x max_seq_len.
         corr_count = torch.where(
             (predictions.to(golds.device) == golds).all(dim=1)
         )[0].size()[0]
-        # Gets the batch size (total_count).
-        total_count = predictions.size(0)
-        return corr_count / total_count
+        return EvalItem(
+            num_correct=corr_count, num_predicted=predictions.size(0)
+        )
 
     @staticmethod
     def finalize_predictions(
         predictions: torch.Tensor,
         end_idx: int,
         pad_idx: int,
     ) -> torch.Tensor:
```

### Comparing `yoyodyne-0.2.4/yoyodyne/models/__init__.py` & `yoyodyne-0.2.5/yoyodyne/models/__init__.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/base.py` & `yoyodyne-0.2.5/yoyodyne/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,40 +280,44 @@
         Returns:
             Dict[str, float]: validation metrics.
         """
         # Greedy decoding.
         # -> B x seq_len x target_vocab_size.
         target_padded = batch.target.padded
         greedy_predictions = self(batch)
-        accuracy = self.evaluator.val_accuracy(
+        val_eval_item = self.evaluator.evaluate(
             greedy_predictions, target_padded, self.end_idx, self.pad_idx
         )
         # -> B x target_vocab_size x seq_len. For loss.
         greedy_predictions = greedy_predictions.transpose(1, 2)
         # Truncates predictions to the size of the target.
         greedy_predictions = torch.narrow(
             greedy_predictions, 2, 0, target_padded.size(1)
         )
         loss = self.loss_func(greedy_predictions, target_padded)
-        return {"val_accuracy": accuracy, "val_loss": loss}
+        return {"val_eval_item": val_eval_item, "val_loss": loss}
 
     def validation_epoch_end(self, validation_step_outputs: Dict) -> Dict:
         """Computes average loss and average accuracy.
 
         Args:
             validation_step_outputs (Dict).
 
         Returns:
             Dict: averaged metrics over all validation steps.
         """
-        keys = validation_step_outputs[0].keys()
-        # Shortens name to do comprehension below.
-        # TODO: there has to be a more elegant way to do this.
-        V = validation_step_outputs
-        metrics = {k: sum([v[k] for v in V]) / len(V) for k in keys}
+        num_steps = len(validation_step_outputs)
+        avg_val_loss = (
+            sum([v["val_loss"] for v in validation_step_outputs]) / num_steps
+        )
+        epoch_eval = sum(v["val_eval_item"] for v in validation_step_outputs)
+        metrics = {
+            "val_loss": avg_val_loss,
+            "val_accuracy": epoch_eval.accuracy,
+        }
         for metric, value in metrics.items():
             self.log(metric, value, prog_bar=True)
         return metrics
 
     def predict_step(
         self,
         batch: data.PaddedBatch,
```

### Comparing `yoyodyne-0.2.4/yoyodyne/models/expert.py` & `yoyodyne-0.2.5/yoyodyne/models/expert.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/lstm.py` & `yoyodyne-0.2.5/yoyodyne/models/lstm.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/modules/__init__.py` & `yoyodyne-0.2.5/yoyodyne/models/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/modules/attention.py` & `yoyodyne-0.2.5/yoyodyne/models/modules/attention.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/modules/base.py` & `yoyodyne-0.2.5/yoyodyne/models/modules/base.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/modules/linear.py` & `yoyodyne-0.2.5/yoyodyne/models/modules/linear.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/modules/lstm.py` & `yoyodyne-0.2.5/yoyodyne/models/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/modules/transformer.py` & `yoyodyne-0.2.5/yoyodyne/models/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/models/pointer_generator.py` & `yoyodyne-0.2.5/yoyodyne/models/pointer_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,18 @@
     def _check_layer_sizes(self) -> None:
         """Checks that encoder and decoder layers are the same number.
 
         Raises:
             Error.
         """
         if self.encoder_layers != self.decoder_layers:
-            msg = "encoder_layers needs to be the same as decoder_layers."
-            msg += f" {self.encoder_layers} != {self.decoder_layers}."
-            raise Error(msg)
+            raise Error(
+                "The number of encoder and decoder layers must match "
+                f"({self.encoder_layers} != {self.decoder_layers})"
+            )
 
     def decode_step(
         self,
         symbol: torch.Tensor,
         last_hiddens: Tuple[torch.Tensor, torch.Tensor],
         source_indices: torch.Tensor,
         source_enc: torch.Tensor,
```

### Comparing `yoyodyne-0.2.4/yoyodyne/models/transducer.py` & `yoyodyne-0.2.5/yoyodyne/models/transducer.py`

 * *Files 2% similar despite different names*

```diff
@@ -529,20 +529,18 @@
         predictions, loss = self(batch)
         # Evaluation requires prediction as a tensor.
         predictions = self.convert_prediction(predictions)
         # Processes for accuracy calculation.
         predictions = self.evaluator.finalize_predictions(
             predictions, self.end_idx, self.pad_idx
         )
-        return {
-            "val_accuracy": self.evaluator.accuracy(
-                predictions, batch.target.padded, self.pad_idx
-            ),
-            "val_loss": loss,
-        }
+        val_eval_item = self.evaluator.get_eval_item(
+            predictions, batch.target.padded, self.pad_idx
+        )
+        return {"val_eval_item": val_eval_item, "val_loss": loss}
 
     def predict_step(self, batch: Tuple[torch.tensor], batch_idx: int) -> Dict:
         predictions, _ = self.forward(
             batch,
         )
         # Evaluation requires prediction tensor.
         return self.convert_prediction(predictions)
```

### Comparing `yoyodyne-0.2.4/yoyodyne/models/transformer.py` & `yoyodyne-0.2.5/yoyodyne/models/transformer.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/predict.py` & `yoyodyne-0.2.5/yoyodyne/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         batch_size=args.batch_size,
         source_col=args.source_col,
         features_col=args.features_col,
         target_col=args.target_col,
         source_sep=args.source_sep,
         features_sep=args.features_sep,
         target_sep=args.target_sep,
-        tied_vocabulary=args.tied_vocabulary,
         separate_features=separate_features,
         max_source_length=args.max_source_length,
         max_target_length=args.max_target_length,
         index=index,
     )
```

### Comparing `yoyodyne-0.2.4/yoyodyne/schedulers.py` & `yoyodyne-0.2.5/yoyodyne/schedulers.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne/train.py` & `yoyodyne-0.2.5/yoyodyne/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import argparse
 from typing import List, Optional
 
 import pytorch_lightning as pl
 import wandb
 from pytorch_lightning import callbacks, loggers
-from torch.utils import data as torch_data
 
 from . import data, defaults, models, schedulers, util
 
 
 class Error(Exception):
     pass
 
@@ -115,33 +114,34 @@
         batch_size=args.batch_size,
         source_col=args.source_col,
         features_col=args.features_col,
         target_col=args.target_col,
         source_sep=args.source_sep,
         features_sep=args.features_sep,
         target_sep=args.target_sep,
-        tied_vocabulary=args.tied_vocabulary,
         separate_features=separate_features,
         max_source_length=args.max_source_length,
         max_target_length=args.max_target_length,
     )
+    if not datamodule.has_target:
+        raise Error("No target column specified")
     datamodule.index.write(args.model_dir, args.experiment)
     datamodule.log_vocabularies()
     return datamodule
 
 
 def get_model_from_argparse_args(
     args: argparse.Namespace,
     datamodule: data.DataModule,
 ) -> models.BaseEncoderDecoder:
     """Creates the model.
 
     Args:
-        train_set (data.BaseDataset).
         args (argparse.Namespace).
+        datamodule (data.DataModule).
 
     Returns:
         models.BaseEncoderDecoder.
     """
     model_cls = models.get_model_cls(args.arch)
     source_encoder_cls = models.modules.get_encoder_cls(
         encoder_arch=args.source_encoder_arch, model_arch=args.arch
@@ -207,32 +207,30 @@
         target_vocab_size=datamodule.index.target_vocab_size,
     )
 
 
 def train(
     trainer: pl.Trainer,
     model: models.BaseEncoderDecoder,
-    train_loader: torch_data.DataLoader,
-    dev_loader: torch_data.DataLoader,
+    datamodule: data.DataModule,
     train_from: Optional[str] = None,
 ) -> str:
     """Trains the model.
 
     Args:
          trainer (pl.Trainer).
          model (models.BaseEncoderDecoder).
-         train_loader (data.DataLoader).
-         dev_loader (data.DataLoader).
+         datamodule (data.DataModule).
          train_from (str, optional): if specified, starts training from this
             checkpoint.
 
     Returns:
         str: path to best checkpoint.
     """
-    trainer.fit(model, train_loader, dev_loader, ckpt_path=train_from)
+    trainer.fit(model, datamodule, ckpt_path=train_from)
     ckp_callback = trainer.callbacks[-1]
     # TODO: feels flimsy.
     assert type(ckp_callback) is callbacks.ModelCheckpoint
     return ckp_callback.best_model_path
 
 
 def add_argparse_args(parser: argparse.ArgumentParser) -> None:
```

### Comparing `yoyodyne-0.2.4/yoyodyne/util.py` & `yoyodyne-0.2.5/yoyodyne/util.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.4/yoyodyne.egg-info/PKG-INFO` & `yoyodyne-0.2.5/yoyodyne.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoyodyne
-Version: 0.2.4
+Version: 0.2.5
 Summary: Small-vocabulary neural sequence-to-sequence models
 Author: Adam Wiemerslage, Kyle Gorman, Travis Bartley
 License: Apache 2.0
 Project-URL: homepage, https://github.com/CUNY-CL/yoyodyne
 Keywords: computational linguistics,morphology,natural language processing,language
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -79,46 +79,48 @@
 must specify the following required arguments:
 
 -   `--model_dir`: path for model metadata and checkpoints
 -   `--experiment`: name of experiment (pick something unique)
 -   `--train`: path to TSV file containing training data
 -   `--val`: path to TSV file containing validation data
 
-The user can also specify various optional training and architectural
-arguments. See below or run [`yoyodyne-train --help`](yoyodyne/train.py) for
-more information.
+The user can also specify various optional training and architectural arguments.
+See below or run [`yoyodyne-train --help`](yoyodyne/train.py) for more
+information.
 
 ### Prediction
 
-Prediction is performed by the [`yoyodyne-predict`](yoyodyne/predict.py)
-script. One must specify the following required arguments:
+Prediction is performed by the [`yoyodyne-predict`](yoyodyne/predict.py) script.
+One must specify the following required arguments:
 
 -   `--model_dir`: path for model metadata
 -   `--experiment`: name of experiment
 -   `--checkpoint`: path to checkpoint
--   `--predict`: path to TSV file containing data to be predicted
+-   `--predict`: path to file containing data to be predicted
 -   `--output`: path for predictions
 
-Run [`yoyodyne-predict --help`](yoyodyne/predict.py) for more information.
+The `--predict` file can either be a TSV file or an ordinary TXT file with one
+source string per line; in the latter case, specify `--target_col 0`. Run
+[`yoyodyne-predict --help`](yoyodyne/predict.py) for more information.
 
 ## Data format
 
 The default data format is a two-column TSV file in which the first column is
 the source string and the second the target string.
 
     source   target
 
 To enable the use of a feature column, one specifies a (non-zero) argument to
-`--features-col`. For instance in the SIGMORPHON 2017 shared task, the first
+`--features_col`. For instance in the SIGMORPHON 2017 shared task, the first-
 column is the source (a lemma), the second is the target (the inflection), and
 the third contains semi-colon delimited feature strings:
 
     source   target    feat1;feat2;...
 
-this format is specified by `--features-col 3`.
+this format is specified by `--features_col 3`.
 
 Alternatively, for the [SIGMORPHON 2016 shared
 task](https://sigmorphon.github.io/sharedtasks/2016/) data:
 
     source   feat1,feat2,...    target
 
 this format is specified by `--features_col 2 --features_sep , --target_col 3`.
@@ -168,15 +170,16 @@
     parameter.
 -   `"lstm"`: This is an LSTM decoder with LSTM encoders (by default); in lieu
     of an attention mechanism, the last non-padding hidden state of the encoder
     is concatenated with the decoder hidden state.
 -   `pointer_generator_lstm`: This is an LSTM decoder with LSTM encoders (by
     default) and a pointer-generator mechanism. Since this model contains a copy
     mechanism, it may be superior to the `lstm` when the input and output
-    vocabularies overlap significantly.
+    vocabularies overlap significantly. Note that this model requires that the
+    number of `--encoder_layers` and `--decoder_layers` match.
 -   `"transducer"`: This is an LSTM decoder with LSTM encoders (by default) and
     a neural transducer mechanism. On model creation, expectation maximization
     is used to learn a sequence of edit operations, and imitation learning is
     used to train the model to implement the oracle policy, with roll-in
     controlled by the `--oracle_factor` flag (default: `1`). Since this model
     assumes monotonic alignment, it may be superior to attentive models when the
     alignment between input and output is roughly monotonic and when input and
```

### Comparing `yoyodyne-0.2.4/yoyodyne.egg-info/SOURCES.txt` & `yoyodyne-0.2.5/yoyodyne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

