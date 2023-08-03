# Comparing `tmp/cnlp-transformers-0.5.0.tar.gz` & `tmp/cnlp-transformers-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnlp-transformers-0.5.0.tar", last modified: Tue Apr  4 17:29:02 2023, max compression
+gzip compressed data, was "cnlp-transformers-0.6.0.tar", last modified: Thu Aug  3 21:16:53 2023, max compression
```

## Comparing `cnlp-transformers-0.5.0.tar` & `cnlp-transformers-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:29:02.117357 cnlp-transformers-0.5.0/
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    11344 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/LICENSE
--rw-rw-r--   0 tmill     (1000) tmill     (1000)       26 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/MANIFEST.in
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    10931 2023-04-04 17:29:02.117357 cnlp-transformers-0.5.0/PKG-INFO
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    10126 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/README.md
--rw-rw-r--   0 tmill     (1000) tmill     (1000)       90 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/pyproject.toml
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     1564 2023-04-04 17:29:02.117357 cnlp-transformers-0.5.0/setup.cfg
-drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:29:02.113357 cnlp-transformers-0.5.0/src/
-drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:29:02.113357 cnlp-transformers-0.5.0/src/cnlp_transformers.egg-info/
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    10931 2023-04-04 17:29:02.000000 cnlp-transformers-0.5.0/src/cnlp_transformers.egg-info/PKG-INFO
--rw-rw-r--   0 tmill     (1000) tmill     (1000)      994 2023-04-04 17:29:02.000000 cnlp-transformers-0.5.0/src/cnlp_transformers.egg-info/SOURCES.txt
--rw-rw-r--   0 tmill     (1000) tmill     (1000)        1 2023-04-04 17:29:02.000000 cnlp-transformers-0.5.0/src/cnlp_transformers.egg-info/dependency_links.txt
--rw-rw-r--   0 tmill     (1000) tmill     (1000)      251 2023-04-04 17:29:02.000000 cnlp-transformers-0.5.0/src/cnlp_transformers.egg-info/entry_points.txt
--rw-rw-r--   0 tmill     (1000) tmill     (1000)      338 2023-04-04 17:29:02.000000 cnlp-transformers-0.5.0/src/cnlp_transformers.egg-info/requires.txt
--rw-rw-r--   0 tmill     (1000) tmill     (1000)        6 2023-04-04 17:29:02.000000 cnlp-transformers-0.5.0/src/cnlp_transformers.egg-info/top_level.txt
-drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:29:02.117357 cnlp-transformers-0.5.0/src/cnlpt/
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     3168 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/BaselineModels.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    24688 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/CnlpModelForClassification.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    15182 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/HierarchicalTransformer.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)        6 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/VERSION
--rw-rw-r--   0 tmill     (1000) tmill     (1000)       67 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/__init__.py
-drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:29:02.117357 cnlp-transformers-0.5.0/src/cnlpt/api/
--rw-rw-r--   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/api/__init__.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     4797 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/api/cnlp_rest.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     3731 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/api/dtr_rest.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     5067 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/api/event_rest.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     2726 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/api/hier_rest.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     3526 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/api/negation_rest.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     8998 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/api/temporal_rest.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     5038 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/api/timex_rest.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    30857 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/cnlp_data.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     6611 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/cnlp_metrics.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     8830 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/cnlp_processors.py
-drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:29:02.117357 cnlp-transformers-0.5.0/src/cnlpt/data/
--rw-rw-r--   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/data/__init__.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     4185 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/data/preprocess_i2b2_2008.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    15084 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/data/transform_prot.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     2609 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/data/transform_uci_drug.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    17958 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/src/cnlpt/thyme_eval.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)    33807 2023-04-04 17:28:11.000000 cnlp-transformers-0.5.0/src/cnlpt/train_system.py
-drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-04-04 17:29:02.117357 cnlp-transformers-0.5.0/test/
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     2809 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/test/test_api.py
--rw-rw-r--   0 tmill     (1000) tmill     (1000)     1896 2023-04-04 17:16:54.000000 cnlp-transformers-0.5.0/test/test_init.py
+drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:16:53.961408 cnlp-transformers-0.6.0/
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    11344 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/LICENSE
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    10881 2023-08-03 21:16:53.961408 cnlp-transformers-0.6.0/PKG-INFO
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    10126 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/README.md
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)       90 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/pyproject.toml
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     1656 2023-08-03 21:16:53.961408 cnlp-transformers-0.6.0/setup.cfg
+drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:16:53.957408 cnlp-transformers-0.6.0/src/
+drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:16:53.957408 cnlp-transformers-0.6.0/src/cnlp_transformers.egg-info/
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    10881 2023-08-03 21:16:53.000000 cnlp-transformers-0.6.0/src/cnlp_transformers.egg-info/PKG-INFO
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     1102 2023-08-03 21:16:53.000000 cnlp-transformers-0.6.0/src/cnlp_transformers.egg-info/SOURCES.txt
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)        1 2023-08-03 21:16:53.000000 cnlp-transformers-0.6.0/src/cnlp_transformers.egg-info/dependency_links.txt
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)      439 2023-08-03 21:16:53.000000 cnlp-transformers-0.6.0/src/cnlp_transformers.egg-info/entry_points.txt
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)      270 2023-08-03 21:16:53.000000 cnlp-transformers-0.6.0/src/cnlp_transformers.egg-info/requires.txt
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)        6 2023-08-03 21:16:53.000000 cnlp-transformers-0.6.0/src/cnlp_transformers.egg-info/top_level.txt
+drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:16:53.961408 cnlp-transformers-0.6.0/src/cnlpt/
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     3756 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/BaselineModels.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    22189 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/CnlpModelForClassification.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    17794 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/HierarchicalTransformer.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)       91 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/__init__.py
+drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:16:53.961408 cnlp-transformers-0.6.0/src/cnlpt/api/
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/__init__.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     4459 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/cnlp_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     3391 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/cnn_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     3132 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/current_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     3682 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/dtr_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     5018 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/event_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     3554 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/hier_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     3506 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/negation_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    11344 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/temporal_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     3157 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/termexists_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     4989 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/api/timex_rest.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     7074 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/cnlp_args.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    37158 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/cnlp_data.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     6685 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/cnlp_metrics.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     3752 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/cnlp_predict.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     9761 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/cnlp_processors.py
+drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:16:53.961408 cnlp-transformers-0.6.0/src/cnlpt/data/
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/data/__init__.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     4185 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/data/preprocess_i2b2_2008.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    15687 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/data/transform_prot.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     2609 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/data/transform_uci_drug.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    17958 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/thyme_eval.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)    26223 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/src/cnlpt/train_system.py
+drwxrwxr-x   0 tmill     (1000) tmill     (1000)        0 2023-08-03 21:16:53.961408 cnlp-transformers-0.6.0/test/
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     2547 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/test/test_api.py
+-rw-rw-r--   0 tmill     (1000) tmill     (1000)     1896 2023-08-03 21:06:36.000000 cnlp-transformers-0.6.0/test/test_init.py
```

### Comparing `cnlp-transformers-0.5.0/LICENSE` & `cnlp-transformers-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnlp-transformers-0.5.0/PKG-INFO` & `cnlp-transformers-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: cnlp-transformers
-Version: 0.5.0
+Version: 0.6.0
 Summary: Transformers for Clinical NLP
 Home-page: https://github.com/Machine-Learning-for-Medical-Language/cnlp_transformers
 Author: Machine Learning for Medical Language Lab @ CHIP
 Author-email: Timothy.Miller@childrens.harvard.edu
 Project-URL: Bug Tracker, https://github.com/Machine-Learning-for-Medical-Language/cnlp_transformers/issues
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Clinical NLP Transformers (cnlp_transformers)
 Transformers for Clinical NLP
 
 This library was created to add abstractions on top of the Huggingface Transformers library for many clinical NLP research use cases.
```

### Comparing `cnlp-transformers-0.5.0/README.md` & `cnlp-transformers-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cnlp-transformers-0.5.0/setup.cfg` & `cnlp-transformers-0.6.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 [metadata]
 name = cnlp-transformers
-version = file: src/cnlpt/VERSION
+version = attr: cnlpt.__version__
 author = Machine Learning for Medical Language Lab @ CHIP
 author_email = Timothy.Miller@childrens.harvard.edu
 description = Transformers for Clinical NLP
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Machine-Learning-for-Medical-Language/cnlp_transformers
 project_urls = 
 	Bug Tracker = https://github.com/Machine-Learning-for-Medical-Language/cnlp_transformers/issues
 classifiers = 
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 	License :: OSI Approved :: Apache Software License
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7, <3.11
+python_requires = >=3.8, <3.11
 install_requires = 
 	anaforatools~=1.1.0
 	datasets~=2.4.0
 	fastapi~=0.88.0
 	filelock~=3.4.0
 	huggingface-hub~=0.9.0
 	nltk~=3.5
-	numpy ~=1.21.5; python_version<'3.8'
-	numpy ~=1.23.3; python_version>='3.8'
+	numpy~=1.23.3
 	pandas~=1.3.5
-	pydantic~=1.8.2
+	pydantic~=1.10.8
 	PyRuSH~=1.0.3.6
 	requests~=2.26.0
 	scikit-learn~=1.0.2
 	seqeval~=1.2.2
 	torch~=1.5
 	transformers~=4.15
 	uvicorn[standard]~=0.16.0
 
 [options.entry_points]
 console_scripts = 
+	cnlpt_current_rest = cnlpt.api.current_rest:rest
 	cnlpt_dtr_rest = cnlpt.api.dtr_rest:rest
 	cnlpt_event_rest = cnlpt.api.event_rest:rest
 	cnlpt_negation_rest = cnlpt.api.negation_rest:rest
 	cnlpt_temporal_rest = cnlpt.api.temporal_rest:rest
+	cnlpt_termexists_rest = cnlpt.api.termexists_rest:rest
 	cnlpt_timex_rest = cnlpt.api.timex_rest:rest
+	cnlpt_hier_rest = cnlpt.api.hier_rest:rest
+	cnlpt_cnn_rest = cnlpt.api.cnn_rest:rest
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cnlp-transformers-0.5.0/src/cnlp_transformers.egg-info/PKG-INFO` & `cnlp-transformers-0.6.0/src/cnlp_transformers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: cnlp-transformers
-Version: 0.5.0
+Version: 0.6.0
 Summary: Transformers for Clinical NLP
 Home-page: https://github.com/Machine-Learning-for-Medical-Language/cnlp_transformers
 Author: Machine Learning for Medical Language Lab @ CHIP
 Author-email: Timothy.Miller@childrens.harvard.edu
 Project-URL: Bug Tracker, https://github.com/Machine-Learning-for-Medical-Language/cnlp_transformers/issues
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Clinical NLP Transformers (cnlp_transformers)
 Transformers for Clinical NLP
 
 This library was created to add abstractions on top of the Huggingface Transformers library for many clinical NLP research use cases.
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/BaselineModels.py` & `cnlp-transformers-0.6.0/src/cnlpt/BaselineModels.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,38 @@
+from typing import Dict, List
+
 import torch
 from torch import nn
 import torch.nn.functional as F
 
 class CnnSentenceClassifier(nn.Module):
-    def __init__(self, vocab_size, embed_dims=100, num_labels_list=[2,], num_filters=25, dropout=0.2, filters=(1,2,3)):
+    def __init__(
+        self,
+        vocab_size,
+        task_names: List[str],
+        num_labels_dict: Dict[str, int],
+        embed_dims=100,
+        num_filters=25,
+        dropout=0.2,
+        filters=(1,2,3)
+    ):
         super(CnnSentenceClassifier, self).__init__()
-        self.dropout =  dropout
+        self.dropout = dropout
 
         self.embed = nn.Embedding(num_embeddings=vocab_size, embedding_dim=embed_dims)
         self.convs = nn.ModuleList( [nn.Conv1d(embed_dims, num_filters, x) for x in filters] )
         self.loss_fn = nn.CrossEntropyLoss()
         
         self.fcs = nn.ModuleList()
-        for task_num_labels in num_labels_list:
-            self.fcs.append(nn.Linear(num_filters * len(filters), task_num_labels))
 
