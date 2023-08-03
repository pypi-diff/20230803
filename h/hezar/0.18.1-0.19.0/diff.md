# Comparing `tmp/hezar-0.18.1.tar.gz` & `tmp/hezar-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.18.1.tar", max compression
+gzip compressed data, was "hezar-0.19.0.tar", max compression
```

## Comparing `hezar-0.18.1.tar` & `hezar-0.19.0.tar`

### file list

```diff
@@ -1,87 +1,92 @@
--rw-r--r--   0        0        0     1065 2023-07-31 06:23:56.132397 hezar-0.18.1/LICENSE
--rw-r--r--   0        0        0     4309 2023-07-31 06:23:56.132397 hezar-0.18.1/README.md
--rw-r--r--   0        0        0      260 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/__init__.py
--rw-r--r--   0        0        0     5336 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/builders.py
--rw-r--r--   0        0        0    11117 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/configs.py
--rw-r--r--   0        0        0     2068 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/__init__.py
--rw-r--r--   0        0        0     6364 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4502 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3627 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      282 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.132397 hezar-0.18.1/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1604 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1634 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11760 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/model.py
--rw-r--r--   0        0        0      152 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3971 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      877 2023-07-31 06:23:56.136397 hezar-0.18.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3666 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3809 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      142 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     3603 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/normalizer.py
--rw-r--r--   0        0        0     3852 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      231 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    19353 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8828 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2643 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2243 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17687 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      164 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5614 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3660 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/logging.py
--rw-r--r--   0        0        0      936 2023-07-31 06:23:56.140397 hezar-0.18.1/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     1648 2023-07-31 06:23:56.140397 hezar-0.18.1/pyproject.toml
--rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 hezar-0.18.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-03 08:30:44.744121 hezar-0.19.0/LICENSE
+-rw-r--r--   0        0        0     3698 2023-08-03 08:30:44.744121 hezar-0.19.0/README.md
+-rw-r--r--   0        0        0      260 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5336 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/builders.py
+-rw-r--r--   0        0        0    11489 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/configs.py
+-rw-r--r--   0        0        0     2072 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6365 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      312 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1709 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4502 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3627 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     3555 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/text_summarization.py
+-rw-r--r--   0        0        0       26 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      273 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1604 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1676 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1634 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11719 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/model.py
+-rw-r--r--   0        0        0      152 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3971 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     4132 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text2text/__init__.py
+-rw-r--r--   0        0        0       89 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text2text/t5/__init__.py
+-rw-r--r--   0        0        0     3838 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text2text/t5/t5_text2text.py
+-rw-r--r--   0        0        0      764 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text2text/t5/t5_text2text_config.py
+-rw-r--r--   0        0        0      240 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3530 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3666 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3809 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0      142 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3603 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/normalizer.py
+-rw-r--r--   0        0        0     4119 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      324 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4965 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    19342 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8828 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2644 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2243 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17688 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      164 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5614 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3660 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0      936 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     1648 2023-08-03 08:30:44.748121 hezar-0.19.0/pyproject.toml
+-rw-r--r--   0        0        0     6180 1970-01-01 00:00:00.000000 hezar-0.19.0/PKG-INFO
```

### Comparing `hezar-0.18.1/LICENSE` & `hezar-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/README.md` & `hezar-0.19.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 _<p align="center"> A seamless AI library for Persian</p>_
 
 **Hezar** (meaning **_thousand_** in Persian) is a multipurpose AI library built to make AI easy for the Persian community!
 
 Hezar is a library that:
 - brings together all the best works in AI for Persian
 - makes using AI models as easy as a couple of lines of code
-- seamlessly integrates with HuggingFace Hub for all of its models
+- seamlessly integrates with Hugging Face Hub for all of its models
 - has a highly developer-friendly interface
 - has a task-based model interface which is more convenient for general users.
 - is packed with additional tools like word embeddings, tokenizers, feature extractors, etc.
 - comes with a lot of supplementary ML tools for deployment, benchmarking, optimization, etc.
 - and more!
 
 ## Installation
@@ -29,46 +29,25 @@
 
 ## Quick Tour
 ### Ready-to-use models from Hub
 There's a bunch of ready-to-use trained models for different tasks on the Hub. See them [here](https://huggingface.co/hezarai)!
 
 For example, you can grab a BERT-based model for sentiment analysis like so: 
 ```python
-from hezar import Model, Tokenizer
-
-# this is our Hub repo
-model_path = "hezarai/bert-fa-sentiment-digikala-snappfood"
-# load model
-model = Model.load(model_path)
+from hezar import Model
 
 example = ["هزار، کتابخانه‌ای کامل برای به کارگیری آسان هوش مصنوعی"]
-# inference
+model = Model.load("hezarai/bert-fa-sentiment-digikala-snappfood")
 outputs = model.predict(example)
-# print outputs
 print(outputs)
 ```
 ```commandline
 {'labels': ['positive'], 'probs': [0.812910258769989]}
 ```
