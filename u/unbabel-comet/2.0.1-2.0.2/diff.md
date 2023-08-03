# Comparing `tmp/unbabel_comet-2.0.1.tar.gz` & `tmp/unbabel_comet-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbabel_comet-2.0.1.tar", max compression
+gzip compressed data, was "unbabel_comet-2.0.2.tar", max compression
```

## Comparing `unbabel_comet-2.0.1.tar` & `unbabel_comet-2.0.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     1838 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     9693 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/LICENSE
--rw-r--r--   0        0        0      710 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/LICENSE.models.md
--rw-r--r--   0        0        0    10006 2023-04-05 10:26:50.752727 unbabel_comet-2.0.1/README.md
--rw-r--r--   0        0        0      865 2023-04-05 10:26:50.752727 unbabel_comet-2.0.1/comet/__init__.py
--rw-r--r--   0        0        0    18409 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/cli/compare.py
--rw-r--r--   0        0        0    11152 2023-03-13 16:07:18.807044 unbabel_comet-2.0.1/comet/cli/mbr.py
--rw-r--r--   0        0        0     9970 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/cli/score.py
--rw-r--r--   0        0        0     6902 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/cli/train.py
--rw-r--r--   0        0        0      913 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/encoders/__init__.py
--rw-r--r--   0        0        0    12946 2023-03-06 13:43:56.436008 unbabel_comet-2.0.1/comet/encoders/base.py
--rw-r--r--   0        0        0     5438 2023-03-06 15:21:37.258210 unbabel_comet-2.0.1/comet/encoders/bert.py
--rw-r--r--   0        0        0     2229 2023-03-06 15:21:37.258210 unbabel_comet-2.0.1/comet/encoders/minilm.py
--rw-r--r--   0        0        0     2458 2023-03-06 15:21:37.258210 unbabel_comet-2.0.1/comet/encoders/rembert.py
--rw-r--r--   0        0        0     3210 2023-03-06 15:21:37.258210 unbabel_comet-2.0.1/comet/encoders/xlmr.py
--rw-r--r--   0        0        0     2382 2023-03-06 15:21:37.258210 unbabel_comet-2.0.1/comet/encoders/xlmr_xl.py
--rw-r--r--   0        0        0     2402 2023-03-21 13:52:45.773748 unbabel_comet-2.0.1/comet/models/__init__.py
--rw-r--r--   0        0        0    24277 2023-03-21 14:21:21.159077 unbabel_comet-2.0.1/comet/models/base.py
--rw-r--r--   0        0        0     9275 2023-04-05 10:26:50.752727 unbabel_comet-2.0.1/comet/models/lru_cache.py
--rw-r--r--   0        0        0     5488 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/models/metrics.py
--rw-r--r--   0        0        0        0 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/models/multitask/__init__.py
--rw-r--r--   0        0        0    27341 2023-03-13 16:07:10.309887 unbabel_comet-2.0.1/comet/models/multitask/unified_metric.py
--rw-r--r--   0        0        0     2625 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/models/pooling_utils.py
--rw-r--r--   0        0        0     1198 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/models/predict_pbar.py
--rw-r--r--   0        0        0     4620 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/models/predict_writer.py
--rw-r--r--   0        0        0        0 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/models/ranking/__init__.py
--rw-r--r--   0        0        0    15768 2023-03-06 15:21:37.258210 unbabel_comet-2.0.1/comet/models/ranking/ranking_metric.py
--rw-r--r--   0        0        0        0 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/models/regression/__init__.py
--rw-r--r--   0        0        0     9299 2023-03-06 15:21:37.258210 unbabel_comet-2.0.1/comet/models/regression/referenceless.py
--rw-r--r--   0        0        0    12520 2023-03-06 15:21:37.262210 unbabel_comet-2.0.1/comet/models/regression/regression_metric.py
--rw-r--r--   0        0        0     2088 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/models/utils.py
--rw-r--r--   0        0        0      104 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/modules/__init__.py
--rw-r--r--   0        0        0     2621 2023-03-06 13:40:11.489441 unbabel_comet-2.0.1/comet/modules/feedforward.py
--rw-r--r--   0        0        0     5455 2023-03-21 12:10:36.161626 unbabel_comet-2.0.1/comet/modules/layerwise_attention.py
--rw-r--r--   0        0        0     1500 2023-04-05 09:08:01.441474 unbabel_comet-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    11510 1970-01-01 00:00:00.000000 unbabel_comet-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1838 2023-02-22 09:47:15.116011 unbabel_comet-2.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     9693 2023-02-21 11:09:52.986089 unbabel_comet-2.0.2/LICENSE
+-rw-r--r--   0        0        0      756 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/LICENSE.models.md
+-rw-r--r--   0        0        0    10233 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/README.md
+-rw-r--r--   0        0        0      865 2023-08-03 12:36:10.488726 unbabel_comet-2.0.2/comet/__init__.py
+-rw-r--r--   0        0        0    18409 2023-02-22 09:47:15.116011 unbabel_comet-2.0.2/comet/cli/compare.py
+-rw-r--r--   0        0        0    11152 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/cli/mbr.py
+-rw-r--r--   0        0        0     9970 2023-02-22 09:47:15.116011 unbabel_comet-2.0.2/comet/cli/score.py
+-rw-r--r--   0        0        0     6902 2023-02-21 11:09:52.986089 unbabel_comet-2.0.2/comet/cli/train.py
+-rw-r--r--   0        0        0      913 2023-02-22 09:47:15.116011 unbabel_comet-2.0.2/comet/encoders/__init__.py
+-rw-r--r--   0        0        0    12946 2023-02-21 11:09:52.986089 unbabel_comet-2.0.2/comet/encoders/base.py
+-rw-r--r--   0        0        0     5438 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/encoders/bert.py
+-rw-r--r--   0        0        0     2229 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/encoders/minilm.py
+-rw-r--r--   0        0        0     2458 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/encoders/rembert.py
+-rw-r--r--   0        0        0     3210 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/encoders/xlmr.py
+-rw-r--r--   0        0        0     2382 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/encoders/xlmr_xl.py
+-rw-r--r--   0        0        0     3370 2023-08-03 13:55:36.687511 unbabel_comet-2.0.2/comet/models/__init__.py
+-rw-r--r--   0        0        0    24277 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/models/base.py
+-rw-r--r--   0        0        0     8629 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/models/download_utils.py
+-rw-r--r--   0        0        0     9275 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/models/lru_cache.py
+-rw-r--r--   0        0        0     5488 2023-02-21 11:09:52.986089 unbabel_comet-2.0.2/comet/models/metrics.py
+-rw-r--r--   0        0        0        0 2023-02-21 11:09:52.986089 unbabel_comet-2.0.2/comet/models/multitask/__init__.py
+-rw-r--r--   0        0        0    27341 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/models/multitask/unified_metric.py
+-rw-r--r--   0        0        0     2625 2023-02-21 11:09:52.990089 unbabel_comet-2.0.2/comet/models/pooling_utils.py
+-rw-r--r--   0        0        0     1198 2023-02-21 11:09:52.990089 unbabel_comet-2.0.2/comet/models/predict_pbar.py
+-rw-r--r--   0        0        0     4620 2023-02-22 09:47:15.116011 unbabel_comet-2.0.2/comet/models/predict_writer.py
+-rw-r--r--   0        0        0        0 2023-02-21 11:09:52.990089 unbabel_comet-2.0.2/comet/models/ranking/__init__.py
+-rw-r--r--   0        0        0    15768 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/models/ranking/ranking_metric.py
+-rw-r--r--   0        0        0        0 2023-02-21 11:09:52.990089 unbabel_comet-2.0.2/comet/models/regression/__init__.py
+-rw-r--r--   0        0        0     9299 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/models/regression/referenceless.py
+-rw-r--r--   0        0        0    12520 2023-08-03 12:30:40.361053 unbabel_comet-2.0.2/comet/models/regression/regression_metric.py
+-rw-r--r--   0        0        0     2088 2023-02-22 09:47:15.116011 unbabel_comet-2.0.2/comet/models/utils.py
+-rw-r--r--   0        0        0      104 2023-02-21 11:09:52.990089 unbabel_comet-2.0.2/comet/modules/__init__.py
+-rw-r--r--   0        0        0     2621 2023-02-21 11:09:52.990089 unbabel_comet-2.0.2/comet/modules/feedforward.py
+-rw-r--r--   0        0        0     5455 2023-08-03 12:30:40.365053 unbabel_comet-2.0.2/comet/modules/layerwise_attention.py
+-rw-r--r--   0        0        0     1501 2023-08-03 12:36:06.776640 unbabel_comet-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11901 1970-01-01 00:00:00.000000 unbabel_comet-2.0.2/setup.py
+-rw-r--r--   0        0        0    11730 1970-01-01 00:00:00.000000 unbabel_comet-2.0.2/PKG-INFO
```

### Comparing `unbabel_comet-2.0.1/CONTRIBUTING.md` & `unbabel_comet-2.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/LICENSE` & `unbabel_comet-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/LICENSE.models.md` & `unbabel_comet-2.0.2/LICENSE.models.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Model Licenses:
 
 All models released before version 2.0 are licensed under Apache 2.0.
 