+        self.task_names = task_names
+        for task_name in self.task_names:
+            if task_name not in num_labels_dict:
+                raise ValueError("Misalignment between task_names and num_labels_dict")
+            self.fcs.append(nn.Linear(num_filters * len(filters), num_labels_dict[task_name]))
 
     def forward(
         self,
         input_ids=None,
         event_tokens=None,
         labels=None,
         **kwargs,
@@ -43,25 +57,37 @@
                     task_labels = labels[:,0,task_ind]
                 loss += self.loss_fn(task_logits, task_labels.type(torch.LongTensor).to(labels.device))
         
         return loss, logits
 
 
 class LstmSentenceClassifier(nn.Module):
-    def __init__(self, vocab_size, embed_dims=100, num_labels_list=[2,], dropout=0.2, hidden_size=100):
+    def __init__(
+        self,
+        vocab_size,
+        task_names: List[str],
+        num_labels_dict: Dict[str, int],
+        embed_dims=100,
+        dropout=0.2,
+        hidden_size=100
+    ):
         super(LstmSentenceClassifier, self).__init__()
-        self.dropout =  dropout
+        self.dropout = dropout
 
         self.embed = nn.Embedding(num_embeddings=vocab_size, embedding_dim=embed_dims)
         self.lstm = nn.LSTM(input_size = embed_dims, hidden_size=hidden_size, bidirectional=True)
         self.loss_fn = nn.CrossEntropyLoss()
         
         self.fcs = nn.ModuleList()
-        for task_num_labels in num_labels_list:
-            self.fcs.append(nn.Linear(4*hidden_size, task_num_labels))
+
+        self.task_names = task_names
+        for task_name in self.task_names:
+            if task_name not in num_labels_dict:
+                raise ValueError("Misalignment between task_names and num_labels_dict")
+            self.fcs.append(nn.Linear(4*hidden_size, num_labels_dict[task_name]))
 
     def forward(
         self,
         input_ids = None,
         event_tokens = None,
         labels = None,
         **kwargs,
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/CnlpModelForClassification.py` & `cnlp-transformers-0.6.0/src/cnlpt/CnlpModelForClassification.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Module containing the CNLP transformer model.
 """
 # from transformers.models.auto import  AutoModel, AutoConfig
 import copy
 import inspect
-from typing import Optional, List, Any, Dict
+from os import PathLike
+from typing import Optional, List, Any, Dict, Union
 
 from transformers import AutoModel, AutoConfig
 from transformers.modeling_utils import PreTrainedModel
 from transformers.configuration_utils import PretrainedConfig
 
 import torch
 from torch import nn
 import logging
 from torch.nn import CrossEntropyLoss, MSELoss
 from transformers.modeling_outputs import SequenceClassifierOutput
 from torch.nn.functional import softmax, relu
 import math
 import random
+from . import __version__ as cnlpt_version
 
 logger = logging.getLogger(__name__)
 
 def generalize_encoder_forward_kwargs(encoder, **kwargs: Any) -> Dict[str, Any]:
     new_kwargs = dict()
     params = inspect.signature(encoder.forward).parameters
     for name, value in kwargs.items():
@@ -67,15 +69,24 @@
     :param layer - Which layer to pull the encoder representation from
     :param tokens - Whether to classify an entity based on the token reprsentation rather than the CLS representation
     :param tagger - Whether the current task is a token tagging task
     :param relations - Whether the current task is relation exttraction
     :param num_attention_heads - For relations, how many "features" to use
     :param head_size - For relations, how big each head should be
     """
-    def __init__(self, config, layer=10, tokens=False, tagger=False, relations=False, num_attention_heads=-1, head_size=64):
+    def __init__(
+        self,
+        config: 'CnlpConfig',
+        layer: int = 10,
+        tokens: bool = False,
+        tagger: bool = False,
+        relations: bool = False,
+        num_attention_heads: int = -1,
+        head_size: int = 64,
+    ):
         super().__init__()
         self.dropout = nn.Dropout(config.hidden_dropout_prob)
         if relations:
             self.dense = nn.Identity()
         else:
             self.dense = nn.Linear(config.hidden_size, config.hidden_size)
             
@@ -138,56 +149,59 @@
 
 
 class CnlpConfig(PretrainedConfig):
     """
     The config class for :class:`CnlpModelForClassification`.
 
     :param encoder_name: the encoder name to use with :meth:`transformers.AutoConfig.from_pretrained`
-    :param typing.Optional[str] finetuning_task: the tasks for which this model is fine-tuned
-    :param typing.List[int] num_labels_list: the number of labels for each task
-    :param int layer: the index of the encoder layer to extract features from
-    :param bool tokens: if true, sentence-level classification is done based on averaged token embeddings for token(s) surrounded by <e> </e> special tokens
-    :param int num_rel_attention_heads: the number of features/attention heads to use in the NxN relation classifier
-    :param int rel_attention_head_dims: the number of parameters in each attention head in the NxN relation classifier
-    :param typing.List[bool] tagger: for each task, whether the task is a sequence tagging task
-    :param typing.List[bool] relations: for each task, whether the task is a relation extraction task
-    :param bool use_prior_tasks: whether to use the outputs from the previous tasks as additional inputs for subsequent tasks
+    :param finetuning_task: the tasks for which this model is fine-tuned
+    :param layer: the index of the encoder layer to extract features from
+    :param tokens: if true, sentence-level classification is done based on averaged token embeddings for token(s) surrounded by <e> </e> special tokens
+    :param num_rel_attention_heads: the number of features/attention heads to use in the NxN relation classifier
+    :param rel_attention_head_dims: the number of parameters in each attention head in the NxN relation classifier
+    :param tagger: for each task, whether the task is a sequence tagging task
+    :param relations: for each task, whether the task is a relation extraction task
+    :param use_prior_tasks: whether to use the outputs from the previous tasks as additional inputs for subsequent tasks
+    :param hier_head_config: If this is a hierarchical model, this is where the config parameters go
+    :param label_dictionary: A mapping from task names to label sets
     :param \**kwargs: arguments for :class:`transformers.PretrainedConfig`
     """
     model_type='cnlpt'
 
     def __init__(
         self,
-        encoder_name='roberta-base',
-        finetuning_task=None,
-        num_labels_list=[],
-        layer=-1,
-        tokens=False,
-        num_rel_attention_heads=12,
-        rel_attention_head_dims=64,
-        tagger = [False],
-        relations = [False],
-        use_prior_tasks=False,
-        hier_head_config=None,
+        *,
+        encoder_name: Union[str, PathLike] = 'roberta-base',
+        finetuning_task: Optional[List[str]] = None,
+        layer: int = -1,
+        tokens: bool = False,
+        num_rel_attention_heads: int = 12,
+        rel_attention_head_dims: int = 64,
+        tagger: Dict[str, bool] = {},
+        relations: Dict[str, bool] = {},
+        use_prior_tasks: bool = False,
+        hier_head_config: Dict[str, Any] = None,
+        label_dictionary: Dict[str, List[str]] = None,
         **kwargs
      ):
         super().__init__(**kwargs)
         # self.name_or_path='cnlpt'
         self.finetuning_task = finetuning_task
-        self.num_labels_list = num_labels_list
         self.layer = layer
         self.tokens = tokens
         self.num_rel_attention_heads = num_rel_attention_heads
         self.rel_attention_head_dims = rel_attention_head_dims
         self.tagger = tagger
         self.relations = relations
         self.use_prior_tasks = use_prior_tasks
         self.encoder_name = encoder_name
         self.encoder_config = AutoConfig.from_pretrained(encoder_name).to_dict()
         self.hier_head_config = hier_head_config
+        self.label_dictionary = label_dictionary
+        self.cnlpt_version = cnlpt_version
         if encoder_name.startswith('distilbert'):
             self.hidden_dropout_prob = self.encoder_config['dropout']
             self.hidden_size = self.encoder_config['dim']
         else:
             try:
                 self.hidden_dropout_prob = self.encoder_config['hidden_dropout_prob']
                 self.hidden_size = self.encoder_config['hidden_size']
@@ -199,88 +213,91 @@
                                  f' APIs are not yet supported (#35).')
 
 
 class CnlpModelForClassification(PreTrainedModel):
     """
     The CNLP transformer model.
 
-    :param typing.Optional[typing.List[float]] class_weights: if provided,
+    :param class_weights: if provided,
         the weights to use for each task when computing the loss
-    :param float final_task_weight: the weight to use for the final task
+    :param final_task_weight: the weight to use for the final task
         when computing the loss; default 1.0.
-    :param float argument_regularization: if provided, the argument
-        regularization to use when computing the loss
-    :param bool freeze: whether to freeze the weights of the encoder
-    :param bool bias_fit: whether to fine-tune only the bias of the encoder
+    :param freeze: what proportion of encoder weights to freeze (-1 for none)
+    :param bias_fit: whether to fine-tune only the bias of the encoder
     """
     base_model_prefix = 'cnlpt'
     config_class = CnlpConfig
 
     def __init__(self,
                  config: config_class,
                  *,
-                 class_weights: Optional[List[float]] = None,
+                 class_weights: Optional[Dict[str, float]] = None,
                  final_task_weight: float = 1.0,
-                 argument_regularization: float = -1,
                  freeze: float = -1.0,
-                 bias_fit=False,
+                 bias_fit: bool = False,
                  ):
 
         super().__init__(config)
 
         encoder_config = AutoConfig.from_pretrained(config.encoder_name)
         encoder_config.vocab_size = config.vocab_size
         config.encoder_config = encoder_config.to_dict()
         encoder_model = AutoModel.from_config(encoder_config)
         self.encoder = encoder_model.from_pretrained(config.encoder_name)
         self.encoder.resize_token_embeddings(encoder_config.vocab_size)
+        
+        # This would seem to be redundant with the label list, which maps from tasks to labels,
+        # but this version is ordered. This will allow the user to specify an order for any methods
+        # where we feed the output of one task into the next.
+        # It also will be used as the canonical order of returning results/logits
+        self.tasks = config.finetuning_task
 
         if config.layer > len(encoder_model.encoder.layer):
             raise ValueError('The layer specified (%d) is too big for the specified encoder which has %d layers' % (
                 config.layer,
                 len(encoder_model.encoder.layer)
             ))
-        self.num_labels = config.num_labels_list
         
         if freeze > 0:
             freeze_encoder_weights(self.encoder, freeze)
 
         if bias_fit:
             for name, param in self.encoder.named_parameters():
                 if not 'bias' in name:
                     param.requires_grad = False
 
-        self.feature_extractors = nn.ModuleList()
-        self.logit_projectors = nn.ModuleList()
-        self.classifiers = nn.ModuleList()
+        self.feature_extractors = nn.ModuleDict()
+        self.classifiers = nn.ModuleDict()
+
         total_prev_task_labels = 0
-        for task_ind,task_num_labels in enumerate(self.num_labels):
-            self.feature_extractors.append(RepresentationProjectionLayer(config, layer=config.layer, tokens=config.tokens, tagger=config.tagger[task_ind], relations=config.relations[task_ind], num_attention_heads=config.num_rel_attention_heads, head_size=config.rel_attention_head_dims))
-            if config.relations[task_ind]:
+        for task_name,task_labels in config.label_dictionary.items():
+            task_num_labels = len(task_labels)
+            self.feature_extractors[task_name] = RepresentationProjectionLayer(config, layer=config.layer, tokens=config.tokens, tagger=config.tagger[task_name], relations=config.relations[task_name], num_attention_heads=config.num_rel_attention_heads, head_size=config.rel_attention_head_dims)
+            if config.relations[task_name]:
                 hidden_size = config.num_rel_attention_heads
                 if config.use_prior_tasks:
                     hidden_size += total_prev_task_labels
 
-                self.classifiers.append(ClassificationHead(config, task_num_labels, hidden_size=hidden_size))
+                self.classifiers[task_name] = ClassificationHead(config, task_num_labels, hidden_size=hidden_size)
             else:
-                self.classifiers.append(ClassificationHead(config, task_num_labels))
+                self.classifiers[task_name] = ClassificationHead(config, task_num_labels)
             total_prev_task_labels += task_num_labels
 
         # Are we operating as a sequence classifier (1 label per input sequence) or a tagger (1 label per input token in the sequence)
         self.tagger = config.tagger
         self.relations = config.relations
 
         if class_weights is None:
-            self.class_weights = [None] * len(self.classifiers)
+            self.class_weights = {x: None for x in config.label_dictionary.keys()}
         else:
             self.class_weights = class_weights
 
+        self.label_dictionary = config.label_dictionary
         self.final_task_weight = final_task_weight
         self.use_prior_tasks = config.use_prior_tasks
-        self.argument_regularization = argument_regularization
         self.reg_temperature = 1.0
 
         # self.init_weights()
 
     def predict_relations_with_previous_logits(self, features, logits):
         seq_len = features.shape[1]
         for prior_task_logits in logits:
@@ -301,15 +318,15 @@
                 logging.warn("It is not implemented to add previous task of any type to a sequence task")
 
         return features
 
     def compute_loss(self,
                      task_logits: torch.FloatTensor,
                      labels: torch.LongTensor,
-                     task_ind,
+                     task_ind: int,
                      task_num_labels,
                      batch_size,
                      seq_len,
                      state: dict,
                      ) -> None:
         """
         Computes the loss for a single batch and a single task.
@@ -320,31 +337,32 @@
             task_ind:
             task_num_labels:
             batch_size:
             seq_len:
             state:
         :meta private:
         """
+        task_name = self.tasks[task_ind]
         if task_num_labels == 1:
             #  We are doing regression
             loss_fct = MSELoss()
             task_loss = loss_fct(task_logits.view(-1), labels.view(-1))
         else:
-            if not self.class_weights[task_ind] is None:
-                class_weights = torch.FloatTensor(self.class_weights[task_ind]).to(self.device)
+            if not self.class_weights[task_name] is None:
+                class_weights = torch.FloatTensor(self.class_weights[task_name]).to(self.device)
             else:
                 class_weights = None
             loss_fct = CrossEntropyLoss(weight=class_weights)
 
-            if self.relations[task_ind]:
+            if self.relations[task_name]:
                 task_labels = labels[:, :, state['task_label_ind']:state['task_label_ind'] + seq_len]
                 state['task_label_ind'] += seq_len
                 task_loss = loss_fct(task_logits.permute(0, 3, 1, 2),
                                      task_labels.type(torch.LongTensor).to(labels.device))
-            elif self.tagger[task_ind]:
+            elif self.tagger[task_name]:
                 # in cases where we are only given a single task the HF code will have one fewer dimension in the labels, so just add a dummy dimension to make our indexing work:
                 if labels.ndim == 2:
                     task_labels = labels
                 elif labels.ndim == 3:
                     # labels = labels.unsqueeze(1)
                     task_labels = labels[:, :, state['task_label_ind']]
                 else:
@@ -368,73 +386,17 @@
 
                 state['task_label_ind'] += 1
                 task_loss = loss_fct(task_logits, task_labels.type(torch.LongTensor).to(labels.device))
 
         if state['loss'] is None:
             state['loss'] = task_loss
         else:
-            task_weight = 1.0 if task_ind + 1 < len(self.num_labels) else self.final_task_weight
+            task_weight = 1.0 if task_ind + 1 < len(self.tasks) else self.final_task_weight
             state['loss'] += (task_weight * task_loss)
 
-    def apply_arg_reg(self,
-                      logits: List[torch.FloatTensor],
-                      attention_mask: torch.LongTensor,
-                      state: dict) -> None:
-        """
-        Applies argument regularization to the logits for a single batch on all tasks.
-
-        Args:
-            logits (`List[torch.FloatTensor]`): the computed logits of the batch.
-            attention_mask (`torch.LongTensor`): the attention mask for the batch.
-            state: the state dict containing the loss for the batch.
-        :meta private:
-        """
-        # standard e2e relation task -- two entity extractors and relation extractor.
-        prob_no_rel = softmax(logits[2], dim=3)[:, :, :, 0]
-
-        ## product gets us something like a joint probability over all relation categories.
-        # the downside is, we're penalizing the event "some relation being more likely than none"
-        # in the joint sense, but we never actually use that event anywhere, i.e., if no
-        # relation meets the threshold we will never create a relation.
-        # so maybe doing something like relu + sum makes more sense.
-        #
-        # prob_a1_norel = prob_no_rel.prod(dim=1)
-        # prob_a2_norel = prob_no_rel.prod(dim=2)
-        # prob_some_rel = relu ( 1 - (prob_a1_norel * prob_a2_norel) - 0.5)
-        # These values will be greater than 0 at position i if there is any relation that
-        # has i as arg1 or i as arg2.
-        prob_a1_rel = relu(0.5 - prob_no_rel).sum(dim=1)
-        prob_a2_rel = relu(0.5 - prob_no_rel).sum(dim=2)
-        prob_some_rel = prob_a1_rel + prob_a2_rel
-
-        # prob_no_e1_type = relu( softmax(logits[0], dim=2)[:,:,0] - 0.5)
-        # prob_no_e2_type = relu( softmax(logits[1], dim=2)[:,:,0] - 0.5)
-        probs_e1 = softmax(logits[0], dim=2)
-        probs_e2 = softmax(logits[1], dim=2)
-
-        # threshold: the penalty is possible if more than this number of probabilities are greater than the
-        # "no entity" threshold. we subtract 2 because we are removing the None category, and C-1 is the default
-        # case where there is no relation, only if more than that is an issue.
-        t1_threshold = self.num_labels[0] - 2
-        t2_threshold = self.num_labels[1] - 2
-
-        # we take p(none) - p(other relations) inside the sign.
-        # then take the sign, if there are any -1s, the sum will be less than tx_threshold and the inner part will be < 0,
-        # and relu will be 0. If there are no -1, the sum will be > tx_threshold and the innter part will be 1, relu also 1.
-        prob_no_e1_type = relu(
-            torch.sign(probs_e1[:, :, 0].unsqueeze(2) - probs_e1[:, :, 1:]).sum(dim=2) - t1_threshold)
-        prob_no_e2_type = relu(
-            torch.sign(probs_e2[:, :, 0].unsqueeze(2) - probs_e2[:, :, 1:]).sum(dim=2) - t2_threshold)
-
-        prob_no_ent = prob_no_e1_type * prob_no_e2_type
-
-        prob_rel_no_ent = prob_some_rel * prob_no_ent * attention_mask
-
-        state["loss"] += self.argument_regularization * prob_rel_no_ent.sum()
-
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         token_type_ids=None,
         position_ids=None,
         head_mask=None,
@@ -494,36 +456,34 @@
         logits = []
 
         state = dict(
             loss=None,
             task_label_ind=0
         )
 
-        for task_ind,task_num_labels in enumerate(self.num_labels):
-            features = self.feature_extractors[task_ind](outputs.hidden_states, event_tokens)
+        for task_ind, task_name in enumerate(self.tasks):
+            task_labels = self.label_dictionary[task_name]
+            features = self.feature_extractors[task_name](outputs.hidden_states, event_tokens)
             if self.use_prior_tasks:
                 # note: this specific way of incorporating previous logits doesn't help in my experiments with thyme/clinical tempeval
-                if self.relations[task_ind]:
+                if self.relations[task_name]:
                     features = self.predict_relations_with_previous_logits(features, logits)
-            task_logits = self.classifiers[task_ind](features)
+            task_logits = self.classifiers[task_name](features)
             logits.append(task_logits)
 
             if labels is not None:
                 self.compute_loss(
                     task_logits,
                     labels,
                     task_ind,
-                    task_num_labels,
+                    len(task_labels),
                     batch_size,
                     seq_len,
                     state
                 )
 
-        if len(self.num_labels) == 3 and self.relations[-1] and self.argument_regularization > 0:
-            self.apply_arg_reg(logits, attention_mask, state)
-
         if self.training:
             return SequenceClassifierOutput(
                 loss=state['loss'], logits=logits, hidden_states=outputs.hidden_states, attentions=outputs.attentions,
             )
         else:
             return SequenceClassifierOutput(loss=state['loss'], logits=logits, attentions=outputs.attentions)
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/HierarchicalTransformer.py` & `cnlp-transformers-0.6.0/src/cnlpt/HierarchicalTransformer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Module containing the Hierarchical Transformer module, adapted from Xin Su.
 """
 import logging
 import copy
 import random
-from typing import Optional, List, cast
+from typing import Optional, List, cast, Dict, Tuple
 
 import numpy as np
 from torch import nn
 import torch.nn.functional as F
 import torch
 from torch.nn import CrossEntropyLoss
-
+from dataclasses import dataclass
 from transformers.modeling_outputs import SequenceClassifierOutput
 from transformers.modeling_utils import PreTrainedModel
 from transformers import AutoModel, AutoConfig
 
 from .CnlpModelForClassification import CnlpConfig, ClassificationHead, generalize_encoder_forward_kwargs, freeze_encoder_weights
 
 logger = logging.getLogger(__name__)
@@ -31,14 +31,17 @@
     """
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     if n_gpu > 0:
         torch.cuda.manual_seed_all(seed)
 
+@dataclass
+class HierarchicalSequenceClassifierOutput(SequenceClassifierOutput):
+    chunk_attentions: Optional[Tuple[torch.FloatTensor]] = None
 
 class MultiHeadAttention(nn.Module):
     """
     Multi-Head Attention module
 
     Original author: Yu-Hsiang Huang (https://github.com/jadore801120/attention-is-all-you-need-pytorch)
 
@@ -224,21 +227,37 @@
         self.encoder.resize_token_embeddings(encoder_config.vocab_size)
 
         if self.config.layer > self.config.hier_head_config["n_layers"]:
             raise ValueError('The layer specified (%d) is too big for the specified chunk transformer which has %d layers' % (
                 self.config.layer,
                 self.config.hier_head_config["n_layers"]
             ))
-        self.layer = self.config.layer
+        
+        if self.config.layer < 0:
+            self.layer = self.config.hier_head_config["n_layers"] + self.config.layer + 1
+            if self.layer < 0:
+                raise ValueError("The layer specified (%d) is a negative value which is larger than the actual number of layers %d" % (
+                    self.config.layer, 
+                    self.config.hier_head_config["n_layers"]
+                ))
+        else:
+            self.layer = self.config.layer
+
+        if self.layer == 0:
+            raise ValueError("The classifier layer derived is 0 which is ambiguous -- there is no usable 0th layer in a hierarchical model. Enter a value for the layer argument that at least 1 (use one layer) or -1 (use the final layer)")
+
+        # This would seem to be redundant with the label list, which maps from tasks to labels,
+        # but this version is ordered. This will allow the user to specify an order for any methods
+        # where we feed the output of one task into the next.
+        # It also will be used as the canonical order of returning results/logits
+        self.tasks = config.finetuning_task
 
         if freeze > 0:
             freeze_encoder_weights(self.encoder, freeze)
 
-        self.num_labels = self.config.num_labels_list
-
         # Document-level transformer layer
         transformer_layer = EncoderLayer(
             d_model=self.config.hidden_size,
             d_inner=self.config.hier_head_config["d_inner"],
             n_head=self.config.hier_head_config["n_head"],
             d_k=self.config.hier_head_config["d_k"],
             d_v=self.config.hier_head_config["d_v"],
@@ -247,20 +266,42 @@
         self.transformer = nn.ModuleList(
             [
                 copy.deepcopy(transformer_layer)
                 for _ in range(self.config.hier_head_config["n_layers"])
             ]
         )
 
-        self.classifiers = nn.ModuleList()
-        for task_num_labels in self.num_labels:
-            self.classifiers.append(ClassificationHead(self.config, task_num_labels))
+        self.classifiers = nn.ModuleDict()
+        # for task_num_labels in self.num_labels:
+        for task_name,task_labels in config.label_dictionary.items():
+            task_num_labels = len(task_labels)
+            self.classifiers[task_name] = ClassificationHead(self.config, task_num_labels)
+
+        self.label_dictionary = config.label_dictionary
+        self.set_class_weights(class_weights)
+
+    def remove_task_classifiers(self, tasks=None):
+        if tasks is None:
+            self.classifiers = nn.ModuleDict()
+            self.tasks = []
+            self.class_weights = {}
+        else:
+            for task in tasks:
+                self.classifiers.pop(task)
+                self.tasks.remove(task)
+                self.class_weights.pop(task)
+
+    def add_task_classifier(self, task_name: str, label_dictionary: Dict[str, List]):
+        self.tasks.append(task_name)
+        self.classifiers[task_name] = ClassificationHead(self.config, len(label_dictionary))
+        self.label_dictionary[task_name] = label_dictionary
 
+    def set_class_weights(self, class_weights: Optional[List[float]] = None):
         if class_weights is None:
-            self.class_weights = [None] * len(self.classifiers)
+            self.class_weights = {x: None for x in self.label_dictionary.keys()}
         else:
             self.class_weights = class_weights
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
@@ -349,52 +390,61 @@
         position_ids = position_ids.unsqueeze(0).expand_as(
             chunks_reps[:, :, 0]
         )  # (B, n_chunk)
         position_embeddings = self.encoder.embeddings.position_embeddings(
             position_ids
         )
         chunks_reps = chunks_reps + position_embeddings
+        chunks_attns = None
 
         # document encoding (B, n_chunk, hidden_size)
         for layer_ind, layer_module in enumerate(self.transformer):
-            chunks_reps, _ = layer_module(chunks_reps)
+            chunks_reps, chunks_attn = layer_module(chunks_reps)
+            if output_attentions:
+                if chunks_attns is None:
+                    chunks_attns = []
+                chunks_attns.append(chunks_attn)
 
             ## this case is mainly for when we are doing subsequent fine-tuning using a pre-trained
             ## hierarchical model and we want to check whether an earlier layer might provide better
             ## classification performance (e.g., if we think the last layer(s) are overfit to the pre-training
             ## objective) Just short circuit rather than doing the whole computation.
             if layer_ind+1 >= self.layer:
                 break
 
         if output_hidden_states:
             hidden_states = chunks_reps
 
         # extract first Documents as rep. (B, hidden_size)
         doc_rep = chunks_reps[:, 0, :]
 
-        total_loss = 0
-        for task_ind, task_num_labels in enumerate(self.num_labels):
-            if not self.class_weights[task_ind] is None:
-                class_weights = torch.FloatTensor(self.class_weights[task_ind]).to(self.device)
+        total_loss = None
+        for task_ind, task_name in enumerate(self.tasks):
+            if not self.class_weights[task_name] is None:
+                class_weights = torch.FloatTensor(self.class_weights[task_name]).to(self.device)
             else:
                 class_weights = None
             loss_fct = CrossEntropyLoss(weight=class_weights)
 
             # predict (B, 5)
-            task_logits = self.classifiers[task_ind](doc_rep)
+            task_logits = self.classifiers[task_name](doc_rep)
             logits.append(task_logits)
 
             if labels is not None:
                 task_labels = labels[:, task_ind]
                 task_loss = loss_fct(task_logits, task_labels.type(torch.LongTensor).to(labels.device))
-                total_loss += task_loss
-            
+                if total_loss is None:
+                    total_loss = task_loss
+                else:
+                    total_loss += task_loss
+
 
         if self.training:
-            return SequenceClassifierOutput(
+            return HierarchicalSequenceClassifierOutput(
                 loss=total_loss,
                 logits=logits,
                 hidden_states=outputs.hidden_states,
                 attentions=outputs.attentions,
+                chunk_attentions=chunks_attns,
             )
         else:
-            return SequenceClassifierOutput(loss=total_loss, logits=logits, hidden_states=hidden_states)
+            return HierarchicalSequenceClassifierOutput(loss=total_loss, logits=logits, hidden_states=hidden_states, attentions=outputs.attentions, chunk_attentions=chunks_attns)
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/api/cnlp_rest.py` & `cnlp-transformers-0.6.0/src/cnlpt/api/cnlp_rest.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,34 +29,32 @@
 
 class EntityDocument(BaseModel):
     ''' doc_text: The raw text of the document
     offset:  A list of entities, where each is a tuple of character offsets into doc_text for that entity'''
     doc_text: str
     entities: List[List[int]]
 
-def get_dataset(inst_list, tokenizer, label_lists, tasks, max_length: int = 128, hier: bool = False, chunk_len: int = 200, num_chunks: int = 40, insert_empty_chunk_at_beginning: bool = False,):
+def get_dataset(inst_list, tokenizer, max_length: int = 128, hier: bool = False, chunk_len: int = 200, num_chunks: int = 40, insert_empty_chunk_at_beginning: bool = False,):
     dataset = Dataset.from_dict({'text':inst_list})
     task_dataset = dataset.map(
                     cnlp_preprocess_data,
                     batched=True,
                     load_from_cache_file=False,
                     desc="Running tokenizer on dataset, organizing labels, creating hierarchical segments if necessary",
                     batch_size=100,
                     fn_kwargs = {
                         'tokenizer':tokenizer,
                         'max_length':max_length,
-                        'label_lists':label_lists,
                         'inference': True,
                         'hierarchical':hier,
                         # TODO: need to get this from the model if necessary
                         'chunk_len':chunk_len,
                         'num_chunks':num_chunks,
                         'insert_empty_chunk_at_beginning':insert_empty_chunk_at_beginning,
                         'truncate_examples': True,
-                        'tasks': tasks,
                 }
     )
     return task_dataset
 
 def create_instance_string(doc_text: str, offsets : List[int]):
     start = max(0, offsets[0]-100)
     end = min(len(doc_text), offsets[1]+100)
@@ -70,50 +68,40 @@
 
     app.state.training_args = training_args
 
     AutoConfig.register("cnlpt", CnlpConfig)
     AutoModel.register(CnlpConfig, CnlpModelForClassification)
 
     config = AutoConfig.from_pretrained(model_name)
+    app.state.config = config
     app.state.tokenizer = AutoTokenizer.from_pretrained(model_name,
                                                   config=config)
     model = CnlpModelForClassification.from_pretrained(model_name, cache_dir=os.getenv('HF_CACHE'), config=config)
     if cuda and not torch.cuda.is_available():
         logging.warning('CUDA is set to True (probably a default) but was not available; setting to False and proceeding. If you have a GPU you need to debug why pytorch cannot see it.')
         cuda = False
     
     if cuda:
         model = model.to('cuda')
     else:
         model = model.to('cpu')
 
+    app.state.model = model
     app.state.trainer = Trainer(
         model=model,
         args=app.state.training_args,
         compute_metrics=None,
     )
 
 def initialize_hier_model(app, model_name, cuda=True, batch_size=1):
     AutoConfig.register("cnlpt", CnlpConfig)
     AutoModel.register(CnlpConfig, HierarchicalModel)
 
     config: CnlpConfig = AutoConfig.from_pretrained(model_name)
-
-    encoder_dim = config.hidden_size
-
-    ## TODO (#122) - replace this with the transformer config when we fix that issue. just use defaults for now.
-    config.hier_head_config = dict(
-        n_layers=2,
-        d_model=encoder_dim,
-        d_inner=2048,
-        n_head=8,
-        d_k=8,
-        d_v=96,
-    )
-
+    app.state.config = config
     app.state.tokenizer = AutoTokenizer.from_pretrained(model_name,
                                                   config=config)
     
     model = AutoModel.from_pretrained(model_name, cache_dir=os.getenv('HF_CACHE'), config=config)
     model.train(False)
 
     if cuda and not torch.cuda.is_available():
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/api/dtr_rest.py` & `cnlp-transformers-0.6.0/src/cnlpt/api/dtr_rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     for ent_ind, offsets in enumerate(doc.entities):
         # logger.debug('Entity ind: %d has offsets (%d, %d)' % (ent_ind, offsets[0], offsets[1]))
         inst_str = create_instance_string(doc_text, offsets)
         logger.debug('Instance string is %s' % (inst_str))
         instances.append(inst_str)
 
-    dataset = get_dataset(instances, app.state.tokenizer, label_lists=[old_dtr_label_list], tasks=['dtr'], max_length=max_length)
+    dataset = get_dataset(instances, app.state.tokenizer, max_length=max_length)
 
     preproc_end = time()
 
     output = app.state.trainer.predict(test_dataset=dataset)
     predictions = output.predictions[0]
     predictions = np.argmax(predictions, axis=1)
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/api/event_rest.py` & `cnlp-transformers-0.6.0/src/cnlpt/api/event_rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     start_time = time()
 
     for sent_ind, token_list in enumerate(sents):
         inst_str = create_instance_string(token_list)
         logger.debug('Instance string is %s' % (inst_str))
         instances.append(inst_str)
 
-    dataset = get_dataset(instances, app.state.tokenizer, label_lists=[event_label_list], tasks=['event'], max_length=max_length)
+    dataset = get_dataset(instances, app.state.tokenizer, max_length=max_length)
     preproc_end = time()
 
     output = app.state.trainer.predict(test_dataset=dataset)
 
     event_predictions = np.argmax(output.predictions[0], axis=2)
 
     pred_end = time()
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/api/hier_rest.py` & `cnlp-transformers-0.6.0/src/cnlpt/api/hier_rest.py`

 * *Files 24% similar despite different names*

```diff
@@ -37,24 +37,37 @@
 @app.on_event("startup")
 async def startup_event():
     initialize_hier_model(app, model_name=model_name)
 
 @app.post("/hier/get_rep")
 async def get_representation(doc: UnannotatedDocument):
     instances = [doc.doc_text]
-    dataset = get_dataset(instances, app.state.tokenizer, label_lists=[], tasks=['fyler-pretraining'], max_length=8000, hier=True, chunk_len=200, num_chunks=40, insert_empty_chunk_at_beginning=False)
+    dataset = get_dataset(instances, app.state.tokenizer, max_length=16000, hier=True, chunk_len=200, num_chunks=80, insert_empty_chunk_at_beginning=False)
     result = app.state.model.forward(input_ids=torch.LongTensor(dataset['input_ids']).to('cuda'),
                                      token_type_ids=torch.LongTensor(dataset['token_type_ids']).to('cuda'),
                                      attention_mask = torch.LongTensor(dataset['attention_mask']).to('cuda'),
                                      output_hidden_states=True)
     
     # Convert to a list so python can send it out
     hidden_states = result['hidden_states'].to('cpu').detach().numpy()[:,0,:].tolist()
     return {'reps': hidden_states[0]}
 
+@app.post("/hier/classify")
+async def classify(doc: UnannotatedDocument):
+    instances = [doc.doc_text]
+    dataset = get_dataset(instances, app.state.tokenizer, max_length=16000, hier=True, chunk_len=200, num_chunks=80, insert_empty_chunk_at_beginning=False)
+    result = app.state.model.forward(input_ids=torch.LongTensor(dataset['input_ids']).to('cuda'),
+                                     token_type_ids=torch.LongTensor(dataset['token_type_ids']).to('cuda'),
+                                     attention_mask = torch.LongTensor(dataset['attention_mask']).to('cuda'),
+                                     output_hidden_states=False)
+    
+    predictions = [int(torch.argmax(logits.to('cpu').detach()).numpy()) for logits in result['logits']]
+    labels = [list(app.state.model.label_dictionary.values())[0][x] for x in predictions]
+    return {'result': labels}
+
 def rest():
     import argparse
 
     parser = argparse.ArgumentParser(description='Run the http server for serving hierarchical model outputs.')
     parser.add_argument('-p', '--port', type=int, help='The port number to run the server on', default=8000)
     args = parser.parse_args()
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/api/negation_rest.py` & `cnlp-transformers-0.6.0/src/cnlpt/api/negation_rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ..CnlpModelForClassification import CnlpModelForClassification, CnlpConfig
 import numpy as np
 
 import logging
 from time import time
 
 app = FastAPI()
-model_name = "tmills/cnlpt-negation-roberta-sharpseed"
+model_name = "mlml-chip/negation_pubmedbert_sharpseed"
 logger = logging.getLogger('Negation_REST_Processor')
 logger.setLevel(logging.DEBUG)
 
 task = 'Negation'
 labels = [-1, 1]
 
 max_length = 128
@@ -56,15 +56,15 @@
 
     for ent_ind, offsets in enumerate(doc.entities):
         # logger.debug('Entity ind: %d has offsets (%d, %d)' % (ent_ind, offsets[0], offsets[1]))
         inst_str = create_instance_string(doc_text, offsets)
         logger.debug('Instance string is %s' % (inst_str))
         instances.append(inst_str)
 
-    dataset = get_dataset(instances, app.state.tokenizer, [labels,], [task,], max_length)
+    dataset = get_dataset(instances, app.state.tokenizer, max_length)
     preproc_end = time()
 
 
     output = app.state.trainer.predict(test_dataset=dataset)
     predictions = output.predictions[0]
     predictions = np.argmax(predictions, axis=1)
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/api/temporal_rest.py` & `cnlp-transformers-0.6.0/src/cnlpt/api/temporal_rest.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from ..CnlpModelForClassification import CnlpModelForClassification, CnlpConfig
 from seqeval.metrics.sequence_labeling import get_entities
 import logging
 from time import time
 from nltk.tokenize import wordpunct_tokenize as tokenize
 
 app = FastAPI()
-model_name = "tmills/thyme1-e2e"
+model_name = "mlml-chip/thyme2_colon_e2e"
 logger = logging.getLogger('Temporal_REST_Processor')
 logger.setLevel(logging.INFO)
 
 labels = ["-1", "1"]
 timex_label_list = ["O", "B-DATE","B-DURATION","B-PREPOSTEXP","B-QUANTIFIER","B-SET","B-TIME","B-SECTIONTIME","B-DOCTIME",
                     "I-DATE","I-DURATION","I-PREPOSTEXP","I-QUANTIFIER","I-SET","I-TIME","I-SECTIONTIME","I-DOCTIME"]
 timex_label_dict = { val:ind for ind,val in enumerate(timex_label_list)}
@@ -42,15 +42,14 @@
 
 relation_label_list = ['None', 'CONTAINS', 'OVERLAP', 'BEFORE', 'BEGINS-ON', 'ENDS-ON']
 relation_label_dict = { val:ind for ind,val in enumerate(relation_label_list)}
 
 dtr_label_list = ["AFTER", "BEFORE", "BEFORE/OVERLAP", "OVERLAP"]
 old_dtr_label_list = ["BEFORE", "OVERLAP", "BEFORE/OVERLAP", "AFTER"]
 
-tasks = ['timex', 'event', 'tlinkx']
 labels = [ timex_label_list, event_label_list, relation_label_list]
 max_length = 128
 
 class SentenceDocument(BaseModel):
     sentence: str
 
 class TokenizedSentenceDocument(BaseModel):
@@ -85,15 +84,54 @@
 
 
 def create_instance_string(tokens: List[str]):
     return ' '.join(tokens)
 
 @app.on_event("startup")
 async def startup_event():
-    initialize_cnlpt_model(app, model_name)
+    global timex_label_list, timex_label_dict, event_label_list, event_label_dict, relation_label_list, relation_label_dict, task_order
+
+    local_model_name = os.getenv('MODEL_NAME', model_name)
+    initialize_cnlpt_model(app, local_model_name)
+
+    config_dict = app.state.trainer.model.config.to_dict()
+    # For newer models (version >= 0.6.0), the label dictionary is saved with the model
+    # config. we can look for it to preserve backwards compatibility for now but
+    # should eventually remove the hardcoded label lists from our inference tools.
+    label_dict = config_dict.get('label_dictionary', None)
+    if label_dict is not None:
+        # some older versions have one label dictionary per dataset, future versions should just
+        # have a task-keyed dictionary
+        if type(label_dict) == list:
+            label_dict = label_dict[0]
+        
+        if 'event' in label_dict:
+            event_label_list = label_dict['event']
+            event_label_dict = { val:ind for ind,val in enumerate(event_label_list)}
+            print(event_label_list)
+        
+        if 'timex' in label_dict:
+            timex_label_list = label_dict['timex']
+            timex_label_dict = { val:ind for ind,val in enumerate(timex_label_list)}
+            print(timex_label_list)
+
+        if 'tlinkx' in label_dict:
+            relation_label_list = label_dict['tlinkx']
+            relation_label_dict = { val:ind for ind,val in enumerate(relation_label_list)}
+            print(relation_label_list)
+
+    app.state.tasks = config_dict.get('finetuning_task', None)
+    app.state.task_order = {}
+    if app.state.tasks is not None:
+        print("Overwriting finetuning task order")
+        for task_ind, task_name in enumerate(app.state.tasks):
+            app.state.task_order[task_name] = task_ind
+        print(app.state.task_order)
+    else:
+        print("Didn't find a new task ordering in the model config")
 
 @app.post("/temporal/process")
 async def process(doc: TokenizedSentenceDocument):
     return process_tokenized_sentence_document(doc)
 
 @app.post("/temporal/process_sentence")
 async def process_sentence(doc: SentenceDocument):
@@ -101,32 +139,37 @@
     doc = TokenizedSentenceDocument(sent_tokens=[tokenized_sent,], metadata='Single sentence')
     return process_tokenized_sentence_document(doc)
 
 def process_tokenized_sentence_document(doc: TokenizedSentenceDocument):
     sents = doc.sent_tokens
     metadata = doc.metadata
 
+    print(event_label_list)
+    print(timex_label_list)
+    print(relation_label_list)
+
     logger.warn('Received document labeled %s with %d sentences' % (metadata, len(sents)))
     instances = []
     start_time = time()
 
     for sent_ind, token_list in enumerate(sents):
         inst_str = create_instance_string(token_list)
         logger.debug('Instance string is %s' % (inst_str))
         instances.append(inst_str)
 
-    dataset = get_dataset(instances, app.state.tokenizer, labels, tasks, max_length)
+    dataset = get_dataset(instances, app.state.tokenizer, max_length)
     preproc_end = time()
 
     output = app.state.trainer.predict(test_dataset=dataset)
 
-    timex_predictions = np.argmax(output.predictions[0], axis=2)
-    event_predictions = np.argmax(output.predictions[1], axis=2)
-    rel_predictions = np.argmax(output.predictions[2], axis=3)
-    rel_inds = np.where(rel_predictions > 0)
+    timex_predictions = np.argmax(output.predictions[app.state.task_order['timex']], axis=2)
+    event_predictions = np.argmax(output.predictions[app.state.task_order['event']], axis=2)
+    rel_predictions = np.argmax(output.predictions[app.state.task_order['tlinkx']], axis=3)
+    rel_inds = np.where(rel_predictions != relation_label_dict["None"])
+
     logging.debug('Found relation indices: %s' % (str(rel_inds)))
 
     rels_by_sent = {}
     for rel_num in range(len(rel_inds[0])):
         sent_ind = rel_inds[0][rel_num]
         if not sent_ind in rels_by_sent:
             rels_by_sent[sent_ind] = []
@@ -162,15 +205,21 @@
             if word_idx != previous_word_idx and word_idx is not None:
                 key = word_pos_idx
                 val = len(wpind_to_ind)
 
                 wpind_to_ind[key] = val
                 # tokeni_to_wpi[val] = key
                 timex_labels.append(timex_label_list[timex_predictions[sent_ind][word_pos_idx]])
-                event_labels.append(event_label_list[event_predictions[sent_ind][word_pos_idx]])
+                try:
+                    event_labels.append(event_label_list[event_predictions[sent_ind][word_pos_idx]])
+                except:
+                    print('exception thrown when sent_ind=%d and word_pos_idx=%d' %( sent_ind, word_pos_idx))
+                    print('prediction is %s' % str(event_predictions[sent_ind][word_pos_idx]))
+                    raise Exception
+                
             previous_word_idx = word_idx
 
         timex_entities = get_entities(timex_labels)
         logging.info("Extracted %d timex entities from the sentence" % (len(timex_entities)))
         timex_results.append( [Timex(timeClass=label[0], begin=label[1], end=label[2]) for label in timex_entities] )
 
         event_entities = get_entities(event_labels)
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/api/timex_rest.py` & `cnlp-transformers-0.6.0/src/cnlpt/api/timex_rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     start_time = time()
 
     for sent_ind, token_list in enumerate(sents):
         inst_str = create_instance_string(token_list)
         logger.debug('Instance string is %s' % (inst_str))
         instances.append(inst_str)
 
-    dataset = get_dataset(instances, app.state.tokenizer, label_lists=[timex_label_list], tasks=['timex'], max_length=max_length)
+    dataset = get_dataset(instances, app.state.tokenizer, max_length=max_length)
     logger.warn('Dataset is as follows: %s' % (str(dataset.features)))
 
     preproc_end = time()
 
     output = app.state.trainer.predict(test_dataset=dataset)
 
     timex_predictions = np.argmax(output.predictions[0], axis=2)
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/cnlp_data.py` & `cnlp-transformers-0.6.0/src/cnlpt/cnlp_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 
 from filelock import FileLock
 from typing import Callable, Dict, Optional, List, Union, Tuple
 
 import numpy as np
 import torch
 from torch.utils.data.dataset import Dataset
-from transformers import BatchEncoding
-# from transformers.data.processors.utils import DataProcessor, InputExample
+from transformers import BatchEncoding, InputExample
 from transformers.tokenization_utils import PreTrainedTokenizer
 from datasets import Features
 from dataclasses import dataclass, field, asdict, astuple
+import datasets
 from enum import Enum
 
 from .cnlp_processors import classification, tagging, relex, mtl, AutoProcessor
 
 special_tokens = ['<e>', '</e>', '<a1>', '</a1>', '<a2>', '</a2>', '<cr>', '<neg>']
+text_columns = ['text', 'text_a', 'text_b']
+none_column = '__None__'
 
 logger = logging.getLogger(__name__)
 
 def list_field(default=None, metadata=None):
     return field(default_factory=lambda: default, metadata=metadata)
 
 class Split(Enum):
@@ -106,24 +108,23 @@
         # pad_token_segment_id=0,
         # use_special_token=True,
 ) -> BatchEncoding:
     """
     Chunk an instance of InputFeatures into an instance of HierarchicalInputFeatures
     for the hierarchical model.
 
-    :param BatchEncoding features: the dictionary containing mappings from properties to lists of values for each instance for each of those properties
-    :param int chunk_len: the maximum length of a chunk
-    :param int num_chunks: the maximum number of chunks in the instance
-    :param int cls_id: the tokenizer's ID representing the CLS token
-    :param int sep_id: the tokenizer's ID representing the SEP token
-    :param int pad_id: the tokenizer's ID representing the PAD token
-    :param bool insert_empty_chunk_at_beginning: whether to insert an
+    :param features: the dictionary containing mappings from properties to lists of values for each instance for each of those properties
+    :param chunk_len: the maximum length of a chunk
+    :param num_chunks: the maximum number of chunks in the instance
+    :param cls_id: the tokenizer's ID representing the CLS token
+    :param sep_id: the tokenizer's ID representing the SEP token
+    :param pad_id: the tokenizer's ID representing the PAD token
+    :param insert_empty_chunk_at_beginning: whether to insert an
         empty chunk at the beginning of the instance
-    :rtype: HierarchicalInputFeatures
-    :return: an instance of `HierarchicalInputFeatures` containing the chunked instance
+    :return: an instance of :class:`transformers.BatchEncoding` containing the chunked instance
     """
 
     for ind in range(len(features['input_ids'])):
         # Get feature variables
         # input_ids_, attention_mask_, token_type_ids_, event_tokens_, label_ = astuple(features)
         input_ids_ = features['input_ids'][ind]
         attention_mask_ = features['attention_mask'][ind]
@@ -227,15 +228,15 @@
             features['token_type_ids'][ind] = chunks_token_type_ids
         features['event_mask'][ind] = chunks_event_tokens
 
     return features
 
 
 def cnlp_preprocess_data(
-    examples,
+    examples: List[InputExample],
     tokenizer: PreTrainedTokenizer,
     max_length: Optional[int] = None,
     tasks: List[str] = None,
     label_lists: Optional[Dict[str,List[str]]] = None,
     output_modes: Optional[Dict[str,str]] = None,
     inference: bool = False,
     hierarchical: bool = False,
@@ -246,52 +247,53 @@
 ) -> Union[List[InputFeatures], List[HierarchicalInputFeatures]]:
     """
     Processes the list of :class:`transformers.InputExample` generated by
     the processor defined in :data:`cnlpt.cnlp_processors.cnlp_processors`
     and converts the examples into a list of :class:`InputFeatures` or
     :class:`HierarchicalInputFeatures`, depending on the model.
 
-    :param typing.List[transformers.data.processors.utils.InputExample] examples:
+    :param examples:
         the list of examples to convert
-    :param transformers.tokenization_utils.PreTrainedTokenizer tokenizer: the tokenizer
-    :param typing.Optional[int] max_length: the maximum sequence length
+    :param tokenizer: the tokenizer
+    :param max_length: the maximum sequence length
         at which to truncate examples
-    :param List[str] tasks: the task name(s) in a list, used to index the labels in the examples list.
-    :param typing.Optional[typing.Dict[str,List[str]]] label_list: a mapping from 
+    :param tasks: the task name(s) in a list, used to index the labels in the examples list.
+    :param label_list: a mapping from
         tasks to the list of labels for each task. If not provided explicitly, it will be retrieved from
         the processor with :meth:`transformers.DataProcessor.get_labels`.
-    :param typing.Optional[Dict[str,str]] output_modes: the output modes for this task.
+    :param output_modes: the output modes for this task.
         If not provided explicitly, it will be retrieved from
         :data:`cnlpt.cnlp_processors.cnlp_output_modes`.
-    :param bool inference: whether we're doing training or inference only -- if inference mode the labels associated with examples can't be trusted.
-    :param bool hierarchical: whether to structure the data for the hierarchical
+    :param inference: whether we're doing training or inference only -- if inference mode the labels associated with examples can't be trusted.
+    :param hierarchical: whether to structure the data for the hierarchical
         model (:class:`cnlpt.HierarchicalTransformer.HierarchicalModel`)
-    :param int chunk_len: for the hierarchical model, the length of each
+    :param chunk_len: for the hierarchical model, the length of each
         chunk in tokens
-    :param int num_chunks: for the hierarchical model, the number of chunks
-    :param bool insert_empty_chunk_at_beginning: for the hierarchical model,
+    :param num_chunks: for the hierarchical model, the number of chunks
+    :param insert_empty_chunk_at_beginning: for the hierarchical model,
         whether to insert an empty chunk at the beginning of the list of chunks
         (equivalent in theory to a CLS chunk).
-    :param bool truncate_examples: whether to truncate the string representation
+    :param truncate_examples: whether to truncate the string representation
         of the example instances printed to the log
-    :rtype: typing.Union[typing.List[InputFeatures], typing.List[HierarchicalInputFeatures]]
     :return: the list of converted input features
     """
     
     if max_length is None:
         max_length = tokenizer.max_len
 
     # Try to infer the structure based on column names
     if 'text' in examples.keys():
         sentences = [example.split(' ') for example in examples['text']]
         num_instances = len(examples['text'])
     elif 'text_b' in examples.keys():
         # FIXME - not sure if this is right but doesn't get used much in our data
         raise NotImplementedError("2-sentence classification has not been re-implemented yet.")
         sentences = (examples['text_a'], examples['text_b'])        
+    else:
+        raise Exception('The data does not seem to have a text column (literally a column labeled "text" is required)')
     
     if hierarchical:
         padding = False
     else:
         padding = 'max_length'
 
     result = tokenizer(
@@ -304,15 +306,19 @@
 
     # Now that we have the labels for each instances, and we've tokenized the input sentences, 
     # we need to solve the problem of aligning labels with word piece indexes for the tasks of tagging
     # (which has one label per pre-wordpiece token) and relations (which are defined as tuples which
     # contain pre-wordpiece token indices)
     if not inference:
         # Create a label map for each task in this dataset: { task1 => {label_0: 0, label_1: 1, label_2:, 2}, task2 => {label_0: 0, label_1:1} }
-        label_map = {task: {label: i for i, label in enumerate(label_lists[task])} for task in tasks}
+        label_map = {task: {label: i for i, label in enumerate(label_lists[task])} for task in label_lists.keys()}
+        for task in tasks:
+            if none_column in label_map[task]:
+                raise Exception("There is a column named %s which is a reserved name" % (none_column))
+            label_map[task][none_column] = -100
 
         raw_labels = []
         labels = []
 
         # Create a list of mapped labels for every task in this dataset, with different mapping tactics for different types,
         # classification vs tagging vs. relations.
         for task_ind,task in enumerate(tasks):
@@ -323,15 +329,15 @@
                 task_labels = [label_map[task][label] for label in raw_labels[task_ind]]
                 # labels is just a list of one label for each instance
             elif output_modes[task] == tagging:
                 task_labels = [ [label_map[task][label] for label in inst_labels.split()] for inst_labels in raw_labels[task_ind]]
                 # labels is a list of lists, where each internal list is the set of tags for that instance.
             elif output_modes[task] == relex:
                 for inst_rels in raw_labels[task_ind]:
-                    if inst_rels == 'None':
+                    if inst_rels is None or inst_rels == 'None':
                         task_labels.append(['None'])
                     else:
                         # The label for a sentence with multiple relations looks like this:
                         # (105,109,OVERLAP) , (64,66,CONTAINS) , (100,105,CONTAINS) , (81,88,CONTAINS) , (81,95,CONTAINS) , (105,106,OVERLAP) , (81,100,CONTAINS)
                         # Split into relations, then remove parens and split with commas into relation components (start offset, end offset, category)
                         inst_labels = []
                         for rel in inst_rels.split(' , '):
@@ -364,29 +370,45 @@
             pad_id=tokenizer.pad_token_id,
             insert_empty_chunk_at_beginning=insert_empty_chunk_at_beginning,
         )
 
     return result
 
 def _build_pytorch_labels(result:BatchEncoding, tasks:List[str], labels:List, output_modes:Dict[str,str], num_instances:int, max_length:int, label_lists: List[List[str]]):
+    '''
+    _build_pytorch_labels: we do two things here: map from labels in input space to ints in a softmax, and in a data
+    structure that can contain multiple task types such that the Trainer class will be happy with, and then that
+    the model.forward() can unpack easily to do the loss calculations.
+    '''
     labels_out = []
+
+    pad_classification = False
+    if relex in output_modes.values() or tagging in output_modes.values():
+        # we have tagging as the highest dimensional output
+        max_dims = 2
+        if classification in output_modes.values():
+            pad_classification = True
+    else:
+        # classification only
+        max_dims = 1
+
     for task_ind, task in enumerate(tasks):
         encoded_labels = []
         if output_modes[task] == tagging:
             for sent_ind in range(num_instances):
                 sent_labels = []
 
                 ## align word-piece tokens to the tokenization we got as input and only assign labels to input tokens
                 word_ids = result.word_ids(batch_index=sent_ind)
                 previous_word_idx = None
                 label_ids = []
                 for word_idx in word_ids:
                     # Special tokens have a word id that is None. We set the label to -100 so they are automatically
-                    # ignored in the loss function.
-                    if word_idx is None:
+                    # ignored in the loss function. Non-tagging tasks will be labeled as [-100], all label ids are -100
+                    if word_idx is None or labels[sent_ind][task_ind] == [-100]:
                         label_ids.append(-100)
                     # We set the label for the first token of each word.
                     elif word_idx != previous_word_idx:
                         label_ids.append(labels[sent_ind][task_ind][word_idx])
                     # For the other tokens in a word, we set the label to either the current label or -100, depending on
                     # the label_all_tokens flag.
                     else:
@@ -440,30 +462,44 @@
                     wpi2 = tokeni_to_wpi[label[1]]
 
                     sent_labels[wpi1][wpi2] = label[2]
 
                 encoded_labels.append(sent_labels)
             labels_out.append(encoded_labels)
             if out_of_bounds > 0:
-                logging.warn(
+                logger.warn(
                     'During relation processing, there were %d relations (out of %d total relations) where at least one argument was truncated so the relation could not be trained/predicted.' % (out_of_bounds, num_relations)
                 )
                 
         elif output_modes[task] == classification:
-            for sent_ind in range(num_instances):
-                encoded_labels.append( (labels[sent_ind][task_ind],) )
+            for inst_ind in range(num_instances):
+                # if we try to combine classification with tagging/relex, we end up with non-rectangular label
+                # arrays. so we need to pad out the classification target to be the length of the sequence
+                # so that we can concatenate it. we'll have to account for this in the forward() and in the
+                # compute metrics code as well.
+                if pad_classification:
+                    padded_inst = np.zeros( (max_length,1) ) - 100
+                    padded_inst[0] = labels[inst_ind][task_ind]
+                    encoded_labels.append( padded_inst )
+                else:
+                    encoded_labels.append(labels[inst_ind][task_ind])
             labels_out.append(np.array(encoded_labels))
     
     labels_unshaped =  list(zip(*labels_out))
     labels_shaped = []
+    
     for ind in range(len(labels_unshaped)):
-        if labels_unshaped[ind][0].ndim == 2:
+        if max_dims == 2:
+            ## relations or tagging and possibly classification too
             labels_shaped.append( np.concatenate( labels_unshaped[ind], axis=1 ) )
-        elif labels_unshaped[ind][0].ndim == 1:
-            labels_shaped.append( np.concatenate( labels_unshaped[ind], axis=0 ) )
+        elif max_dims == 1:
+            ## classification only
+            labels_shaped.append( labels_unshaped[ind] )
+        else:
+            raise Exception('This should not be possible that max_dims > 2.')
     
     return labels_shaped
 
 def _build_event_mask(result:BatchEncoding, num_insts:int, event_start_token_id, event_end_token_id):
 
     event_tokens = []
     for i in range(num_insts):
@@ -483,21 +519,19 @@
         else:
             inst_event_tokens = [1] * len(input_ids)
 
         event_tokens.append(inst_event_tokens)
 
     return event_tokens
 
-def truncate_features(feature: Union[InputFeatures, HierarchicalInputFeatures]):
+def truncate_features(feature: Union[InputFeatures, HierarchicalInputFeatures]) -> str:
     """
     Method to produce a truncated string representation of a feature.
 
-    :param typing.Union[InputFeatures, HierarchicalInputFeatures] feature:
-        the feature to represent
-    :rtype: str
+    :param feature: the feature to represent
     :return: the truncated representation of the feature
     :meta private:
     """
     return (
         f"{feature.__class__.__name__}"
         "("
         f"input_ids={summarize(feature.input_ids)}, "
@@ -591,21 +625,21 @@
 
 
 class ClinicalNlpDataset(Dataset):
     """
     Copy-pasted from GlueDataset with glue task-specific code changed;
     moved into here to be self-contained.
 
-    :param DataTrainingArguments args: the data training args for this experiment
-    :param transformers.tokenization_utils.PreTrainedTokenizer tokenizer: the tokenizer
-    :param typing.Optional[int] limit_length: if provided, the number of
+    :param args: the data training args for this experiment
+    :param tokenizer: the tokenizer
+    :param limit_length: if provided, the number of
         examples to include in the dataset
-    :param typing.Optional[str] cache_dir: if provided, the directory to save/load a cache
+    :param cache_dir: if provided, the directory to save/load a cache
         of this dataset
-    :param bool hierarchical: whether to structure the data for the hierarchical
+    :param hierarchical: whether to structure the data for the hierarchical
         model (:class:`cnlpt.HierarchicalTransformer.HierarchicalModel`)
     """
     args: DataTrainingArguments
     features: List[InputFeatures]
 
     def __init__(
         self,
@@ -613,90 +647,184 @@
         tokenizer: PreTrainedTokenizer,
         limit_length: Optional[int] = None,
         cache_dir: Optional[str] = None,
         hierarchical: bool = False,
     ):
         self.args = args
         self.processors = []
-        self.class_weights = []
-        self.label_lists = []
+        self.class_weights = None
+        self.tasks_to_labels = {}
         self.hierarchical = hierarchical
-        self.features = None
         self.datasets = []
+        self.processed_dataset = []
+        self.output_modes = {}
 
         # Load data features from cache or dataset file
         self.label_lists = []
         self.num_train_instances = 0
 
         if self.hierarchical:
             implicit_max_len = self.args.chunk_len * self.args.num_chunks
             if self.args.max_seq_length < implicit_max_len:
                 raise ValueError('For the hierarchical model, the max seq length should be equal to the chunk length * num_chunks, otherwise what is the point?')
 
-        tasks = None if args.task_name is None else set(args.task_name)
+        # if cli supplies no tasks, the processor will assume we want all the tasks, but we do need to have a conventional order
+        # for the model to use, so we need to still create a tasks variable.
+        tasks = None if args.task_name is None else list(args.task_name)
         for data_dir_ind, data_dir in enumerate(args.data_dir):
             dataset_processor = AutoProcessor(data_dir, tasks, max_train_items=args.max_train_items)
             self.processors.append(dataset_processor)
             
-            ## TODO get this working again
-            for classifier in range(dataset_processor.get_num_tasks()):
-                self.class_weights.append(None)
-
-
-            num_subtasks = dataset_processor.get_num_tasks()
-            self.label_lists.append(dataset_processor.get_labels())
-            task_dataset = dataset_processor.dataset.map(
-                cnlp_preprocess_data,
-                batched=True,
-                load_from_cache_file=not args.overwrite_cache,
-                desc="Running tokenizer on dataset, organizing labels, creating hierarchical segments if necessary",
-                batch_size=100,
-                fn_kwargs = {
-                    'tokenizer':tokenizer,
-                    'max_length':args.max_seq_length,
-                    'label_lists':self.label_lists[data_dir_ind],
-                    'output_modes':dataset_processor.get_output_modes(),
-                    'inference': not 'train' in dataset_processor.dataset,
-                    'hierarchical':self.hierarchical,
-                    'chunk_len':self.args.chunk_len,
-                    'num_chunks':self.args.num_chunks,
-                    'insert_empty_chunk_at_beginning':self.args.insert_empty_chunk_at_beginning,
-                    'truncate_examples':self.args.truncate_examples,
-                    'tasks': dataset_processor.get_classifiers(),
-                }
-            )
+            # Make sure that any overlapping task names have the same label sets and output mode definitions
+            self._reconcile_labels_lists(dataset_processor)
+            self._reconcile_output_modes(dataset_processor)
+
+            self.datasets.append(dataset_processor.dataset)
+
+        ## Each processed dataset will have been pruned to remove columns that the user _didn't_ ask for,
+        ## but we need to add columns for tasks that it doesn't have that the user did ask for, with the 
+        ## appropriate task types and  special values so pytorch knows not to compute losses over those 
+        ## tasks for those inputs. Need to  do that after we've read all datasets and inferred all the task 
+        ## types and label spaces.
+        self._reconcile_columns()
+        combined_dataset = self._concatenate_datasets()
+
+        if tasks is None:
+            # i.e., cli did not supply any task ordering:
+            if 'train' in combined_dataset:
+                split = 'train'
+            elif 'dev' in combined_dataset:
+                split = 'dev'
+            else:
+                split = 'test'
 
-            if args.max_eval_items > 0:
-                new_validation = task_dataset['validation'].train_test_split(test_size=args.max_eval_items)['test']
-                task_dataset['validation'] = new_validation
+            tasks = list(combined_dataset[split].features.keys() - {'text', 'text_a', 'text_b'})
 
-            self.datasets.append(task_dataset)
-            self.num_train_instances += task_dataset['train'].num_rows
+        self.tasks = tasks
+        
+        self.processed_dataset = combined_dataset.map(
+            cnlp_preprocess_data,
+            batched=True,
+            load_from_cache_file=not args.overwrite_cache,
+            desc="Running tokenizer on dataset, organizing labels, creating hierarchical segments if necessary",
+            batch_size=100,
+            fn_kwargs = {
+                'tokenizer':tokenizer,
+                'max_length':args.max_seq_length,
+                'label_lists':self.tasks_to_labels,
+                'output_modes':self.output_modes,
+                'inference': not 'train' in combined_dataset,
+                'hierarchical':self.hierarchical,
+                'chunk_len':self.args.chunk_len,
+                'num_chunks':self.args.num_chunks,
+                'insert_empty_chunk_at_beginning':self.args.insert_empty_chunk_at_beginning,
+                'truncate_examples':self.args.truncate_examples,
+                'tasks': tasks,
+            }
+        )
+
+        if args.max_eval_items > 0:
+            new_validation = self.processed_dataset['validation'].train_test_split(test_size=args.max_eval_items)['test']
+            self.processed_dataset['validation'] = new_validation
+
+        self.num_train_instances += self.processed_dataset['train'].num_rows
+
+    def _reconcile_labels_lists(self, processor):
+        '''
+        given a new data processor, which extracted a label list for every task it contained,
+        we reconcile it with existing label list for the same task
+        '''
+        for task,labels in processor.get_labels().items():
+            if task in self.tasks_to_labels:
+                ## a subset of existing labels (WARN), superset of existing labels (WARN), mixture, or no overlap (ERROR)
+                new_labels = set(labels)
+                old_labels = set(self.tasks_to_labels[task])
+                if new_labels.isdisjoint(old_labels):
+                    raise Exception("The same task name has disjoint sets of labels in different dataset: %s vs. %s" % (str(old_labels), str(new_labels)))
+                elif new_labels != old_labels:
+                    logger.warn("Two different datasets have the same task name but not completely equal label lists: %s vs. %s. We will merge them." % (str(old_labels), str(new_labels)))
+                    self.tasks_to_labels[task] = old_labels.union(new_labels)
+                else:
+                    ## they match completely, nothing to be done
+                    pass
+            else:
+                self.tasks_to_labels[task] = labels
+    
+    def _reconcile_output_modes(self, processor):
+        '''
+        given a new data processor, which inferred output modes for its tasks, make
+        sure those output modes agree with existing inferred output modes for any
+        same-named tasks.
+        '''
+        for task,output_mode in processor.get_output_modes().items():
+            if task in self.output_modes:
+                # There is an existing task with this name
+                existing_output_mode = self.output_modes[task]
+                if output_mode != existing_output_mode:
+                    raise Exception("The task %s has two different output modes in different datasets and might not be the same task: %s vs. %s" % (task, existing_output_mode, output_mode))
+            else:
+                self.output_modes[task] = output_mode
 
+    def _reconcile_columns(self):
+        '''
+        The overall dataset should get the superset of all task columns, even if some of the tasks aren't in
+        all of the component datasets
+        '''
+        tasks = self.tasks_to_labels.keys()
+
+        for dataset in self.datasets:
+            for split_name in dataset.keys():
+                for task in tasks:
+                    if task not in dataset[split_name].column_names:
+                        if self.output_modes[task] == tagging:
+                            dataset[split_name] = dataset[split_name].add_column(task, [none_column] * len(dataset[split_name]))
+                        elif self.output_modes[task] == relex:
+                            pass
+                        elif self.output_modes[task] == classification:
+                            dataset[split_name] = dataset[split_name].add_column(task, [none_column] * len(dataset[split_name]))
+
+
+                for column in dataset[split_name].column_names:
+                    if column not in tasks and column not in text_columns:
+                        dataset[split_name] = dataset[split_name].remove_columns(column)
+
+    def _concatenate_datasets(self):
+        """
+        We have multiple dataset dicts, we need to create a single dataset dict
+        where we concatenate each of the splits first.
+        """
+        datasets_by_split = {}
+        for dataset in self.datasets:
+            for split in dataset:
+                if split not in datasets_by_split:
+                    datasets_by_split[split] = []
+                datasets_by_split[split].append(dataset[split])
+        
+        for split_name, split_data in datasets_by_split.items():
+            datasets_by_split[split_name] = datasets.concatenate_datasets(split_data)
+        
+        return datasets.DatasetDict(datasets_by_split)
 
     def __len__(self) -> int:
         """
         Length method for this class.
 
-        :rtype: int
-        :return: the number of instances in the dataset
+        :return: the number of datasets included in this dataset
         """
-        return len(self.features)
+        return len(self.datasets)
 
-    def __getitem__(self, i):
+    def __getitem__(self, i) -> Union[InputFeatures, HierarchicalInputFeatures]:
         """
         Getitem method for this class.
 
         :param i: the index of the example to retrieve
-        :rtype: typing.Union[InputFeatures, HierarchicalInputFeatures]
         :return: the example at index `i`
         """
         return self.features[i]
 
-    def get_labels(self):
+    def get_labels(self) -> Dict[str, List[str]]:
         """
         Retrieve the label lists for all the tasks for the dataset.
 
-        :rtype: typing.List[typing.List[str]]
-        :return: the list of label lists
+        :return: the dictionary of label lists indexed by task name
         """
-        return self.label_lists
+        return self.tasks_to_labels
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/cnlp_metrics.py` & `cnlp-transformers-0.6.0/src/cnlpt/cnlp_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
+from typing import Set, Any, Dict
+
 import numpy as np
 from sklearn.metrics import matthews_corrcoef, f1_score, recall_score, precision_score, classification_report, accuracy_score
 from seqeval.metrics import f1_score as seq_f1, classification_report as seq_cls
 from .cnlp_processors import classification, mtl, tagging, relex
-
+from .cnlp_data import ClinicalNlpDataset
 
 logger = logging.getLogger(__name__)
 
 def fix_np_types(input_variable):
     """
     In the mtl classification setting, f1 is an array, and when the HF library
     tries to write out the training history to a json file it will throw an error.
@@ -16,15 +18,20 @@
     :meta private:
     """
     if isinstance(input_variable, np.ndarray):
         return list(input_variable)
     
     return input_variable
 
-def tagging_metrics(processor, preds, labels, task_name):
+def tagging_metrics(
+    label_set: Set[str],
+    preds: np.ndarray,
+    labels: np.ndarray,
+    task_name: str,
+) -> Dict[str, Any]:
     """
     One of the metrics functions for use in :func:`cnlp_compute_metrics`.
 
     Generates evaluation metrics for sequence tagging tasks.
 
     Ignores tags for which the true label is -100.
 
@@ -33,22 +40,20 @@
         {
             'acc': accuracy
             'token_f1': token-wise F1 score
             'f1': seqeval F1 score
             'report': seqeval classification report
         }
 
-    :param DataProcessor processor: the data processor that was used to read in the data files
-    :param numpy.ndarray preds: the predicted labels from the model
-    :param numpy.ndarray labels: the true labels
-    :rtype: typing.Dict[str, typing.Any]
+    :param label_set: The set of labels for this task
+    :param preds: the predicted labels from the model
+    :param labels: the true labels
+    :param task_name: the name of the relevant task (unused)
     :return: a dictionary containing evaluation metrics
     """
-    label_set = processor.get_labels()[task_name]
-
     preds = preds.flatten()
     labels = labels.flatten().astype('int')
 
     pred_inds = np.where(labels != -100)
     preds = preds[pred_inds]
     labels = labels[pred_inds]
 
@@ -58,15 +63,20 @@
     num_correct = (preds==labels).sum()
 
     acc = num_correct / len(preds)
     f1 = f1_score(labels, preds, average=None, zero_division=0)
 
     return {'acc': acc, 'token_f1': fix_np_types(f1), 'f1': fix_np_types(seq_f1([label_seq], [pred_seq])), 'report':'\n'+seq_cls([label_seq], [pred_seq])}
 
-def relation_metrics(processor, preds, labels, task_name):
+def relation_metrics(
+    label_set: Set[str],
+    preds: np.ndarray,
+    labels: np.ndarray,
+    task_name: str,
+) -> Dict[str, Any]:
     """
     One of the metrics functions for use in :func:`cnlp_compute_metrics`.
 
     Generates evaluation metrics for relation extraction tasks.
 
     Ignores tags for which the true label is -100.
 
@@ -75,22 +85,20 @@
         {
             'f1': F1 score
             'acc': accuracy
             'recall': recall
             'precision': precision
         }
 
-    :param DataProcessor processor: the data processor that was used to read in the data files
-    :param numpy.ndarray preds: the predicted labels from the model
-    :param numpy.ndarray labels: the true labels
-    :rtype: typing.Dict[str, typing.Any]
+    :param label_set: the set of labels for this task
+    :param preds: the predicted labels from the model
+    :param labels: the true labels
     :return: a dictionary containing evaluation metrics
     """
 
-    label_set = processor.get_labels()[task_name]
 
     # If we are using the attention-based relation extractor, many impossible pairs
     # are set to -100 so pytorch loss functions ignore them. We need to make sure the
     # scorer also ignores them.
     relevant_inds = np.where(labels != -100)
     relevant_labels = labels[relevant_inds].astype('int')
     relevant_preds = preds[relevant_inds]
@@ -102,15 +110,15 @@
     precision = precision_score(y_pred=relevant_preds, y_true=relevant_labels, average=None, zero_division=0)
     f1_scores = fix_np_types(f1_score(y_true=relevant_labels, y_pred=relevant_preds, average=None, zero_division=0))
     report_dict = classification_report(y_true=relevant_labels, y_pred=relevant_preds, output_dict=True)
     report_str = classification_report(y_true=relevant_labels, y_pred=relevant_preds)
 
     return {'f1': f1_scores, 'acc': acc, 'recall':fix_np_types(recall), 'precision':fix_np_types(precision), 'report_dict':report_dict, 'report_str':report_str }
 
-def acc_and_f1(preds, labels):
+def acc_and_f1(preds: np.ndarray, labels: np.ndarray) -> Dict[str, Any]:
     """
     One of the metrics functions for use in :func:`cnlp_compute_metrics`.
 
     Generates evaluation metrics for generic tasks.
 
     The returned dict is structured as follows::
 
@@ -118,17 +126,16 @@
             'acc': accuracy
             'f1': F1 score
             'acc_and_f1': mean of accuracy and F1 score
             'recall': recall
             'precision': precision
         }
 