-### Build models from scratch
-Wanna use models without any pretrained weights? Easy!
-
-Build a raw BERT-based model for text classification with a single line of code!
-```python
-from hezar import build_model
 
-model = build_model("bert_text_classification", id2label={0: "negative", 1: "positive"})
-print(model)
-```
-You can also import model directly:
-```python
-from hezar import BertTextClassification, BertTextClassificationConfig
-
-bert_tc = BertTextClassification(BertTextClassificationConfig(num_labels=2))
-```
 ### Write your own model
 It's fairly easy to extend this library or add your own model. Hezar has its own `Model` base class that is simply a normal PyTorch `nn.Module` but with some extra features!
 
 Here's a simple example:
 ```python
 from dataclasses import dataclass
```

### Comparing `hezar-0.18.1/hezar/builders.py` & `hezar-0.19.0/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/configs.py` & `hezar-0.19.0/hezar/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,63 +172,77 @@
         dict_config.pop("name", None)
         dict_config.pop("config_type", None)
 
         config = cls(**{k: v for k, v in dict_config.items() if hasattr(cls, k)})  # noqa
 
         return config
 
-    def save(self, save_dir: Union[str, os.PathLike], filename: str, subfolder: Optional[str] = None):
+    def save(
+        self,
+        save_dir: Union[str, os.PathLike],
+        filename: str,
+        subfolder: Optional[str] = None,
+        skip_none_fields: Optional[bool] = True,
+    ):
         """
         Save the *config.yaml file to a local path
 
         Args:
              save_dir: Save directory path
              filename: Config file name
              subfolder: Subfolder to save the config file
+             skip_none_fields (bool): Whether to skip saving None values or not
         """
         subfolder = subfolder or ""
         config = self.dict()
-        # exclude None items
-        config = {k: v for k, v in config.items() if v is not None}
+
+        if skip_none_fields:
+            # exclude None items
+            config = {k: v for k, v in config.items() if v is not None}
+
         # convert enums to value
         config = {k: v.value if isinstance(v, Enum) else v for k, v in config.items()}
+
         # make and save to directory
         os.makedirs(os.path.join(save_dir, subfolder), exist_ok=True)
         save_path = os.path.join(save_dir, subfolder, filename)
         OmegaConf.save(config, save_path)
+
         return save_path
 
     def push_to_hub(
         self,
         repo_id: str,
         filename: str,
         subfolder: Optional[str] = None,
         repo_type: Optional[str] = "model",
+        skip_none_fields: Optional[bool] = True,
         private: Optional[bool] = False,
         commit_message: Optional[str] = None,
     ):
         """
         Push the config file to the hub
 
         Args:
             repo_id (str): Repo name or id on the Hub
             filename (str): config file name
             subfolder (str): subfolder to save the config
             repo_type (str): Type of the repo e.g, model, dataset, space
+            skip_none_fields (bool): Whether to skip saving None values or not
             private (bool): Whether the repo type should be private or not (ignored if the repo exists)
             commit_message (str): Push commit message
         """
         path_in_repo = f"{subfolder}/{filename}" if subfolder else filename
         subfolder = subfolder or ""
 
         # create remote repo
         create_repo(repo_id, repo_type=repo_type, private=private, exist_ok=True)
         # save to tmp and prepare for push
         cache_path = tempfile.mkdtemp()
