# Comparing `tmp/syngen-0.1.9.tar.gz` & `tmp/syngen-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.1.9.tar", last modified: Thu May 25 13:48:35 2023, max compression
+gzip compressed data, was "syngen-0.2.0rc0.tar", last modified: Thu Aug  3 11:07:02 2023, max compression
```

## Comparing `syngen-0.1.9.tar` & `syngen-0.2.0rc0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.556030 syngen-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-25 13:41:59.000000 syngen-0.1.9/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-25 13:41:59.000000 syngen-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-25 13:41:59.000000 syngen-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    17434 2023-05-25 13:48:35.556030 syngen-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16695 2023-05-25 13:41:59.000000 syngen-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-25 13:41:59.000000 syngen-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-25 13:48:35.556030 syngen-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.544030 syngen-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/custom_logger/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/custom_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/custom_logger/custom_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.544030 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43552 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6053 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33156 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.556030 syngen-0.1.9/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.556030 syngen-0.1.9/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13244 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     4681 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17434 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21652 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20910 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.271280 syngen-0.2.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.275280 syngen-0.2.0rc0/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.275280 syngen-0.2.0rc0/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.275280 syngen-0.2.0rc0/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/context/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11674 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16303 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723170 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5183 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.271280 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46130 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6859 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7731 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36772 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24485 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10565 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11221 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5231 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11869 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.275280 syngen-0.2.0rc0/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21652 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.1.9/LICENSE` & `syngen-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.1.9/PKG-INFO` & `syngen-0.2.0rc0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: syngen
-Version: 0.1.9
-Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
-Home-page: https://github.com/tdspora/syngen
-Author: EPAM Systems, Inc.
-Maintainer: Pavel Bobyrev
-License: GPLv3 License
-Keywords: data,generation,synthetic,vae,tabular
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # EPAM Syngen
 
 EPAM Syngen is an unsupervised tabular data generation tool. It is useful for generation of test data with a given table as a template. Most datatypes including floats, integers, datetime, text, categorical, binary are supported. The linked tables i.e., tables sharing a key can also be generated using the simple statistical approach. 
 The source of data might be in CSV, Avro format and should be located locally and be in UTF-8 encoding.
 
 The tool is based on the variational autoencoder model (VAE). The Bayesian Gaussian Mixture model is used to further detangle the latent space.
 
@@ -50,18 +31,18 @@
 <i>Please notice that the name should match the one you used in the training process.</i><br>
 This will create a csv file with the synthetic table in <i>./model_artifacts/tmp_store/TABLE_NAME/merged_infer_TABLE_NAME.csv</i>.<br>
 
 Here is a quick example:
 
 ```bash
 pip install syngen
-train --source ./example-data/housing.csv –-table_name Housing
+train --source ./examples/example-data/housing.csv –-table_name Housing
 infer --table_name Housing
 ```
-As the example you can use the dataset <i>"Housing"</i> in [example-data/housing.csv](example-data/housing.csv).
+As the example you can use the dataset <i>"Housing"</i> in [examples/example-data/housing.csv](examples/example-data/housing.csv).
 In this example, our real-world data is <a href="https://www.kaggle.com/datasets/camnugent/california-housing-prices" target="_blank">"Housing"</a> from Kaggle.
 
 ## Features
 
 ### Training
 
 You can add flexibility to the training and inference processes using additional hyperparameters.<br>
@@ -167,115 +148,152 @@
 You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
 they will be ignored in the CLI call.
 
 <i>Note:</i> By using metadata file, you can also generate tables with absent relationships. 
 In this case, the tables will be generated independently.
 
 The yaml metadata file should match the following template:
-
-    CUSTOMER:                                       # Table name. Required parameter
-        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats. Required parameter
-                 
-        train_settings:                             # Settings for training process. Optional parameter
-            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
-            drop_null: False                        # Drop rows with NULL values. Optional parameter
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
-                    - gender
-                    - marital_status
-                 
-        infer_settings:                             # Settings for infer process. Optional parameter
-            size: 100                               # Size for generated data. Optional parameter
-            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
-            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
-        keys:                                       # Keys of the table. Optional parameter
-            PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
-                type: "PK"                          # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
-                columns:                            # Array of column names
-                    - customer_id
+```yaml
+global:                                     # Global settings. Optional parameter. In this section you can specify training and inference settings which will be set for all tables
+  train_settings:                           # Settings for training process. Optional parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    
+  infer_settings:                           # Settings for infer process. Optional parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+
+CUSTOMER:                                   # Table name. Required parameter               
+  train_settings:                           # Settings for training process. Required parameter
+    source: "./files/customer.csv"          # The path to the original data. Supported formats include local files in CSV, Avro formats. Required parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    column_types:
+      categorical:                          # Force listed columns to have categorical type (use dictionary of values). Optional parameter
+        - gender
+        - marital_status
+        
+  format:                                   # Settings for reading and writing data in 'csv' format. Optional parameter
+    sep: ','                                # Delimiter to use. Optional parameter
+    quotechar: '"'                          # The character used to denote the start and end of a quoted item. Optional parameter
+    quoting: minimal                        # Control field quoting behavior per constants - ["all", "minimal", "non-numeric", "none"]. Optional parameter
+    escapechar: '"'                         # One-character string used to escape other characters. Optional parameter
+    encoding: null                          # A string representing the encoding to use in the output file. Optional parameter
+    header: infer                           # Row number(s) to use as the column names, and the start of the data. Optional parameter  
+    skiprows: null                          # Line numbers to skip (0-indexed) or number of lines to skip (int) at the start of the file. Optional parameter
+    on_bad_lines: error                     # Specifies what to do upon encountering a bad line (a line with too many fields) - ["error", "warn", "skip"]. Optional parameter
+    engine: null                            # Parser engine to use - ["c", "python"]. Optional parameter             
+  infer_settings:                           # Settings for infer process. Optional parameter
+    destination: "./files/generated_data_customer.csv"# The path where the generated data will be stored. Supported formats include local files in CSV, Avro formats. Required parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+  keys:                                     # Keys of the table. Optional parameter
+    PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
+      type: "PK"                            # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
+      columns:                              # Array of column names
+        - customer_id
      
-            UQ1:                                    # Name of a key
-                type: "UQ"                          # One or many unique keys
-                columns:
-                    - e_mail
+    UQ1:                                    # Name of a key
+      type: "UQ"                            # One or many unique keys
+      columns:
+        - e_mail
      
-            FK1:                                    # One or many foreign keys
-                type: "FK"
-                columns:                            # Array of columns in the current table
-                    - e_mail
-                    - alias
-                references:
-                    table: "PROFILE"                # Name of the parent table
-                    columns:                        # Array of columns in the parent table
-                        - e_mail
-                        - alias
+    FK1:                                    # One or many foreign keys
+      type: "FK"
+      columns:                              # Array of columns in the current table
+        - e_mail
+        - alias
+      references:
+        table: "PROFILE"                    # Name of the parent table
+        columns:                            # Array of columns in the parent table
+          - e_mail
+          - alias
        
-            FK2:
-                type: "FK"
-                columns:
-                    - address_id
-                references:
-                    table: "ADDRESS"
-                    columns:
-                        - address_id
+    FK2:
+      type: "FK"
+      columns:
+        - address_id
+      references:
+        table: "ADDRESS"
+        columns:
+          - address_id
 
      
-    ORDER:                                          # Table name. Required parameter
-        source: "./files/order.csv"                 # Supported formats include local files in CSV, Avro formats. Required parameter
+ORDER:                                      # Table name. Required parameter    
+  train_settings:                           # Settings for training process. Required parameter
+    source: "./files/order.csv"             # The path to the original data. Supported formats include local files in CSV, Avro formats. Required parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    column_types:
+    categorical:                            # Force listed columns to have categorical type (use dictionary of values). Optional parameter
+      - gender
+      - marital_status
      
-        train_settings:                             # Settings for training process. Optional parameter
-            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
-            drop_null: False                        # Drop rows with NULL values. Optional parameter
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
-                    - gender
-                    - marital_status
+  infer_settings:                           # Settings for infer process. Optional parameter
+    destination: "./files/generated_data_order.csv"# The path where the generated data will be stored. Supported formats include local files in CSV, Avro formats. Required parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+  format:                                   # Settings for reading and writing data in 'csv' format. Optional parameter
+    sep: ','                                # Delimiter to use. Optional parameter
+    quotechar: '"'                          # The character used to denote the start and end of a quoted item. Optional parameter
+    quoting: minimal                        # Control field quoting behavior per constants - ["all", "minimal", "non-numeric", "none"]. Optional parameter
+    escapechar: '"'                         # One-character string used to escape other characters. Optional parameter
+    encoding: null                          # A string representing the encoding to use in the output file. Optional parameter
+    header: infer                           # Row number(s) to use as the column names, and the start of the data. Optional parameter  
+    skiprows: null                          # Line numbers to skip (0-indexed) or number of lines to skip (int) at the start of the file. Optional parameter
+    on_bad_lines: error                     # Specifies what to do upon encountering a bad line (a line with too many fields) - ["error", "warn", "skip"]. Optional parameter
+    engine: null                            # Parser engine to use - ["c", "python"]. Optional parameter
+  keys:                                     # Keys of the table. Optional parameter
+    pk_order_id:
+      type: "PK"
+      columns:
+        - order_id
      
-        infer_settings:                             # Settings for infer process. Optional parameter
-            size: 100                               # Size for generated data. Optional parameter
-            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
-            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
-        keys:                                       # Keys of the table. Optional parameter
-            pk_order_id:
-                type: "PK"
-                columns:
-                    - order_id
-     
-            FK1:
-                type: "FK"
-                columns:
-                    - customer_id
-                references:
-                    table: "CUSTOMER"
-                    columns:
-                        - customer_id
+    FK1:
+      type: "FK"
+      columns:
+        - customer_id
+      references:
+        table: "CUSTOMER"
+        columns:
+          - customer_id
+```
+<i>Note:</i>In the section <i>"global"</i> you can specify training and inference settings for all tables. If the same settings are specified for a specific table, they will override the global settings.<br>
 
-<i>You can find the example of metadata file in [example-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)</i><br>
+<i>You can find the example of metadata file in [examples/example-metadata/housing_metadata.yaml](examples/example-metadata/housing_metadata.yaml)</i><br>
 
 By providing the necessary information through a metadata file, you can initiate training and inference processes using the following commands:
 
 ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE
 infer --metadata_path=PATH_TO_YAML_METADATA_FILE
 ```
 Here is a quick example:
 
 ```bash
-train --metadata_path="./example-metadata/housing_metadata.yaml"
-infer --metadata_path="./example-metadata/housing_metadata.yaml"
+train --metadata_path="./examples/example-metadata/housing_metadata.yaml"
+infer --metadata_path="./examples/example-metadata/housing_metadata.yaml"
 ```
 
 If `--metadata_path` is present and the metadata contains the necessary parameters, other CLI parameters will be ignored.<br>
 
 ### Docker images
 
 The train and inference components of <i>syngen</i> is available as public docker images:
```

#### html2text {}

```diff
@@ -1,19 +1,9 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.9 Summary: The tool uncovers
-patterns, trends, and correlations hidden within your production datasets.
-Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
-Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
-data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
-Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
-Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
-GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-
-Python: >3.7 Description-Content-Type: text/markdown License-File: LICENSE #
-EPAM Syngen EPAM Syngen is an unsupervised tabular data generation tool. It is
-useful for generation of test data with a given table as a template. Most
+# EPAM Syngen EPAM Syngen is an unsupervised tabular data generation tool. It
+is useful for generation of test data with a given table as a template. Most
 datatypes including floats, integers, datetime, text, categorical, binary are
 supported. The linked tables i.e., tables sharing a key can also be generated
 using the simple statistical approach. The source of data might be in CSV, Avro
 format and should be located locally and be in UTF-8 encoding. The tool is
 based on the variational autoencoder model (VAE). The Bayesian Gaussian Mixture
 model is used to further detangle the latent space. ## Getting started Use pip
 to install the library: `pip install syngen` The training and inference
@@ -23,20 +13,21 @@
 To start training with defaults parameters run: ```bash train --source
 PATH_TO_ORIGINAL_CSV \ --table_name TABLE_NAME ``` This will train a model and
 save the model artifacts to disk. To generate with defaults parameters data
 simply call: ```bash infer --table_name TABLE_NAME ``` Please notice that the
 name should match the one you used in the training process.
 This will create a csv file with the synthetic table in ./model_artifacts/
 tmp_store/TABLE_NAME/merged_infer_TABLE_NAME.csv.
-Here is a quick example: ```bash pip install syngen train --source ./example-
-data/housing.csv â-table_name Housing infer --table_name Housing ``` As the
-example you can use the dataset "Housing" in [example-data/housing.csv]
-(example-data/housing.csv). In this example, our real-world data is "Housing"
-from Kaggle. ## Features ### Training You can add flexibility to the training
-and inference processes using additional hyperparameters.
+Here is a quick example: ```bash pip install syngen train --source ./examples/
+example-data/housing.csv â-table_name Housing infer --table_name Housing ```
+As the example you can use the dataset "Housing" in [examples/example-data/
+housing.csv](examples/example-data/housing.csv). In this example, our real-
+world data is "Housing" from Kaggle. ## Features ### Training You can add
+flexibility to the training and inference processes using additional
+hyperparameters.
 For training of single table call: ```bash train --source PATH_TO_ORIGINAL_CSV
 \ --table_name TABLE_NAME \ --epochs INT \ --row_limit INT \ --drop_null BOOL \
 --print_report BOOL \ --batch_size INT ``` To train one or more tables using a
 metadata file, you can use the following command: ```bash train --metadata_path
 PATH_TO_METADATA_YAML ``` The parameters which you can set up for training
 process: - source â required parameter for training of single table, a path
 to the file that you want to use as a reference - table_name â required
@@ -90,69 +81,119 @@
 yaml format. By providing information about the relationships between tables
 via metadata, it becomes possible to manage complex relationships across any
 number of tables. You can also specify additional parameters needed for
 training and inference in the metadata file and in this case, they will be
 ignored in the CLI call. Note: By using metadata file, you can also generate
 tables with absent relationships. In this case, the tables will be generated
 independently. The yaml metadata file should match the following template:
-CUSTOMER: # Table name. Required parameter source: "./files/customer.csv" #
-Supported formats include local files in CSV, Avro formats. Required parameter
+```yaml global: # Global settings. Optional parameter. In this section you can
+specify training and inference settings which will be set for all tables
 train_settings: # Settings for training process. Optional parameter epochs: 10
 # Number of epochs if different from the default in the command line options.
 Optional parameter drop_null: False # Drop rows with NULL values. Optional
-parameter row_limit: None # Number of rows to train over. A number less than
+parameter row_limit: null # Number of rows to train over. A number less than
 the original table length will randomly subset the specified rows number.
 Optional parameter batch_size: 32 # If specified, the training is split into
 batches. This can save the RAM. Optional parameter print_report: False # Turn
-on or turn off generation of the report. Optional parameter column_types:
-categorical: # Force listed columns to have categorical type (use dictionary of
-values). Optional parameter - gender - marital_status infer_settings: #
+on or turn off generation of the report. Optional parameter infer_settings: #
 Settings for infer process. Optional parameter size: 100 # Size for generated
 data. Optional parameter run_parallel: False # Turn on or turn off parallel
 training process. Optional parameter print_report: False # Turn on or turn off
-generation of the report. Optional parameter batch_size: None # If specified,
+generation of the report. Optional parameter batch_size: null # If specified,
 the generation is split into batches. This can save the RAM. Optional parameter
-random_seed: None # If specified, generates a reproducible result. Optional
-parameter keys: # Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name
-of a key. Only one PK per table. type: "PK" # The key type. Supported: PK -
-primary key, FK - foreign key, TKN - token key columns: # Array of column names
-- customer_id UQ1: # Name of a key type: "UQ" # One or many unique keys
-columns: - e_mail FK1: # One or many foreign keys type: "FK" columns: # Array
-of columns in the current table - e_mail - alias references: table: "PROFILE" #
-Name of the parent table columns: # Array of columns in the parent table -
-e_mail - alias FK2: type: "FK" columns: - address_id references: table:
-"ADDRESS" columns: - address_id ORDER: # Table name. Required parameter source:
-"./files/order.csv" # Supported formats include local files in CSV, Avro
-formats. Required parameter train_settings: # Settings for training process.
-Optional parameter epochs: 10 # Number of epochs if different from the default
-in the command line options. Optional parameter drop_null: False # Drop rows
-with NULL values. Optional parameter row_limit: None # Number of rows to train
-over. A number less than the original table length will randomly subset the
-specified rows number. Optional parameter batch_size: 32 # If specified, the
-training is split into batches. This can save the RAM. Optional parameter
+random_seed: null # If specified, generates a reproducible result. Optional
+parameter CUSTOMER: # Table name. Required parameter train_settings: # Settings
+for training process. Required parameter source: "./files/customer.csv" # The
+path to the original data. Supported formats include local files in CSV, Avro
+formats. Required parameter epochs: 10 # Number of epochs if different from the
+default in the command line options. Optional parameter drop_null: False # Drop
+rows with NULL values. Optional parameter row_limit: null # Number of rows to
+train over. A number less than the original table length will randomly subset
+the specified rows number. Optional parameter batch_size: 32 # If specified,
+the training is split into batches. This can save the RAM. Optional parameter
 print_report: False # Turn on or turn off generation of the report. Optional
 parameter column_types: categorical: # Force listed columns to have categorical
 type (use dictionary of values). Optional parameter - gender - marital_status