-    :param numpy.ndarray preds: the predicted labels from the model
-    :param numpy.ndarray labels: the true labels
-    :rtype: typing.Dict[str, typing.Any]
+    :param preds: the predicted labels from the model
+    :param labels: the true labels
     :return: a dictionary containing evaluation metrics
     """
     acc = accuracy_score(y_pred=preds, y_true=labels)
     recall = recall_score(y_true=labels, y_pred=preds, average=None)
     precision = precision_score(y_true=labels, y_pred=preds, average=None, zero_division=0)
     f1 = f1_score(y_true=labels, y_pred=preds, average=None, zero_division=0)
     
@@ -136,33 +143,42 @@
         "acc": fix_np_types(acc),
         "f1": fix_np_types(f1),
         "acc_and_f1": fix_np_types((acc + f1) / 2),
         "recall": fix_np_types(recall),
         "precision": fix_np_types(precision)
     }
 
-def cnlp_compute_metrics(task_name, task_ind, preds, labels, processor, output_mode):
+
+def cnlp_compute_metrics(
+    task_name: str,
+    preds: np.ndarray,
+    labels: np.ndarray,
+    output_mode: str,
+    label_set: Set[str],
+) -> Dict[str, Any]:
     """
     Function that defines and computes the metrics used for each task.
 
     When adding a task definition to this file, add a branch to this
     function defining what its evaluation metric invocation should be.
     If the new task is a simple classification task, a sensible default
     is defined; falling back on this will trigger a warning.
 
