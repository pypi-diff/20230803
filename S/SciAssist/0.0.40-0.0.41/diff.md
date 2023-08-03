# Comparing `tmp/SciAssist-0.0.40.tar.gz` & `tmp/SciAssist-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciAssist-0.0.40.tar", last modified: Thu Aug  3 18:08:15 2023, max compression
+gzip compressed data, was "SciAssist-0.0.41.tar", last modified: Thu Aug  3 18:14:40 2023, max compression
```

## Comparing `SciAssist-0.0.40.tar` & `SciAssist-0.0.41.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.381629 SciAssist-0.0.40/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2023-08-03 17:53:25.000000 SciAssist-0.0.40/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2023-08-03 17:53:25.000000 SciAssist-0.0.40/MANIFEST.in
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    32200 2023-08-03 18:08:15.381629 SciAssist-0.0.40/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7572 2023-08-03 17:53:25.000000 SciAssist-0.0.40/README.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1443 2023-08-03 18:07:49.000000 SciAssist-0.0.40/pyproject.toml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-08-03 18:08:15.381629 SciAssist-0.0.40/setup.cfg
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2023-08-03 17:53:25.000000 SciAssist-0.0.40/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.373628 SciAssist-0.0.40/src/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.373628 SciAssist-0.0.40/src/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.373628 SciAssist-0.0.40/src/SciAssist/bin/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.373628 SciAssist-0.0.40/src/SciAssist/bin/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.373628 SciAssist-0.0.40/src/SciAssist/bin/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.373628 SciAssist-0.0.40/src/SciAssist/bin/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.373628 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/config.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-3
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cp
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2023-08-03 17:53:25.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/s2orc.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/bin/doc2json/scripts/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/bin/doc2json/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/datamodules/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/datamodules/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/components/cora_label.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/cora_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/dataset_extraction_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/general_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/mup_scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5991 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/datamodules/test_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.377629 SciAssist-0.0.40/src/SciAssist/models/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/models/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.381629 SciAssist-0.0.40/src/SciAssist/models/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/models/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/models/components/bart_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2489 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/models/components/bert_dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/models/components/bert_token_classifier.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-08-03 17:53:24.000000 SciAssist-0.0.40/src/SciAssist/models/components/flant5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/models/cora_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/models/dataset_extraction_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/models/mup_bart_module.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.381629 SciAssist-0.0.40/src/SciAssist/pipelines/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3690 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/pipelines/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/pipelines/dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/pipelines/pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/pipelines/reference_string_parsing.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    14045 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/pipelines/summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/pipelines/summarization_origin.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/pipelines/testing_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/pipelines/training_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/test.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/train.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/training_args.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.381629 SciAssist-0.0.40/src/SciAssist/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.381629 SciAssist-0.0.40/src/SciAssist/utils/collators/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/utils/collators/CollatorForFid.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/utils/collators/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/utils/data_reader.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    53624 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/utils/data_utils.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5722 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/utils/pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2432 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/utils/windows_pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1499 2023-08-03 17:53:23.000000 SciAssist-0.0.40/src/SciAssist/utils/xml2txt.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.373628 SciAssist-0.0.40/src/SciAssist.egg-info/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    32200 2023-08-03 18:08:15.000000 SciAssist-0.0.40/src/SciAssist.egg-info/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4529 2023-08-03 18:08:15.000000 SciAssist-0.0.40/src/SciAssist.egg-info/SOURCES.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-08-03 18:08:15.000000 SciAssist-0.0.40/src/SciAssist.egg-info/dependency_links.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-08-03 18:08:15.000000 SciAssist-0.0.40/src/SciAssist.egg-info/entry_points.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      388 2023-08-03 18:08:15.000000 SciAssist-0.0.40/src/SciAssist.egg-info/requires.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       10 2023-08-03 18:08:15.000000 SciAssist-0.0.40/src/SciAssist.egg-info/top_level.txt
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:08:15.381629 SciAssist-0.0.40/tests/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2023-08-03 17:53:23.000000 SciAssist-0.0.40/tests/test_rsp.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2023-08-03 17:53:23.000000 SciAssist-0.0.40/tests/test_summ.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.631504 SciAssist-0.0.41/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2023-08-03 17:53:25.000000 SciAssist-0.0.41/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2023-08-03 17:53:25.000000 SciAssist-0.0.41/MANIFEST.in
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    32200 2023-08-03 18:14:40.631504 SciAssist-0.0.41/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7572 2023-08-03 17:53:25.000000 SciAssist-0.0.41/README.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1444 2023-08-03 18:14:32.000000 SciAssist-0.0.41/pyproject.toml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-08-03 18:14:40.631504 SciAssist-0.0.41/setup.cfg
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2023-08-03 17:53:25.000000 SciAssist-0.0.41/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.619504 SciAssist-0.0.41/src/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/bin/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/bin/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/config.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-3
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cp
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2023-08-03 17:53:25.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/s2orc.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/bin/doc2json/scripts/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/bin/doc2json/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/datamodules/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/datamodules/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/components/cora_label.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/cora_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/dataset_extraction_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/general_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/mup_scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5991 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/datamodules/test_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/models/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/models/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/models/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/models/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/models/components/bart_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2489 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/models/components/bert_dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/models/components/bert_token_classifier.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-08-03 17:53:24.000000 SciAssist-0.0.41/src/SciAssist/models/components/flant5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/models/cora_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/models/dataset_extraction_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/models/mup_bart_module.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.627504 SciAssist-0.0.41/src/SciAssist/pipelines/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3690 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/pipelines/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/pipelines/dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/pipelines/pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/pipelines/reference_string_parsing.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    14045 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/pipelines/summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/pipelines/summarization_origin.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/pipelines/testing_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/pipelines/training_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/test.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/train.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/training_args.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.631504 SciAssist-0.0.41/src/SciAssist/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.631504 SciAssist-0.0.41/src/SciAssist/utils/collators/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/utils/collators/CollatorForFid.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/utils/collators/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/utils/data_reader.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    53624 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/utils/data_utils.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5722 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/utils/pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2432 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/utils/windows_pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1499 2023-08-03 17:53:23.000000 SciAssist-0.0.41/src/SciAssist/utils/xml2txt.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.623504 SciAssist-0.0.41/src/SciAssist.egg-info/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    32200 2023-08-03 18:14:40.000000 SciAssist-0.0.41/src/SciAssist.egg-info/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4529 2023-08-03 18:14:40.000000 SciAssist-0.0.41/src/SciAssist.egg-info/SOURCES.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-08-03 18:14:40.000000 SciAssist-0.0.41/src/SciAssist.egg-info/dependency_links.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-08-03 18:14:40.000000 SciAssist-0.0.41/src/SciAssist.egg-info/entry_points.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      389 2023-08-03 18:14:40.000000 SciAssist-0.0.41/src/SciAssist.egg-info/requires.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       10 2023-08-03 18:14:40.000000 SciAssist-0.0.41/src/SciAssist.egg-info/top_level.txt
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-08-03 18:14:40.631504 SciAssist-0.0.41/tests/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2023-08-03 17:53:23.000000 SciAssist-0.0.41/tests/test_rsp.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2023-08-03 17:53:23.000000 SciAssist-0.0.41/tests/test_summ.py
```

### Comparing `SciAssist-0.0.40/LICENSE` & `SciAssist-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/PKG-INFO` & `SciAssist-0.0.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.40
+Version: 0.0.41
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.40/README.md` & `SciAssist-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/pyproject.toml` & `SciAssist-0.0.41/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SciAssist"
-version = "0.0.40"
+version = "0.0.41"
 authors = [
   { name="WING-NUS", email="dingyixi@hotmail.com" },
 ]
 maintainers = [
   { name="Yixi Ding", email="dingyixi@hotmail.com" },
 ]
 description = "A toolkit for Scientific Document Processing"