-infer_settings: # Settings for infer process. Optional parameter size: 100 #
-Size for generated data. Optional parameter run_parallel: False # Turn on or
-turn off parallel training process. Optional parameter print_report: False #
-Turn on or turn off generation of the report. Optional parameter batch_size:
-None # If specified, the generation is split into batches. This can save the
-RAM. Optional parameter random_seed: None # If specified, generates a
-reproducible result. Optional parameter keys: # Keys of the table. Optional
-parameter pk_order_id: type: "PK" columns: - order_id FK1: type: "FK" columns:
-- customer_id references: table: "CUSTOMER" columns: - customer_id You can find
-the example of metadata file in [example-metadata/housing_metadata.yaml]
-(example-metadata/housing_metadata.yaml)
+format: # Settings for reading and writing data in 'csv' format. Optional
+parameter sep: ',' # Delimiter to use. Optional parameter quotechar: '"' # The
+character used to denote the start and end of a quoted item. Optional parameter
+quoting: minimal # Control field quoting behavior per constants - ["all",
+"minimal", "non-numeric", "none"]. Optional parameter escapechar: '"' # One-
+character string used to escape other characters. Optional parameter encoding:
+null # A string representing the encoding to use in the output file. Optional
+parameter header: infer # Row number(s) to use as the column names, and the
+start of the data. Optional parameter skiprows: null # Line numbers to skip (0-
+indexed) or number of lines to skip (int) at the start of the file. Optional
+parameter on_bad_lines: error # Specifies what to do upon encountering a bad
+line (a line with too many fields) - ["error", "warn", "skip"]. Optional
+parameter engine: null # Parser engine to use - ["c", "python"]. Optional
+parameter infer_settings: # Settings for infer process. Optional parameter
+destination: "./files/generated_data_customer.csv"# The path where the
+generated data will be stored. Supported formats include local files in CSV,
+Avro formats. Required parameter size: 100 # Size for generated data. Optional
+parameter run_parallel: False # Turn on or turn off parallel training process.
+Optional parameter print_report: False # Turn on or turn off generation of the
+report. Optional parameter batch_size: null # If specified, the generation is
+split into batches. This can save the RAM. Optional parameter random_seed: null
+# If specified, generates a reproducible result. Optional parameter keys: #
+Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name of a key. Only one
+PK per table. type: "PK" # The key type. Supported: PK - primary key, FK -
+foreign key, TKN - token key columns: # Array of column names - customer_id
+UQ1: # Name of a key type: "UQ" # One or many unique keys columns: - e_mail
+FK1: # One or many foreign keys type: "FK" columns: # Array of columns in the
+current table - e_mail - alias references: table: "PROFILE" # Name of the
+parent table columns: # Array of columns in the parent table - e_mail - alias
+FK2: type: "FK" columns: - address_id references: table: "ADDRESS" columns: -
+address_id ORDER: # Table name. Required parameter train_settings: # Settings
+for training process. Required parameter source: "./files/order.csv" # The path
+to the original data. Supported formats include local files in CSV, Avro
+formats. Required parameter epochs: 10 # Number of epochs if different from the
+default in the command line options. Optional parameter drop_null: False # Drop
+rows with NULL values. Optional parameter row_limit: null # Number of rows to
+train over. A number less than the original table length will randomly subset
+the specified rows number. Optional parameter batch_size: 32 # If specified,
+the training is split into batches. This can save the RAM. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter column_types: categorical: # Force listed columns to have categorical
+type (use dictionary of values). Optional parameter - gender - marital_status
+infer_settings: # Settings for infer process. Optional parameter destination:
+"./files/generated_data_order.csv"# The path where the generated data will be
+stored. Supported formats include local files in CSV, Avro formats. Required
+parameter size: 100 # Size for generated data. Optional parameter run_parallel:
+False # Turn on or turn off parallel training process. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter batch_size: null # If specified, the generation is split into
+batches. This can save the RAM. Optional parameter random_seed: null # If
+specified, generates a reproducible result. Optional parameter format: #
+Settings for reading and writing data in 'csv' format. Optional parameter sep:
+',' # Delimiter to use. Optional parameter quotechar: '"' # The character used
+to denote the start and end of a quoted item. Optional parameter quoting:
+minimal # Control field quoting behavior per constants - ["all", "minimal",
+"non-numeric", "none"]. Optional parameter escapechar: '"' # One-character
+string used to escape other characters. Optional parameter encoding: null # A
+string representing the encoding to use in the output file. Optional parameter
+header: infer # Row number(s) to use as the column names, and the start of the
+data. Optional parameter skiprows: null # Line numbers to skip (0-indexed) or
+number of lines to skip (int) at the start of the file. Optional parameter
+on_bad_lines: error # Specifies what to do upon encountering a bad line (a line
+with too many fields) - ["error", "warn", "skip"]. Optional parameter engine:
+null # Parser engine to use - ["c", "python"]. Optional parameter keys: # Keys
+of the table. Optional parameter pk_order_id: type: "PK" columns: - order_id
+FK1: type: "FK" columns: - customer_id references: table: "CUSTOMER" columns: -
+customer_id ``` Note:In the section "global" you can specify training and
+inference settings for all tables. If the same settings are specified for a
+specific table, they will override the global settings.
+You can find the example of metadata file in [examples/example-metadata/
+housing_metadata.yaml](examples/example-metadata/housing_metadata.yaml)
 By providing the necessary information through a metadata file, you can
 initiate training and inference processes using the following commands: ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE infer --
 metadata_path=PATH_TO_YAML_METADATA_FILE ``` Here is a quick example: ```bash
-train --metadata_path="./example-metadata/housing_metadata.yaml" infer --
-metadata_path="./example-metadata/housing_metadata.yaml" ``` If `--
+train --metadata_path="./examples/example-metadata/housing_metadata.yaml" infer
+--metadata_path="./examples/example-metadata/housing_metadata.yaml" ``` If `--
 metadata_path` is present and the metadata contains the necessary parameters,
 other CLI parameters will be ignored.
 ### Docker images The train and inference components of syngen is available as
 public docker images:
 hub.docker.com/r/tdspora/syngen-train>
 hub.docker.com/r/tdspora/syngen-infer> To run dockerized code (see parameters
 description in *Training* and *Inference* sections) for one table call: ```bash
```

### Comparing `syngen-0.1.9/README.md` & `syngen-0.2.0rc0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: syngen
+Version: 0.2.0rc0
+Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
+Home-page: https://github.com/tdspora/syngen
+Author: EPAM Systems, Inc.
+Maintainer: Pavel Bobyrev
+License: GPLv3 License
+Keywords: data,generation,synthetic,vae,tabular
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # EPAM Syngen
 
 EPAM Syngen is an unsupervised tabular data generation tool. It is useful for generation of test data with a given table as a template. Most datatypes including floats, integers, datetime, text, categorical, binary are supported. The linked tables i.e., tables sharing a key can also be generated using the simple statistical approach. 
 The source of data might be in CSV, Avro format and should be located locally and be in UTF-8 encoding.
 
 The tool is based on the variational autoencoder model (VAE). The Bayesian Gaussian Mixture model is used to further detangle the latent space.
 
@@ -31,18 +50,18 @@
 <i>Please notice that the name should match the one you used in the training process.</i><br>
 This will create a csv file with the synthetic table in <i>./model_artifacts/tmp_store/TABLE_NAME/merged_infer_TABLE_NAME.csv</i>.<br>
 
 Here is a quick example:
 
 ```bash
 pip install syngen
-train --source ./example-data/housing.csv –-table_name Housing
+train --source ./examples/example-data/housing.csv –-table_name Housing
 infer --table_name Housing
 ```
-As the example you can use the dataset <i>"Housing"</i> in [example-data/housing.csv](example-data/housing.csv).
+As the example you can use the dataset <i>"Housing"</i> in [examples/example-data/housing.csv](examples/example-data/housing.csv).
 In this example, our real-world data is <a href="https://www.kaggle.com/datasets/camnugent/california-housing-prices" target="_blank">"Housing"</a> from Kaggle.
 
 ## Features
 
 ### Training
 
 You can add flexibility to the training and inference processes using additional hyperparameters.<br>
@@ -148,115 +167,152 @@
 You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
 they will be ignored in the CLI call.
 
 <i>Note:</i> By using metadata file, you can also generate tables with absent relationships. 
 In this case, the tables will be generated independently.
 
 The yaml metadata file should match the following template:
-
-    CUSTOMER:                                       # Table name. Required parameter
-        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats. Required parameter
-                 
-        train_settings:                             # Settings for training process. Optional parameter
-            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
-            drop_null: False                        # Drop rows with NULL values. Optional parameter
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
-                    - gender
-                    - marital_status
-                 
-        infer_settings:                             # Settings for infer process. Optional parameter
-            size: 100                               # Size for generated data. Optional parameter
-            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
-            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
-        keys:                                       # Keys of the table. Optional parameter
-            PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
-                type: "PK"                          # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
-                columns:                            # Array of column names
-                    - customer_id
+```yaml
+global:                                     # Global settings. Optional parameter. In this section you can specify training and inference settings which will be set for all tables
+  train_settings:                           # Settings for training process. Optional parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    
+  infer_settings:                           # Settings for infer process. Optional parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+
+CUSTOMER:                                   # Table name. Required parameter               
+  train_settings:                           # Settings for training process. Required parameter
+    source: "./files/customer.csv"          # The path to the original data. Supported formats include local files in CSV, Avro formats. Required parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    column_types:
+      categorical:                          # Force listed columns to have categorical type (use dictionary of values). Optional parameter
+        - gender
+        - marital_status
+        
+  format:                                   # Settings for reading and writing data in 'csv' format. Optional parameter
+    sep: ','                                # Delimiter to use. Optional parameter
+    quotechar: '"'                          # The character used to denote the start and end of a quoted item. Optional parameter
+    quoting: minimal                        # Control field quoting behavior per constants - ["all", "minimal", "non-numeric", "none"]. Optional parameter
+    escapechar: '"'                         # One-character string used to escape other characters. Optional parameter
+    encoding: null                          # A string representing the encoding to use in the output file. Optional parameter
+    header: infer                           # Row number(s) to use as the column names, and the start of the data. Optional parameter  
+    skiprows: null                          # Line numbers to skip (0-indexed) or number of lines to skip (int) at the start of the file. Optional parameter
+    on_bad_lines: error                     # Specifies what to do upon encountering a bad line (a line with too many fields) - ["error", "warn", "skip"]. Optional parameter
+    engine: null                            # Parser engine to use - ["c", "python"]. Optional parameter             
+  infer_settings:                           # Settings for infer process. Optional parameter
+    destination: "./files/generated_data_customer.csv"# The path where the generated data will be stored. Supported formats include local files in CSV, Avro formats. Required parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+  keys:                                     # Keys of the table. Optional parameter
+    PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
+      type: "PK"                            # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
+      columns:                              # Array of column names
+        - customer_id
      
-            UQ1:                                    # Name of a key
-                type: "UQ"                          # One or many unique keys
-                columns:
-                    - e_mail
+    UQ1:                                    # Name of a key
+      type: "UQ"                            # One or many unique keys
+      columns:
+        - e_mail
      
-            FK1:                                    # One or many foreign keys
-                type: "FK"
-                columns:                            # Array of columns in the current table
-                    - e_mail
-                    - alias
-                references:
-                    table: "PROFILE"                # Name of the parent table
-                    columns:                        # Array of columns in the parent table
-                        - e_mail
-                        - alias
+    FK1:                                    # One or many foreign keys
+      type: "FK"
+      columns:                              # Array of columns in the current table
+        - e_mail
+        - alias
+      references:
+        table: "PROFILE"                    # Name of the parent table
+        columns:                            # Array of columns in the parent table
+          - e_mail
+          - alias
        
-            FK2:
-                type: "FK"
-                columns:
-                    - address_id
-                references:
-                    table: "ADDRESS"
-                    columns:
-                        - address_id
+    FK2:
+      type: "FK"
+      columns:
+        - address_id
+      references:
+        table: "ADDRESS"
+        columns:
+          - address_id
 
      
-    ORDER:                                          # Table name. Required parameter
-        source: "./files/order.csv"                 # Supported formats include local files in CSV, Avro formats. Required parameter
+ORDER:                                      # Table name. Required parameter    
+  train_settings:                           # Settings for training process. Required parameter
+    source: "./files/order.csv"             # The path to the original data. Supported formats include local files in CSV, Avro formats. Required parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    column_types:
+    categorical:                            # Force listed columns to have categorical type (use dictionary of values). Optional parameter
+      - gender
+      - marital_status
      
-        train_settings:                             # Settings for training process. Optional parameter
-            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
-            drop_null: False                        # Drop rows with NULL values. Optional parameter
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
-                    - gender
-                    - marital_status
+  infer_settings:                           # Settings for infer process. Optional parameter
+    destination: "./files/generated_data_order.csv"# The path where the generated data will be stored. Supported formats include local files in CSV, Avro formats. Required parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+  format:                                   # Settings for reading and writing data in 'csv' format. Optional parameter
+    sep: ','                                # Delimiter to use. Optional parameter
+    quotechar: '"'                          # The character used to denote the start and end of a quoted item. Optional parameter
+    quoting: minimal                        # Control field quoting behavior per constants - ["all", "minimal", "non-numeric", "none"]. Optional parameter
+    escapechar: '"'                         # One-character string used to escape other characters. Optional parameter
+    encoding: null                          # A string representing the encoding to use in the output file. Optional parameter
+    header: infer                           # Row number(s) to use as the column names, and the start of the data. Optional parameter  
+    skiprows: null                          # Line numbers to skip (0-indexed) or number of lines to skip (int) at the start of the file. Optional parameter
+    on_bad_lines: error                     # Specifies what to do upon encountering a bad line (a line with too many fields) - ["error", "warn", "skip"]. Optional parameter
+    engine: null                            # Parser engine to use - ["c", "python"]. Optional parameter
+  keys:                                     # Keys of the table. Optional parameter
+    pk_order_id:
+      type: "PK"
+      columns:
+        - order_id
      
-        infer_settings:                             # Settings for infer process. Optional parameter
-            size: 100                               # Size for generated data. Optional parameter
-            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
-            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
-        keys:                                       # Keys of the table. Optional parameter
-            pk_order_id:
-                type: "PK"
-                columns:
-                    - order_id
-     
-            FK1:
-                type: "FK"
-                columns:
-                    - customer_id
-                references:
-                    table: "CUSTOMER"
-                    columns:
-                        - customer_id
+    FK1:
+      type: "FK"
+      columns:
+        - customer_id
+      references:
+        table: "CUSTOMER"
+        columns:
+          - customer_id
+```
+<i>Note:</i>In the section <i>"global"</i> you can specify training and inference settings for all tables. If the same settings are specified for a specific table, they will override the global settings.<br>
 
-<i>You can find the example of metadata file in [example-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)</i><br>
+<i>You can find the example of metadata file in [examples/example-metadata/housing_metadata.yaml](examples/example-metadata/housing_metadata.yaml)</i><br>
 
 By providing the necessary information through a metadata file, you can initiate training and inference processes using the following commands:
 
 ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE
 infer --metadata_path=PATH_TO_YAML_METADATA_FILE
 ```
 Here is a quick example:
 
 ```bash
-train --metadata_path="./example-metadata/housing_metadata.yaml"
-infer --metadata_path="./example-metadata/housing_metadata.yaml"
+train --metadata_path="./examples/example-metadata/housing_metadata.yaml"
+infer --metadata_path="./examples/example-metadata/housing_metadata.yaml"
 ```
 
 If `--metadata_path` is present and the metadata contains the necessary parameters, other CLI parameters will be ignored.<br>
 
 ### Docker images
 
 The train and inference components of <i>syngen</i> is available as public docker images:
```

#### html2text {}

```diff
@@ -1,9 +1,19 @@
-# EPAM Syngen EPAM Syngen is an unsupervised tabular data generation tool. It
-is useful for generation of test data with a given table as a template. Most
+Metadata-Version: 2.1 Name: syngen Version: 0.2.0rc0 Summary: The tool uncovers
+patterns, trends, and correlations hidden within your production datasets.
+Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
+Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
+data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
+Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
+GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-
+Python: >3.7 Description-Content-Type: text/markdown License-File: LICENSE #
+EPAM Syngen EPAM Syngen is an unsupervised tabular data generation tool. It is
+useful for generation of test data with a given table as a template. Most
 datatypes including floats, integers, datetime, text, categorical, binary are
 supported. The linked tables i.e., tables sharing a key can also be generated
 using the simple statistical approach. The source of data might be in CSV, Avro
 format and should be located locally and be in UTF-8 encoding. The tool is
 based on the variational autoencoder model (VAE). The Bayesian Gaussian Mixture
 model is used to further detangle the latent space. ## Getting started Use pip
 to install the library: `pip install syngen` The training and inference
@@ -13,20 +23,21 @@
 To start training with defaults parameters run: ```bash train --source
 PATH_TO_ORIGINAL_CSV \ --table_name TABLE_NAME ``` This will train a model and
 save the model artifacts to disk. To generate with defaults parameters data
 simply call: ```bash infer --table_name TABLE_NAME ``` Please notice that the
 name should match the one you used in the training process.
 This will create a csv file with the synthetic table in ./model_artifacts/
 tmp_store/TABLE_NAME/merged_infer_TABLE_NAME.csv.
-Here is a quick example: ```bash pip install syngen train --source ./example-
-data/housing.csv â-table_name Housing infer --table_name Housing ``` As the
-example you can use the dataset "Housing" in [example-data/housing.csv]
-(example-data/housing.csv). In this example, our real-world data is "Housing"
-from Kaggle. ## Features ### Training You can add flexibility to the training
-and inference processes using additional hyperparameters.
+Here is a quick example: ```bash pip install syngen train --source ./examples/
+example-data/housing.csv â-table_name Housing infer --table_name Housing ```
+As the example you can use the dataset "Housing" in [examples/example-data/
+housing.csv](examples/example-data/housing.csv). In this example, our real-
+world data is "Housing" from Kaggle. ## Features ### Training You can add
+flexibility to the training and inference processes using additional
+hyperparameters.
 For training of single table call: ```bash train --source PATH_TO_ORIGINAL_CSV
 \ --table_name TABLE_NAME \ --epochs INT \ --row_limit INT \ --drop_null BOOL \
 --print_report BOOL \ --batch_size INT ``` To train one or more tables using a
 metadata file, you can use the following command: ```bash train --metadata_path
 PATH_TO_METADATA_YAML ``` The parameters which you can set up for training
 process: - source â required parameter for training of single table, a path
 to the file that you want to use as a reference - table_name â required
@@ -80,69 +91,119 @@
 yaml format. By providing information about the relationships between tables
 via metadata, it becomes possible to manage complex relationships across any
 number of tables. You can also specify additional parameters needed for
 training and inference in the metadata file and in this case, they will be
 ignored in the CLI call. Note: By using metadata file, you can also generate
 tables with absent relationships. In this case, the tables will be generated
 independently. The yaml metadata file should match the following template:
-CUSTOMER: # Table name. Required parameter source: "./files/customer.csv" #
-Supported formats include local files in CSV, Avro formats. Required parameter
+```yaml global: # Global settings. Optional parameter. In this section you can
+specify training and inference settings which will be set for all tables
 train_settings: # Settings for training process. Optional parameter epochs: 10
 # Number of epochs if different from the default in the command line options.
 Optional parameter drop_null: False # Drop rows with NULL values. Optional
-parameter row_limit: None # Number of rows to train over. A number less than
+parameter row_limit: null # Number of rows to train over. A number less than
 the original table length will randomly subset the specified rows number.
 Optional parameter batch_size: 32 # If specified, the training is split into
 batches. This can save the RAM. Optional parameter print_report: False # Turn
-on or turn off generation of the report. Optional parameter column_types:
-categorical: # Force listed columns to have categorical type (use dictionary of
-values). Optional parameter - gender - marital_status infer_settings: #
+on or turn off generation of the report. Optional parameter infer_settings: #
 Settings for infer process. Optional parameter size: 100 # Size for generated
 data. Optional parameter run_parallel: False # Turn on or turn off parallel
 training process. Optional parameter print_report: False # Turn on or turn off
-generation of the report. Optional parameter batch_size: None # If specified,
+generation of the report. Optional parameter batch_size: null # If specified,
 the generation is split into batches. This can save the RAM. Optional parameter