-    :param str task_name: the task name used to index into cnlp_processors
-    :param numpy.ndarray preds: the predicted labels from the model
-    :param numpy.ndarray labels: the true labels
-    :rtype: typing.Dict[str, typing.Any]
+    :param task_name: the task name used to index into cnlp_processors
+    :param preds: the predicted labels from the model
+    :param labels: the true labels
+    :param output_mode: the output mode of the classifier
+    :param label_set: the set of output label names for the classifier
     :return: a dictionary containing evaluation metrics
     """
+
     assert len(preds) == len(
         labels
     ), f"Predictions and labels have mismatched lengths {len(preds)} and {len(labels)}"
     if output_mode == classification:
         return acc_and_f1(preds=preds, labels=labels)
     elif output_mode == tagging:
-        return tagging_metrics(processor, preds=preds, labels=labels, task_name=task_name)
+        return tagging_metrics(label_set, preds=preds, labels=labels, task_name=task_name)
     elif output_mode == relex:
-        return relation_metrics(processor, preds=preds, labels=labels, task_name=task_name)
+        return relation_metrics(label_set, preds=preds, labels=labels, task_name=task_name)
     else:
         raise Exception('There is no metric defined for this task in function cnlp_compute_metrics()')
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/cnlp_processors.py` & `cnlp-transformers-0.6.0/src/cnlpt/cnlp_processors.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from transformers.data.processors.utils import DataProcessor, InputExample
 from datasets import load_dataset
 import torch
 from torch.utils.data.dataset import Dataset
 from transformers.tokenization_utils import PreTrainedTokenizer
 import numpy as np
 import numpy  # for Sphinx
+from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 
 mtl = 'mtl'
 classification = 'classification'
 tagging = 'tagging'
 relex = 'relations'
@@ -154,18 +155,17 @@
             self.dataset = load_dataset('csv', sep=sep, data_files=data_files)
 
             ## find out what tasks are available to this dataset, and see the overlap with what the
             ## user specified at the cli, remove those tasks so we don't also get them from other datasets
             ## and overwrite these.
             first_split = next(iter(self.dataset.values()))
             dataset_tasks = first_split.features.keys() - set(['text', 'text_a', 'text_b'])
-            active_tasks = tasks.intersection(dataset_tasks)
+            active_tasks = set(tasks).intersection(dataset_tasks)           
             active_tasks = list(active_tasks)
             active_tasks.sort()
-            self.dataset.tasks = active_tasks
             self.dataset.task_output_modes = {}
         elif ext_check_file.endswith('json'):
             self.dataset = load_dataset('json', data_files=data_files, field='data')
             with open(join(data_dir, ext_check_file), 'rt', encoding="utf-8") as f:
                 json_file = json.load(f)
                 if 'metadata' in json_file:
                     metadata = json_file['metadata']
@@ -174,33 +174,46 @@
                         metadata = json.load(mf)
                 else:
                     raise Exception('No metadata was available in the data file or in the same directory!')
                 
                 dataset_task2output = {}
                 for subtask in metadata['subtasks']:
                     dataset_task2output[subtask['task_name']] = subtask['output_mode']
-                
+
+            dataset_tasks = list(dataset_task2output.keys())
             if tasks is None:
                 active_tasks = set(dataset_task2output.keys())
             else:
-                active_tasks = tasks.intersection(set(dataset_task2output.keys()))
+                active_tasks = set(tasks).intersection(set(dataset_task2output.keys()))
             
             active_tasks = list(active_tasks)
             active_tasks.sort()
 
-            self.dataset.tasks = active_tasks
             self.dataset.task_output_modes = dataset_task2output
         else:
             raise ValueError('Data file %s has an extension that we cannot handle (tried csv and json)' % (train_file))
 
-
+        logger.info('This dataset contains these tasks: %s' % (str(dataset_tasks)))
+        logger.info('These tasks overlap with user input: %s' % (str(active_tasks)))
             
+        self.dataset.tasks = active_tasks
         if len(self.dataset.task_output_modes) == 0:
             self.dataset.task_output_modes = infer_output_modes(self.dataset)
 
+        # convert label columns to strings
+        logger.info("Converting columns to strings")
+        for task in tqdm(self.dataset.tasks):
+            if self.dataset.task_output_modes[task] == classification:
+                task_str = task + '_str'
+                for split in self.dataset:
+                    # create a new column casting every element to string, remove old (int) column, rename new (str) column
+                    self.dataset[split] = self.dataset[split].add_column(task_str, [str(x) for x in self.dataset[split][task]])
+                    self.dataset[split] = self.dataset[split].remove_columns(task)
+                    self.dataset[split] = self.dataset[split].rename_column(task_str, task)
+
         # get any split of the data and ask for the set of unique labels for each task in the dataset from that split
         self.labels = get_unique_labels(self.dataset, self.dataset.tasks, self.dataset.task_output_modes)
 
         self.dataset = get_task_pruned_dataset(self.dataset, self.dataset.tasks, self.labels)
 
         self.classifiers = self.dataset.tasks
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/data/preprocess_i2b2_2008.py` & `cnlp-transformers-0.6.0/src/cnlpt/data/preprocess_i2b2_2008.py`

 * *Files identical despite different names*

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/data/transform_prot.py` & `cnlp-transformers-0.6.0/src/cnlpt/data/transform_prot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,28 @@
 from itertools import chain
 from collections import defaultdict
 from itertools import groupby, tee
 from heapq import merge
 
 TEST_DIR = "chemprot_development"
 TRAIN_DIR = "chemprot_training"
-nlp = spacy.load("en_core_sci_sm")
+
+# allow script to run only if scispacy is installed
+#  (gated behind certain Python versions and platforms)
+nlp = None
+try:
+    import scispacy
+    nlp = spacy.load("en_core_sci_sm")
+except ImportError:
+    import platform
+    print(f"scispacy not installed; cannot run transform_prot.\n"
+          f"Note: transform_prot is not runnable on ARM and non-Linux platforms, "
+          f"and is only tested on Linux x86_64 platforms.")
+    print(f"Current platform: {sys.platform} {platform.machine()}")
+    sys.exit(1)
 
 
 def remove_newline(review):
     review = review.replace("&#039;", "'")
     review = review.replace("\n", " <cr> ")
     review = review.replace("\r", " <cr> ")
     review = review.replace("\t", " ")
@@ -52,15 +65,18 @@
             sup = min(i[1] for i in ls)
             # if inf != sup:
             out.append((inf, sup))
     return out
 
 
 def to_stanza_style_dict(text):
-    processed_doc = nlp(text)
+    if nlp is not None:
+        processed_doc = nlp(text)
+    else:
+        raise RuntimeError("nlp object not initialized but execution proceeded??")
 
     def sent_dict(spacy_sent):
         return [
             {
                 "id": i + 1,
                 "text": tok.text,
                 "start_char": tok.idx,
```

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/data/transform_uci_drug.py` & `cnlp-transformers-0.6.0/src/cnlpt/data/transform_uci_drug.py`

 * *Files identical despite different names*

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/thyme_eval.py` & `cnlp-transformers-0.6.0/src/cnlpt/thyme_eval.py`

 * *Files identical despite different names*

### Comparing `cnlp-transformers-0.5.0/src/cnlpt/train_system.py` & `cnlp-transformers-0.6.0/src/cnlpt/train_system.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,253 +10,109 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ Finetuning the library models for sequence classification on clinical NLP tasks"""
-
-
-import dataclasses
 import logging
 import os
 from os.path import basename, dirname, join, exists
 import sys