@@ -34,15 +34,15 @@
     "python_magic~=0.4.18",
     "pytorch_lightning~=1.7.1",
     "requests~=2.21.0",
     "rich~=12.4.4",
     "seaborn~=0.11.2",
     "setuptools>=61.0",
     "torch>=1.12.0",
-    "torchmetrics>=0.7.0",
+    "torchmetrics==0.11.4",
     "transformers~=4.19.2",
     "wandb~=0.12.19",
     "pdfminer.six",
     "pandas~=1.4.3",
     "pytorch-crf",
     "torchcrf",
     "sacremoses",
```

### Comparing `SciAssist-0.0.40/setup.cfg` & `SciAssist-0.0.41/setup.cfg`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/__init__.py` & `SciAssist-0.0.41/src/SciAssist/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/__init__.py` & `SciAssist-0.0.41/src/SciAssist/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc` & `SciAssist-0.0.41/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/LICENSE` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-3` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-3`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cp` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cp`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/s2orc.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/s2orc.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh` & `SciAssist-0.0.41/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/datamodules/cora_datamodule.py` & `SciAssist-0.0.41/src/SciAssist/datamodules/cora_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/datamodules/dataset_extraction_datamodule.py` & `SciAssist-0.0.41/src/SciAssist/datamodules/dataset_extraction_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/datamodules/general_datamodule.py` & `SciAssist-0.0.41/src/SciAssist/datamodules/general_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/datamodules/mup_datamodule.py` & `SciAssist-0.0.41/src/SciAssist/datamodules/mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/datamodules/mup_scisumm_datamodule.py` & `SciAssist-0.0.41/src/SciAssist/datamodules/mup_scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py` & `SciAssist-0.0.41/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/datamodules/test_datamodule.py` & `SciAssist-0.0.41/src/SciAssist/datamodules/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/models/components/bart_summarization.py` & `SciAssist-0.0.41/src/SciAssist/models/components/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/models/components/bert_dataset_extraction.py` & `SciAssist-0.0.41/src/SciAssist/models/components/bert_dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/models/components/bert_token_classifier.py` & `SciAssist-0.0.41/src/SciAssist/models/components/bert_token_classifier.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/models/components/flant5_summarization.py` & `SciAssist-0.0.41/src/SciAssist/models/components/flant5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/models/cora_module.py` & `SciAssist-0.0.41/src/SciAssist/models/cora_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/models/dataset_extraction_module.py` & `SciAssist-0.0.41/src/SciAssist/models/dataset_extraction_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/models/mup_bart_module.py` & `SciAssist-0.0.41/src/SciAssist/models/mup_bart_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/pipelines/__init__.py` & `SciAssist-0.0.41/src/SciAssist/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/pipelines/dataset_extraction.py` & `SciAssist-0.0.41/src/SciAssist/pipelines/dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/pipelines/pipeline.py` & `SciAssist-0.0.41/src/SciAssist/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/pipelines/reference_string_parsing.py` & `SciAssist-0.0.41/src/SciAssist/pipelines/reference_string_parsing.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/pipelines/summarization.py` & `SciAssist-0.0.41/src/SciAssist/pipelines/summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/pipelines/summarization_origin.py` & `SciAssist-0.0.41/src/SciAssist/pipelines/summarization_origin.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/pipelines/testing_pipeline.py` & `SciAssist-0.0.41/src/SciAssist/pipelines/testing_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/pipelines/training_pipeline.py` & `SciAssist-0.0.41/src/SciAssist/pipelines/training_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/test.py` & `SciAssist-0.0.41/src/SciAssist/test.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/train.py` & `SciAssist-0.0.41/src/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/training_args.py` & `SciAssist-0.0.41/src/SciAssist/training_args.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/utils/__init__.py` & `SciAssist-0.0.41/src/SciAssist/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/utils/collators/CollatorForFid.py` & `SciAssist-0.0.41/src/SciAssist/utils/collators/CollatorForFid.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/utils/data_reader.py` & `SciAssist-0.0.41/src/SciAssist/utils/data_reader.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/utils/data_utils.py` & `SciAssist-0.0.41/src/SciAssist/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/utils/pdf2text.py` & `SciAssist-0.0.41/src/SciAssist/utils/pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/utils/windows_pdf2text.py` & `SciAssist-0.0.41/src/SciAssist/utils/windows_pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist/utils/xml2txt.py` & `SciAssist-0.0.41/src/SciAssist/utils/xml2txt.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/src/SciAssist.egg-info/PKG-INFO` & `SciAssist-0.0.41/src/SciAssist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.40
+Version: 0.0.41
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.40/src/SciAssist.egg-info/SOURCES.txt` & `SciAssist-0.0.41/src/SciAssist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/tests/test_rsp.py` & `SciAssist-0.0.41/tests/test_rsp.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.40/tests/test_summ.py` & `SciAssist-0.0.41/tests/test_summ.py`

 * *Files identical despite different names*