-random_seed: None # If specified, generates a reproducible result. Optional
-parameter keys: # Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name
-of a key. Only one PK per table. type: "PK" # The key type. Supported: PK -
-primary key, FK - foreign key, TKN - token key columns: # Array of column names
-- customer_id UQ1: # Name of a key type: "UQ" # One or many unique keys
-columns: - e_mail FK1: # One or many foreign keys type: "FK" columns: # Array
-of columns in the current table - e_mail - alias references: table: "PROFILE" #
-Name of the parent table columns: # Array of columns in the parent table -
-e_mail - alias FK2: type: "FK" columns: - address_id references: table:
-"ADDRESS" columns: - address_id ORDER: # Table name. Required parameter source:
-"./files/order.csv" # Supported formats include local files in CSV, Avro
-formats. Required parameter train_settings: # Settings for training process.
-Optional parameter epochs: 10 # Number of epochs if different from the default
-in the command line options. Optional parameter drop_null: False # Drop rows
-with NULL values. Optional parameter row_limit: None # Number of rows to train
-over. A number less than the original table length will randomly subset the
-specified rows number. Optional parameter batch_size: 32 # If specified, the
-training is split into batches. This can save the RAM. Optional parameter
+random_seed: null # If specified, generates a reproducible result. Optional
+parameter CUSTOMER: # Table name. Required parameter train_settings: # Settings
+for training process. Required parameter source: "./files/customer.csv" # The
+path to the original data. Supported formats include local files in CSV, Avro
+formats. Required parameter epochs: 10 # Number of epochs if different from the
+default in the command line options. Optional parameter drop_null: False # Drop
+rows with NULL values. Optional parameter row_limit: null # Number of rows to
+train over. A number less than the original table length will randomly subset
+the specified rows number. Optional parameter batch_size: 32 # If specified,
+the training is split into batches. This can save the RAM. Optional parameter
 print_report: False # Turn on or turn off generation of the report. Optional
 parameter column_types: categorical: # Force listed columns to have categorical
 type (use dictionary of values). Optional parameter - gender - marital_status
-infer_settings: # Settings for infer process. Optional parameter size: 100 #
-Size for generated data. Optional parameter run_parallel: False # Turn on or
-turn off parallel training process. Optional parameter print_report: False #
-Turn on or turn off generation of the report. Optional parameter batch_size:
-None # If specified, the generation is split into batches. This can save the
-RAM. Optional parameter random_seed: None # If specified, generates a
-reproducible result. Optional parameter keys: # Keys of the table. Optional
-parameter pk_order_id: type: "PK" columns: - order_id FK1: type: "FK" columns:
-- customer_id references: table: "CUSTOMER" columns: - customer_id You can find
-the example of metadata file in [example-metadata/housing_metadata.yaml]
-(example-metadata/housing_metadata.yaml)
+format: # Settings for reading and writing data in 'csv' format. Optional
+parameter sep: ',' # Delimiter to use. Optional parameter quotechar: '"' # The
+character used to denote the start and end of a quoted item. Optional parameter
+quoting: minimal # Control field quoting behavior per constants - ["all",
+"minimal", "non-numeric", "none"]. Optional parameter escapechar: '"' # One-
+character string used to escape other characters. Optional parameter encoding:
+null # A string representing the encoding to use in the output file. Optional
+parameter header: infer # Row number(s) to use as the column names, and the
+start of the data. Optional parameter skiprows: null # Line numbers to skip (0-
+indexed) or number of lines to skip (int) at the start of the file. Optional
+parameter on_bad_lines: error # Specifies what to do upon encountering a bad
+line (a line with too many fields) - ["error", "warn", "skip"]. Optional
+parameter engine: null # Parser engine to use - ["c", "python"]. Optional
+parameter infer_settings: # Settings for infer process. Optional parameter
+destination: "./files/generated_data_customer.csv"# The path where the
+generated data will be stored. Supported formats include local files in CSV,
+Avro formats. Required parameter size: 100 # Size for generated data. Optional
+parameter run_parallel: False # Turn on or turn off parallel training process.
+Optional parameter print_report: False # Turn on or turn off generation of the
+report. Optional parameter batch_size: null # If specified, the generation is
+split into batches. This can save the RAM. Optional parameter random_seed: null
+# If specified, generates a reproducible result. Optional parameter keys: #
+Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name of a key. Only one
+PK per table. type: "PK" # The key type. Supported: PK - primary key, FK -
+foreign key, TKN - token key columns: # Array of column names - customer_id
+UQ1: # Name of a key type: "UQ" # One or many unique keys columns: - e_mail
+FK1: # One or many foreign keys type: "FK" columns: # Array of columns in the
+current table - e_mail - alias references: table: "PROFILE" # Name of the
+parent table columns: # Array of columns in the parent table - e_mail - alias
+FK2: type: "FK" columns: - address_id references: table: "ADDRESS" columns: -
+address_id ORDER: # Table name. Required parameter train_settings: # Settings
+for training process. Required parameter source: "./files/order.csv" # The path
+to the original data. Supported formats include local files in CSV, Avro
+formats. Required parameter epochs: 10 # Number of epochs if different from the
+default in the command line options. Optional parameter drop_null: False # Drop
+rows with NULL values. Optional parameter row_limit: null # Number of rows to
+train over. A number less than the original table length will randomly subset
+the specified rows number. Optional parameter batch_size: 32 # If specified,
+the training is split into batches. This can save the RAM. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter column_types: categorical: # Force listed columns to have categorical
+type (use dictionary of values). Optional parameter - gender - marital_status
+infer_settings: # Settings for infer process. Optional parameter destination:
+"./files/generated_data_order.csv"# The path where the generated data will be
+stored. Supported formats include local files in CSV, Avro formats. Required
+parameter size: 100 # Size for generated data. Optional parameter run_parallel:
+False # Turn on or turn off parallel training process. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter batch_size: null # If specified, the generation is split into
+batches. This can save the RAM. Optional parameter random_seed: null # If
+specified, generates a reproducible result. Optional parameter format: #
+Settings for reading and writing data in 'csv' format. Optional parameter sep:
+',' # Delimiter to use. Optional parameter quotechar: '"' # The character used
+to denote the start and end of a quoted item. Optional parameter quoting:
+minimal # Control field quoting behavior per constants - ["all", "minimal",
+"non-numeric", "none"]. Optional parameter escapechar: '"' # One-character
+string used to escape other characters. Optional parameter encoding: null # A
+string representing the encoding to use in the output file. Optional parameter
+header: infer # Row number(s) to use as the column names, and the start of the
+data. Optional parameter skiprows: null # Line numbers to skip (0-indexed) or
+number of lines to skip (int) at the start of the file. Optional parameter
+on_bad_lines: error # Specifies what to do upon encountering a bad line (a line
+with too many fields) - ["error", "warn", "skip"]. Optional parameter engine:
+null # Parser engine to use - ["c", "python"]. Optional parameter keys: # Keys
+of the table. Optional parameter pk_order_id: type: "PK" columns: - order_id
+FK1: type: "FK" columns: - customer_id references: table: "CUSTOMER" columns: -
+customer_id ``` Note:In the section "global" you can specify training and
+inference settings for all tables. If the same settings are specified for a
+specific table, they will override the global settings.
+You can find the example of metadata file in [examples/example-metadata/
+housing_metadata.yaml](examples/example-metadata/housing_metadata.yaml)
 By providing the necessary information through a metadata file, you can
 initiate training and inference processes using the following commands: ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE infer --
 metadata_path=PATH_TO_YAML_METADATA_FILE ``` Here is a quick example: ```bash
-train --metadata_path="./example-metadata/housing_metadata.yaml" infer --
-metadata_path="./example-metadata/housing_metadata.yaml" ``` If `--
+train --metadata_path="./examples/example-metadata/housing_metadata.yaml" infer
+--metadata_path="./examples/example-metadata/housing_metadata.yaml" ``` If `--
 metadata_path` is present and the metadata contains the necessary parameters,
 other CLI parameters will be ignored.
 ### Docker images The train and inference components of syngen is available as
 public docker images:
 hub.docker.com/r/tdspora/syngen-train>
 hub.docker.com/r/tdspora/syngen-infer> To run dockerized code (see parameters
 description in *Training* and *Inference* sections) for one table call: ```bash
```

### Comparing `syngen-0.1.9/setup.cfg` & `syngen-0.2.0rc0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -20,44 +20,41 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
 python_requires = >3.7
 install_requires = 
-	attr
-	attrs==21.4.*
 	category_encoders==2.5.*
 	click
 	ipython==8.4.*
-	keras==2.8.*
+	keras==2.12.*
 	lazy==1.4
 	loguru
 	matplotlib==3.5.*
-	numpy==1.20.*
+	numpy==1.22.*
 	pandas==1.3.*
 	pandavro==1.7.*
 	pathos==0.2.*
 	scikit_learn==1.1.*
 	scipy==1.7.*
 	seaborn==0.11.*
-	tensorflow==2.8.*
+	tensorflow==2.12.*
 	tqdm==4.64.*
-	protobuf==3.19.*
 	PyYAML==6.*
 	MarkupSafe==2.0.1
 	Jinja2
-	schema
 	avro
 	python-slugify[unidecode]>=7.0.0
 	pytest
 	pytest-reportportal
 	reportportal-client
 	base32-crockford
 	py-ulid
+	marshmallow==3.19.*
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.py, *.html, *.ttf, *.svg, *.css, *.js
```

### Comparing `syngen-0.1.9/src/syngen/infer.py` & `syngen-0.2.0rc0/src/syngen/infer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import os
 from typing import Optional
 
 import click
 from loguru import logger
 
 from syngen.ml.worker import Worker
-from syngen.ml.custom_logger import setup_logger
+from syngen.ml.utils import setup_logger
 
 
 @click.command()
 @click.option("--metadata_path", type=str, default=None, help="Path to the metadata file")
 @click.option("--size", default=100, type=click.IntRange(1),
               help="Desired number of rows to generate. If absent, it's defaulted to 100")
 @click.option("--table_name", default=None, type=str, help="Name of the table, same as in training")
@@ -46,18 +47,20 @@
     batch_size
     print_report
     random_seed
     log_level
     -------
 
     """
-    setup_logger(log_level)
+    os.environ["LOGURU_LEVEL"] = log_level
+    setup_logger()
     if not metadata_path and not table_name:
         raise AttributeError("It seems that the information of 'metadata_path' or 'table_name' is absent. "
-                             "Please provide either the information of 'metadata_path' or the information of 'table_name'")
+                             "Please provide either the information of 'metadata_path' or the information "
+                             "of 'table_name'")
     if metadata_path and table_name:
         logger.warning("The information of 'metadata_path' was provided. "
                        "In this case the information of 'table_name' will be ignored")
         table_name = None
     logger.warning(
         "The inference process will be executed according to the information mentioned in 'infer_settings' "
         "in the metadata file. If appropriate information is absent from the metadata file, then the values "
@@ -69,14 +72,16 @@
         "batch_size": batch_size,
         "print_report": print_report,
         "random_seed": random_seed
     }
     worker = Worker(
         table_name=table_name,
         metadata_path=metadata_path,
-        settings=settings
+        settings=settings,
+        log_level=log_level,
+        type="infer"
     )
     worker.launch_infer()
 
 
 if __name__ == "__main__":
     launch_infer()
```

### Comparing `syngen-0.1.9/src/syngen/ml/config/configurations.py` & `syngen-0.2.0rc0/src/syngen/ml/config/configurations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass, field
-from typing import Optional, Dict, Tuple, Set
+from typing import Optional, Dict, Tuple, Set, List
 import os
+import shutil
 
-from loguru import logger
 import pandas as pd
+from loguru import logger
 
 from syngen.ml.data_loaders import DataLoader
 from syngen.ml.utils import slugify_attribute
 
 
 @dataclass
 class TrainConfig:
@@ -22,21 +23,27 @@
     metadata_path: Optional[str]
     print_report: bool
     batch_size: int
     paths: Dict = field(init=False)
     row_subset: int = field(init=False)
     schema: Dict = field(init=False)
     slugify_table_name: str = field(init=False)
+    columns: List = field(init=False)
+    dropped_columns: Set = field(init=False)
 
     def __post_init__(self):
         self.paths = self._set_paths()
+        self._remove_existed_artifacts()
         self._prepare_dirs()
 
     def preprocess_data(self):
         data, self.schema = self._extract_data()
+        data = self._remove_empty_columns(data)
+        self._mark_removed_columns(data)
+        self.columns = list(data.columns)
         self._prepare_data(data)
         self._set_batch_size()
 
     def to_dict(self) -> Dict:
         """
         Return the values of the settings of training process
         """
@@ -49,14 +56,25 @@
 
     def _set_batch_size(self):
         """
         Set up "batch_size" for training process
         """
         self.batch_size = min(self.batch_size, self.row_subset)
 
+    def _remove_existed_artifacts(self):
+        """
+        Remove existed artifacts from previous train process
+        """
+        if os.path.exists(self.paths["resources_path"]):
+            shutil.rmtree(self.paths["resources_path"])
+            logger.info(f"The artifacts located in the path - '{self.paths['resources_path']}' were removed")
+        if os.path.exists(self.paths["tmp_store_path"]):
+            shutil.rmtree(self.paths["tmp_store_path"])
+            logger.info(f"The artifacts located in the path - '{self.paths['tmp_store_path']}' were removed")
+
     def _prepare_dirs(self):
         """
         Create main directories for saving original, synthetic data and model artifacts
         """
         os.makedirs(self.paths["model_artifacts_path"], exist_ok=True)
         tmp_store_path = self.paths["tmp_store_path"]
         os.makedirs(self.paths["state_path"], exist_ok=True)
@@ -64,51 +82,54 @@
 
     def _load_source(self) -> Tuple[pd.DataFrame, Dict]:
         """
         Return dataframe and schema of original data
         """
         return DataLoader(self.source).load_data()
 
-    @staticmethod
-    def _remove_empty_columns(data: pd.DataFrame) -> Tuple[pd.DataFrame, Set]:
+    def _remove_empty_columns(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Remove completely empty columns from dataframe
         """
         data_columns = set(data.columns)
         data = data.dropna(how="all", axis=1)
 
-        dropped_cols = data_columns - set(data.columns)
-        if len(dropped_cols) > 0:
-            logger.info(f"Empty columns - {', '.join(dropped_cols)} were removed")
-        return data, dropped_cols
+        self.dropped_columns = data_columns - set(data.columns)
+        if len(self.dropped_columns) > 0:
+            logger.info(f"Empty columns - {', '.join(self.dropped_columns)} were removed")
+        return data
 
-    @staticmethod
-    def _mark_removed_columns(data: pd.DataFrame, schema: Optional[Dict], dropped_columns: Set) -> Dict:
+    def _mark_removed_columns(self, data: pd.DataFrame):
         """
         Mark removed columns in the schema
         """