-from dataclasses import dataclass, field
+
 from typing import Callable, Dict, Optional, List, Union, Any
 from filelock import FileLock
-import time
 import tempfile
 import math
 
 from enum import Enum
 
 import numpy as np
-from seqeval.metrics.sequence_labeling import get_entities
 
 import torch
 from torch.utils.data.dataset import Dataset
 from transformers import AutoConfig, AutoTokenizer, AutoModel, EvalPrediction
 from transformers.training_args import IntervalStrategy
 from transformers.data.processors.utils import InputFeatures
 from transformers.tokenization_utils import PreTrainedTokenizer
-from transformers.data.metrics import acc_and_f1
 from transformers.data.processors.utils import DataProcessor, InputExample, InputFeatures
 from transformers import ALL_PRETRAINED_CONFIG_ARCHIVE_MAP
-from transformers.optimization import get_scheduler
 from torch.optim import AdamW
-from transformers.trainer_pt_utils import get_parameter_names
 from transformers.file_utils import CONFIG_NAME
 from huggingface_hub import hf_hub_url
 
+import sys
+sys.path.append(os.path.join(os.getcwd()))
 from .cnlp_processors import tagging, relex, classification
 from .cnlp_data import ClinicalNlpDataset, DataTrainingArguments
 from .cnlp_metrics import cnlp_compute_metrics