-        config_path = self.save(cache_path, filename=filename, subfolder=subfolder)
+        config_path = self.save(cache_path, filename=filename, subfolder=subfolder, skip_none_fields=skip_none_fields)
         # push to hub
         if commit_message is None:
             commit_message = f"Hezar: Upload {filename}"
         upload_file(
             path_or_fileobj=config_path,
             path_in_repo=path_in_repo,
             repo_id=repo_id,
```

### Comparing `hezar-0.18.1/hezar/constants.py` & `hezar-0.19.0/hezar/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     AUDIO_CLASSIFICATION = "audio_classification"
     IMAGE2TEXT = "image2text"
     LANGUAGE_MODELING = "language_modeling"
     SEQUENCE_LABELING = "sequence_labeling"
     SPEECH_RECOGNITION = "speech_recognition"
     TEXT_CLASSIFICATION = "text_classification"
     TEXT_DETECTION = "text_detection"
-    SEQ2SEQ = "seq2seq"
+    TEXT2TEXT = "text2text"
 
 
 class ConfigType(str, Enum):
     BASE = "base"
     MODEL = "model"
     DATASET = "dataset"
     PREPROCESSOR = "preprocessor"
```

### Comparing `hezar-0.18.1/hezar/data/data_collators.py` & `hezar-0.19.0/hezar/data/data_collators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import torch
 
 from ..data.utils import convert_batch_dict_dtype
 from ..preprocessors import Tokenizer
 from ..utils import get_logger
 
+
 __all__ = [
     "TextPaddingDataCollator",
     "SequenceLabelingDataCollator",
 ]
 
 logger = get_logger(__name__)
```

### Comparing `hezar-0.18.1/hezar/data/datasets/dataset.py` & `hezar-0.19.0/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.19.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.19.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/data/utils/data_utils.py` & `hezar-0.19.0/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/embeddings/embedding.py` & `hezar-0.19.0/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/embeddings/fasttext.py` & `hezar-0.19.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/embeddings/word2vec.py` & `hezar-0.19.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/metrics/f1.py` & `hezar-0.19.0/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/metrics/metric.py` & `hezar-0.19.0/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/metrics/recall.py` & `hezar-0.19.0/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/metrics/seqeval.py` & `hezar-0.19.0/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.19.0/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.19.0/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.19.0/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.19.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.19.0/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.19.0/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/model.py` & `hezar-0.19.0/hezar/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,16 +173,15 @@
         os.makedirs(path, exist_ok=True)
         model_save_path = os.path.join(path, filename)
         torch.save(self.state_dict(), model_save_path)
         if save_config:
             self.config.save(save_dir=path, filename=config_filename)
         if save_preprocessor:
             if self.preprocessor is not None:
-                for p in self.preprocessor.values():
-                    p.save(path)
+                self.preprocessor.save(path)
         return model_save_path
 
     def push_to_hub(
         self,
         repo_id: str,
         filename: Optional[str] = None,
         config_filename: Optional[str] = None,
```

### Comparing `hezar-0.18.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.19.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.19.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.19.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         )
         return inputs
 
     def post_process(self, inputs, **kwargs):
         # TODO sequence labeling outputs should consider rejoining split words into single words with proper tag
         logits = inputs["logits"]
         tokens = inputs["tokens"]
-        word_ids = inputs["word_ids"]
+        word_ids = inputs["word_ids"]  # noqa
         predictions = logits.argmax(2).cpu()
         predictions = [[self.config.id2label[p.item()] for p in prediction] for prediction in predictions]
         outputs = []
         for tokens_list, prediction in zip(tokens, predictions):
             results = []
             for token, tag in zip(tokens_list, prediction):
                 if token not in self.config.prediction_skip_tokens:
```

### Comparing `hezar-0.18.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.19.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.19.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.19.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.19.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.19.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.19.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.19.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/preprocessors/normalizer.py` & `hezar-0.19.0/hezar/preprocessors/normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/preprocessors/preprocessor.py` & `hezar-0.19.0/hezar/preprocessors/preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,16 +97,26 @@
 
 
 class PreprocessorsContainer(OrderedDict):
     """
     A class to hold the preprocessors by their name
     """
 
+    def save(self, path):
+        """
+        Save every preprocessor item in the container
+        """
+        for name, preprocessor in self.items():
+            preprocessor.save(path)
+
     def push_to_hub(
         self,
         repo_id,
         subfolder=None,
         commit_message=None,
         private=None,
     ):
+        """
+        Push every preprocessor item in the container
+        """
         for name, preprocessor in self.items():
             preprocessor.push_to_hub(repo_id, subfolder=subfolder, commit_message=commit_message, private=private)
```

### Comparing `hezar-0.18.1/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.19.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.19.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.19.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -410,14 +410,15 @@
         tokenizer = build_preprocessor(config.name, config, **kwargs)
         return tokenizer
 
     def save(self, path, save_config=True, pretty=True):
         os.makedirs(path, exist_ok=True)
         # save config
         if save_config:
+            self.config.vocab_size = self.get_vocab_size(with_added_tokens=True)
             self.config.save(path, filename=self.tokenizer_config_filename, subfolder=self.preprocessor_subfolder)
         # save tokenizer.json
         save_path = os.path.join(path, self.preprocessor_subfolder, self.tokenizer_filename)
         self._tokenizer.save(save_path, pretty=pretty)
 
     def push_to_hub(
         self,
@@ -445,16 +446,15 @@
 
         # create remote repo
         create_repo(repo_id, exist_ok=True, private=private)
         # save to tmp and prepare for push
         cache_path = tempfile.mkdtemp()
         # save tokenizer.json
         tokenizer_save_path = os.path.join(cache_path, subfolder, tokenizer_filename)
-        os.makedirs(os.path.join(cache_path, subfolder), exist_ok=True)
-        self._tokenizer.save(tokenizer_save_path, pretty=True)
+        self.save(cache_path, pretty=True)
 
         if commit_message is None:
             commit_message = "Hezar: Upload tokenizer and config"
 
         # upload config
         self.config.push_to_hub(
             repo_id=repo_id,
```

### Comparing `hezar-0.18.1/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.19.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/registry.py` & `hezar-0.19.0/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.19.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Callable
 
 import numpy as np
 import torch
 
-from ..trainer import Trainer
 from ...configs import TrainerConfig
 from ...constants import MetricType
 from ...data.datasets import Dataset
 from ...models import Model
 from ...utils import get_logger
+from ..trainer import Trainer
+
 
 logger = get_logger(__name__)
 
 
 class SequenceLabelingTrainer(Trainer):
     """
     A trainer for all text classification models
```

### Comparing `hezar-0.18.1/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.19.0/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/trainers/trainer.py` & `hezar-0.19.0/hezar/trainers/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 import random
-from typing import Any, Dict, Tuple, Union, Callable
+from typing import Any, Callable, Dict, Tuple, Union
 
 import numpy as np
 import torch
 from huggingface_hub import create_repo, hf_hub_download
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
 from tqdm import tqdm
 
-from .trainer_utils import MetricsTracker
 from ..builders import build_metric
 from ..configs import LRSchedulerConfig, MetricConfig, OptimizerConfig, TrainerConfig
 from ..constants import (
     DEFAULT_DATASET_CONFIG_FILE,
     DEFAULT_TRAINER_CONFIG_FILE,
     DEFAULT_TRAINER_SUBFOLDER,
     HEZAR_CACHE_DIR,
     TQDM_BAR_FORMAT,
 )
 from ..data.datasets import Dataset
 from ..models import Model
 from ..preprocessors import Preprocessor, PreprocessorsContainer
 from ..utils import get_logger
+from .trainer_utils import MetricsTracker
+
 
 logger = get_logger(__name__)
 
 optimizers = {
     "adam": torch.optim.Adam,
     "adamw": torch.optim.AdamW,
     "sgd": torch.optim.SGD,
```

### Comparing `hezar-0.18.1/hezar/trainers/trainer_utils.py` & `hezar-0.19.0/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/utils/common_utils.py` & `hezar-0.19.0/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/utils/core_utils.py` & `hezar-0.19.0/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/utils/hub_utils.py` & `hezar-0.19.0/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/hezar/utils/registry_utils.py` & `hezar-0.19.0/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.18.1/pyproject.toml` & `hezar-0.19.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.18.1"
+version = "0.19.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.18.1/PKG-INFO` & `hezar-0.19.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.18.1
+Version: 0.19.0
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
@@ -42,15 +42,15 @@
 _<p align="center"> A seamless AI library for Persian</p>_
 
 **Hezar** (meaning **_thousand_** in Persian) is a multipurpose AI library built to make AI easy for the Persian community!
 
 Hezar is a library that:
 - brings together all the best works in AI for Persian
 - makes using AI models as easy as a couple of lines of code
-- seamlessly integrates with HuggingFace Hub for all of its models
+- seamlessly integrates with Hugging Face Hub for all of its models
 - has a highly developer-friendly interface
 - has a task-based model interface which is more convenient for general users.
 - is packed with additional tools like word embeddings, tokenizers, feature extractors, etc.
 - comes with a lot of supplementary ML tools for deployment, benchmarking, optimization, etc.
 - and more!
 
 ## Installation
@@ -67,46 +67,25 @@
 
 ## Quick Tour
 ### Ready-to-use models from Hub
 There's a bunch of ready-to-use trained models for different tasks on the Hub. See them [here](https://huggingface.co/hezarai)!
 
 For example, you can grab a BERT-based model for sentiment analysis like so: 
 ```python
-from hezar import Model, Tokenizer
-
-# this is our Hub repo
-model_path = "hezarai/bert-fa-sentiment-digikala-snappfood"
-# load model
-model = Model.load(model_path)
+from hezar import Model
 
 example = ["هزار، کتابخانه‌ای کامل برای به کارگیری آسان هوش مصنوعی"]
-# inference
+model = Model.load("hezarai/bert-fa-sentiment-digikala-snappfood")
 outputs = model.predict(example)
-# print outputs
 print(outputs)
 ```
 ```commandline
 {'labels': ['positive'], 'probs': [0.812910258769989]}
 ```
-### Build models from scratch
-Wanna use models without any pretrained weights? Easy!
-
-Build a raw BERT-based model for text classification with a single line of code!
-```python
-from hezar import build_model
 
-model = build_model("bert_text_classification", id2label={0: "negative", 1: "positive"})
-print(model)
-```
-You can also import model directly:
-```python
-from hezar import BertTextClassification, BertTextClassificationConfig
-
-bert_tc = BertTextClassification(BertTextClassificationConfig(num_labels=2))
-```
 ### Write your own model
 It's fairly easy to extend this library or add your own model. Hezar has its own `Model` base class that is simply a normal PyTorch `nn.Module` but with some extra features!
 
 Here's a simple example:
 ```python
 from dataclasses import dataclass
```