-        if schema.get("format") == "CSV":
-            schema["fields"] = dict()
-            schema["fields"] = {
+        if self.schema.get("format") == "CSV":
+            self.schema["fields"] = dict()
+            self.schema["fields"] = {
                 column: "removed"
-                for column in dropped_columns
+                for column in self.dropped_columns
             }
         else:
-            for column, data_type in schema.get("fields", {}).items():
+            for column, data_type in self.schema.get("fields", {}).items():
                 if column not in data.columns:
-                    schema["fields"][column] = "removed"
-        return schema
+                    self.schema["fields"][column] = "removed"
+
+    def _check_if_data_is_empty(self, data: pd.DataFrame):
+        """
+        Check if the provided data is empty
+        """
+        if data.shape[0] < 1:
+            raise ValueError(f"The empty table was provided. Unable to train the table - '{self.table_name}'")
 
     def _extract_data(self) -> Tuple[pd.DataFrame, Dict]:
         """
         Extract data and schema necessary for training process
         """
         data, schema = self._load_source()
-        data, dropped_columns = self._remove_empty_columns(data)
-        schema = self._mark_removed_columns(data, schema, dropped_columns)
+        self._check_if_data_is_empty(data)
         return data, schema
 
     def _preprocess_data(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Preprocess data and set the parameter "row_subset" for training process
         """
         if self.drop_null:
@@ -138,58 +159,60 @@
         return data
 
     def _save_input_data(self, data: pd.DataFrame):
         DataLoader(self.paths["input_data_path"]).save_data(self.paths["input_data_path"], data)
 
     def _prepare_data(self, data: pd.DataFrame):
         """
-        Preprocess and save data necessary for training process
+        Preprocess and save the data necessary for the training process
         """
         data = self._preprocess_data(data)
         self._save_input_data(data)
 
     @slugify_attribute(table_name="slugify_table_name")
     def _set_paths(self) -> Dict:
         """
         Create the paths which used in training process
         """
 
         return {
             "model_artifacts_path": "model_artifacts/",
-            "tmp_store_path": f"model_artifacts/tmp_store/{self.slugify_table_name}",
+            "resources_path": f"model_artifacts/resources/{self.slugify_table_name}/",
+            "tmp_store_path": f"model_artifacts/tmp_store/{self.slugify_table_name}/",
             "source_path": self.source,
             "draws_path": f"model_artifacts/tmp_store/{self.slugify_table_name}/draws",
             "input_data_path":
                 f"model_artifacts/tmp_store/{self.slugify_table_name}/input_data_{self.slugify_table_name}.pkl",
             "state_path": f"model_artifacts/resources/{self.slugify_table_name}/vae/checkpoints",
             "train_config_pickle_path": f"model_artifacts/resources/{self.slugify_table_name}/vae/checkpoints/train_config.pkl",
             "dataset_pickle_path":
                 f"model_artifacts/resources/{self.slugify_table_name}/vae/checkpoints/model_dataset.pkl",
-            "fk_kde_path": f"model_artifacts/resources/{self.slugify_table_name}/vae/checkpoints/",
+            "fk_kde_path": f"model_artifacts/resources/{self.slugify_table_name}/vae/checkpoints/stat_keys/",
             "original_data_path":
                 f"model_artifacts/tmp_store/{self.slugify_table_name}/input_data_{self.slugify_table_name}.pkl",
-            "synthetic_data_path":
-                f"model_artifacts/tmp_store/{self.slugify_table_name}/merged_infer_{self.slugify_table_name}.csv",
+            "path_to_merged_infer": f"model_artifacts/tmp_store/{self.slugify_table_name}/merged_infer_{self.slugify_table_name}.csv",
             "no_ml_state_path": f"model_artifacts/resources/{self.slugify_table_name}/no_ml/checkpoints/"
         }
 
 
 @dataclass
 class InferConfig:
     """
     The configuration class to set up the work of infer process
     """
+    destination: Optional[str]
     size: Optional[int]
     table_name: Optional[str]
     run_parallel: bool
     batch_size: Optional[int]
     metadata_path: Optional[str]
     random_seed: Optional[int]
     print_report: bool
     both_keys: bool
+    log_level: str
     slugify_table_name: str = field(init=False)
 
     def __post_init__(self):
         self.paths = self._set_paths()
         self._set_up_reporting()
         self._set_up_size()
         self._set_up_batch_size()
@@ -235,19 +258,19 @@
     def _set_paths(self) -> Dict:
         """
         Create the paths which used in inference process
         """
         dynamic_name = self.slugify_table_name[:-3] if self.both_keys else self.slugify_table_name
         return {
             "original_data_path": f"model_artifacts/tmp_store/{dynamic_name}/input_data_{dynamic_name}.pkl",
-            "synthetic_data_path": f"model_artifacts/tmp_store/{dynamic_name}/merged_infer_{dynamic_name}.csv",
             "draws_path": f"model_artifacts/tmp_store/{dynamic_name}/draws",
             "input_data_path": f"model_artifacts/tmp_store/{dynamic_name}/input_data_{dynamic_name}.pkl",
-            "path_to_merged_infer": f"model_artifacts/tmp_store/{dynamic_name}/merged_infer_{dynamic_name}.csv",
+            "path_to_merged_infer": self.destination if self.destination is not None \
+                else f"model_artifacts/tmp_store/{dynamic_name}/merged_infer_{dynamic_name}.csv",
             "state_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints",
             "train_config_pickle_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/train_config.pkl",
             "tmp_store_path": f"model_artifacts/tmp_store/{dynamic_name}",
             "vae_resources_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/",
             "dataset_pickle_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/model_dataset.pkl",
-            "fk_kde_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/",
-            "path_to_no_ml": f"model_artifacts/resources/{dynamic_name}/no_ml/checkpoints/kde_params.pkl",
+            "fk_kde_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/stat_keys/",
+            "path_to_no_ml": f"model_artifacts/resources/{dynamic_name}/no_ml/checkpoints/kde_params.pkl"
         }
```

### Comparing `syngen-0.1.9/src/syngen/ml/convertor/convertor.py` & `syngen-0.2.0rc0/src/syngen/ml/convertor/convertor.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def __init__(self, schema, df):
         super().__init__(schema, df)
 
     def _convert_schema_and_df(self, schema, df) -> Tuple[Dict, pd.DataFrame]:
         preprocessed_df = self._preprocess_df(schema, df)
         return schema, preprocessed_df
 
+
 class AvroConvertor(Convertor):
     """
     Class for converting fetched avro schema
     """
     def __init__(self, schema, df):
         super().__init__(schema, df)
```

### Comparing `syngen-0.1.9/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.2.0rc0/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import os
 from pathlib import Path
 from abc import ABC, abstractmethod
 from typing import Optional, Dict, Tuple
 import pickle
+import csv
+import inspect
 
 import pandas as pd
+import pandas.errors
 import pandavro as pdx
 import yaml
-from yaml import Loader
+from yaml import SafeLoader
 from avro.datafile import DataFileReader
 from avro.io import DatumReader
 from loguru import logger
 
-from syngen.ml.validation_schema import validate_schema, configuration_schema
+from syngen.ml.validation_schema import ValidationSchema
 from syngen.ml.convertor import CSVConvertor, AvroConvertor
 from syngen.ml.utils import trim_string
+from syngen.ml.context import get_context, global_context
+
+
+DELIMITERS = {
+    "\\t": "\t"
+}
 
 
 class BaseDataLoader(ABC):
     """
     Abstract class for data loader
     """
 
@@ -48,78 +57,155 @@
             return True
         return False
 
     def __get_file_loader(self):
         path = Path(self.path)
         if path.suffix == '.avro':
             return AvroLoader()
-        elif path.suffix == '.csv':
+        elif path.suffix in ['.csv', '.txt']:
             return CSVLoader()
+        elif path.suffix == '.tsv':
+            return CSVLoader(sep="\t")
+        elif path.suffix == '.psv':
+            return CSVLoader(sep="|")
         elif path.suffix == ".pkl":
             return BinaryLoader()
         else:
-            raise NotImplementedError("File format not supported")
+            raise NotImplementedError(f"File format not supported for extension {path.suffix}")
 
-    def load_data(self) -> Tuple[pd.DataFrame, Dict]:
+    def load_data(self, **kwargs) -> Tuple[pd.DataFrame, Dict]:
         try:
-            df, schema = self.file_loader.load_data(self.path)
-            if df.shape[0] < 1:
-                raise ValueError("Empty file was provided. Unable to train")
+            df, schema = self.file_loader.load_data(self.path, **kwargs)
             return df, schema
         except UnicodeDecodeError as error:
             message = f"It seems that the content of the data in the path - '{self.path}' " \
                       f"doesn't have the encoding UTF-8. The details of the error - {error}.\n" \
                       f"Please, use the data in UTF-8 encoding"
             logger.error(message)
             raise ValueError(message)
+        except pandas.errors.EmptyDataError as error:
+            message = f"The empty file was provided. Unable to load data from the path - '{self.path}'. " \
+                      f"The details of the error - {error}"
+            logger.error(message)
+            raise ValueError(message)
 
     def save_data(self, path: str, df: pd.DataFrame, **kwargs):
-        self.file_loader.save_data(path, df)
+        self.file_loader.save_data(path, df, **kwargs)
 
 
-class CSVLoader(BaseDataLoader):
+class CSVLoader:
     """
-    Class for loading and saving data in csv format
+    Class for loading and saving data in CSV format.
     """
+    def __init__(self, **kwargs):
+        self.format = get_context().get_config()
+        self.format.update(kwargs)
+        global_context(self.format)
+
+    @staticmethod
+    def _get_quoting(quoting: Optional[str]) -> int:
+        quoting_map = {
+            "minimal": csv.QUOTE_MINIMAL,
+            "all": csv.QUOTE_ALL,
+            "non-numeric": csv.QUOTE_NONNUMERIC,
+            "none": csv.QUOTE_NONE
+        }
+        if isinstance(quoting, int):
+            return quoting
+        else:
+            return quoting_map.get(quoting.lower(), csv.QUOTE_NONE) if quoting else csv.QUOTE_NONE
+
+    @staticmethod
+    def _get_csv_params(**kwargs):
+        params = {}
+        format_params = kwargs.get("format")
+        
+        if format_params:
+            params.update(format_params)
+            quoting = format_params.get("quoting", None)
+            params["quoting"] = CSVLoader._get_quoting(quoting)
+            
+        return params
 
     @staticmethod
     def _load_data(path, **kwargs) -> Tuple[pd.DataFrame, Dict]:
-        df = pd.DataFrame()
+        params = CSVLoader._get_csv_params(**kwargs)
         try:
-            df = pd.read_csv(path, engine="c", **kwargs).apply(trim_string, axis=0)
-            return df, CSVConvertor({"fields": {}, "format": "CSV"}, df).schema
+            df = pd.read_csv(path, **params).apply(trim_string, axis=0)
+            if all([isinstance(column, int) for column in df.columns]):
+                df.rename(
+                    columns={k: f"column_{v}" for k, v in zip(df.columns, list(range(len(df.columns))))},
+                    inplace=True
+                )
+            sep = params.get("sep", ",")
+            if len(sep) > 1:
+                params["sep"] = ","
+            params["skiprows"] = None
+            global_context(params)
         except FileNotFoundError as error:
-            message = f"It seems that the path to the table isn't valid.\n" \
+            message = f"It seems that the path to the table isn't valid.\n"\
                       f"The details of the error - {error}.\n" \
                       f"Please, check the path to the table"
             logger.error(message)
             raise FileNotFoundError(message)
+        
+        return df, CSVConvertor({"fields": {}, "format": "CSV"}, df).schema
 
     def load_data(self, path, **kwargs):
-        return self._load_data(path, **kwargs)
+        return self._load_data(path, format=self.format, **kwargs)
 
     @staticmethod
     def _save_data(path: Optional[str], df: pd.DataFrame, **kwargs):
+        """
+        Save the provided DataFrame to a CSV file.
+        
+        :param path: The file path to save the DataFrame.
+        :param df: The DataFrame to be saved.
+        :param kwargs: Additional keyword arguments to be passed to the to_csv method.
+        """
+        format_params = CSVLoader._get_csv_params(**kwargs)
         if df is not None:
-            df.to_csv(path, **kwargs, index=False)
+            # Extract valid parameters
+            valid_parameters = inspect.signature(pd.DataFrame.to_csv).parameters
+            
+            # Filter out any keyword arguments that are not valid parameters
+            filtered_kwargs = {k: v for k, v in format_params.items() if k in valid_parameters}
+            for k, v in filtered_kwargs.items():
+                if isinstance(v, str) and v in DELIMITERS.keys():
+                    filtered_kwargs[k] = v.replace(v, DELIMITERS[v])
+
+            if "header" in filtered_kwargs and filtered_kwargs.get("header", None) is None:
+                filtered_kwargs["header"] = False
+            else:
+                filtered_kwargs["header"] = True
+
+            if "sep" in filtered_kwargs and len(filtered_kwargs.get("sep", None)) > 1:
+                filtered_kwargs["sep"] = ","
+                logger.warning(
+                    "As the length of the value of the parameter 'separator' is more than 1 character,"
+                    "the 'separator' will be set to ',' in accordance with the standard 'RFC 4180'"
+                )
+
+            # Save the DataFrame to a CSV file
+            df.to_csv(path, **filtered_kwargs, index=False)
 
     def save_data(self, path: str, df: pd.DataFrame, **kwargs):
         self._save_data(path, df, **kwargs)
 
 
 class AvroLoader(BaseDataLoader):
     """
     Class for loading and saving data in avro format
     """
 
     @staticmethod
     def _load_df(path) -> pd.DataFrame:
         """
         Load data in Avro format
-        :param path: the path to the the file
+        :param path: the path to the file
         :return: dataframe
         """
         return pdx.from_avro(path)
 
     def load_data(self, path: str, **kwargs) -> Tuple[pd.DataFrame, Dict]:
         """
         Load data in Avro format from AWS S3, Azure Storage or locally
@@ -140,15 +226,15 @@
                       f"Please, check the path to the table"
             logger.error(message)
             raise FileNotFoundError(message)
 
     @staticmethod
     def save_data(path: str, df: pd.DataFrame, **kwargs):
         if df is not None:
-            pdx.to_avro(path, df, **kwargs)
+            pdx.to_avro(path, df)
 
     @staticmethod
     def _load_schema(f, df) -> Tuple[Dict[str, str], pd.DataFrame]:
         """
         Load schema of the metadata of the table in Avro format and preprocess dataframe
         :param f: object of the class 'smart_open.Reader'
         :return: dictionary where key is the name of the column, value is the data type of the column
@@ -186,42 +272,48 @@
 
 class YAMLLoader(BaseDataLoader):
     """
     Class for loading and saving data in YAML format
     """
     def load_data(self, metadata_path: str) -> dict:
         with open(metadata_path, "r", encoding="utf-8") as metadata_file:
-            metadata = yaml.load(metadata_file, Loader=Loader)
-            validate_schema(configuration_schema, metadata)
+            metadata = yaml.load(metadata_file, Loader=SafeLoader)
+            ValidationSchema(metadata).validate_schema()
             parameters = ["train_settings", "infer_settings", "keys"]
             metadata = self.replace_none_values_of_metadata_settings(parameters, metadata)
         return metadata
 
     @staticmethod
     def replace_none_values_of_metadata_settings(parameters, metadata: dict):
         """
-        Replace None values for parameters
-        in the metadata
+        Replace None values for parameters in the metadata
         """
-        for table in metadata.keys():
+        metadata["global"] = dict() if metadata.get("global") is None else metadata.get("global")
+        if metadata["global"]:
+            for settings in metadata["global"].keys():
+                metadata["global"][settings] = dict() if metadata["global"].get(settings) is None \
+                        else metadata["global"].get(settings)
+        for key in metadata.keys():
+            if key == "global":
+                continue
             for parameter in parameters:
-                if metadata.get(table).get(parameter) is None:
-                    metadata[table][parameter] = {}
+                if metadata.get(key).get(parameter) is None:
+                    metadata[key][parameter] = {}
         return metadata
 
     def save_data(self, path: str, df: pd.DataFrame, **kwargs):
         raise NotImplementedError("Saving YAML files is not supported")
 
 
 class BinaryLoader(BaseDataLoader):
     """
     Class for loading and saving data using byte stream
     """
 
-    def load_data(self, path: str, *kwargs) -> Tuple[pd.DataFrame, None]:
+    def load_data(self, path: str, **kwargs) -> Tuple[pd.DataFrame, None]:
         with open(path, "rb") as f:
             data = pickle.load(f)
         return data, None
 
     def save_data(self, path: str, data, **kwargs):
         with open(path, "wb") as f:
             pickle.dump(data, f)
```

### Comparing `syngen-0.1.9/src/syngen/ml/metrics/__init__.py` & `syngen-0.2.0rc0/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,17 @@
 			}
 
 			.bivariate-img-container--item .flex-container .h3-title {
 				display: inline-block;
 			}
 
 			.bivariate-title {
+				overflow-wrap: break-word;
+				hyphens: auto;
+				max-width: 46%;
 				top: 2.5vh;
 				position: relative;
 				margin-bottom: 0 !important;
 			}
 
 			.parameters>div>ul {
 				font-size: 20px;
```

### Comparing `syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     Clustering,
     Utility
 )
 from syngen.ml.metrics.utils import transform_to_base64
 from syngen.ml.utils import fetch_training_config
 
 
-
 class BaseTest(ABC):
     def __init__(
             self,
             original: pd.DataFrame,
             synthetic: pd.DataFrame,
             paths: dict,
             table_name: str,
@@ -99,19 +98,17 @@
         # Generate html report
         with open(f"{os.path.dirname(os.path.realpath(__file__))}/accuracy_report.html") as file_:
             template = jinja2.Template(file_.read())
 
         draws_acc_path = f"{self.paths['draws_path']}/accuracy"
         uni_images = {
             title: transform_to_base64(path) for title, path in uni_images.items()
-            if "word_count" not in title
         }
         bi_images = {
             title: transform_to_base64(path) for title, path in bi_images.items()
-            if "char_len" not in title and "word_count" not in title
         }
         html = template.render(accuracy_value=acc_median,
                                accuracy_heatmap=transform_to_base64(f"{draws_acc_path}/accuracy_heatmap.svg"),
                                uni_imgs=uni_images,
                                correlations_heatmap=transform_to_base64(f"{draws_acc_path}/correlations_heatmap.svg"),
                                clusters_barplot=transform_to_base64(f"{draws_acc_path}/clusters_barplot.svg"),
                                clustering_value=clustering_result,
```

### Comparing `syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.1.9/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.2.0rc0/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from typing import Union, List, Optional
+from typing import Union, List, Optional, Dict
 from abc import ABC
 from itertools import combinations
 from collections import Counter
 import re
+import random
 
 import tqdm
 from sklearn.cluster import KMeans
 from sklearn.preprocessing import MinMaxScaler, StandardScaler
 from sklearn.metrics import r2_score, accuracy_score
-from loguru import logger
 import matplotlib
 from matplotlib.colors import LinearSegmentedColormap
 from matplotlib.patches import Patch
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy.stats as st
 import seaborn as sns
 from slugify import slugify
+from loguru import logger
 
 from syngen.ml.utils import (
     get_nan_labels,
     nan_labels_to_float,
     convert_to_time
 )
 
@@ -315,29 +316,32 @@
             y_tick_labels_synth = [convert_to_time(i) for i in y_tick_labels_synth]
         else:
             x_tick_labels_orig = [convert_to_time(i) for i in x_tick_labels_orig]
             x_tick_labels_synth = [convert_to_time(i) for i in x_tick_labels_synth]
         return (heatmap_orig, x_tick_labels_orig, y_tick_labels_orig), \
                (heatmap_synth, x_tick_labels_synth, y_tick_labels_synth)
 
-
     def calculate_all(
         self,
         cont_columns: List[str],
         categ_columns: List[str],
         date_columns: Optional[List[str]],
         num_not_na_cont_ticks: int = 10,
+        max_num_combinations: int = 100,
     ):
         self.date_columns = date_columns if date_columns else []
         self.num_not_na_ticks = num_not_na_cont_ticks
-        all_columns = set(cont_columns) | set(categ_columns)
-        column_pairs = list(combinations(all_columns, 2))
+        fetched_columns = set(cont_columns) | set(categ_columns)
+        excluded_cols = {col for col in fetched_columns if col.endswith(("_word_count", "_char_len"))}
+        all_columns = fetched_columns - excluded_cols
+        all_column_pairs = list(combinations(all_columns, 2))
+        column_pairs = random.sample(all_column_pairs, min(max_num_combinations, len(all_column_pairs)))
         bi_imgs = {}
         for i, (first_col, second_col) in tqdm.tqdm(iterable=enumerate(column_pairs),
-                                                    desc="Generating images...",
+                                                    desc="Generating bivariate distributions...",
                                                     total=len(column_pairs)):
             fig, self._axes = plt.subplots(1, 2, figsize=(30, 15), gridspec_kw={'width_ratios': [7, 8.7]})
             if first_col in cont_columns:
                 if second_col in cont_columns:
                     (
                         heatmap_orig_data,
                         heatmap_synthetic_data,
@@ -441,39 +445,61 @@
         cbar=True,
     ):
         ax = self._axes.flat[plt_index]
         ax.tick_params(labelsize=14)
         heatmap, x_tick_labels, y_tick_labels = heatmap_data
         x_tick_labels = self.__format_float_tick_labels(x_tick_labels)
         y_tick_labels = self.__format_float_tick_labels(y_tick_labels)
-        sns.heatmap(
+        ax = sns.heatmap(
             heatmap,
             xticklabels=x_tick_labels,
             yticklabels=y_tick_labels,
             ax=ax,
             vmin=vmin,
             vmax=vmax,
             cmap=self.cmap,
             cbar=cbar
         )
+        if cbar:
+            cbar = ax.collections[0].colorbar
+            cbar.ax.tick_params(axis="y", labelsize=20)
 
     def _get_continuous_ticks(self, col_name: str):
         original_col_values = self.original[col_name].dropna().values
         synthetic_col_values = self.original[col_name].dropna().values
         col_values = np.concatenate((original_col_values, synthetic_col_values))
         return np.percentile(col_values, list(range(0, 101, self.num_not_na_ticks)))
 
-    def _get_categorical_ticks(self, col_name: str):
+    def _get_categorical_ticks(self, col_name: str, ticks_count: int = 50):
+        """
+        Select the ticks for a categorical column
+        """
+        min_ticks = int(ticks_count * 0.2)
+        max_ticks = int(ticks_count * 0.2)
+        other_ticks = ticks_count - min_ticks - max_ticks
+
         categ_ticks = sorted(
             set(
                 set(self.original[col_name].fillna("?"))
                 | set(self.synthetic[col_name].fillna("?"))
             )
         )
-        return categ_ticks
+        # Select the first min_ticks elements
+        selected_min_ticks = categ_ticks[:min_ticks]
+
+        # Select the last max_ticks elements
+        selected_max_ticks = categ_ticks[-max_ticks:]
+
+        # Remove the already selected elements from categ_ticks
+        remaining_ticks = categ_ticks[min_ticks:-max_ticks]
+
+        # Randomly select other_ticks elements from the remaining list
+        selected_other_ticks = random.sample(remaining_ticks, min(other_ticks, len(remaining_ticks)))
+
+        return selected_min_ticks + selected_other_ticks + selected_max_ticks
 
     @staticmethod
     def _format_categorical_labels(labels):
         return [
             str(label) if len(str(label)) < 15 else str(label[:12]) + "..."
             for label in labels
         ]
@@ -642,23 +668,46 @@
         self,
         cont_columns: List[str],
         categ_columns: List[str],
         date_columns: Optional[List[str]],
         print_nan: bool = False
     ):
         cont_columns = list(cont_columns)
+        excluded_cols = {col for col in cont_columns if "word_count" if col.endswith("_word_count")}
+        cont_columns = set(cont_columns) - excluded_cols
+        excluded_cols = {col for col in categ_columns if "word_count" if col.endswith("_word_count")}
+        categ_columns = set(categ_columns) - excluded_cols
         images = {}
         uni_categ_images = {}
         for col in cont_columns:
             images.update(self.__calc_continuous(column=col, print_nan=print_nan, isdate=col in date_columns))
         for col in categ_columns:
             uni_categ_images.update(self.__calc_categ(col))
         images.update(uni_categ_images)
         return images
 
+    @staticmethod
+    def _get_ratio_counts(ratio_counts, count: int = 30) -> Dict:
+        """
+        Select the most common, least common and some random items between them from the ratio_counts
+        """
+        ratio_counts = Counter(ratio_counts)
+
+        most_least_count = int(count * 0.2)
+        other_items = count - 2 * most_least_count
+
+        most_common_items = ratio_counts.most_common(most_least_count)
+        least_common_items = ratio_counts.most_common()[:-most_least_count - 1:-1]
+        between_items = ratio_counts.most_common()[most_least_count:-most_least_count]
+        selected_between_items = random.sample(between_items, min(other_items, len(between_items)))
+
+        updated_ratio_counts = dict(most_common_items + selected_between_items + least_common_items)
+
+        return updated_ratio_counts
+
     def __calc_categ(self, column):
         def plot_dist(column_data, sort=True, full_set=None):
             counts = Counter(column_data)
             if full_set is not None:
                 absent_keys = full_set - set(counts.keys())
                 if len(absent_keys) > 0:
                     for k in absent_keys:
@@ -676,24 +725,28 @@
             return re.sub("\$|\^", "", label)
 
         original_column = self.original[column].fillna("?")
         synthetic_column = self.synthetic[column].fillna("?")
         full_values_set = set(original_column.values) | set(synthetic_column.values)
 
         original_ratio_counts = plot_dist(original_column, True, full_values_set)
+        original_ratio_counts = self._get_ratio_counts(original_ratio_counts)
         original_labels = list(original_ratio_counts.keys())
         original_ratio = list(original_ratio_counts.values())
 
         synthetic_ratio_counts = plot_dist(synthetic_column, False, full_values_set)
-        synthetic_ratio = [synthetic_ratio_counts[label] for label in original_labels]
+        synthetic_ratio = [
+            synthetic_ratio_counts[label] for label in original_labels
+            if synthetic_ratio_counts.get(label) is not None
+        ]
 
         uni_images = {}
 
         if self.plot:
-            fig = plt.figure(figsize=(8, 6.5))
+            fig = plt.figure(figsize=(9.5, 6.5))
 
             width = 0.35
             x = np.arange(len(original_labels))
             plt.bar(
                 x - width / 2,
                 original_ratio,
                 width=width,
```

### Comparing `syngen-0.1.9/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.9/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.9/src/syngen/ml/metrics/utils.py` & `syngen-0.2.0rc0/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.9/src/syngen/ml/reporters/reporters.py` & `syngen-0.2.0rc0/src/syngen/ml/reporters/reporters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import abstractmethod
-from typing import List, Dict
+from typing import Dict
+import itertools
 
 import pandas as pd
 import numpy as np
 from loguru import logger
 
 from syngen.ml.utils import (
     get_nan_labels,
@@ -18,26 +19,25 @@
 class Reporter:
     """
     Abstract class for reporters
     """
 
     def __init__(
             self,
-            metadata: Dict[str, str],
+            table_name: str,
             paths: Dict[str, str],
             config: Dict[str, str]
     ):
-        self.metadata = metadata
-        self.table_name = metadata["table_name"]
+        self.table_name = table_name
         self.paths = paths
         self.config = config
 
-    def extract_report_data(self):
+    def _extract_report_data(self):
         original, schema = DataLoader(self.paths["original_data_path"]).load_data()
-        synthetic, schema = DataLoader(self.paths["synthetic_data_path"]).load_data()
+        synthetic, schema = DataLoader(self.paths["path_to_merged_infer"]).load_data()
         return original, synthetic
 
     def fetch_data_types(self):
         dataset = fetch_dataset(self.paths["dataset_pickle_path"])
         types = (
             dataset.str_columns, dataset.date_columns,
             dataset.int_columns, dataset.float_columns,
@@ -47,15 +47,15 @@
         return types
 
     def preprocess_data(self):
         """
         Preprocess original and synthetic data.
         Return original data, synthetic data, float columns, integer columns, categorical columns
         """
-        original, synthetic = self.extract_report_data()
+        original, synthetic = self._extract_report_data()
         missing_columns = set(original) - set(synthetic)
         for col in missing_columns:
             synthetic[col] = np.nan
         columns_nan_labels = get_nan_labels(original)
         original = nan_labels_to_float(original, columns_nan_labels)
         synthetic = nan_labels_to_float(synthetic, columns_nan_labels)
         types = self.fetch_data_types()
@@ -105,48 +105,58 @@
 
 
 class Report:
     """
     Singleton metaclass for registration all needed reporters
     """
 
-    __reporters: List[Reporter] = []
+    _reporters: Dict[str, Reporter] = {}
 
     def __new__(cls):
         if not hasattr(cls, "instance"):
             cls.instance = super(Report, cls).__new__(cls)
         return cls.instance
 
     @classmethod
-    def register_reporter(cls, reporter: Reporter):
+    def register_reporter(cls, table: str, reporter: Reporter):
         """
         Register all needed reporters
         """
-        cls.__reporters.append(reporter)
+        list_of_reporters = cls._reporters.get(table, [])
+        list_of_reporters.append(reporter)
+        cls._reporters[table] = list_of_reporters
 
     @classmethod
     def clear_report(cls):
         """
         Delete unnecessary reporters
         """
-        cls.__reporters.clear()
+        cls._reporters.clear()
 
     @classmethod
     def generate_report(cls):
         """
         Generate all needed reports
         """
-        for reporter in cls.__reporters:
+        list_of_reporters = itertools.chain.from_iterable(cls._reporters.values())
+        for reporter in list_of_reporters:
+            logger.info(f"Generation of {reporter.__class__.report_type} report "
+                        f"for the table - '{reporter.table_name}'")
             reporter.report()
 
+    @property
+    def reporters(self) -> Dict[str, Reporter]:
+        return self._reporters
+
 
 class AccuracyReporter(Reporter):
     """
     Reporter for running accuracy test
     """
+    report_type = "accuracy"
 
     def report(self):
         """
         Run the report
         """
         (
             original,
@@ -168,16 +178,17 @@
         )
 
 
 class SampleAccuracyReporter(Reporter):
     """
     Reporter for running accuracy test
     """
+    report_type = "sample"
 
-    def extract_report_data(self):
+    def _extract_report_data(self):
         original, schema = DataLoader(self.paths["source_path"]).load_data()
         sampled, schema = DataLoader(self.paths["input_data_path"]).load_data()
         return original, sampled
 
     def report(self):
         """
         Run the report
```

### Comparing `syngen-0.1.9/src/syngen/ml/strategies/strategies.py` & `syngen-0.2.0rc0/src/syngen/ml/strategies/strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from abc import ABC, abstractmethod
 import os
 import traceback
-os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
-
 from loguru import logger
-from syngen.ml.train_chain import RootHandler
+os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
+
+from syngen.ml.handlers import RootHandler
 from syngen.ml.reporters import (
     Report,
     AccuracyReporter,
     SampleAccuracyReporter
 )
 from syngen.ml.config import (
     TrainConfig,
     InferConfig
 )
-from syngen.ml.train_chain import (
+from syngen.ml.handlers import (
     LongTextsHandler,
     VaeTrainHandler,
     VaeInferHandler
 )
 from syngen.ml.vae import VanillaVAEWrapper
 from syngen.ml.data_loaders import BinaryLoader
 
+
 class Strategy(ABC):
     """
     Abstract class for the strategies of training or infer process
     """
     def __init__(self):
         self.handler = None
         self.config = None
@@ -116,19 +117,22 @@
 
         self.handler = root_handler
         return self
 
     def add_reporters(self, **kwargs):
         if self.config.print_report:
             sample_reporter = SampleAccuracyReporter(
-                metadata={"table_name": self.config.table_name},
+                table_name=self.config.table_name,
                 paths=self.config.paths,
                 config=self.config.to_dict()
             )
-            Report().register_reporter(sample_reporter)
+            Report().register_reporter(
+                table=self.config.table_name,
+                reporter=sample_reporter
+            )
 
         return self
 
     def run(
             self,
             **kwargs
     ):
@@ -185,44 +189,50 @@
             table_name=self.config.table_name,
             paths=self.config.paths,
             wrapper_name=VanillaVAEWrapper.__name__,
             size=self.config.size,
             random_seed=self.config.random_seed,
             batch_size=self.config.batch_size,
             run_parallel=self.config.run_parallel,
-            print_report=self.config.print_report
+            print_report=self.config.print_report,
+            log_level=self.config.log_level
         )
         return self
 
     def add_reporters(self):
         if self.config.print_report:
             accuracy_reporter = AccuracyReporter(
-                metadata={"table_name": self.config.table_name},
+                table_name=self.config.table_name,
                 paths=self.config.paths,
                 config=self.config.to_dict()
             )
-            Report().register_reporter(accuracy_reporter)
+            Report().register_reporter(
+                table=self.config.table_name,
+                reporter=accuracy_reporter
+            )
 
         return self
 
     def run(
             self,
             **kwargs
     ):
         """
         Launch the infer process
         """
         self.set_config(
+            destination=kwargs["destination"],
             size=kwargs["size"],
             table_name=kwargs["table_name"],
             metadata_path=kwargs["metadata_path"],
             run_parallel=kwargs["run_parallel"],
             batch_size=kwargs["batch_size"],
             random_seed=kwargs["random_seed"],
             print_report=kwargs["print_report"],
+            log_level=kwargs["log_level"],
             both_keys=kwargs["both_keys"],
         ).\
             add_reporters(). \
             set_metadata(kwargs["metadata"]).\
             add_handler()
 
         try:
```

### Comparing `syngen-0.1.9/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.2.0rc0/src/syngen/ml/handlers/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-import random
 from typing import Tuple, Optional, Dict, List
 from abc import ABC, abstractmethod
 import os
 import math
-import uuid
 from ulid import ULID
 from uuid import UUID
 from dataclasses import dataclass, field
 
 import pandas as pd
 import numpy as np
-from loguru import logger
 from numpy.random import seed, choice
 from pathos.multiprocessing import ProcessingPool
 import dill
 from scipy.stats import gaussian_kde
 from collections import OrderedDict
 from tensorflow.keras.preprocessing.text import Tokenizer
+from slugify import slugify
+from loguru import logger
 
 from syngen.ml.vae import *
 from syngen.ml.data_loaders import DataLoader
 from syngen.ml.utils import (
-    slugify_parameters,
     fetch_dataset,
     check_if_features_assigned,
-    generate_uuid,
-    generate_uuids
+    generate_uuid
 )
+from syngen.ml.context import get_context
+from syngen.ml.utils import setup_logger
 
 
 class AbstractHandler(ABC):
     @abstractmethod
     def set_next(self, handler):
         pass
 
@@ -130,17 +129,15 @@
                     bw_method=bw_width
                 )
                 features[col] = {"counts": counts, "indexes": ordered_indexes, "kde": kde}
 
             self._save_no_ml_checkpoints(features)
 
         else:
-            logger.info(
-                f"No columns to train kde over found"
-            )
+            logger.info(f"No columns to train kde over found")
         return super().handle(data, **kwargs)
 
 
 @dataclass
 class VaeTrainHandler(BaseHandler):
     wrapper_name: str
     schema: Dict
@@ -197,14 +194,15 @@
     metadata_path: str
     random_seed: Optional[int]
     size: int
     batch_size: int
     run_parallel: bool
     print_report: bool
     wrapper_name: str
+    log_level: str
     random_seed_list: List = field(init=False)
     vae: Optional[VAEWrapper] = field(init=False)
     has_vae: bool = field(init=False)
     has_no_ml: bool = field(init=False)
 
     def __post_init__(self):
         if self.random_seed:
@@ -265,16 +263,17 @@
             counts = features[col]["counts"]
             generated_column = [" ".join([self.synth_word(s, indexes, counts) for s in
                                           np.maximum(np.random.normal(i / j, 1, j).astype('int32'), 2)])
                                 for i, j in zip(*text_structures)]
             synthetic_infer[col] = generated_column
         return synthetic_infer
 
-
     def run_separate(self, params: Tuple):
+        os.environ["LOGURU_LEVEL"] = self.log_level
+        setup_logger()
         i, size = params
 
         if self.random_seed:
             seed(self.random_seeds_list[i])
 
         input_data_existed = DataLoader(self.paths["input_data_path"]).has_existed_path
 
@@ -338,21 +337,20 @@
         except FileNotFoundError:
             logger.warning(f"The mapper for the {fk_label} text key is not found. Making simple sampling")
             synth_fk = pk.sample(size, replace=True).reset_index(drop=True)
             synth_fk = synth_fk.rename(fk_label)
 
         return synth_fk
 
-    @staticmethod
-    @slugify_parameters()
-    def _set_pk_path(pk_table) -> str:
+    def _set_pk_path(self, pk_table) -> str:
         """
         Set the path to synthetic data of corresponding pk table
         """
-        pk_path = f"model_artifacts/tmp_store/{pk_table}/merged_infer_{pk_table}.csv"
+        destination_to_pk_table = self.metadata[pk_table].get("destination")
+        pk_path = destination_to_pk_table if destination_to_pk_table is not None else f"model_artifacts/tmp_store/{slugify(pk_table)}/merged_infer_{slugify(pk_table)}.csv"
         if not os.path.exists(pk_path):
             raise FileNotFoundError(
                 "The table with a primary key specified in the metadata file does not "
                 "exist or is not trained. Ensure that the metadata contains the "
                 "name of referenced table with a primary key in the foreign key declaration section."
             )
         return pk_path
@@ -379,14 +377,23 @@
                     not_null_column_mask = generated[null_column_name].astype("float64") <= 0.5
                     synth_fk = synth_fk.where(not_null_column_mask, np.nan)
                     generated = generated.drop(null_column_name, axis=1)
 
                 generated[fk_column_name] = synth_fk
         return generated
 
+    def _restore_empty_columns(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Restore empty columns in the generated table
+        """
+        empty_columns = fetch_dataset(self.paths["dataset_pickle_path"]).dropped_columns
+        empty_df = pd.DataFrame(index=df.index, columns=empty_columns)
+        df = pd.concat([df, empty_df], axis=1)
+        return df
+
     def handle(
             self,
             **kwargs
     ):
         self._prepare_dir()
 
         batch_num = math.ceil(self.size / self.batch_size)
@@ -394,20 +401,26 @@
             f"Infer model with parameters: size={self.size}, run_parallel={self.run_parallel}, "
             f"batch_size={self.batch_size}, random_seed={self.random_seed}, print_report={self.print_report}"
         )
         logger.info(f"Total of {batch_num} batch(es)")
         batches = self.split_by_batches(self.size, batch_num)
         prepared_batches = [self.run(batch, self.run_parallel) for batch in batches]
         prepared_data = self._concat_slices_with_unique_pk(prepared_batches) if len(prepared_batches) > 0 else pd.DataFrame()
+        prepared_data = self._restore_empty_columns(prepared_data)
 
         is_pk = self._is_pk()
+
         if self.metadata_path is not None:
             if not is_pk:
                 generated_data = self.generate_keys(prepared_data, self.size, self.metadata, self.table_name)
                 if generated_data is None:
-                    prepared_data.to_csv(self.paths["path_to_merged_infer"], index=False)
+                    DataLoader(self.paths["path_to_merged_infer"]).save_data(
+                        self.paths["path_to_merged_infer"], prepared_data, format=get_context().get_config())
                 else:
-                    generated_data.to_csv(self.paths["path_to_merged_infer"], index=False)
+                    DataLoader(self.paths["path_to_merged_infer"]).save_data(
+                        self.paths["path_to_merged_infer"], generated_data, format=get_context().get_config())
             else:
-                prepared_data.to_csv(self.paths["path_to_merged_infer"], index=False)
+                DataLoader(self.paths["path_to_merged_infer"]).save_data(
+                    self.paths["path_to_merged_infer"], prepared_data, format=get_context().get_config())
         if self.metadata_path is None:
-            prepared_data.to_csv(self.paths["path_to_merged_infer"], index=False)
+            DataLoader(self.paths["path_to_merged_infer"]).save_data(
+                self.paths["path_to_merged_infer"], prepared_data, format=get_context().get_config())
```

### Comparing `syngen-0.1.9/src/syngen/ml/utils/utils.py` & `syngen-0.2.0rc0/src/syngen/ml/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import os
+import sys
 from typing import List, Dict
 from dateutil.parser import parse
 import pickle
 from datetime import datetime, timedelta
-import sys
 
 import pandas as pd
 import numpy as np
 from slugify import slugify
-from loguru import logger
 import pickle as pkl
 import uuid
 from ulid import ULID
 import random
+from loguru import logger
+
 
 def generate_uuids(version: int, size: int):
     ulid = ULID()
     generated_uuid_column = []
     for i in range(size):
         if version != "ulid":
             generated_uuid_column.append(uuid.UUID(int=random.getrandbits(128), version=int(version)))
@@ -33,16 +35,18 @@
 
 def get_date_columns(df: pd.DataFrame, str_columns: List[str]):
     def date_finder(x, fuzzy=False):
         x_wo_na = x.dropna()
         count = 0
         for x in x_wo_na.values:
             try:
-                parse(x, fuzzy=fuzzy)
-                count += 1
+                date_for_check = datetime(8557, 7, 20)
+                datetime_object = parse(x, default=date_for_check)
+                # Check if the parsed date contains only the time component. If it does, then skip it.
+                count += 1 if datetime_object.date() != date_for_check.date() else 0
             except (ValueError, OverflowError):
                 continue
         if count > len(x_wo_na) * 0.8:
             return 1
         else:
             return np.nan
 
@@ -123,15 +127,47 @@
 
 
 def fetch_dataset(dataset_pickle_path: str):
     """
     Deserialize and return the object of class Dataset
     """
     with open(dataset_pickle_path, "rb") as f:
-        return pickle.loads(f.read())
+        dataset = pickle.loads(f.read())
+    # Check if the serialized class has associated dataframe and
+    # drop it as it might contain sensitive data. Save columns from the dataframe for later use.
+    if hasattr(dataset, "df"):
+        dataset = update_dataset(dataset)
+        dataset.order_of_columns = dataset.df.columns.tolist()
+        del dataset.df
+        with open(dataset_pickle_path, "wb") as f:
+            f.write(pickle.dumps(dataset))
+    return dataset
+
+
+def define_existent_columns(columns, original_columns):
+    existent_columns = []
+    for column in columns:
+        if column in original_columns:
+            existent_columns.append(column)
+        continue
+    return existent_columns
+
+
+def update_dataset(dataset):
+    for attr in vars(dataset):
+        if attr in ["primary_keys_mapping", "unique_keys_mapping", "foreign_keys_mapping"]:
+            attr_value = getattr(dataset, attr)
+            updated_attr_value = attr_value.copy()
+            for key, config in attr_value.items():
+                updated_columns = define_existent_columns(config.get("columns", []), dataset.df.columns)
+                config["columns"] = updated_columns
+                updated_attr_value[key] = config
+
+            setattr(dataset, attr, updated_attr_value)
+    return dataset
 
 
 def slugify_attribute(**kwargs):
     """
     Slugify the value of the attribute of the instance
     and set it to the new attribute
     """
@@ -196,13 +232,22 @@
     """
     features = fetch_dataset(dataset_pickle_path).features
     if len(features) == 0:
         logger.info("No features to train VAE on")
         return False
     return True
 
+
 def fetch_training_config(train_config_pickle_path):
     """
     Fetch the parameters of the training configuration
     """
     with open(train_config_pickle_path, "rb") as f:
         return pkl.load(f)
+
+
+def setup_logger():
+    """
+    Setup logger with the specified level
+    """
+    logger.remove()
+    logger.add(sys.stderr, level=os.getenv("LOGURU_LEVEL"))
```

### Comparing `syngen-0.1.9/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.2.0rc0/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.9/src/syngen/ml/vae/models/dataset.py` & `syngen-0.2.0rc0/src/syngen/ml/vae/models/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Dict, Optional, List, Tuple
+from typing import Dict, Optional, List, Tuple, Set
 from dataclasses import dataclass, field
 import pickle
 from uuid import UUID
 from datetime import datetime
 import base32_crockford
+import os
 
-from loguru import logger
 import numpy as np
 import dill
 import pandas as pd
 from scipy.stats import gaussian_kde
 import tqdm
+from loguru import logger
 
 from syngen.ml.vae.models.features import (
     CategoricalFeature,
     CharBasedTextFeature,
     ContinuousFeature,
     DateFeature,
     BinaryFeature,
@@ -23,43 +24,71 @@
     get_nan_labels,
     nan_labels_to_float,
     get_tmp_df,
     get_date_columns
 )
 from syngen.ml.data_loaders import DataLoader
 from syngen.ml.utils import slugify_parameters
+from syngen.ml.utils import fetch_training_config
 
 
 @dataclass
 class Dataset:
     df: pd.DataFrame
     schema: Optional[Dict]
-    metadata: Optional[Dict]
+    metadata: Dict
     table_name: str
-    fk_kde_path: str
+    paths: Dict
     features: Dict = field(init=False)
     columns: Dict = field(init=False)
     is_fitted: bool = field(init=False)
     all_columns: List = field(init=False)
     null_num_column_names: List = field(init=False)
     zero_num_column_names: List = field(init=False)
     nan_labels_dict: Dict = field(init=False)
+    uuid_columns: Set = field(init=False)
+    uuid_columns_types: Dict = field(init=False)
+    dropped_columns: Set = field(init=False)
+    order_of_columns: List = field(init=False)
+    non_existent_columns: Set = field(init=False)
 
     def __post_init__(self):
         self._predefine_fields()
+        self.__prepare_dir()
         self._set_metadata()
 
+    def __getstate__(self) -> Dict:
+        """
+        Return a dictionary of the dataset's state
+        """
+        dataset_instance = self.__dict__.copy()
+        attribute_keys_to_remove = ["df", "non_existent_columns"]
+
+        for attr_key in attribute_keys_to_remove:
+            if attr_key in dataset_instance:
+                del dataset_instance[attr_key]
+
+        return dataset_instance
+
     def _predefine_fields(self):
         self.features = dict()
         self.columns = dict()
         self.is_fitted = False
         self.all_columns = list()
         self.null_num_column_names = list()
         self.zero_num_column_names = list()
         self.nan_labels_dict = dict()
+        self.uuid_columns = set()
+        self.uuid_columns_types = {}
+        self.dropped_columns = fetch_training_config(self.paths["train_config_pickle_path"]).dropped_columns
+        self.non_existent_columns = set()
+        self.order_of_columns = self.df.columns.tolist()
+
+    def __prepare_dir(self):
+        os.makedirs(self.paths["fk_kde_path"], exist_ok=True)
 
     def __set_pk_key(self, config_of_keys: Dict):
         """
         Set up primary key for the table
         """
         self.primary_keys_mapping = {
             key: value for (key, value) in config_of_keys.items()
@@ -89,51 +118,71 @@
         self.uq_columns = [col for uq_cols in uq_columns_lists for col in uq_cols]
 
         if self.unique_keys_list:
             logger.info(f"The unique keys were set: {self.unique_keys_list}")
         if not self.unique_keys_list:
             logger.info("No unique keys were set.")
 
+    def _filter_dropped_keys(self, config_of_keys: Dict, type_of_key: str) -> Tuple[Dict, Set]:
+        """
+        Filter out keys that contain empty columns
+        """
+        filtered_keys = {}
+        dropped_keys = set()
+
+        for key, value in config_of_keys.items():
+            if value.get("type") == type_of_key:
+                if any(column for column in value.get("columns") if column in self.dropped_columns):
+                    dropped_keys.add(key)
+                else:
+                    filtered_keys[key] = value
+
+        return filtered_keys, dropped_keys
+
     def __set_fk_keys(self, config_of_keys: Dict):
         """
         Set up foreign keys for the table
         """
-        self.foreign_keys_mapping = {
-            key: value for (key, value) in config_of_keys.items()
-            if config_of_keys.get(key).get("type") == "FK"
-        }
+        self.foreign_keys_mapping, dropped_fk_keys = self._filter_dropped_keys(config_of_keys, "FK")
         self.foreign_keys_list = list(self.foreign_keys_mapping.keys())
         fk_columns_lists = [val['columns'] for val in self.foreign_keys_mapping.values()]
         self.fk_columns = [col for fk_cols in fk_columns_lists for col in fk_cols]
 
+        if dropped_fk_keys:
+            logger.info(
+                f"The following foreign keys were dropped: {', '.join(dropped_fk_keys)} "
+                f"as they contain empty columns: {', '.join(self.dropped_columns.union(self.fk_columns))}"
+            )
+
         if self.foreign_keys_list:
-            logger.info(f"The following foreign keys were set: {self.foreign_keys_list}")
+            logger.info(f"The following foreign keys were set: {', '.join(self.foreign_keys_list)}")
         if not self.foreign_keys_list:
             logger.info("No foreign keys were set.")
 
     def __set_types(self, pk_uq_keys_mapping):
         """
         Set up list of data types of primary and unique keys
         """
         self.pk_uq_keys_types = {}
         for key_name, config in pk_uq_keys_mapping.items():
             key_columns = config.get("columns")
             for column in key_columns:
                 column_type = \
                     str if column in (
-                        self.str_columns | self.categ_columns | self.date_columns | self.long_text_columns | self.uuid_columns
+                            self.str_columns | self.categ_columns | self.date_columns |
+                            self.long_text_columns | self.uuid_columns
                     ) \
-                    else float
+                        else float
                 self.pk_uq_keys_types[column] = column_type
 
     def __map_text_pk(self):
         for pk, pk_type in self.pk_uq_keys_types.items():
             if pk_type is str:
                 mapper = {k: n for n, k in enumerate(self.df[pk])}
-                with open(f"{self.fk_kde_path}{pk}_mapper.pkl", "wb") as file:
+                with open(f"{self.paths['fk_kde_path']}{pk}_mapper.pkl", "wb") as file:
                     pickle.dump(mapper, file)
 
     def __set_metadata(self, metadata: dict, table_name: str):
         config_of_keys = metadata.get(table_name, {}).get("keys")
 
         if config_of_keys is not None:
             self.__set_pk_key(config_of_keys)
@@ -149,14 +198,17 @@
             self.unique_keys_list = []
             self.uq_columns = []
             self.foreign_keys_mapping = {}
             self.foreign_keys_list = []
             self.fk_columns = []
 
     def _set_metadata(self):
+        table_config = self.metadata.get(self.table_name, {})
+        self._set_non_existent_columns(table_config)
+        self._update_table_config(table_config)
         self.__set_metadata(self.metadata, self.table_name)
         self.__data_pipeline(self.df, self.schema)
 
     @staticmethod
     def _update_schema(schema: Dict[str, Dict[str, str]], df: pd.DataFrame):
         """
         Synchronize the schema of the table with dataframe
@@ -208,15 +260,15 @@
         Exclude the column from the list of categorical columns
         if it relates to certain type of key
         """
         if column in column_list:
             logger.warning(
                 f"The column '{column}' was excluded from the list of categorical columns "
                 f"as far as this column was set as the {key_type} of the table - '{self.table_name}'")
-            self.categ_columns.remove(column)
+            self.categ_columns.discard(column)
 
     def _check_if_not_key_column(self):
         """
         Exclude the column from the list of categorical columns
         if it relates to primary key, unique key or foreign key
         """
         for col in list(self.categ_columns):
@@ -309,15 +361,16 @@
             self.long_text_columns -= self.categ_columns
             if self.long_text_columns:
                 logger.info(
                     f"Please note that the columns - {self.long_text_columns} contain long texts (> 200 symbols). "
                     f"Such texts' handling consumes significant resources and results in poor quality content, "
                     f"therefore this column(-s) will be generated using a simplified statistical approach")
 
-    def _is_valid_ulid(self, uuid):
+    @staticmethod
+    def _is_valid_ulid(uuid):
         """
         Check if uuid_to_test is a valid ULID (https://github.com/ulid/spec)
         """
         ulid_timestamp = uuid[:10]
         try:
             assert len(uuid) == 26
             ulid_timestamp_int = base32_crockford.decode(ulid_timestamp)
@@ -327,45 +380,84 @@
             return
 
     def _is_valid_uuid(self, x):
         """
         Check if uuid_to_test is a valid UUID
         """
         result = []
-        for i in x:
+        for i in x.dropna():
             for v in [1, 2, 3, 4, 5]:
                 try:
                     uuid_obj = UUID(i, version=v)
                     if str(uuid_obj) == i or str(uuid_obj).replace("-", "") == i:
                         result.append(v)
                 except ValueError:
-                    continue
-            result.append(self._is_valid_ulid(i))
-        # returning the mode of the list, i.e. the most frequent element
+                    result.append(self._is_valid_ulid(i))
         if result:
             return max(set(result), key=result.count)
         else:
             return 0
 
     def _set_uuid_columns(self, df: pd.DataFrame):
         """
-        Set up the list of columns with uuid
+        Set up the list of columns with UUIDs
         """
 
         data_subset = self._select_str_columns(df)
 
-        self.uuid_columns = set()
-        self.uuid_columns_types = {}
         if not data_subset.empty:
-            data_subset = data_subset.dropna().apply(self._is_valid_uuid)
+            data_subset = data_subset.apply(self._is_valid_uuid)
             self.uuid_columns_types = dict(data_subset[data_subset.isin([1, 2, 3, 4, 5, "ulid"])])
             self.uuid_columns = set(self.uuid_columns_types.keys())
-            if self.uuid_columns:
-                logger.info(
-                    f"The columns - {self.uuid_columns} contain UUIDs")
+
+    def _set_date_columns(self, df: pd.DataFrame):
+        """
+        Set up the list of date columns
+        """
+        self.date_columns = \
+            get_date_columns(df, list(self.str_columns)) - self.categ_columns - \
+            self.binary_columns - self.long_text_columns
+
+    def _remove_non_existent_columns(self, columns: list, key: str, key_type: str) -> list:
+        """
+        Remove the columns from the table metadata which are absent in the table
+        """
+        updated_columns = []
+        for column in columns:
+            if column in self.non_existent_columns:
+                logger.warning(
+                    f"The column - '{column}' was excluded from the {key_type} - "
+                    f"'{key}' as far as this column doesn't exist in the table - '{self.table_name}'"
+                )
+            else:
+                updated_columns.append(column)
+        return updated_columns
+
+    def _update_table_config(self, table_config: Dict):
+        """
+        Update the table metadata by removing the columns which are absent in the table
+        but mentioned in the metadata
+        """
+        for key, key_config in table_config.get("keys", {}).items():
+            key_type = key_config.get("type")
+            updated_columns = self._remove_non_existent_columns(key_config.get("columns", []), key, key_type)
+            key_config["columns"] = updated_columns
+
+    def _set_non_existent_columns(self, table_config: Dict):
+        """
+        Set up the list of columns which are absent in the table
+        """
+        non_existent_columns = {
+            column
+            for key_config in table_config.get("keys", {}).values()
+            for column in key_config.get("columns", [])
+            if column not in self.df.columns
+        }
+
+        self.non_existent_columns = non_existent_columns - self.dropped_columns
 
     def _general_data_pipeline(self, df: pd.DataFrame, schema: Dict, check_object_on_float: bool = True):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table is absent
 
         :param df: dataframe
@@ -389,45 +481,43 @@
             if all(x.is_integer() for x in tmp_df[col]):
                 float_to_int_cols.add(col)
 
         self.int_columns = (self.int_columns | float_to_int_cols) - (self.categ_columns | self.binary_columns)
         self.float_columns = self.float_columns - self.categ_columns - self.int_columns - self.binary_columns
         self.str_columns = \
             set(tmp_df.columns) - self.float_columns - self.categ_columns - \
-            self.int_columns - self.binary_columns - self.long_text_columns - set(self.uuid_columns)
+            self.int_columns - self.binary_columns - self.long_text_columns - self.uuid_columns
         self.categ_columns -= self.long_text_columns
-        self.date_columns = \
-            get_date_columns(df, list(self.str_columns)) - self.categ_columns - \
-            self.binary_columns - self.long_text_columns
+        self._set_date_columns(df)
         self.str_columns -= self.date_columns
         self.uuid_columns = self.uuid_columns - self.categ_columns - self.binary_columns
         self.uuid_columns_types = {k: v for k, v in self.uuid_columns_types.items() if k in self.uuid_columns}
 
     def _avro_data_pipeline(self, df, schema):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table in Avro format is present
         """
         logger.info(f"The schema of table - {self.table_name} was received")
+        self._set_uuid_columns(df)
         self._set_binary_columns(df)
         self._set_categorical_columns(df, schema)
         self._set_long_text_columns(df)
         self.int_columns = set(column for column, data_type in schema.items() if data_type == 'int')
         self.int_columns = self.int_columns - self.categ_columns - self.binary_columns
         self.float_columns = set(column for column, data_type in schema.items() if data_type == 'float')
         self.float_columns = self.float_columns - self.categ_columns - self.binary_columns
         self.str_columns = set(column for column, data_type in schema.items() if data_type == 'string')
         self.categ_columns -= self.long_text_columns
-        self.str_columns = \
-            self.str_columns - self.categ_columns - self.int_columns - self.binary_columns - self.long_text_columns
-        self.date_columns = \
-            get_date_columns(df, list(self.str_columns)) - self.categ_columns - \
-            self.binary_columns - self.long_text_columns
+        self.str_columns = self.str_columns - self.categ_columns - self.binary_columns \
+                           - self.long_text_columns - self.uuid_columns
+        self._set_date_columns(df)
         self.str_columns -= self.date_columns
-        self.long_text_columns -= self.uuid_columns
+        self.uuid_columns = self.uuid_columns - self.categ_columns - self.binary_columns
+        self.uuid_columns_types = {k: v for k, v in self.uuid_columns_types.items() if k in self.uuid_columns}
 
     def __data_pipeline(self, df: pd.DataFrame, schema: Optional[Dict]):
         if schema.get("format") == "CSV":
             self._general_data_pipeline(df, schema)
         elif schema.get("format") == 'Avro':
             schema = self._update_schema(schema, df)
             self._avro_data_pipeline(df, schema.get("fields"))
@@ -436,25 +526,28 @@
                len(self.float_columns) + \
                len(self.int_columns) + \
                len(self.date_columns) + \
                len(self.categ_columns) + \
                len(self.binary_columns) + \
                len(self.long_text_columns) + \
                len(self.uuid_columns) == len(df.columns), "According to number of columns with defined types, " \
-                                                               "column types are not identified correctly"
+                                                          "column types are not identified correctly"
 
         logger.debug(
             f"Count of string columns: {len(self.str_columns)}; "
             + f"Count of float columns: {len(self.float_columns)}; "
             + f"Count of int columns: {len(self.int_columns)}; "
             + f"Count of categorical columns: {len(self.categ_columns)}; "
             + f"Count of date columns: {len(self.date_columns)}; "
             + f"Count of binary columns: {len(self.binary_columns)}; "
-            + f"Count of long text columns: {len(self.long_text_columns)}"
+            + f"Count of long text columns: {len(self.long_text_columns)}; "
+            + f"Count of uuid columns: {len(self.uuid_columns)}"
         )
+        for column in self.uuid_columns:
+            logger.info(f"Column '{column}' defined as UUID column")
 
     def assign_feature(self, feature, columns):
         name = feature.original_name
 
         if name in self.features:
             raise Exception(f"{name} is already contained in features")
 
@@ -619,37 +712,35 @@
             fk_columns = self.foreign_keys_mapping.get(fk).get("columns")
             for fk_column in fk_columns:
                 fk_column_values = self.df[fk_column]
                 correspondent_pk_table = self.foreign_keys_mapping[fk]["references"]["table"]
                 correspondent_pk_col = self.foreign_keys_mapping[fk]["references"]["columns"][0]
                 if fk_column_values.dtype in (pd.StringDtype(), "object"):
                     mapper = self._fetch_mapper(
-                        fk_kde_path=self.fk_kde_path,
+                        fk_kde_path=self.paths["fk_kde_path"],
                         table_name=self.table_name,
                         pk_table=correspondent_pk_table,
                         pk_column=correspondent_pk_col,
                         fk_column=fk_column
                     )
                     if mapper is None:
                         continue
                     fk_column_values = fk_column_values.map(mapper)
                 noise_to_prevent_singularity = np.random.normal(0, 0.0001, len(fk_column_values))
                 kde = gaussian_kde(fk_column_values + noise_to_prevent_singularity)
-                self._save_kde_artifacts(kde=kde, fk_kde_path=self.fk_kde_path, fk_column=fk_column)
+                self._save_kde_artifacts(kde=kde, fk_kde_path=self.paths["fk_kde_path"], fk_column=fk_column)
 
-    def __drop_fk_columns(self):
+    def _drop_fk_columns(self):
         """
         Drop columns in dataframe which defined as foreign key
         """
-        for fk in self.foreign_keys_list:
-            fk_columns = self.foreign_keys_mapping.get(fk).get("columns")
-            for fk_column in fk_columns:
-                self.df = self.df.drop(fk_column, axis=1)
-                logger.debug(f"The column - '{fk_column}' of foreign key '{fk}' dropped from training "
-                             f"and will be sampled from the PK table")
+        for fk_column in set(self.fk_columns):
+            self.df = self.df.drop(fk_column, axis=1)
+            logger.debug(f"The column - '{fk_column}' dropped from the training process as it is defined as FK column "
+                         f"and will be sampled from the PK table")
 
     def __sample_only_joined_rows(self, fk):
         references = self.foreign_keys_mapping.get(fk).get("references")
         pk_table = references.get("table")
         pk_table_data, schema = \
             DataLoader(f"model_artifacts/tmp_store/{pk_table}/input_data_{pk_table}.csv").load_data()
         pk_column_label = references.get("columns")[0]
@@ -667,15 +758,15 @@
         max_len, rnn_units = self._preprocess_str_params(feature)
         self.assign_feature(
             CharBasedTextFeature(
                 feature, text_max_len=max_len, rnn_units=rnn_units
             ),
             feature,
         )
-        logger.debug(f"Column '{feature}' assigned as text based feature")
+        logger.info(f"Column '{feature}' assigned as text based feature")
 
     def _assign_float_feature(self, feature):
         """
         Assign float based feature to float columns
         """
         # num_bins = self.find_clusters(df, float_columns)
         features = self._preprocess_nan_cols(feature, fillna_strategy="mean")
@@ -685,61 +776,60 @@
             self.zero_num_column_names.append(features[1])
         if len(features) == 3:
             self.zero_num_column_names.append(features[2])
         for feature in features:
             self.assign_feature(
                 ContinuousFeature(feature, column_type=float), feature
             )
-            logger.debug(f"Column '{feature}' assigned as float based feature")
+            logger.info(f"Column '{feature}' assigned as float based feature")
 
     def _assign_int_feature(self, feature):
         """
         Assign int based feature to int columns
         """
-        # num_bins = self.find_clusters(df, int_columns)
         features = self._preprocess_nan_cols(feature, fillna_strategy="mean")
         if len(features) == 2 and features[1].endswith("_null"):
             self.null_num_column_names.append(features[1])
         if len(features) == 2 and features[1].endswith('_zero'):
             self.zero_num_column_names.append(features[1])
         if len(features) == 3:
             self.zero_num_column_names.append(features[2])
         for feature in features:
             self.assign_feature(
                 ContinuousFeature(feature, column_type=int), feature
             )
-            logger.debug(f"Column '{feature}' assigned as int based feature")
+            logger.info(f"Column '{feature}' assigned as int based feature")
 
     def _assign_categ_feature(self, feature):
         """
         Assign categorical based feature to categorical columns
         """
         feature = self._preprocess_categ_params(feature)
         self.assign_feature(CategoricalFeature(feature), feature)
-        logger.debug(f"Column '{feature}' assigned as categorical based feature")
+        logger.info(f"Column '{feature}' assigned as categorical based feature")
 
     def _assign_date_feature(self, feature):
         """
         Assign date feature to date columns
         """
         features = self._preprocess_nan_cols(feature, fillna_strategy="mode")
         self.assign_feature(DateFeature(features[0]), features[0])
-        logger.debug(f"Column '{features[0]}' assigned as date feature")
+        logger.info(f"Column '{features[0]}' assigned as date feature")
         if len(features) == 2:
             self.null_num_column_names.append(features[1])
             self.assign_feature(ContinuousFeature(features[1], column_type=int), features[1])
-            logger.debug(f"Column '{features[1]}' assigned as int feature")
+            logger.info(f"Column '{features[1]}' assigned as int feature")
 
     def _assign_binary_feature(self, feature):
         """
         Assign binary feature to binary columns
         """
         feature = self._preprocess_categ_params(feature)
         self.assign_feature(BinaryFeature(feature), feature)
-        logger.debug(f"Column '{feature}' assigned as binary feature")
+        logger.info(f"Column '{feature}' assigned as binary feature")
 
     def _assign_fk_feature(self):
         """
         Assign corresponding to FK null column and preprocess if required.
         """
         for fk_name, config in self.foreign_keys_mapping.items():
             if "joined_sample" in config and config["joined_sample"]:
@@ -755,15 +845,15 @@
     def pipeline(self) -> pd.DataFrame:
         columns_nan_labels = get_nan_labels(self.df)
         self.df = nan_labels_to_float(self.df, columns_nan_labels)
 
         if self.foreign_keys_list:
             self._assign_fk_feature()
             self._preprocess_fk_params()
-            self.__drop_fk_columns()
+            self._drop_fk_columns()
 
         self.primary_keys_mapping.update(self.unique_keys_mapping)
         pk_uq_keys_mapping = self.primary_keys_mapping
         if pk_uq_keys_mapping:
             self.__set_types(pk_uq_keys_mapping)
             self.__map_text_pk()
```

### Comparing `syngen-0.1.9/src/syngen/ml/vae/models/features.py` & `syngen-0.2.0rc0/src/syngen/ml/vae/models/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -650,29 +650,21 @@
         return self.scaler.transform(data)
 
     def inverse_transform(self, data):
         max_allowed_time_ns = int(9.2E18)
         min_allowed_time_ns = int(-9.2E18)
         unscaled = self.scaler.inverse_transform(data)
         unscaled = chain.from_iterable(unscaled)
-        if self.is_positive:
-            return list(
+        return list(
                 map(
                     lambda l: pd.Timestamp(
-                        abs(min(max_allowed_time_ns, int(l)))
-                    ).strftime(self.date_format),
-                    unscaled,
-                )
-            )
-        else:
-            return list(
-                map(
-                    lambda l: pd.Timestamp(
-                        max(min(max_allowed_time_ns, int(l)), min_allowed_time_ns)
-                    ).strftime(self.date_format),
+                        min(max_allowed_time_ns, int(l))
+                    ).strftime(self.date_format)
+                    if l >= 0
+                    else pd.Timestamp(max(min_allowed_time_ns, int(l))).strftime(self.date_format),
                     unscaled,
                 )
             )
 
     @lazy
     def input(self):
         return Input(
```

### Comparing `syngen-0.1.9/src/syngen/ml/vae/models/model.py` & `syngen-0.2.0rc0/src/syngen/ml/vae/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 
 import tensorflow as tf
-from loguru import logger
 import pickle
 from tensorflow.keras.models import Model
 from tensorflow.keras.layers import (
     Input,
     Dense,
     Dropout,
     LeakyReLU,
@@ -13,18 +12,22 @@
     Lambda,
     BatchNormalization,
     Activation,
 )
 from sklearn.mixture import BayesianGaussianMixture
 import numpy as np
 import pandas as pd
+from loguru import logger
+from IPython.display import SVG
+from keras.utils.vis_utils import model_to_dot
 
 from syngen.ml.vae.models.custom_layers import FeatureLossLayer
 from syngen.ml.utils import slugify_parameters
 
+
 class CVAE:
     """
     A class implementing the model architecture.
     """
 
     def __init__(
         self,
@@ -34,15 +37,15 @@
         intermediate_dim,
         latent_components
     ):
         self.dataset = dataset
         self.intermediate_dim = intermediate_dim
         self.batch_size = batch_size
         self.latent_dim = latent_dim
-        self.latent_components = min(latent_components, len(self.dataset.df))
+        self.latent_components = min(latent_components, len(self.dataset.order_of_columns))
         self.model = None
         self.latent_model = None
         self.metrics = {}
         self.cond_features = {}
         self.is_cond = False
 
     def sample_z(self, args):
@@ -212,15 +215,15 @@
         latent_sample = self.latent_model.sample(nb_samples)[0]
         np.random.shuffle(latent_sample)
 
         synthetic_prediction = self.generator_model.predict(latent_sample)
         self.inverse_transformed_df = self.dataset.inverse_transform(synthetic_prediction)
         pk_uq_keys_mapping = self.dataset.primary_keys_mapping
         if pk_uq_keys_mapping:
-            self.__make_pk_uq_unique(pk_uq_keys_mapping)
+            self.__make_pk_uq_unique(pk_uq_keys_mapping, self.dataset.dropped_columns)
         return self.inverse_transformed_df
 
     def less_likely_sample(
         self, nb_samples: int, temp: float = 0.05, variaty: int = 3
     ) -> pd.DataFrame:
         def pop_npoints(latent_vector, log):
             log_probs = {prob: idx for idx, prob in enumerate(log)}
@@ -240,26 +243,24 @@
 
     def __check_pk_numeric_convertability(self, column, key_type):
         if key_type is str and column not in self.dataset.long_text_columns | self.dataset.uuid_columns:
             return self.inverse_transformed_df[column].dropna().str.isnumeric().all()
         else:
             return False
 
-    def __make_pk_uq_unique(self, pk_uq_keys_mapping):
+    def __make_pk_uq_unique(self, pk_uq_keys_mapping, empty_columns):
         for key_name, config in pk_uq_keys_mapping.items():
-            key_columns = config.get("columns")
+            key_columns = [column for column in config.get("columns") if column not in empty_columns]
             for column in key_columns:
                 key_type = self.dataset.pk_uq_keys_types[column]
                 if key_type is float or self.__check_pk_numeric_convertability(column, key_type):
                     mapped_keys = np.arange(len(self.inverse_transformed_df[column])) + 1
                     self.inverse_transformed_df[column] = mapped_keys
 
     def show_model(self):
-        from IPython.display import SVG
-        from keras.utils.vis_utils import model_to_dot
         return SVG(model_to_dot(self.model).create(prog="dot", format="svg"))
 
     def save_state(self, path: str):
         pth = Path(path)
 
         if self.model is not None:
             self.model.save_weights(str(pth / "vae.ckpt"))
```

### Comparing `syngen-0.1.9/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.2.0rc0/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import warnings
 import pickle
 import tensorflow as tf
 from tensorflow.python.data.experimental import AutoShardPolicy
 import matplotlib.pyplot as plt
 import time
 import tqdm
-from loguru import logger
 import pandas as pd
 import numpy as np
+from loguru import logger
 
 from syngen.ml.vae.models.model import CVAE
 from syngen.ml.vae.models import Dataset
 from syngen.ml.utils import (
     fetch_dataset,
     check_if_features_assigned
 )
@@ -107,45 +107,42 @@
         self.schema = schema
         self.process = process
         self.batch_size = batch_size
         self.latent_dim = latent_dim
         self.latent_components = latent_components
         self.metadata = metadata
         self.table_name = table_name
-        self.vae_resources_path = paths["state_path"]
-        self.dataset_pickle_path = paths["dataset_pickle_path"]
-        self.fk_kde_path = paths["fk_kde_path"]
+        self.paths = paths
 
     def __post__init__(self):
         if self.process == "train":
             self.dataset = Dataset(
                 df=self.df,
                 schema=self.schema,
                 metadata=self.metadata,
                 table_name=self.table_name,
-                fk_kde_path=self.fk_kde_path
+                paths=self.paths
             )
         elif self.process == "infer":
-            self.dataset = fetch_dataset(self.dataset_pickle_path)
+            self.dataset = fetch_dataset(self.paths["dataset_pickle_path"])
 
     def _save_dataset(self):
         """
         Save dataset object on the disk
         """
-        with open(self.dataset_pickle_path, "wb") as f:
+        with open(self.paths["dataset_pickle_path"], "wb") as f:
             f.write(pickle.dumps(self.dataset))
 
     def _pipeline(self):
         """
         Launch the pipeline in the dataset
         """
         self.df = self.dataset.pipeline()
         self._save_dataset()
 
-
     def _restore_zero_values(self, df):
         for column in self.dataset.zero_num_column_names:
             if column.endswith("_zero"):
                 # remove _zero to get original column name
                 num_column_name = column[:-5]
                 num_column = df[num_column_name].copy()
                 zero_column_mask = df[column].astype("float") >= 0.5
@@ -194,15 +191,15 @@
     def fit_on_df(
         self,
         df: pd.DataFrame,
         epochs: int,
         columns_subset: List[str] = None,  # TODO columns_subset does not work
     ):
         self._pipeline()
-        if not check_if_features_assigned(self.dataset_pickle_path):
+        if not check_if_features_assigned(self.paths["dataset_pickle_path"]):
             return
         self._init_model()
 
         if columns_subset is None:
             columns_subset = self.df.columns
         else:
             # if a column is in columns_subset, its null column should also be added if present
@@ -228,15 +225,15 @@
         step = self._train_step
 
         self.feature_losses = defaultdict(list)
         loss_grows_num_epochs = 0
         prev_total_loss = float("inf")
         es_min_delta = 0.005
         es_patience = 10
-        pth = Path(self.vae_resources_path)
+        pth = Path(self.paths["state_path"])
 
         for epoch in range(epochs):
             num_batches = 0.0
             total_loss = 0.0
             t1 = time.time()
 
             # Iterate over the batches of the dataset.
@@ -291,15 +288,15 @@
         with tf.GradientTape() as tape:
             self.vae(batch)
 
             # Compute reconstruction loss
             loss = sum(self.vae.losses)
 
         self.optimizer.minimize(
-            loss=loss, var_list=[self.vae.trainable_weights], tape=tape
+            loss=loss, var_list=self.vae.trainable_weights, tape=tape
         )
         self.loss_metric(loss)
         return loss
 
     def display_losses(self):
         for name, l in self.feature_losses.items():
             plt.plot(l, label=name)
```

### Comparing `syngen-0.1.9/src/syngen/train.py` & `syngen-0.2.0rc0/src/syngen/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 import os
-os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
+os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
 
 import click
 from loguru import logger
 
 from syngen.ml.worker import Worker
-from syngen.ml.custom_logger import setup_logger
+from syngen.ml.utils import setup_logger
 
 
 @click.command()
 @click.option("--metadata_path", type=str, default=None, help="Path to the metadata file")
 @click.option("--source", type=str, default=None, help="Path to the table that you want to use as a reference")
 @click.option("--table_name", type=str, default=None, help="Arbitrary string to name the directories")
 @click.option("--epochs", default=10, type=click.IntRange(1),
@@ -52,15 +52,16 @@
     row_limit
     print_report
     log_level
     batch_size
     -------
 
     """
-    setup_logger(log_level)
+    os.environ["LOGURU_LEVEL"] = log_level
+    setup_logger()
     if not metadata_path and not source and not table_name:
         raise AttributeError("It seems that the information of 'metadata_path' or 'table_name' and 'source' is absent. "
                              "Please provide either the information of 'metadata_path' or "
                              "the information of 'source' and 'table_name'")
     elif metadata_path and table_name and source:
         logger.warning("The information of 'metadata_path' was provided. "
                        "In this case the information of 'table_name' and 'source' will be ignored")
@@ -92,14 +93,26 @@
         "row_limit": row_limit,
         "batch_size": batch_size,
         "print_report": print_report
     }
     worker = Worker(
         table_name=table_name,
         metadata_path=metadata_path,
-        settings=settings
+        settings=settings,
+        log_level=log_level,
+        type="train"
     )
     worker.launch_train()
 
 
+def preprocess_data():
+    """
+    Preprocess the data before the training process
+    """
+    path_to_script = f"{os.getcwd()}/model_artifacts/script.py"
+    if os.path.exists(path_to_script):
+        os.system(f"python3 {path_to_script}")
+
+
 if __name__ == "__main__":
+    preprocess_data()
     launch_train()
```

### Comparing `syngen-0.1.9/src/syngen.egg-info/PKG-INFO` & `syngen-0.2.0rc0/src/syngen.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.9
+Version: 0.2.0rc0
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,18 +50,18 @@
 <i>Please notice that the name should match the one you used in the training process.</i><br>
 This will create a csv file with the synthetic table in <i>./model_artifacts/tmp_store/TABLE_NAME/merged_infer_TABLE_NAME.csv</i>.<br>
 
 Here is a quick example:
 
 ```bash
 pip install syngen
-train --source ./example-data/housing.csv –-table_name Housing
+train --source ./examples/example-data/housing.csv –-table_name Housing
 infer --table_name Housing
 ```
-As the example you can use the dataset <i>"Housing"</i> in [example-data/housing.csv](example-data/housing.csv).
+As the example you can use the dataset <i>"Housing"</i> in [examples/example-data/housing.csv](examples/example-data/housing.csv).
 In this example, our real-world data is <a href="https://www.kaggle.com/datasets/camnugent/california-housing-prices" target="_blank">"Housing"</a> from Kaggle.
 
 ## Features
 
 ### Training
 
 You can add flexibility to the training and inference processes using additional hyperparameters.<br>
@@ -167,115 +167,152 @@
 You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
 they will be ignored in the CLI call.
 
 <i>Note:</i> By using metadata file, you can also generate tables with absent relationships. 
 In this case, the tables will be generated independently.
 
 The yaml metadata file should match the following template:
-
-    CUSTOMER:                                       # Table name. Required parameter
-        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats. Required parameter
-                 
-        train_settings:                             # Settings for training process. Optional parameter
-            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
-            drop_null: False                        # Drop rows with NULL values. Optional parameter
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
-                    - gender
-                    - marital_status
-                 
-        infer_settings:                             # Settings for infer process. Optional parameter
-            size: 100                               # Size for generated data. Optional parameter
-            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
-            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
-        keys:                                       # Keys of the table. Optional parameter
-            PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
-                type: "PK"                          # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
-                columns:                            # Array of column names
-                    - customer_id
+```yaml
+global:                                     # Global settings. Optional parameter. In this section you can specify training and inference settings which will be set for all tables
+  train_settings:                           # Settings for training process. Optional parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    
+  infer_settings:                           # Settings for infer process. Optional parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+
+CUSTOMER:                                   # Table name. Required parameter               
+  train_settings:                           # Settings for training process. Required parameter
+    source: "./files/customer.csv"          # The path to the original data. Supported formats include local files in CSV, Avro formats. Required parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    column_types:
+      categorical:                          # Force listed columns to have categorical type (use dictionary of values). Optional parameter
+        - gender
+        - marital_status
+        
+  format:                                   # Settings for reading and writing data in 'csv' format. Optional parameter
+    sep: ','                                # Delimiter to use. Optional parameter
+    quotechar: '"'                          # The character used to denote the start and end of a quoted item. Optional parameter
+    quoting: minimal                        # Control field quoting behavior per constants - ["all", "minimal", "non-numeric", "none"]. Optional parameter
+    escapechar: '"'                         # One-character string used to escape other characters. Optional parameter
+    encoding: null                          # A string representing the encoding to use in the output file. Optional parameter
+    header: infer                           # Row number(s) to use as the column names, and the start of the data. Optional parameter  
+    skiprows: null                          # Line numbers to skip (0-indexed) or number of lines to skip (int) at the start of the file. Optional parameter
+    on_bad_lines: error                     # Specifies what to do upon encountering a bad line (a line with too many fields) - ["error", "warn", "skip"]. Optional parameter
+    engine: null                            # Parser engine to use - ["c", "python"]. Optional parameter             
+  infer_settings:                           # Settings for infer process. Optional parameter
+    destination: "./files/generated_data_customer.csv"# The path where the generated data will be stored. Supported formats include local files in CSV, Avro formats. Required parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+  keys:                                     # Keys of the table. Optional parameter
+    PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
+      type: "PK"                            # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
+      columns:                              # Array of column names
+        - customer_id
      
-            UQ1:                                    # Name of a key
-                type: "UQ"                          # One or many unique keys
-                columns:
-                    - e_mail
+    UQ1:                                    # Name of a key
+      type: "UQ"                            # One or many unique keys
+      columns:
+        - e_mail
      
-            FK1:                                    # One or many foreign keys
-                type: "FK"
-                columns:                            # Array of columns in the current table
-                    - e_mail
-                    - alias
-                references:
-                    table: "PROFILE"                # Name of the parent table
-                    columns:                        # Array of columns in the parent table
-                        - e_mail
-                        - alias
+    FK1:                                    # One or many foreign keys
+      type: "FK"
+      columns:                              # Array of columns in the current table
+        - e_mail
+        - alias
+      references:
+        table: "PROFILE"                    # Name of the parent table
+        columns:                            # Array of columns in the parent table
+          - e_mail
+          - alias
        
-            FK2:
-                type: "FK"
-                columns:
-                    - address_id
-                references:
-                    table: "ADDRESS"
-                    columns:
-                        - address_id
+    FK2:
+      type: "FK"
+      columns:
+        - address_id
+      references:
+        table: "ADDRESS"
+        columns:
+          - address_id
 
      
-    ORDER:                                          # Table name. Required parameter
-        source: "./files/order.csv"                 # Supported formats include local files in CSV, Avro formats. Required parameter
-     
-        train_settings:                             # Settings for training process. Optional parameter
-            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
-            drop_null: False                        # Drop rows with NULL values. Optional parameter
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
-                    - gender
-                    - marital_status
+ORDER:                                      # Table name. Required parameter    
+  train_settings:                           # Settings for training process. Required parameter
+    source: "./files/order.csv"             # The path to the original data. Supported formats include local files in CSV, Avro formats. Required parameter
+    epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+    drop_null: False                        # Drop rows with NULL values. Optional parameter
+    row_limit: null                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+    batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    column_types:
+    categorical:                            # Force listed columns to have categorical type (use dictionary of values). Optional parameter
+      - gender
+      - marital_status
      
-        infer_settings:                             # Settings for infer process. Optional parameter
-            size: 100                               # Size for generated data. Optional parameter
-            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
-            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
-            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
-        keys:                                       # Keys of the table. Optional parameter
-            pk_order_id:
-                type: "PK"
-                columns:
-                    - order_id
+  infer_settings:                           # Settings for infer process. Optional parameter
+    destination: "./files/generated_data_order.csv"# The path where the generated data will be stored. Supported formats include local files in CSV, Avro formats. Required parameter
+    size: 100                               # Size for generated data. Optional parameter
+    run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+    print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+    batch_size: null                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+    random_seed: null                       # If specified, generates a reproducible result. Optional parameter
+  format:                                   # Settings for reading and writing data in 'csv' format. Optional parameter
+    sep: ','                                # Delimiter to use. Optional parameter
+    quotechar: '"'                          # The character used to denote the start and end of a quoted item. Optional parameter
+    quoting: minimal                        # Control field quoting behavior per constants - ["all", "minimal", "non-numeric", "none"]. Optional parameter
+    escapechar: '"'                         # One-character string used to escape other characters. Optional parameter
+    encoding: null                          # A string representing the encoding to use in the output file. Optional parameter
+    header: infer                           # Row number(s) to use as the column names, and the start of the data. Optional parameter  
+    skiprows: null                          # Line numbers to skip (0-indexed) or number of lines to skip (int) at the start of the file. Optional parameter
+    on_bad_lines: error                     # Specifies what to do upon encountering a bad line (a line with too many fields) - ["error", "warn", "skip"]. Optional parameter
+    engine: null                            # Parser engine to use - ["c", "python"]. Optional parameter
+  keys:                                     # Keys of the table. Optional parameter
+    pk_order_id:
+      type: "PK"
+      columns:
+        - order_id
      
-            FK1:
-                type: "FK"
-                columns:
-                    - customer_id
-                references:
-                    table: "CUSTOMER"
-                    columns:
-                        - customer_id
+    FK1:
+      type: "FK"
+      columns:
+        - customer_id
+      references:
+        table: "CUSTOMER"
+        columns:
+          - customer_id
+```
+<i>Note:</i>In the section <i>"global"</i> you can specify training and inference settings for all tables. If the same settings are specified for a specific table, they will override the global settings.<br>
 
-<i>You can find the example of metadata file in [example-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)</i><br>
+<i>You can find the example of metadata file in [examples/example-metadata/housing_metadata.yaml](examples/example-metadata/housing_metadata.yaml)</i><br>
 
 By providing the necessary information through a metadata file, you can initiate training and inference processes using the following commands:
 
 ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE
 infer --metadata_path=PATH_TO_YAML_METADATA_FILE
 ```
 Here is a quick example:
 
 ```bash
-train --metadata_path="./example-metadata/housing_metadata.yaml"
-infer --metadata_path="./example-metadata/housing_metadata.yaml"
+train --metadata_path="./examples/example-metadata/housing_metadata.yaml"
+infer --metadata_path="./examples/example-metadata/housing_metadata.yaml"
 ```
 
 If `--metadata_path` is present and the metadata contains the necessary parameters, other CLI parameters will be ignored.<br>
 
 ### Docker images
 
 The train and inference components of <i>syngen</i> is available as public docker images:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.9 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.2.0rc0 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -23,20 +23,21 @@
 To start training with defaults parameters run: ```bash train --source
 PATH_TO_ORIGINAL_CSV \ --table_name TABLE_NAME ``` This will train a model and
 save the model artifacts to disk. To generate with defaults parameters data
 simply call: ```bash infer --table_name TABLE_NAME ``` Please notice that the
 name should match the one you used in the training process.
 This will create a csv file with the synthetic table in ./model_artifacts/
 tmp_store/TABLE_NAME/merged_infer_TABLE_NAME.csv.
-Here is a quick example: ```bash pip install syngen train --source ./example-
-data/housing.csv â-table_name Housing infer --table_name Housing ``` As the
-example you can use the dataset "Housing" in [example-data/housing.csv]
-(example-data/housing.csv). In this example, our real-world data is "Housing"
-from Kaggle. ## Features ### Training You can add flexibility to the training
-and inference processes using additional hyperparameters.
+Here is a quick example: ```bash pip install syngen train --source ./examples/
+example-data/housing.csv â-table_name Housing infer --table_name Housing ```
+As the example you can use the dataset "Housing" in [examples/example-data/
+housing.csv](examples/example-data/housing.csv). In this example, our real-
+world data is "Housing" from Kaggle. ## Features ### Training You can add
+flexibility to the training and inference processes using additional
+hyperparameters.
 For training of single table call: ```bash train --source PATH_TO_ORIGINAL_CSV
 \ --table_name TABLE_NAME \ --epochs INT \ --row_limit INT \ --drop_null BOOL \
 --print_report BOOL \ --batch_size INT ``` To train one or more tables using a
 metadata file, you can use the following command: ```bash train --metadata_path
 PATH_TO_METADATA_YAML ``` The parameters which you can set up for training
 process: - source â required parameter for training of single table, a path
 to the file that you want to use as a reference - table_name â required
@@ -90,69 +91,119 @@
 yaml format. By providing information about the relationships between tables
 via metadata, it becomes possible to manage complex relationships across any
 number of tables. You can also specify additional parameters needed for
 training and inference in the metadata file and in this case, they will be
 ignored in the CLI call. Note: By using metadata file, you can also generate
 tables with absent relationships. In this case, the tables will be generated
 independently. The yaml metadata file should match the following template:
-CUSTOMER: # Table name. Required parameter source: "./files/customer.csv" #
-Supported formats include local files in CSV, Avro formats. Required parameter
+```yaml global: # Global settings. Optional parameter. In this section you can
+specify training and inference settings which will be set for all tables
 train_settings: # Settings for training process. Optional parameter epochs: 10
 # Number of epochs if different from the default in the command line options.
 Optional parameter drop_null: False # Drop rows with NULL values. Optional
-parameter row_limit: None # Number of rows to train over. A number less than
+parameter row_limit: null # Number of rows to train over. A number less than
 the original table length will randomly subset the specified rows number.
 Optional parameter batch_size: 32 # If specified, the training is split into
 batches. This can save the RAM. Optional parameter print_report: False # Turn
-on or turn off generation of the report. Optional parameter column_types:
-categorical: # Force listed columns to have categorical type (use dictionary of
-values). Optional parameter - gender - marital_status infer_settings: #
+on or turn off generation of the report. Optional parameter infer_settings: #
 Settings for infer process. Optional parameter size: 100 # Size for generated
 data. Optional parameter run_parallel: False # Turn on or turn off parallel
 training process. Optional parameter print_report: False # Turn on or turn off
-generation of the report. Optional parameter batch_size: None # If specified,
+generation of the report. Optional parameter batch_size: null # If specified,
 the generation is split into batches. This can save the RAM. Optional parameter
-random_seed: None # If specified, generates a reproducible result. Optional
-parameter keys: # Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name
-of a key. Only one PK per table. type: "PK" # The key type. Supported: PK -
-primary key, FK - foreign key, TKN - token key columns: # Array of column names
-- customer_id UQ1: # Name of a key type: "UQ" # One or many unique keys
-columns: - e_mail FK1: # One or many foreign keys type: "FK" columns: # Array
-of columns in the current table - e_mail - alias references: table: "PROFILE" #
-Name of the parent table columns: # Array of columns in the parent table -
-e_mail - alias FK2: type: "FK" columns: - address_id references: table:
-"ADDRESS" columns: - address_id ORDER: # Table name. Required parameter source:
-"./files/order.csv" # Supported formats include local files in CSV, Avro
-formats. Required parameter train_settings: # Settings for training process.
-Optional parameter epochs: 10 # Number of epochs if different from the default
-in the command line options. Optional parameter drop_null: False # Drop rows
-with NULL values. Optional parameter row_limit: None # Number of rows to train
-over. A number less than the original table length will randomly subset the
-specified rows number. Optional parameter batch_size: 32 # If specified, the
-training is split into batches. This can save the RAM. Optional parameter
+random_seed: null # If specified, generates a reproducible result. Optional
+parameter CUSTOMER: # Table name. Required parameter train_settings: # Settings
+for training process. Required parameter source: "./files/customer.csv" # The
+path to the original data. Supported formats include local files in CSV, Avro
+formats. Required parameter epochs: 10 # Number of epochs if different from the
+default in the command line options. Optional parameter drop_null: False # Drop
+rows with NULL values. Optional parameter row_limit: null # Number of rows to
+train over. A number less than the original table length will randomly subset
+the specified rows number. Optional parameter batch_size: 32 # If specified,
+the training is split into batches. This can save the RAM. Optional parameter
 print_report: False # Turn on or turn off generation of the report. Optional
 parameter column_types: categorical: # Force listed columns to have categorical
 type (use dictionary of values). Optional parameter - gender - marital_status
-infer_settings: # Settings for infer process. Optional parameter size: 100 #
-Size for generated data. Optional parameter run_parallel: False # Turn on or
-turn off parallel training process. Optional parameter print_report: False #
-Turn on or turn off generation of the report. Optional parameter batch_size:
-None # If specified, the generation is split into batches. This can save the
-RAM. Optional parameter random_seed: None # If specified, generates a
-reproducible result. Optional parameter keys: # Keys of the table. Optional
-parameter pk_order_id: type: "PK" columns: - order_id FK1: type: "FK" columns:
-- customer_id references: table: "CUSTOMER" columns: - customer_id You can find
-the example of metadata file in [example-metadata/housing_metadata.yaml]
-(example-metadata/housing_metadata.yaml)
+format: # Settings for reading and writing data in 'csv' format. Optional
+parameter sep: ',' # Delimiter to use. Optional parameter quotechar: '"' # The
+character used to denote the start and end of a quoted item. Optional parameter
+quoting: minimal # Control field quoting behavior per constants - ["all",
+"minimal", "non-numeric", "none"]. Optional parameter escapechar: '"' # One-
+character string used to escape other characters. Optional parameter encoding:
+null # A string representing the encoding to use in the output file. Optional
+parameter header: infer # Row number(s) to use as the column names, and the
+start of the data. Optional parameter skiprows: null # Line numbers to skip (0-
+indexed) or number of lines to skip (int) at the start of the file. Optional
+parameter on_bad_lines: error # Specifies what to do upon encountering a bad
+line (a line with too many fields) - ["error", "warn", "skip"]. Optional
+parameter engine: null # Parser engine to use - ["c", "python"]. Optional
+parameter infer_settings: # Settings for infer process. Optional parameter
+destination: "./files/generated_data_customer.csv"# The path where the
+generated data will be stored. Supported formats include local files in CSV,
+Avro formats. Required parameter size: 100 # Size for generated data. Optional
+parameter run_parallel: False # Turn on or turn off parallel training process.
+Optional parameter print_report: False # Turn on or turn off generation of the
+report. Optional parameter batch_size: null # If specified, the generation is
+split into batches. This can save the RAM. Optional parameter random_seed: null
+# If specified, generates a reproducible result. Optional parameter keys: #
+Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name of a key. Only one
+PK per table. type: "PK" # The key type. Supported: PK - primary key, FK -
+foreign key, TKN - token key columns: # Array of column names - customer_id
+UQ1: # Name of a key type: "UQ" # One or many unique keys columns: - e_mail
+FK1: # One or many foreign keys type: "FK" columns: # Array of columns in the
+current table - e_mail - alias references: table: "PROFILE" # Name of the
+parent table columns: # Array of columns in the parent table - e_mail - alias
+FK2: type: "FK" columns: - address_id references: table: "ADDRESS" columns: -
+address_id ORDER: # Table name. Required parameter train_settings: # Settings
+for training process. Required parameter source: "./files/order.csv" # The path
+to the original data. Supported formats include local files in CSV, Avro
+formats. Required parameter epochs: 10 # Number of epochs if different from the
+default in the command line options. Optional parameter drop_null: False # Drop
+rows with NULL values. Optional parameter row_limit: null # Number of rows to
+train over. A number less than the original table length will randomly subset
+the specified rows number. Optional parameter batch_size: 32 # If specified,
+the training is split into batches. This can save the RAM. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter column_types: categorical: # Force listed columns to have categorical
+type (use dictionary of values). Optional parameter - gender - marital_status
+infer_settings: # Settings for infer process. Optional parameter destination:
+"./files/generated_data_order.csv"# The path where the generated data will be
+stored. Supported formats include local files in CSV, Avro formats. Required
+parameter size: 100 # Size for generated data. Optional parameter run_parallel:
+False # Turn on or turn off parallel training process. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter batch_size: null # If specified, the generation is split into
+batches. This can save the RAM. Optional parameter random_seed: null # If
+specified, generates a reproducible result. Optional parameter format: #
+Settings for reading and writing data in 'csv' format. Optional parameter sep:
+',' # Delimiter to use. Optional parameter quotechar: '"' # The character used
+to denote the start and end of a quoted item. Optional parameter quoting:
+minimal # Control field quoting behavior per constants - ["all", "minimal",
+"non-numeric", "none"]. Optional parameter escapechar: '"' # One-character
+string used to escape other characters. Optional parameter encoding: null # A
+string representing the encoding to use in the output file. Optional parameter
+header: infer # Row number(s) to use as the column names, and the start of the
+data. Optional parameter skiprows: null # Line numbers to skip (0-indexed) or
+number of lines to skip (int) at the start of the file. Optional parameter
+on_bad_lines: error # Specifies what to do upon encountering a bad line (a line
+with too many fields) - ["error", "warn", "skip"]. Optional parameter engine:
+null # Parser engine to use - ["c", "python"]. Optional parameter keys: # Keys
+of the table. Optional parameter pk_order_id: type: "PK" columns: - order_id
+FK1: type: "FK" columns: - customer_id references: table: "CUSTOMER" columns: -
+customer_id ``` Note:In the section "global" you can specify training and
+inference settings for all tables. If the same settings are specified for a
+specific table, they will override the global settings.
+You can find the example of metadata file in [examples/example-metadata/
+housing_metadata.yaml](examples/example-metadata/housing_metadata.yaml)
 By providing the necessary information through a metadata file, you can
 initiate training and inference processes using the following commands: ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE infer --
 metadata_path=PATH_TO_YAML_METADATA_FILE ``` Here is a quick example: ```bash
-train --metadata_path="./example-metadata/housing_metadata.yaml" infer --
-metadata_path="./example-metadata/housing_metadata.yaml" ``` If `--
+train --metadata_path="./examples/example-metadata/housing_metadata.yaml" infer
+--metadata_path="./examples/example-metadata/housing_metadata.yaml" ``` If `--
 metadata_path` is present and the metadata contains the necessary parameters,
 other CLI parameters will be ignored.
 ### Docker images The train and inference components of syngen is available as
 public docker images:
 hub.docker.com/r/tdspora/syngen-train>
 hub.docker.com/r/tdspora/syngen-infer> To run dockerized code (see parameters
 description in *Training* and *Inference* sections) for one table call: ```bash
```