-
+from .cnlp_args import CnlpTrainingArguments, ModelArguments
+from .cnlp_predict import write_predictions_for_dataset
 from .CnlpModelForClassification import CnlpModelForClassification, CnlpConfig
 from .BaselineModels import CnnSentenceClassifier, LstmSentenceClassifier
 from .HierarchicalTransformer import HierarchicalModel
 
 import requests
 
 from transformers import (
     HfArgumentParser,
     Trainer,
-    TrainingArguments,
     set_seed,
 )
+import json
 
-cnlpt_models = ['cnn', 'lstm', 'hier', 'cnlpt']
+AutoConfig.register("cnlpt", CnlpConfig)
 
 logger = logging.getLogger(__name__)
 
-@dataclass
-class CnlpTrainingArguments(TrainingArguments):
-    """
-    Additional arguments specific to this class.
-    See all possible arguments in :class:`transformers.TrainingArguments`
-    or by passing the ``--help`` flag to this script.
-    """
-    evals_per_epoch: Optional[int] = field(
-        default = -1, metadata={"help": "Number of times to evaluate and possibly save model per training epoch (allows for a lazy kind of early stopping)"}
-    )
-    final_task_weight: Optional[float] = field(
-        default=1.0, metadata={"help": "Amount to up/down-weight final task in task list (other tasks weighted 1.0)"}
-    )
-    freeze: float = field(
-        default=-1.0, metadata={"help": "Freeze the encoder layers and only train the layer between the encoder and classification architecture. Probably works best with --token flag since [CLS] may not be well-trained for anything in particular. If not specified, no weight freezing will be done. If specified as a flag (no arguments), 100%% of weights will be frozen. If a float (0..1.0) is specified, each weight will be frozen with that probability.", 'nargs':'?', "const":1.0 }
-    )
-    arg_reg: Optional[float] = field(
-        default=-1, metadata={"help": "Weight to use on argument regularization term (penalizes end-to-end system if a discovered relation has low probability of being any entity type). Value < 0 (default) turns off this penalty."}
-    )
-    bias_fit: bool = field(
-        default=False, metadata={"help": "Only optimize the bias parameters of the encoder (and the weights of the classifier heads), as proposed in the BitFit paper by Ben Zaken et al. 2021 (https://arxiv.org/abs/2106.10199)"}
-    )
-
-@dataclass
-class ModelArguments:
-    """
-    Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
-    See all possible arguments by passing the ``--help`` flag to this script.
-    """
-    model: Optional[str] = field( default='cnlpt', 
-        metadata={'help': "Model type", 'choices':cnlpt_models}
-    )
-    encoder_name: Optional[str] = field(default='roberta-base',
-        metadata={"help": "Path to pretrained model or model identifier from huggingface.co/models"}
-    )
-    config_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained config name or path if not the same as model_name"}
-    )
-    tokenizer_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained tokenizer name or path if not the same as model_name"}
-    )
-    cache_dir: Optional[str] = field(
-        default=None, metadata={"help": "Where do you want to store the pretrained models downloaded from s3"}
-    )
-    layer: Optional[int] = field(
-        default=-1, metadata={"help": "Which layer's CLS ('<s>') token to use"}
-    )
-    token: bool = field(
-        default=False, metadata={"help": "Classify over an actual token rather than the [CLS] ('<s>') token -- requires that the tokens to be classified are surrounded by <e>/</e> tokens"}
-    )
-
-    # NxN relation classifier-specific arguments
-    num_rel_feats: Optional[int] = field(
-        default=12, metadata={"help": "Number of features/attention heads to use in the NxN relation classifier"}
-    )
-    head_features: Optional[int] = field(
-        default=64, metadata={"help": "Number of parameters in each attention head in the NxN relation classifier"}
-    )
-
-    # CNN-specific arguments
-    cnn_embed_dim: Optional[int] = field(
-        default=100,
-        metadata={
-            'help': "For the CNN baseline model, the size of the word embedding space."
-        }
-    )
-    cnn_num_filters: Optional[int] = field(
-        default=25,
-        metadata={
-            'help': (
-                'For the CNN baseline model, the number of '
-                'convolution filters to use for each filter size.'
-            )
-        }
-    )
-
-    cnn_filter_sizes: Optional[List[int]] = field(
-        default_factory=lambda: [1, 2, 3],
-        metadata={
-            "help": (
-                "For the CNN baseline model, a space-separated list "
-                "of size(s) of the filters (kernels)"
-            )
-        }
-    )
-
-    # LSTM-specific arguments
-    lstm_embed_dim: Optional[int] = field(
-        default=100,
-        metadata={
-            'help': "For the LSTM baseline model, the size of the word embedding space."
-        }
-    )
-    lstm_hidden_size: Optional[int] = field(
-        default=100,
-        metadata={
-            "help": "For the LSTM baseline model, the hidden size of the LSTM layer"
-        }
-    )
+def is_hub_model(model_name):
+    # check if it's a model on the huggingface model hub:
+    try:
+        url = hf_hub_url(model_name, CONFIG_NAME)
+        r = requests.head(url)
+        if r.status_code == 200:
+            return True
+    except:
+        pass
 