-Starting at version 2.0 new models will be hosted on [Hugging Face Hub](https://huggingface.co/docs/hub/index) and have specific licenses.
+Starting at version 2.0 new models will be hosted on [Hugging Face Hub](https://huggingface.co/docs/hub/index) and have specific licenses. You can find the license of each model in it's Hub page. E.g:
 
 | Model | License |
 |:----: | :-----: |
 | **Default model:** [`Unbabel/wmt22-comet-da`](https://huggingface.co/Unbabel/wmt22-comet-da) | [Apache-2.0](https://huggingface.co/Unbabel/wmt22-comet-da/blob/main/LICENSE) | 
-| **Upcoming model:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/Unbabel/wmt22-cometkiwi-da) | [CC-BY-NC-SA](https://huggingface.co/Unbabel/wmt22-cometkiwi-da/blob/main/LICENSE) |
+| **Reference-free:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/Unbabel/wmt22-cometkiwi-da) | [CC-BY-NC-SA](https://huggingface.co/Unbabel/wmt22-cometkiwi-da/blob/main/LICENSE) |
 
-Please check the [model licenses](LICENSE.models.md) before using it.
+Please check the `models licenses` before using them.
```

### Comparing `unbabel_comet-2.0.1/README.md` & `unbabel_comet-2.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
   <br />
   <a href="https://github.com/Unbabel/COMET/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/github/license/Unbabel/COMET" /></a>
   <a href="https://github.com/Unbabel/COMET/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/Unbabel/COMET" /></a>
   <a href=""><img alt="PyPI" src="https://img.shields.io/pypi/v/unbabel-comet" /></a>
   <a href="https://github.com/psf/black"><img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-black" /></a>
 </p>
 
+**NEWS:** CometKiwi model from WMT22 is officially released and available on Hugging Face Hub. Please check all [available models here](https://github.com/Unbabel/COMET/blob/master/MODELS.md)
+ 
 # Quick Installation
 
 COMET requires python 3.8 or above! 
 
 Simple installation from PyPI
 
 ```bash
@@ -68,18 +70,18 @@
 ```bash
 comet-score -s src.de -t hyp1.en -r ref.en --quiet --only_system
 ```
 
 ### Reference-free evaluation:
 
 ```bash
-comet-score -s src.de -t hyp1.en --model Unbabel/wmt20-comet-qe-da
+comet-score -s src.de -t hyp1.en --model Unbabel/wmt22-cometkiwi-da
 ```
 
-**Note:** We are currently working on Licensing and releasing `Unbabel/wmt22-cometkiwi-da` but meanwhile that models is not available.
+**Note:** To use the `Unbabel/wmt22-cometkiwi-da` you first have to acknowledge its license on [Hugging Face Hub](https://huggingface.co/Unbabel/wmt22-cometkiwi-da).
 
 ### Comparing multiple systems:
 
 When comparing multiple MT systems we encourage you to run the `comet-compare` command to get **statistical significance** with Paired T-Test and bootstrap resampling [(Koehn, et al 2004)](https://aclanthology.org/W04-3250/).
 
 ```bash
 comet-compare -s src.de -t hyp1.en hyp2.en hyp3.en -r ref.en
@@ -94,23 +96,23 @@
 ```
 
 If working with a very large candidate list you can use `--rerank_top_k` flag to prune the topK most promissing candidates according to a reference-free metric.
 
 Example for a candidate list of 1000 samples:
 
 ```bash
-comet-mbr -s [SOURCE].txt -t [MT_SAMPLES].txt -o [OUTPUT_FILE].txt --num_sample 1000 --rerank_top_k 100 --gpus 4 --qe_model Unbabel/wmt20-comet-qe-da
+comet-mbr -s [SOURCE].txt -t [MT_SAMPLES].txt -o [OUTPUT_FILE].txt --num_sample 1000 --rerank_top_k 100 --gpus 4 --qe_model Unbabel/wmt22-cometkiwi-da
 ```
 
 # COMET Models:
 
 To evaluate your translations, we suggest using one of two models:
 
 - **Default model:** [`Unbabel/wmt22-comet-da`](https://huggingface.co/Unbabel/wmt22-comet-da) - This model uses a reference-based regression approach and is built on top of XLM-R. It has been trained on direct assessments from WMT17 to WMT20 and provides scores ranging from 0 to 1, where 1 represents a perfect translation.
-- **Upcoming model:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/Unbabel/wmt22-cometkiwi-da) - This reference-free model uses a regression approach and is built on top of InfoXLM. It has been trained on direct assessments from WMT17 to WMT20, as well as direct assessments from the MLQE-PE corpus. Like the default model, it also provides scores ranging from 0 to 1.
+- **Reference-free:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/Unbabel/wmt22-cometkiwi-da) - This reference-free model uses a regression approach and is built on top of InfoXLM. It has been trained on direct assessments from WMT17 to WMT20, as well as direct assessments from the MLQE-PE corpus. Like the default model, it also provides scores ranging from 0 to 1.
 
 For versions prior to 2.0, you can still use [`Unbabel/wmt20-comet-da`](https://huggingface.co/Unbabel/wmt20-comet-da), which is the primary metric, and [`Unbabel/wmt20-comet-qe-da`](https://huggingface.co/Unbabel/wmt20-comet-qe-da) for the **respective reference-free version**. You can find a list of all other models developed in previous versions on our [MODELS](MODELS.md) page. For more information, please refer to the [model licenses](LICENSE.models.md).
 
 ## Interpreting Scores:
 
 When using COMET to evaluate machine translation, it's important to understand how to interpret the scores it produces.
```

#### html2text {}

```diff
@@ -1,53 +1,56 @@
  [https://raw.githubusercontent.com/Unbabel/COMET/master/docs/source/_static/
                           img/COMET_lockup-dark.png]
 
                  [License] [GitHub_stars] [PyPI] [Code_Style]
-# Quick Installation COMET requires python 3.8 or above! Simple installation
-from PyPI ```bash pip install --upgrade pip # ensures that pip is current pip
-install unbabel-comet ``` To develop locally install run the following
-commands: ```bash git clone https://github.com/Unbabel/COMET cd COMET pip
-install poetry poetry install ``` For development, you can run the CLI tools
-directly, e.g., ```bash PYTHONPATH=. ./comet/cli/score.py ``` # Scoring MT
-outputs: ## CLI Usage: Test examples: ```bash echo -e "Dem Feuer konnte Einhalt
-geboten werden\nSchulen und KindergÃ¤rten wurden erÃ¶ffnet." >> src.de echo -
-e "The fire could be stopped\nSchools and kindergartens were open" >> hyp1.en
-echo -e "The fire could have been stopped\nSchools and pre-school were open" >>
-hyp2.en echo -e "They were able to control the fire.\nSchools and kindergartens
-opened" >> ref.en ``` Basic scoring command: ```bash comet-score -s src.de -
-t hyp1.en -r ref.en ``` > you can set the number of gpus using `--gpus` (0 to
-test on CPU). Scoring multiple systems: ```bash comet-score -s src.de -
-t hyp1.en hyp2.en -r ref.en ``` WMT test sets via [SacreBLEU](https://
-github.com/mjpost/sacrebleu): ```bash comet-score -d wmt22:en-de -t PATH/TO/
-TRANSLATIONS ``` If you are only interested in a system-level score use the
-following command: ```bash comet-score -s src.de -t hyp1.en -r ref.en --quiet -
--only_system ``` ### Reference-free evaluation: ```bash comet-score -s src.de -
-t hyp1.en --model Unbabel/wmt20-comet-qe-da ``` **Note:** We are currently
-working on Licensing and releasing `Unbabel/wmt22-cometkiwi-da` but meanwhile
-that models is not available. ### Comparing multiple systems: When comparing
-multiple MT systems we encourage you to run the `comet-compare` command to get
+**NEWS:** CometKiwi model from WMT22 is officially released and available on
+Hugging Face Hub. Please check all [available models here](https://github.com/
+Unbabel/COMET/blob/master/MODELS.md) # Quick Installation COMET requires python
+3.8 or above! Simple installation from PyPI ```bash pip install --upgrade pip #
+ensures that pip is current pip install unbabel-comet ``` To develop locally
+install run the following commands: ```bash git clone https://github.com/
+Unbabel/COMET cd COMET pip install poetry poetry install ``` For development,
+you can run the CLI tools directly, e.g., ```bash PYTHONPATH=. ./comet/cli/
+score.py ``` # Scoring MT outputs: ## CLI Usage: Test examples: ```bash echo -
+e "Dem Feuer konnte Einhalt geboten werden\nSchulen und KindergÃ¤rten wurden
+erÃ¶ffnet." >> src.de echo -e "The fire could be stopped\nSchools and
+kindergartens were open" >> hyp1.en echo -e "The fire could have been
+stopped\nSchools and pre-school were open" >> hyp2.en echo -e "They were able
+to control the fire.\nSchools and kindergartens opened" >> ref.en ``` Basic
+scoring command: ```bash comet-score -s src.de -t hyp1.en -r ref.en ``` > you
+can set the number of gpus using `--gpus` (0 to test on CPU). Scoring multiple
+systems: ```bash comet-score -s src.de -t hyp1.en hyp2.en -r ref.en ``` WMT
+test sets via [SacreBLEU](https://github.com/mjpost/sacrebleu): ```bash comet-
+score -d wmt22:en-de -t PATH/TO/TRANSLATIONS ``` If you are only interested in
+a system-level score use the following command: ```bash comet-score -s src.de -
+t hyp1.en -r ref.en --quiet --only_system ``` ### Reference-free evaluation:
+```bash comet-score -s src.de -t hyp1.en --model Unbabel/wmt22-cometkiwi-da ```
+**Note:** To use the `Unbabel/wmt22-cometkiwi-da` you first have to acknowledge
+its license on [Hugging Face Hub](https://huggingface.co/Unbabel/wmt22-
+cometkiwi-da). ### Comparing multiple systems: When comparing multiple MT
+systems we encourage you to run the `comet-compare` command to get
 **statistical significance** with Paired T-Test and bootstrap resampling [
 (Koehn, et al 2004)](https://aclanthology.org/W04-3250/). ```bash comet-compare
 -s src.de -t hyp1.en hyp2.en hyp3.en -r ref.en ``` ### Minimum Bayes Risk
 Decoding: The MBR command allows you to rank translations and select the best
 one according to COMET metrics. For more details you can read our paper on
 [Quality-Aware Decoding for Neural Machine Translation](https://
 aclanthology.org/2022.naacl-main.100.pdf). ```bash comet-mbr -s [SOURCE].txt -
 t [MT_SAMPLES].txt --num_sample [X] -o [OUTPUT_FILE].txt ``` If working with a
 very large candidate list you can use `--rerank_top_k` flag to prune the topK
 most promissing candidates according to a reference-free metric. Example for a
 candidate list of 1000 samples: ```bash comet-mbr -s [SOURCE].txt -t
 [MT_SAMPLES].txt -o [OUTPUT_FILE].txt --num_sample 1000 --rerank_top_k 100 --
-gpus 4 --qe_model Unbabel/wmt20-comet-qe-da ``` # COMET Models: To evaluate
+gpus 4 --qe_model Unbabel/wmt22-cometkiwi-da ``` # COMET Models: To evaluate
 your translations, we suggest using one of two models: - **Default model:**
 [`Unbabel/wmt22-comet-da`](https://huggingface.co/Unbabel/wmt22-comet-da) -
 This model uses a reference-based regression approach and is built on top of
 XLM-R. It has been trained on direct assessments from WMT17 to WMT20 and
 provides scores ranging from 0 to 1, where 1 represents a perfect translation.
-- **Upcoming model:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/
+- **Reference-free:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/
 Unbabel/wmt22-cometkiwi-da) - This reference-free model uses a regression
 approach and is built on top of InfoXLM. It has been trained on direct
 assessments from WMT17 to WMT20, as well as direct assessments from the MLQE-PE
 corpus. Like the default model, it also provides scores ranging from 0 to 1.
 For versions prior to 2.0, you can still use [`Unbabel/wmt20-comet-da`](https:/
 /huggingface.co/Unbabel/wmt20-comet-da), which is the primary metric, and
 [`Unbabel/wmt20-comet-qe-da`](https://huggingface.co/Unbabel/wmt20-comet-qe-da)
```

### Comparing `unbabel_comet-2.0.1/comet/__init__.py` & `unbabel_comet-2.0.2/comet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
 from .models import load_from_checkpoint, download_model
 
 logging.basicConfig(level=logging.INFO, format="%(message)s")
 logger = logging.getLogger(__name__)
 
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 __copyright__ = "2020 Unbabel. All rights reserved."
```

### Comparing `unbabel_comet-2.0.1/comet/cli/compare.py` & `unbabel_comet-2.0.2/comet/cli/compare.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/cli/mbr.py` & `unbabel_comet-2.0.2/comet/cli/mbr.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/cli/score.py` & `unbabel_comet-2.0.2/comet/cli/score.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/cli/train.py` & `unbabel_comet-2.0.2/comet/cli/train.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/encoders/__init__.py` & `unbabel_comet-2.0.2/comet/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/encoders/base.py` & `unbabel_comet-2.0.2/comet/encoders/base.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/encoders/bert.py` & `unbabel_comet-2.0.2/comet/encoders/bert.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/encoders/minilm.py` & `unbabel_comet-2.0.2/comet/encoders/minilm.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/encoders/rembert.py` & `unbabel_comet-2.0.2/comet/encoders/rembert.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/encoders/xlmr.py` & `unbabel_comet-2.0.2/comet/encoders/xlmr.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/encoders/xlmr_xl.py` & `unbabel_comet-2.0.2/comet/encoders/xlmr_xl.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/__init__.py` & `unbabel_comet-2.0.2/comet/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,58 +13,83 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 from pathlib import Path
 from typing import Union
 
+import torch
 import yaml
 from huggingface_hub import snapshot_download
 
 from .base import CometModel
 from .multitask.unified_metric import UnifiedMetric
 from .ranking.ranking_metric import RankingMetric
 from .regression.referenceless import ReferencelessRegression
 from .regression.regression_metric import RegressionMetric
+from .download_utils import download_model_legacy
+
 
 str2model = {
     "referenceless_regression_metric": ReferencelessRegression,
     "regression_metric": RegressionMetric,
     "ranking_metric": RankingMetric,
     "unified_metric": UnifiedMetric,
 }
 
+
 def download_model(
-    model: str, 
-    saving_directory: Union[str, Path, None] = None
+    model: str,
+    saving_directory: Union[str, Path, None] = None,
+    local_files_only: bool = False,
 ) -> str:
-    model_path = snapshot_download(repo_id=model, cache_dir=saving_directory)
-    checkpoint_path = os.path.join(*[model_path, "checkpoints", "model.ckpt"])
+    try:
+        model_path = snapshot_download(
+            repo_id=model, cache_dir=saving_directory, local_files_only=local_files_only
+        )
+    except Exception:
+        try:
+            checkpoint_path = download_model_legacy(model, saving_directory)
+        except Exception:
+            raise KeyError(f"Model '{model}' not supported by COMET.")
+    else:
+        checkpoint_path = os.path.join(*[model_path, "checkpoints", "model.ckpt"])
     return checkpoint_path
 
-def load_from_checkpoint(checkpoint_path: str) -> CometModel:
+
+def load_from_checkpoint(
+    checkpoint_path: str, reload_hparams: bool = False, strict: bool = False
+) -> CometModel:
     """Loads models from a checkpoint path.
 
     Args:
         checkpoint_path (str): Path to a model checkpoint.
-
+        reload_hparams (bool): hparams.yaml file located in the parent folder is
+            only use for deciding the `class_identifier`. By setting this flag
+            to True all hparams will be reloaded.
+        strict (bool): Strictly enforce that the keys in checkpoint_path match the
+            keys returned by this module's state dict. Defaults to False
     Return:
         COMET model.
     """
     checkpoint_path = Path(checkpoint_path)
 
     if not checkpoint_path.is_file():
         raise Exception(f"Invalid checkpoint path: {checkpoint_path}")
-    
-    parent_folder = checkpoint_path.parents[1] # .parent.parent
+
+    parent_folder = checkpoint_path.parents[1]  # .parent.parent
     hparams_file = parent_folder / "hparams.yaml"
 
     if hparams_file.is_file():
         with open(hparams_file) as yaml_file:
             hparams = yaml.load(yaml_file.read(), Loader=yaml.FullLoader)
         model_class = str2model[hparams["class_identifier"]]
         model = model_class.load_from_checkpoint(
-            checkpoint_path, load_pretrained_weights=False
+            checkpoint_path,
+            load_pretrained_weights=False,
+            hparams_file=hparams_file if reload_hparams else None,
+            map_location=torch.device("cpu"),
+            strict=strict,
         )
         return model
     else:
         raise Exception(f"hparams.yaml file is missing from {parent_folder}!")
```

### Comparing `unbabel_comet-2.0.1/comet/models/base.py` & `unbabel_comet-2.0.2/comet/models/base.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/lru_cache.py` & `unbabel_comet-2.0.2/comet/models/lru_cache.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/metrics.py` & `unbabel_comet-2.0.2/comet/models/metrics.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/multitask/unified_metric.py` & `unbabel_comet-2.0.2/comet/models/multitask/unified_metric.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/pooling_utils.py` & `unbabel_comet-2.0.2/comet/models/pooling_utils.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/predict_pbar.py` & `unbabel_comet-2.0.2/comet/models/predict_pbar.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/predict_writer.py` & `unbabel_comet-2.0.2/comet/models/predict_writer.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/ranking/ranking_metric.py` & `unbabel_comet-2.0.2/comet/models/ranking/ranking_metric.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/regression/referenceless.py` & `unbabel_comet-2.0.2/comet/models/regression/referenceless.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/regression/regression_metric.py` & `unbabel_comet-2.0.2/comet/models/regression/regression_metric.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/models/utils.py` & `unbabel_comet-2.0.2/comet/models/utils.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/modules/feedforward.py` & `unbabel_comet-2.0.2/comet/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/comet/modules/layerwise_attention.py` & `unbabel_comet-2.0.2/comet/modules/layerwise_attention.py`

 * *Files identical despite different names*

### Comparing `unbabel_comet-2.0.1/pyproject.toml` & `unbabel_comet-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unbabel-comet"
-version = "2.0.1"
+version = "2.0.2"
 description = "High-quality Machine Translation Evaluation"
 authors = ["Ricardo Rei, Craig Stewart, Catarina Farinha, Alon Lavie"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Unbabel/COMET"
 repository = "https://github.com/Unbabel/COMET"
 documentation = "https://unbabel.github.io/COMET/html/index.html"
@@ -34,25 +34,25 @@
 comet-score = 'comet.cli.score:score_command'
 comet-compare = 'comet.cli.compare:compare_command'
 comet-mbr = 'comet.cli.mbr:mbr_command'
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 sentencepiece = "^0.1.96"
-pandas = "^1.4.1"
+pandas = ">=1.4.1"
 transformers = "^4.17"
 pytorch-lightning = "^1.6.4"
 jsonargparse = "3.13.1"
 torch = ">=1.6.0"
 numpy = "^1.20.0"
 torchmetrics = "0.8.2"
 sacrebleu = "^2.0.0"
 scipy = "^1.5.4"
 entmax = "^1.1"
-huggingface-hub = "^0.12.0"
+huggingface-hub = "^0.16.0"
 
 [tool.poetry.dev-dependencies]
 sphinx-markdown-tables = "0.0.15"
 coverage = "^5.5"
 scikit-learn = "0.24"
 
 [build-system]
```

### Comparing `unbabel_comet-2.0.1/PKG-INFO` & `unbabel_comet-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbabel-comet
-Version: 2.0.1
+Version: 2.0.2
 Summary: High-quality Machine Translation Evaluation
 Home-page: https://github.com/Unbabel/COMET
 License: Apache-2.0
 Keywords: Machine Translation,Evaluation,Unbabel,COMET
 Author: Ricardo Rei, Craig Stewart, Catarina Farinha, Alon Lavie
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: entmax (>=1.1,<2.0)
-Requires-Dist: huggingface-hub (>=0.12.0,<0.13.0)
+Requires-Dist: huggingface-hub (>=0.16.0,<0.17.0)
 Requires-Dist: jsonargparse (==3.13.1)
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
-Requires-Dist: pandas (>=1.4.1,<2.0.0)
+Requires-Dist: pandas (>=1.4.1)
 Requires-Dist: pytorch-lightning (>=1.6.4,<2.0.0)
 Requires-Dist: sacrebleu (>=2.0.0,<3.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0)
 Requires-Dist: sentencepiece (>=0.1.96,<0.2.0)
 Requires-Dist: torch (>=1.6.0)
 Requires-Dist: torchmetrics (==0.8.2)
 Requires-Dist: transformers (>=4.17,<5.0)
@@ -39,14 +39,16 @@
   <br />
   <a href="https://github.com/Unbabel/COMET/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/github/license/Unbabel/COMET" /></a>
   <a href="https://github.com/Unbabel/COMET/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/Unbabel/COMET" /></a>
   <a href=""><img alt="PyPI" src="https://img.shields.io/pypi/v/unbabel-comet" /></a>
   <a href="https://github.com/psf/black"><img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-black" /></a>
 </p>
 
+**NEWS:** CometKiwi model from WMT22 is officially released and available on Hugging Face Hub. Please check all [available models here](https://github.com/Unbabel/COMET/blob/master/MODELS.md)
+ 
 # Quick Installation
 
 COMET requires python 3.8 or above! 
 
 Simple installation from PyPI
 
 ```bash
@@ -103,18 +105,18 @@
 ```bash
 comet-score -s src.de -t hyp1.en -r ref.en --quiet --only_system
 ```
 
 ### Reference-free evaluation:
 
 ```bash
-comet-score -s src.de -t hyp1.en --model Unbabel/wmt20-comet-qe-da
+comet-score -s src.de -t hyp1.en --model Unbabel/wmt22-cometkiwi-da
 ```
 
-**Note:** We are currently working on Licensing and releasing `Unbabel/wmt22-cometkiwi-da` but meanwhile that models is not available.
+**Note:** To use the `Unbabel/wmt22-cometkiwi-da` you first have to acknowledge its license on [Hugging Face Hub](https://huggingface.co/Unbabel/wmt22-cometkiwi-da).
 
 ### Comparing multiple systems:
 
 When comparing multiple MT systems we encourage you to run the `comet-compare` command to get **statistical significance** with Paired T-Test and bootstrap resampling [(Koehn, et al 2004)](https://aclanthology.org/W04-3250/).
 
 ```bash
 comet-compare -s src.de -t hyp1.en hyp2.en hyp3.en -r ref.en
@@ -129,23 +131,23 @@
 ```
 
 If working with a very large candidate list you can use `--rerank_top_k` flag to prune the topK most promissing candidates according to a reference-free metric.
 
 Example for a candidate list of 1000 samples:
 
 ```bash
-comet-mbr -s [SOURCE].txt -t [MT_SAMPLES].txt -o [OUTPUT_FILE].txt --num_sample 1000 --rerank_top_k 100 --gpus 4 --qe_model Unbabel/wmt20-comet-qe-da
+comet-mbr -s [SOURCE].txt -t [MT_SAMPLES].txt -o [OUTPUT_FILE].txt --num_sample 1000 --rerank_top_k 100 --gpus 4 --qe_model Unbabel/wmt22-cometkiwi-da
 ```
 
 # COMET Models:
 
 To evaluate your translations, we suggest using one of two models:
 
 - **Default model:** [`Unbabel/wmt22-comet-da`](https://huggingface.co/Unbabel/wmt22-comet-da) - This model uses a reference-based regression approach and is built on top of XLM-R. It has been trained on direct assessments from WMT17 to WMT20 and provides scores ranging from 0 to 1, where 1 represents a perfect translation.
-- **Upcoming model:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/Unbabel/wmt22-cometkiwi-da) - This reference-free model uses a regression approach and is built on top of InfoXLM. It has been trained on direct assessments from WMT17 to WMT20, as well as direct assessments from the MLQE-PE corpus. Like the default model, it also provides scores ranging from 0 to 1.
+- **Reference-free:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/Unbabel/wmt22-cometkiwi-da) - This reference-free model uses a regression approach and is built on top of InfoXLM. It has been trained on direct assessments from WMT17 to WMT20, as well as direct assessments from the MLQE-PE corpus. Like the default model, it also provides scores ranging from 0 to 1.
 
 For versions prior to 2.0, you can still use [`Unbabel/wmt20-comet-da`](https://huggingface.co/Unbabel/wmt20-comet-da), which is the primary metric, and [`Unbabel/wmt20-comet-qe-da`](https://huggingface.co/Unbabel/wmt20-comet-qe-da) for the **respective reference-free version**. You can find a list of all other models developed in previous versions on our [MODELS](MODELS.md) page. For more information, please refer to the [model licenses](LICENSE.models.md).
 
 ## Interpreting Scores:
 
 When using COMET to evaluate machine translation, it's important to understand how to interpret the scores it produces.
```

#### html2text {}

```diff
@@ -1,73 +1,76 @@
-Metadata-Version: 2.1 Name: unbabel-comet Version: 2.0.1 Summary: High-quality
+Metadata-Version: 2.1 Name: unbabel-comet Version: 2.0.2 Summary: High-quality
 Machine Translation Evaluation Home-page: https://github.com/Unbabel/COMET
 License: Apache-2.0 Keywords: Machine Translation,Evaluation,Unbabel,COMET
 Author: Ricardo Rei, Craig Stewart, Catarina Farinha, Alon Lavie Requires-
 Python: >=3.8.0,<4.0.0 Classifier: Development Status :: 4 - Beta Classifier:
 Environment :: Console Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Dist: entmax (>=1.1,<2.0) Requires-Dist: huggingface-hub
-(>=0.12.0,<0.13.0) Requires-Dist: jsonargparse (==3.13.1) Requires-Dist: numpy
-(>=1.20.0,<2.0.0) Requires-Dist: pandas (>=1.4.1,<2.0.0) Requires-Dist:
-pytorch-lightning (>=1.6.4,<2.0.0) Requires-Dist: sacrebleu (>=2.0.0,<3.0.0)
-Requires-Dist: scipy (>=1.5.4,<2.0.0) Requires-Dist: sentencepiece
-(>=0.1.96,<0.2.0) Requires-Dist: torch (>=1.6.0) Requires-Dist: torchmetrics
-(==0.8.2) Requires-Dist: transformers (>=4.17,<5.0) Project-URL: Documentation,
-https://unbabel.github.io/COMET/html/index.html Project-URL: Repository, https:
-//github.com/Unbabel/COMET Description-Content-Type: text/markdown
+(>=0.16.0,<0.17.0) Requires-Dist: jsonargparse (==3.13.1) Requires-Dist: numpy
+(>=1.20.0,<2.0.0) Requires-Dist: pandas (>=1.4.1) Requires-Dist: pytorch-
+lightning (>=1.6.4,<2.0.0) Requires-Dist: sacrebleu (>=2.0.0,<3.0.0) Requires-
+Dist: scipy (>=1.5.4,<2.0.0) Requires-Dist: sentencepiece (>=0.1.96,<0.2.0)
+Requires-Dist: torch (>=1.6.0) Requires-Dist: torchmetrics (==0.8.2) Requires-
+Dist: transformers (>=4.17,<5.0) Project-URL: Documentation, https://
+unbabel.github.io/COMET/html/index.html Project-URL: Repository, https://
+github.com/Unbabel/COMET Description-Content-Type: text/markdown
  [https://raw.githubusercontent.com/Unbabel/COMET/master/docs/source/_static/
                           img/COMET_lockup-dark.png]
 
                  [License] [GitHub_stars] [PyPI] [Code_Style]
-# Quick Installation COMET requires python 3.8 or above! Simple installation
-from PyPI ```bash pip install --upgrade pip # ensures that pip is current pip
-install unbabel-comet ``` To develop locally install run the following
-commands: ```bash git clone https://github.com/Unbabel/COMET cd COMET pip
-install poetry poetry install ``` For development, you can run the CLI tools
-directly, e.g., ```bash PYTHONPATH=. ./comet/cli/score.py ``` # Scoring MT
-outputs: ## CLI Usage: Test examples: ```bash echo -e "Dem Feuer konnte Einhalt
-geboten werden\nSchulen und KindergÃ¤rten wurden erÃ¶ffnet." >> src.de echo -
-e "The fire could be stopped\nSchools and kindergartens were open" >> hyp1.en
-echo -e "The fire could have been stopped\nSchools and pre-school were open" >>
-hyp2.en echo -e "They were able to control the fire.\nSchools and kindergartens
-opened" >> ref.en ``` Basic scoring command: ```bash comet-score -s src.de -
-t hyp1.en -r ref.en ``` > you can set the number of gpus using `--gpus` (0 to
-test on CPU). Scoring multiple systems: ```bash comet-score -s src.de -
-t hyp1.en hyp2.en -r ref.en ``` WMT test sets via [SacreBLEU](https://
-github.com/mjpost/sacrebleu): ```bash comet-score -d wmt22:en-de -t PATH/TO/
-TRANSLATIONS ``` If you are only interested in a system-level score use the
-following command: ```bash comet-score -s src.de -t hyp1.en -r ref.en --quiet -
--only_system ``` ### Reference-free evaluation: ```bash comet-score -s src.de -
-t hyp1.en --model Unbabel/wmt20-comet-qe-da ``` **Note:** We are currently
-working on Licensing and releasing `Unbabel/wmt22-cometkiwi-da` but meanwhile
-that models is not available. ### Comparing multiple systems: When comparing
-multiple MT systems we encourage you to run the `comet-compare` command to get
+**NEWS:** CometKiwi model from WMT22 is officially released and available on
+Hugging Face Hub. Please check all [available models here](https://github.com/
+Unbabel/COMET/blob/master/MODELS.md) # Quick Installation COMET requires python
+3.8 or above! Simple installation from PyPI ```bash pip install --upgrade pip #
+ensures that pip is current pip install unbabel-comet ``` To develop locally
+install run the following commands: ```bash git clone https://github.com/
+Unbabel/COMET cd COMET pip install poetry poetry install ``` For development,
+you can run the CLI tools directly, e.g., ```bash PYTHONPATH=. ./comet/cli/
+score.py ``` # Scoring MT outputs: ## CLI Usage: Test examples: ```bash echo -
+e "Dem Feuer konnte Einhalt geboten werden\nSchulen und KindergÃ¤rten wurden
+erÃ¶ffnet." >> src.de echo -e "The fire could be stopped\nSchools and
+kindergartens were open" >> hyp1.en echo -e "The fire could have been
+stopped\nSchools and pre-school were open" >> hyp2.en echo -e "They were able
+to control the fire.\nSchools and kindergartens opened" >> ref.en ``` Basic
+scoring command: ```bash comet-score -s src.de -t hyp1.en -r ref.en ``` > you
+can set the number of gpus using `--gpus` (0 to test on CPU). Scoring multiple
+systems: ```bash comet-score -s src.de -t hyp1.en hyp2.en -r ref.en ``` WMT
+test sets via [SacreBLEU](https://github.com/mjpost/sacrebleu): ```bash comet-
+score -d wmt22:en-de -t PATH/TO/TRANSLATIONS ``` If you are only interested in
+a system-level score use the following command: ```bash comet-score -s src.de -
+t hyp1.en -r ref.en --quiet --only_system ``` ### Reference-free evaluation:
+```bash comet-score -s src.de -t hyp1.en --model Unbabel/wmt22-cometkiwi-da ```
+**Note:** To use the `Unbabel/wmt22-cometkiwi-da` you first have to acknowledge
+its license on [Hugging Face Hub](https://huggingface.co/Unbabel/wmt22-
+cometkiwi-da). ### Comparing multiple systems: When comparing multiple MT
+systems we encourage you to run the `comet-compare` command to get
 **statistical significance** with Paired T-Test and bootstrap resampling [
 (Koehn, et al 2004)](https://aclanthology.org/W04-3250/). ```bash comet-compare
 -s src.de -t hyp1.en hyp2.en hyp3.en -r ref.en ``` ### Minimum Bayes Risk
 Decoding: The MBR command allows you to rank translations and select the best
 one according to COMET metrics. For more details you can read our paper on
 [Quality-Aware Decoding for Neural Machine Translation](https://
 aclanthology.org/2022.naacl-main.100.pdf). ```bash comet-mbr -s [SOURCE].txt -
 t [MT_SAMPLES].txt --num_sample [X] -o [OUTPUT_FILE].txt ``` If working with a
 very large candidate list you can use `--rerank_top_k` flag to prune the topK
 most promissing candidates according to a reference-free metric. Example for a
 candidate list of 1000 samples: ```bash comet-mbr -s [SOURCE].txt -t
 [MT_SAMPLES].txt -o [OUTPUT_FILE].txt --num_sample 1000 --rerank_top_k 100 --
-gpus 4 --qe_model Unbabel/wmt20-comet-qe-da ``` # COMET Models: To evaluate
+gpus 4 --qe_model Unbabel/wmt22-cometkiwi-da ``` # COMET Models: To evaluate
 your translations, we suggest using one of two models: - **Default model:**
 [`Unbabel/wmt22-comet-da`](https://huggingface.co/Unbabel/wmt22-comet-da) -
 This model uses a reference-based regression approach and is built on top of
 XLM-R. It has been trained on direct assessments from WMT17 to WMT20 and
 provides scores ranging from 0 to 1, where 1 represents a perfect translation.
-- **Upcoming model:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/
+- **Reference-free:** [`Unbabel/wmt22-cometkiwi-da`](https://huggingface.co/
 Unbabel/wmt22-cometkiwi-da) - This reference-free model uses a regression
 approach and is built on top of InfoXLM. It has been trained on direct
 assessments from WMT17 to WMT20, as well as direct assessments from the MLQE-PE
 corpus. Like the default model, it also provides scores ranging from 0 to 1.
 For versions prior to 2.0, you can still use [`Unbabel/wmt20-comet-da`](https:/
 /huggingface.co/Unbabel/wmt20-comet-da), which is the primary metric, and
 [`Unbabel/wmt20-comet-qe-da`](https://huggingface.co/Unbabel/wmt20-comet-qe-da)
```