### Comparing `syngen-0.1.9/src/syngen.egg-info/SOURCES.txt` & `syngen-0.2.0rc0/src/syngen.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 src/syngen.egg-info/dependency_links.txt
 src/syngen.egg-info/entry_points.txt
 src/syngen.egg-info/requires.txt
 src/syngen.egg-info/top_level.txt
 src/syngen/ml/__init__.py
 src/syngen/ml/config/__init__.py
 src/syngen/ml/config/configurations.py
+src/syngen/ml/context/__init__.py
+src/syngen/ml/context/context.py
 src/syngen/ml/convertor/__init__.py
 src/syngen/ml/convertor/convertor.py
-src/syngen/ml/custom_logger/__init__.py
-src/syngen/ml/custom_logger/custom_logger.py
 src/syngen/ml/data_loaders/__init__.py
 src/syngen/ml/data_loaders/data_loaders.py
+src/syngen/ml/handlers/__init__.py
+src/syngen/ml/handlers/handlers.py
 src/syngen/ml/metrics/__init__.py
 src/syngen/ml/metrics/utils.py
 src/syngen/ml/metrics/accuracy_test/__init__.py
 src/syngen/ml/metrics/accuracy_test/accuracy_report.html
 src/syngen/ml/metrics/accuracy_test/accuracy_test.py
 src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
 src/syngen/ml/metrics/metrics_classes/__init__.py
@@ -34,16 +36,14 @@
 src/syngen/ml/metrics/sample_test/__init__.py
 src/syngen/ml/metrics/sample_test/sample_report_template.html
 src/syngen/ml/metrics/sample_test/sample_test.py
 src/syngen/ml/reporters/__init__.py
 src/syngen/ml/reporters/reporters.py
 src/syngen/ml/strategies/__init__.py
 src/syngen/ml/strategies/strategies.py
-src/syngen/ml/train_chain/__init__.py
-src/syngen/ml/train_chain/train_chain.py
 src/syngen/ml/utils/__init__.py
 src/syngen/ml/utils/utils.py
 src/syngen/ml/vae/__init__.py
 src/syngen/ml/vae/models/__init__.py
 src/syngen/ml/vae/models/custom_layers.py
 src/syngen/ml/vae/models/dataset.py
 src/syngen/ml/vae/models/features.py
```