-    # Multi-task classifier-specific arguments
-    use_prior_tasks: bool = field(
-        default=False, metadata={"help": "In the multi-task setting, incorporate the logits from the previous tasks into subsequent representation layers. This will be done in the task order specified in the command line."}
-    )
+    return False
 
-    # Hierarchical Transformer-specific arguments
-    hier_num_layers: Optional[int] = field(
-        default=2,
-        metadata={
-            "help": (
-                "For the hierarchical model, the number of document-level transformer "
-                "layers"
-            )
-        },
-    )
-    hier_hidden_dim: Optional[int] = field(
-        default=2048,
-        metadata={
-            "help": (
-                "For the hierarchical model, the inner hidden size of the positionwise "
-                "FFN in the document-level transformer layers"
-            )
-        },
-    )
-    hier_n_head: Optional[int] = field(
-        default=8,
-        metadata={
-            "help": (
-                "For the hierarchical model, the number of attention heads in the "
-                "document-level transformer layers"
-            )
-        },
-    )
-    hier_d_k: Optional[int] = field(
-        default=8,
-        metadata={
-            "help": (
-                "For the hierarchical model, the size of the query and key vectors in "
-                "the document-level transformer layers"
-            )
-        },
-    )
-    hier_d_v: Optional[int] = field(
-        default=96,
-        metadata={
-            "help": (
-                "For the hierarchical model, the size of the value vectors in the "
-                "document-level transformer layers"
-            )
-        },
-    )
-    hier_dropout: Optional[float] = field(
-        default=0.1,
-        metadata={
-            "help": "For the hierarchical model, the dropout probability for the "
-                    "document-level transformer layers"
-        }
-    )
 
+def is_cnlpt_model(model_path: str) -> bool:
+    """
+    Infer whether a model path refers to a cnlpt
+    model checkpoint (if not, we assume it is an
+    encoder)
+    :param model_path: the path to the model
+    :return: whether the model is a cnlpt classifier model
+    """
+    encoder_config = AutoConfig.from_pretrained(model_path)
+    return encoder_config.model_type == "cnlpt"
 
-def is_hub_model(model_name):
-    # check if it's a model on the huggingface model hub:
-    url = hf_hub_url(model_name, CONFIG_NAME)
-    r = requests.head(url)
-    if r.status_code == 200:
-        return True
 
-    return False
+def encoder_inferred(model_name_or_path: str) -> bool:
+    return is_hub_model(model_name_or_path) or not is_cnlpt_model(model_name_or_path)
 
 
-def main(json_file: Optional[str] = None, json_obj: Optional[Dict[str, Any]] = None):
+def main(
+    json_file: Optional[str] = None,
+    json_obj: Optional[Dict[str, Any]] = None,
+) -> Dict[str, Dict[str, Any]]:
     """
     See all possible arguments in :class:`transformers.TrainingArguments`
     or by passing the --help flag to this script.
 
     We now keep distinct sets of args, for a cleaner separation of concerns.
 
-    :param typing.Optional[str] json_file: if passed, a path to a JSON file
+    :param json_file: if passed, a path to a JSON file
         to use as the model, data, and training arguments instead of
         retrieving them from the CLI (mutually exclusive with ``json_obj``)
-    :param typing.Optional[dict] json_obj: if passed, a JSON dictionary
+    :param json_obj: if passed, a JSON dictionary
         to use as the model, data, and training arguments instead of
         retrieving them from the CLI (mutually exclusive with ``json_file``)
-    :rtype: typing.Dict[str, typing.Dict[str, typing.Any]]
     :return: the evaluation results (will be empty if ``--do_eval`` not passed)
     """
     parser = HfArgumentParser((ModelArguments, DataTrainingArguments, CnlpTrainingArguments))
     model_args: ModelArguments
     data_args: DataTrainingArguments
     training_args: CnlpTrainingArguments
 
@@ -318,79 +174,70 @@
 
     # Get datasets
     dataset = (
         ClinicalNlpDataset(data_args, tokenizer=tokenizer, cache_dir=model_args.cache_dir, hierarchical=hierarchical,)
     )
 
     try:
-        task_names = []
-        num_labels = []
-        output_mode = []
-        tagger = []
-        relations = []
-        tasks_to_processors = {}
-        for dataset_ind in range(len(data_args.data_dir)):
-            processor = dataset.processors[dataset_ind]
-            # if processor.get_num_tasks() > 1:
-            for subtask_num in range(processor.get_num_tasks()):
-                task_names.append(processor.get_classifiers()[subtask_num])
-                num_labels.append(len(processor.get_labels()[task_names[-1]]))
-                task_output_mode = processor.get_output_mode(task_names[-1])
-                output_mode.append(task_output_mode)
-                tagger.append(task_output_mode == tagging)
-                relations.append(task_output_mode == relex)
-                tasks_to_processors[task_names[-1]] = processor
-
-                # tagger.append(False)
-                # relations.append(False)
-
-                tasks_to_processors[task_names[-1]] = processor
+        task_names = data_args.task_name
+        num_labels = {}
+        output_mode = {}
+        tagger = {}
+        relations = {}
+        for task in dataset.tasks_to_labels.keys():
+            num_labels[task] = len(dataset.tasks_to_labels[task])
+            task_output_mode = dataset.output_modes[task]
+            output_mode[task] = task_output_mode
+            tagger[task] = (task_output_mode == tagging)
+            relations[task] = (task_output_mode == relex)
 
     except KeyError:
         raise ValueError("Task not found: %s" % (data_args.task_name))
 
     # Load pretrained model and tokenizer
     #
     # Distributed training:
     # The .from_pretrained methods guarantee that only one local process can concurrently
     # download model & vocab.
     if model_name == 'cnn':
-        model = CnnSentenceClassifier(len(tokenizer), 
-                                      num_labels_list=num_labels,
+        model = CnnSentenceClassifier(len(tokenizer),
+                                      task_names=task_names,
+                                      num_labels_dict=num_labels,
                                       embed_dims=model_args.cnn_embed_dim,
                                       num_filters=model_args.cnn_num_filters,
                                       filters=model_args.cnn_filter_sizes,
                                       )
         # Check if the caller specified a saved model to load (e.g., for an inference-only run)
         model_path = join(model_args.encoder_name, 'pytorch_model.bin')
         if exists(model_path):
             model.load_state_dict(torch.load(model_path))
     elif model_name == 'lstm':
         model = LstmSentenceClassifier(len(tokenizer),
-                                       num_labels_list=num_labels,
+                                       task_names=task_names,
+                                       num_labels_dict=num_labels,
                                        embed_dims=model_args.lstm_embed_dim,
                                        hidden_size=model_args.lstm_hidden_size,
                                        )
         # Check if the caller specified a saved model to load (e.g., for an inference-only run)
         model_path = join(model_args.encoder_name, 'pytorch_model.bin')
         if exists(model_path):
             model.load_state_dict(torch.load(model_path))
     elif model_name == 'hier':
         encoder_name = model_args.config_name if model_args.config_name else model_args.encoder_name
-        if is_hub_model(encoder_name):
+        if encoder_inferred(encoder_name):
             config = CnlpConfig(
-                encoder_name,
-                data_args.task_name,
-                num_labels,
+                encoder_name=encoder_name,
+                finetuning_task=data_args.task_name if data_args.task_name is not None else dataset.tasks,
                 layer=model_args.layer,
                 tokens=model_args.token,
                 num_rel_attention_heads=model_args.num_rel_feats,
                 rel_attention_head_dims=model_args.head_features,
                 tagger=tagger,
                 relations=relations,
+                label_dictionary=dataset.get_labels(),
                 hier_head_config=dict(
                     n_layers=model_args.hier_num_layers,
                     d_inner=model_args.hier_hidden_dim,
                     n_head=model_args.hier_n_head,
                     d_k=model_args.hier_d_k,
                     d_v=model_args.hier_d_v,
                     dropout=model_args.hier_dropout,
@@ -402,56 +249,65 @@
             model = HierarchicalModel(
                 config=config,
                 class_weights=dataset.class_weights,
                 freeze=training_args.freeze,
             )
         else:
             # use a checkpoint from an existing model
-            AutoConfig.register("cnlpt", CnlpConfig)
             AutoModel.register(CnlpConfig, HierarchicalModel)
 
             config = AutoConfig.from_pretrained(
                     encoder_name,
                     cache_dir=model_args.cache_dir,
+                    layer=model_args.layer
                 )
+            config.finetuning_task = data_args.task_name
+            config.relations = relations
+            config.tagger = tagger
+            config.label_dictionary = {} # this gets filled in later
 
             ## TODO: check if user overwrote parameters in command line that could change behavior of the model and warn
             #if data_args.chunk_len is not None:
 
             logger.info("Loading pre-trained hierarchical model...")
             model = AutoModel.from_pretrained(encoder_name, config=config)
+
+            model.remove_task_classifiers()
+            for task in data_args.task_name:
+                model.add_task_classifier(task, dataset.get_labels()[task])
+            model.set_class_weights(dataset.class_weights)
+
     else:
         # by default cnlpt model, but need to check which encoder they want
         encoder_name = model_args.encoder_name
 
-        # TODO check when download any pretrained language model to local disk, if 
+        # TODO check when download any pretrained language model to local disk, if
         # the following condition "is_hub_model(encoder_name)" works or not.
-        if not is_hub_model(encoder_name):
+        if not encoder_inferred(encoder_name):
             # we are loading one of our own trained models as a starting point.
             #
             # 1) if training_args.do_train is true:
-            # sometimes we may want to use an encoder that has been had continued pre-training, either on
+            # sometimes we may want to use an encoder that has had continued pre-training, either on
             # in-domain MLM or another task we think might be useful. In that case our encoder will just
-            # be a link to a directory. If the encoder-name is not recognized as a pre-trianed model, special
+            # be a link to a directory. If the encoder-name is not recognized as a pre-trained model, special
             # logic for ad hoc encoders follows:
             # we will load it as-is initially, then delete its classifier head, save the encoder
             # as a temp file, and make that temp file
             # the model file to be loaded down below the normal way. since that temp file
             # doesn't have a stored classifier it will use the randomly-inited classifier head
             # with the size of the supplied config (for the new task).
             # TODO This setting 1) is not tested yet.
             # 2) if training_args.do_train is false:
             # we evaluate or make predictions of our trained models. 
             # Both two setting require the registeration of CnlpConfig, and use 
             # AutoConfig.from_pretrained() to load the configuration file
-            AutoConfig.register("cnlpt", CnlpConfig)
             AutoModel.register(CnlpConfig, CnlpModelForClassification)
 
             
-            # Load the cnlp configuration using AutoConfig, this will not override 
+            # Load the cnlp configuration using AutoConfig, this will not override
             # the arguments from trained cnlp models. While using CnlpConfig will override
             # the model_type and model_name of the encoder.
             config = AutoConfig.from_pretrained(
                 model_args.config_name if model_args.config_name else model_args.encoder_name,
                 cache_dir=model_args.cache_dir,
             )
 
@@ -478,48 +334,45 @@
                 # setting 2) evaluate or make predictions
                 model = CnlpModelForClassification.from_pretrained(
                     model_args.encoder_name,
                     config=config,
                     class_weights=dataset.class_weights,
                     final_task_weight=training_args.final_task_weight,
                     freeze=training_args.freeze,
-                    bias_fit=training_args.bias_fit,
-                    argument_regularization=training_args.arg_reg)
+                    bias_fit=training_args.bias_fit)
 
         else:
             # This only works when model_args.encoder_name is one of the 
             # model card from https://huggingface.co/models
             # By default, we use model card as the starting point to fine-tune
             encoder_name = model_args.config_name if model_args.config_name else model_args.encoder_name
-            config = CnlpConfig(encoder_name,
-                                data_args.task_name,
-                                num_labels,
-                                layer=model_args.layer,
-                                tokens=model_args.token,
-                                num_rel_attention_heads=model_args.num_rel_feats,
-                                rel_attention_head_dims=model_args.head_features,
-                                tagger=tagger,
-                                relations=relations,)
-                                #num_tokens=len(tokenizer))
+            config = CnlpConfig(
+                encoder_name=encoder_name,
+                finetuning_task=data_args.task_name,
+                layer=model_args.layer,
+                tokens=model_args.token,
+                num_rel_attention_heads=model_args.num_rel_feats,
+                rel_attention_head_dims=model_args.head_features,
+                tagger=tagger,
+                relations=relations,
+                label_dictionary=dataset.get_labels(),
+                #num_tokens=len(tokenizer),
+            )
             config.vocab_size = len(tokenizer)
             model = CnlpModelForClassification(
                 config=config,
                 class_weights=dataset.class_weights,
                 final_task_weight=training_args.final_task_weight,
                 freeze=training_args.freeze,
-                bias_fit=training_args.bias_fit,
-                argument_regularization=training_args.arg_reg)
+                bias_fit=training_args.bias_fit,)
 
     best_eval_results = None
     output_eval_file = os.path.join(
         training_args.output_dir, f"eval_results.txt"
     )
-    output_eval_predictions = os.path.join(
-        training_args.output_dir, f'eval_predictions.txt'
-    )
 
     if training_args.do_train:
         # TODO: This assumes that if there are multiple training sets, they all have the same length, but
         # in the future it would be nice to be able to have multiple heterogeneous datasets
         batches_per_epoch = math.ceil(dataset.num_train_instances / training_args.train_batch_size)
         total_steps = int(training_args.num_train_epochs * batches_per_epoch // training_args.gradient_accumulation_steps)
 
@@ -531,185 +384,169 @@
             training_args.evaluation_strategy = IntervalStrategy.STEPS
             # This will save model per epoch
             # training_args.save_strategy = IntervalStrategy.EPOCH
         elif training_args.do_eval:
             logger.info('Evaluation strategy not specified so evaluating every epoch')
             training_args.evaluation_strategy = IntervalStrategy.EPOCH
 
-    def build_compute_metrics_fn(task_names: List[str], model, processors: Dict[str,DataProcessor]) -> Callable[[EvalPrediction], Dict]:
+    def build_compute_metrics_fn(task_names: List[str], model, dataset: ClinicalNlpDataset) -> Callable[[EvalPrediction], Dict]:
         def compute_metrics_fn(p: EvalPrediction):
 
             metrics = {}
             task_scores = []
             task_label_ind = 0
-
+            
             for task_ind,task_name in enumerate(task_names):
-                if tagger[task_ind]:
+                if tagger[task_name]:
                     preds = np.argmax(p.predictions[task_ind], axis=2)
                     # labels will be -100 where we don't need to tag
-                elif relations[task_ind]:
+                elif relations[task_name]:
                     preds = np.argmax(p.predictions[task_ind], axis=3)
                 else:
                     preds = np.argmax(p.predictions[task_ind], axis=1)
 
-                if relations[task_ind]:
+                if relations[task_name]:
                     # relation labels
                     labels = p.label_ids[:,:,task_label_ind:task_label_ind+data_args.max_seq_length].squeeze()
                     task_label_ind += data_args.max_seq_length
                 elif p.label_ids.ndim == 3:
-                    labels = p.label_ids[:,:, task_label_ind:task_label_ind+1].squeeze()
+                    if tagger[task_name]:
+                        labels = p.label_ids[:,:, task_label_ind:task_label_ind+1].squeeze()
+                    else:
+                        labels = p.label_ids[:, 0, task_label_ind].squeeze()
                     task_label_ind += 1
                 elif p.label_ids.ndim == 2:
                     labels = p.label_ids[:,task_ind].squeeze()
 
-                processor = processors[task_name]
-                metrics[task_name] = cnlp_compute_metrics(task_name, task_ind, preds, labels, processor, processor.get_output_mode(task_name))
+                metrics[task_name] = cnlp_compute_metrics(task_name, preds, labels, 
+                                                          dataset.output_modes[task_name], 
+                                                          dataset.tasks_to_labels[task_name])
                 # FIXME - Defaulting to accuracy for model selection score, when it should be task-specific
                 task_scores.append( metrics[task_name].get('one_score', np.mean(metrics[task_name].get('f1'))))
                 #task_scores.append(processor.get_one_score(metrics.get(task_name, metrics.get(task_name.split('-')[0], None))))
 
             one_score = sum(task_scores) / len(task_scores)
 
             if not model is None:
                 if not hasattr(model, 'best_score') or one_score > model.best_score:
                     # For convenience, we also re-save the tokenizer to the same directory,
                     # so that you can share your model easily on huggingface.co/models =)
                     if trainer.is_world_process_zero():
                         if training_args.do_train:
                             trainer.save_model()
                             tokenizer.save_pretrained(training_args.output_dir)
+                            if model_name == 'cnn' or model_name == 'lstm':
+                                with open(os.path.join(training_args.output_dir, 'config.json'), 'w') as f:
+                                    json.dump(model_args.to_dict(), f)
                         for task_ind,task_name in enumerate(metrics):
                             with open(output_eval_file, "w") as writer:
                                 # logger.info("***** Eval results for task %s *****" % (task_name))
                                 for key, value in metrics[task_name].items():
                                     # logger.info("  %s = %s", key, value)
                                     writer.write("%s = %s\n" % (key, value))
                     model.best_score = one_score
                     model.best_eval_results = metrics
 
             return metrics
 
         return compute_metrics_fn
 
     # Initialize our Trainer
+    training_args.load_best_model_at_end = True
+    training_args.metric_for_best_model='one_score'
     trainer = Trainer(
         model=model,
         args=training_args,
-        train_dataset=dataset.datasets[0].get('train', None),
-        eval_dataset=dataset.datasets[0].get('validation', None),
-        compute_metrics=build_compute_metrics_fn(task_names, model, tasks_to_processors),
+        train_dataset=dataset.processed_dataset.get('train', None),
+        eval_dataset=dataset.processed_dataset.get('validation', None),
+        compute_metrics=build_compute_metrics_fn(task_names, model, dataset),
     )
 
     # Training
     if training_args.do_train:
         trainer.train(
             # resume_from_checkpoint=model_args.model_name_or_path if os.path.isdir(model_args.model_name_or_path) else None
         )
 
+        # if we didn't do any evaluations during training then no model
+        # would have ever been saved. we'll save the model here
         if not hasattr(model, 'best_score'):
             # For convenience, we also re-save the tokenizer to the same directory,
             # so that you can share your model easily on huggingface.co/models =)
             if trainer.is_world_process_zero():
                 trainer.save_model()
                 tokenizer.save_pretrained(training_args.output_dir)
+                if model_name == 'cnn' or model_name == 'lstm':
+                    with open(os.path.join(training_args.output_dir, 'config.json'), 'w') as f:
+                        json.dump(model_args, f)
 
     # Evaluation
     eval_results = {}
     if training_args.do_eval:
         logger.info("*** Evaluate ***")
-        eval_dataset=dataset.datasets[0]['validation']
-        try:
-            eval_result = model.best_eval_results
-        except:
+        eval_dataset=dataset.processed_dataset['validation']
+        # no evaluation was done prior to now, so we need to evaluate
+        if not hasattr(model, 'best_eval_results'):
             eval_result = trainer.evaluate(eval_dataset=eval_dataset)
+        else:
+            eval_result = model.best_eval_results
+        
+        # if there is a stored model, restore it so writing outputs uses a good model
+
         
+        trainer.compute_metrics = None
         if trainer.is_world_process_zero():
             with open(output_eval_file, "w") as writer:
-                logger.info("***** Eval results *****")
+                logger.info("***** Eval results on combined dataset *****")
                 for key, value in eval_result.items():
                     logger.info("  %s = %s", key, value)
                     writer.write("%s = %s\n" % (key, value))
 
-            with open(output_eval_predictions, 'w') as writer:
-                #Chen wrote the below but it doesn't work for all settings
-                predictions = trainer.predict(test_dataset=eval_dataset).predictions
-                dataset_labels = dataset.get_labels()
-                for dataset_ind in range(len(data_args.data_dir)):
-                    processor = dataset.processors[dataset_ind]
-                    for task_ind in range(processor.get_num_tasks()):
-                        task_name = processor.get_classifiers()[task_ind]
-                # for task_ind, task_name in enumerate(task_names):
-                        if output_mode[task_ind] == classification:
-                            task_predictions = np.argmax(predictions[task_ind], axis=1)
-                            for index, item in enumerate(task_predictions):
-                                if len(task_names) > len(dataset_labels):
-                                    subtask_ind = 0
-                                else:
-                                    subtask_ind = task_ind
-                                item = dataset_labels[dataset_ind][task_name][item]
-                                writer.write("Task %d (%s) - Index %d - %s\n" % (task_ind, task_name, index, item))
-                        elif output_mode[task_ind] == tagging:
-                            task_predictions = np.argmax(predictions[task_ind], axis=2)
-                            task_labels = dataset_labels[dataset_ind][task_name]
-                            for index, pred_seq in enumerate(task_predictions):
-                                wpind_to_ind = {}
-                                chunk_labels = []
-
-                                token_inds = eval_dataset['input_ids'][index]
-                                tokens = tokenizer.convert_ids_to_tokens(token_inds)
-                                for token_ind in range(1,len(tokens)):
-                                    if token_inds[token_ind] <= 2:
-                                        break
-                                    if tokens[token_ind].startswith('Ġ'):
-                                        wpind_to_ind[token_ind] = len(wpind_to_ind)
-                                        chunk_labels.append(task_labels[task_predictions[index][token_ind]])
-
-                                entities = get_entities(chunk_labels)
-                                writer.write('Task %d (%s) - Index %d: %s\n' % (task_ind, task_name, index, str(entities)))
-                        elif output_mode[task_ind] == relex:
-                            task_predictions = np.argmax(predictions[task_ind], axis=3)
-                            task_labels = dataset_labels[dataset_ind][task_name]
-                            # assert task_labels[0] == 'None', 'The first labeled relation category should always be "None" but for task %s it is %s' % (task_names[task_ind], task_labels[0])
-                            
-                            for inst_ind in range(task_predictions.shape[0]):
-                                inst_preds = task_predictions[inst_ind]
-                                a1s, a2s = np.where(inst_preds > 0)
-                                for arg_ind in range(len(a1s)):
-                                    a1_ind = a1s[arg_ind]
-                                    a2_ind = a2s[arg_ind]
-                                    cat = task_labels[ inst_preds[a1_ind][a2_ind] ]
-                                    writer.write("Task %d (%s) - Index %d - %s(%d, %d)\n" % (task_ind, task_name, inst_ind, cat, a1_ind, a2_ind))
-                        else:
-                            raise NotImplementedError('Writing predictions is not implemented for this output_mode!')
+            # here we probably want separate predictions for each dataset:
+            if training_args.load_best_model_at_end:
+                model.load_state_dict(torch.load(join(training_args.output_dir, 'pytorch_model.bin')))  # load best model
+                trainer = Trainer(  # maake trainer from best model
+                    model=model,
+                    args=training_args,
+                    train_dataset=dataset.processed_dataset.get('train', None),
+                    eval_dataset=dataset.processed_dataset.get('validation', None),
+                    compute_metrics=build_compute_metrics_fn(task_names, model, dataset),
+                ) 
+                # use trainer to predict 
+            for dataset_ind,dataset_path in enumerate(data_args.data_dir):
+                subdir = os.path.split(dataset_path.rstrip('/'))[1]
+                output_eval_predictions_file = os.path.join(training_args.output_dir, f'eval_predictions_%s_%d.txt' % (subdir, dataset_ind))
+                write_predictions_for_dataset(output_eval_predictions_file, 
+                                              trainer,
+                                              dataset,
+                                              'validation',
+                                              dataset_ind,
+                                              output_mode,
+                                              tokenizer)
 
         eval_results.update(eval_result)
 
     if training_args.do_predict:
         logging.info("*** Test ***")
-        test_dataset=dataset.datasets[0]['test']
+        trainer.compute_metrics = None
         # FIXME: this part hasn't been updated for the MTL setup so it doesn't work anymore since
         # predictions is generalized to be a list of predictions and the output needs to be different for each kin.
         # maybe it's ok to only handle classification since it has a very straightforward output format and evaluation,
         # while for relations we can punt to the user to just write their own eval code.
-        predictions = trainer.predict(test_dataset=test_dataset).predictions
-        for task_ind, task_name in enumerate(task_names):
-            if output_mode[task_ind] == "classification":
-                task_predictions = np.argmax(predictions[task_ind], axis=1)
-            else:
-                raise NotImplementedError('Writing predictions is not implemented for this output_mode!')
-        
-            output_test_file = os.path.join(
-                training_args.output_dir, f"test_results.txt"
-            )
-            if trainer.is_world_process_zero():
-                with open(output_test_file, "w") as writer:
-                    logger.info("***** Test results *****")
-                    for index, item in enumerate(task_predictions):
-                        item = test_dataset.get_labels()[task_name][item]
-                        writer.write("%s\n" % (item))
+        if trainer.is_world_process_zero():
+            for dataset_ind, dataset_path in enumerate(data_args.data_dir):
+                subdir = os.path.split(dataset_path.rstrip('/'))[1]
+                output_test_predictions_file = os.path.join(training_args.output_dir, f'test_predictions_%s_%d.txt' % (subdir, dataset_ind))
+                write_predictions_for_dataset(output_test_predictions_file, 
+                                                trainer,
+                                                dataset,
+                                                'test',
+                                                dataset_ind,
+                                                output_mode,
+                                                tokenizer)
 
     return eval_results
 
 
 def _mp_fn(index):
     # For xla_spawn (TPUs)
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cnlp-transformers-0.5.0/test/test_api.py` & `cnlp-transformers-0.6.0/test/test_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,16 +47,21 @@
         )
         out = asyncio.run(temporal_process_sentence(doc))
         expected_out = TemporalResults.parse_obj(
             {'events': [[{'begin': 3, 'dtr': 'BEFORE', 'end': 3},
                          {'begin': 5, 'dtr': 'BEFORE', 'end': 5},
                          {'begin': 13, 'dtr': 'AFTER', 'end': 13},
                          {'begin': 15, 'dtr': 'AFTER', 'end': 15}]],
-             'relations': [[{'arg1': 'EVENT-0', 'arg2': 'EVENT-1', 'category': 'OVERLAP', 'arg1_start': 3, 'arg2_start': 5}, 
-                            {'arg1': 'TIMEX-0', 'arg2': 'EVENT-0', 'category': 'CONTAINS', 'arg1_start': 6, 'arg2_start': 3}, 
-                            {'arg1': 'EVENT-3', 'arg2': 'EVENT-2', 'category': 'BEGINS-ON', 'arg1_start': 15, 'arg2_start': 13}, 
-                            {'arg1': 'TIMEX-1', 'arg2': 'EVENT-2', 'category': 'CONTAINS', 'arg1_start': 16, 'arg2_start': 13}, 
-                            {'arg1': 'TIMEX-1', 'arg2': 'EVENT-3', 'category': 'CONTAINS', 'arg1_start': 16, 'arg2_start': 15}]],
+             'relations': [[{'arg1': 'TIMEX-0',
+                 'arg1_start': 6,
+                 'arg2': 'EVENT-0',
+                 'arg2_start': 3,
+                 'category': 'CONTAINS'},
+                {'arg1': 'TIMEX-1',
+                 'arg1_start': 16,
+                 'arg2': 'EVENT-2',
+                 'arg2_start': 13,
+                 'category': 'CONTAINS'}]],
              'timexes': [[{'begin': 6, 'end': 9, 'timeClass': 'DATE'},
                           {'begin': 16, 'end': 17, 'timeClass': 'DATE'}]]}
         )
         assert out == expected_out
```

### Comparing `cnlp-transformers-0.5.0/test/test_init.py` & `cnlp-transformers-0.6.0/test/test_init.py`

 * *Files identical despite different names*

