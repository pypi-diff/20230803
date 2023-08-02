# Comparing `tmp/decontext-0.1.2.tar.gz` & `tmp/decontext-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decontext-0.1.2.tar", last modified: Mon Jul 17 19:26:07 2023, max compression
+gzip compressed data, was "decontext-0.1.3.tar", last modified: Wed Aug  2 22:46:00 2023, max compression
```

## Comparing `decontext-0.1.2.tar` & `decontext-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.788131 decontext-0.1.2/
--rw-r--r--   0 benjaminn  (5207) users      (100)    13878 2023-07-17 19:26:07.786131 decontext-0.1.2/PKG-INFO
--rw-r--r--   0 benjaminn  (5207) users      (100)    12758 2023-07-14 20:36:02.000000 decontext-0.1.2/README.md
--rw-r--r--   0 benjaminn  (5207) users      (100)     3093 2023-07-17 19:25:34.000000 decontext-0.1.2/pyproject.toml
--rw-r--r--   0 benjaminn  (5207) users      (100)       38 2023-07-17 19:26:07.788131 decontext-0.1.2/setup.cfg
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.651137 decontext-0.1.2/src/
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.703135 decontext-0.1.2/src/decontext/
--rw-r--r--   0 benjaminn  (5207) users      (100)      120 2023-07-14 01:43:45.000000 decontext-0.1.2/src/decontext/__init__.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     6676 2023-07-14 20:16:15.000000 decontext-0.1.2/src/decontext/cache.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     6503 2023-07-14 01:23:06.000000 decontext-0.1.2/src/decontext/data_types.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      115 2023-07-13 17:38:14.000000 decontext-0.1.2/src/decontext/logging.py
--rw-r--r--   0 benjaminn  (5207) users      (100)    13289 2023-07-14 01:05:17.000000 decontext-0.1.2/src/decontext/model.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     2650 2023-07-14 02:03:38.000000 decontext-0.1.2/src/decontext/pipeline.py
--rw-r--r--   0 benjaminn  (5207) users      (100)        0 2023-07-07 20:57:14.000000 decontext-0.1.2/src/decontext/py.typed
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.744133 decontext-0.1.2/src/decontext/step/
--rw-r--r--   0 benjaminn  (5207) users      (100)     6062 2023-07-16 15:46:42.000000 decontext-0.1.2/src/decontext/step/qa.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      767 2023-07-16 15:53:33.000000 decontext-0.1.2/src/decontext/step/qgen.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     1033 2023-07-14 15:49:13.000000 decontext-0.1.2/src/decontext/step/step.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      788 2023-07-14 16:37:13.000000 decontext-0.1.2/src/decontext/step/synth.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     4115 2023-07-16 15:54:26.000000 decontext-0.1.2/src/decontext/template.py
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.765132 decontext-0.1.2/src/decontext/templates/
--rw-r--r--   0 benjaminn  (5207) users      (100)        0 2023-07-14 15:40:25.000000 decontext-0.1.2/src/decontext/templates/__init__.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      624 2023-07-12 00:22:38.000000 decontext-0.1.2/src/decontext/templates/qa_fulltext.yaml
--rw-r--r--   0 benjaminn  (5207) users      (100)      957 2023-07-12 20:55:22.000000 decontext-0.1.2/src/decontext/templates/qa_retrieval.yaml
--rw-r--r--   0 benjaminn  (5207) users      (100)     1045 2023-07-12 00:21:41.000000 decontext-0.1.2/src/decontext/templates/qgen.yaml
--rw-r--r--   0 benjaminn  (5207) users      (100)     1456 2023-07-12 00:19:47.000000 decontext-0.1.2/src/decontext/templates/synth.yaml
--rw-r--r--   0 benjaminn  (5207) users      (100)      920 2023-07-14 00:52:27.000000 decontext-0.1.2/src/decontext/utils.py
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.727134 decontext-0.1.2/src/decontext.egg-info/
--rw-r--r--   0 benjaminn  (5207) users      (100)    13878 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/PKG-INFO
--rw-r--r--   0 benjaminn  (5207) users      (100)      814 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminn  (5207) users      (100)        1 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminn  (5207) users      (100)      477 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/requires.txt
--rw-r--r--   0 benjaminn  (5207) users      (100)       10 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.783131 decontext-0.1.2/tests/
--rw-r--r--   0 benjaminn  (5207) users      (100)     1641 2023-07-16 15:53:55.000000 decontext-0.1.2/tests/test_cache.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     1052 2023-07-14 02:43:59.000000 decontext-0.1.2/tests/test_data_types.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     8590 2023-07-17 19:02:09.000000 decontext-0.1.2/tests/test_pipeline.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      348 2023-07-14 00:52:27.000000 decontext-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-02 22:46:00.923920 decontext-0.1.3/
+-rw-r--r--   0 benjaminn   (502) staff       (20)    13886 2023-08-02 22:46:00.923696 decontext-0.1.3/PKG-INFO
+-rw-r--r--   0 benjaminn   (502) staff       (20)    12767 2023-08-02 22:45:19.000000 decontext-0.1.3/README.md
+-rw-r--r--   0 benjaminn   (502) staff       (20)     3281 2023-08-02 22:45:19.000000 decontext-0.1.3/pyproject.toml
+-rw-r--r--   0 benjaminn   (502) staff       (20)       38 2023-08-02 22:46:00.923972 decontext-0.1.3/setup.cfg
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-02 22:46:00.917283 decontext-0.1.3/src/
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-02 22:46:00.920232 decontext-0.1.3/src/decontext/
+-rw-r--r--   0 benjaminn   (502) staff       (20)      120 2023-08-02 21:27:06.000000 decontext-0.1.3/src/decontext/__init__.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     6676 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/cache.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     6503 2023-08-02 22:45:19.000000 decontext-0.1.3/src/decontext/data_types.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      115 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/logging.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)    13536 2023-08-02 22:45:19.000000 decontext-0.1.3/src/decontext/model.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     2782 2023-08-02 22:45:19.000000 decontext-0.1.3/src/decontext/pipeline.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)        0 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/py.typed
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-02 22:46:00.921785 decontext-0.1.3/src/decontext/step/
+-rw-r--r--   0 benjaminn   (502) staff       (20)     6148 2023-08-02 22:45:19.000000 decontext-0.1.3/src/decontext/step/qa.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      767 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/step/qgen.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1033 2023-08-02 21:29:03.000000 decontext-0.1.3/src/decontext/step/step.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      788 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/step/synth.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     4115 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/template.py
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-02 22:46:00.922614 decontext-0.1.3/src/decontext/templates/
+-rw-r--r--   0 benjaminn   (502) staff       (20)        0 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/templates/__init__.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      624 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/templates/qa_fulltext.yaml
+-rw-r--r--   0 benjaminn   (502) staff       (20)      957 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/templates/qa_retrieval.yaml
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1045 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/templates/qgen.yaml
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1456 2023-08-01 22:11:18.000000 decontext-0.1.3/src/decontext/templates/synth.yaml
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1124 2023-08-02 22:45:19.000000 decontext-0.1.3/src/decontext/utils.py
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-02 22:46:00.921034 decontext-0.1.3/src/decontext.egg-info/
+-rw-r--r--   0 benjaminn   (502) staff       (20)    13886 2023-08-02 22:46:00.000000 decontext-0.1.3/src/decontext.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminn   (502) staff       (20)      834 2023-08-02 22:46:00.000000 decontext-0.1.3/src/decontext.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminn   (502) staff       (20)        1 2023-08-02 22:46:00.000000 decontext-0.1.3/src/decontext.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminn   (502) staff       (20)      489 2023-08-02 22:46:00.000000 decontext-0.1.3/src/decontext.egg-info/requires.txt
+-rw-r--r--   0 benjaminn   (502) staff       (20)       10 2023-08-02 22:46:00.000000 decontext-0.1.3/src/decontext.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-08-02 22:46:00.923458 decontext-0.1.3/tests/
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1641 2023-08-01 22:11:18.000000 decontext-0.1.3/tests/test_cache.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     1052 2023-08-01 22:11:18.000000 decontext-0.1.3/tests/test_data_types.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      653 2023-08-02 22:45:19.000000 decontext-0.1.3/tests/test_model.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)     8590 2023-08-01 22:11:18.000000 decontext-0.1.3/tests/test_pipeline.py
+-rw-r--r--   0 benjaminn   (502) staff       (20)      493 2023-08-02 22:45:19.000000 decontext-0.1.3/tests/test_utils.py
```

### Comparing `decontext-0.1.2/PKG-INFO` & `decontext-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decontext
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pipeline for decontextualization of scientific snippets.
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Benjamin Newman <bnewmancommercial@gmail.com>, Luca Soldaini <luca@soldaini.net>, Kyle Lo <kylel@allenai.org>
 Maintainer-email: Benjamin Newman <bnewmancommercial@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Repository, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Bug Tracker, https://github.com/bnewm0609/qa-decontextualization/issues
@@ -106,15 +106,15 @@
 
 The context can be loaded in using the `PaperContext.parse_raw` method:
 ```python
 PaperContext.parse_raw("""{
     "title": "<title>",
     "abstract": "<abstract>",
     "full_text": [{
-        "name" : "<section_title>",
+        "section_name" : "<section_title>",
         "paragraphs": ["<paragraph>", ...]
     }, ...]
 }""")
 ```
 
 Additionally, the `decontext` function also supports using multiple papers as context:
 ```python
```

### Comparing `decontext-0.1.2/README.md` & `decontext-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 The context can be loaded in using the `PaperContext.parse_raw` method:
 ```python
 PaperContext.parse_raw("""{
     "title": "<title>",
     "abstract": "<abstract>",
     "full_text": [{
-        "name" : "<section_title>",
+        "section_name" : "<section_title>",
         "paragraphs": ["<paragraph>", ...]
     }, ...]
 }""")
 ```
 
 Additionally, the `decontext` function also supports using multiple papers as context:
 ```python
@@ -220,8 +220,8 @@
 
     Returns:
         string with the decontextualized version of the snippet.
 
         if `return_metadata = True`, additionally return the intermediate results for each step of the pipeline
         as described above.
     """
-```
+```
```

### Comparing `decontext-0.1.2/pyproject.toml` & `decontext-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "decontext"
-version = "0.1.2"
+version = "0.1.3"
 description = """\
 Pipeline for decontextualization of scientific snippets.
 """
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "anthropic==0.2.10",
     "diskcache==5.6.1",
     "filelock==3.12.2",
     "Jinja2==3.1.2",
     "shadow-scholar==0.6.1",
-    "omegaconf==2.2.3",
+    "omegaconf>=2.3.0",
     "openai==0.27.7",
     "pydantic==1.9.1",
     "tiktoken==0.4.0",
     "numpy==1.23.2",
     "spacy==3.4.1",
     "torch<2.0.0",
     "scikit-learn==1.1.2",
@@ -81,22 +81,23 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "black[jupyter]>=21.12b0",
     "isort>=5.8.0",
     "mypy>=0.971",
-    "pytest>=5.2",
     "ipython>=8.4.0",
     "autopep8>=1.7.0",
     "flake8>=5.0",
     "ipdb>=0.13.0",
     "flake8-pyi>=22.8.1",
     "Flake8-pyproject>=1.1.0",
     "pytest==7.1.3",
+    "pytest-xdist",
+    "pytest-cov",
 ]
 
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 (
@@ -139,13 +140,24 @@
 per-file-ignores = [
     '*.py:E203',
     '__init__.py:F401',
     '*.pyi:E302,E305'
 ]
 
 [tool.pytest.ini_options]
+addopts = '-n auto --cov=.'
 testpaths = ["tests/"]
 python_classes = ["Test*", "*Test"]
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 markers = []
 filterwarnings = []
+
+[tool.coverage.run]
+omit = [
+    '*__init__*',
+    '*Test*',
+    'tests/fixtures/*',
+    'tests/*',
+]
+[tool.coverage.report]
+fail_under = 25
```

### Comparing `decontext-0.1.2/src/decontext/cache.py` & `decontext-0.1.3/src/decontext/cache.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext/data_types.py` & `decontext-0.1.3/src/decontext/data_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             sections = [""] * len(additional_paragraphs)
 
         for qae in self.qae:
             if qae.qid == qid:
                 if qae.evidence is None:
                     qae.evidence = []
                 for section, additional_paragraph in zip(
-                    additional_paragraphs, sections
+                    sections, additional_paragraphs
                 ):
                     qae.evidence.append(
                         EvidenceParagraph(
                             section=section,
                             paragraph=additional_paragraph,
                             paper_id=paper_id,
                         )
```

### Comparing `decontext-0.1.2/src/decontext/model.py` & `decontext-0.1.3/src/decontext/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from decontext.data_types import (
     OpenAIChatMessage,
     OpenAIChatResponse,
     OpenAICompletionResponse,
     AnthropicResponse,
     ModelResponse,
 )
+from decontext.logging import warn
 
 OPENAI_CHAT_MODEL_NAMES = {
     "gpt-3.5-turbo",
     "gpt-3.5-turbo-0301",
     "gpt-3.5-turbo-0613",
     "gpt-3.5-turbo-16k-0613",
     "gpt-4",
@@ -44,15 +45,19 @@
         This involves setting up the cache, API key, and default parameters.
 
         Args:
             args (DictConfig): Experiment configuration arguments.
         """
         self._name = model_name
         self.cache = DiskCache.load()
-        openai.api_key = os.environ["OPENAI_API_KEY"]
+        if "OPENAI_API_KEY" not in os.environ:
+            warn("OPENAI_API_KEY not found in environment variables."
+                "Set OPEN_API_KEY with your API key to use the OpenAI API.")
+        else:
+            openai.api_key = os.environ["OPENAI_API_KEY"]
 
         self.params = {
             "model": self.name,
             "logprobs": 5,
             "user": "[ANON]",
             "temperature": params.get("temperature", 0.7),
             "top_p": params.get("top_p", 1.0),
```

### Comparing `decontext-0.1.2/src/decontext/pipeline.py` & `decontext-0.1.3/src/decontext/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List, Optional, Tuple, Union
 
 from pydantic import BaseModel
 
-
 from decontext.data_types import (
     PaperContext,
     PaperSnippet,
 )
 from decontext.step.step import PipelineStep
 from decontext.step.qa import TemplateRetrievalQAStep, TemplateFullTextQAStep
 from decontext.step.qgen import TemplateQGenStep
@@ -16,29 +15,33 @@
 
 class Pipeline(BaseModel):
     steps: List[PipelineStep]
 
     class Config:
         arbitrary_types_allowed = True
 
-
+# We don't want to instantiatate the pipelines here
 class RetrievalQAPipeline(Pipeline):
-    steps: List[PipelineStep] = [
-        TemplateQGenStep(),
-        TemplateRetrievalQAStep(),
-        TemplateSynthStep(),
-    ]
+
+    def __init__(self, **data):
+        data["steps"] = [
+            TemplateQGenStep(),
+            TemplateRetrievalQAStep(),
+            TemplateSynthStep(),
+        ]
 
 
 class FullTextQAPipeline(Pipeline):
-    steps: List[PipelineStep] = [
-        TemplateQGenStep(),
-        TemplateFullTextQAStep(),
-        TemplateSynthStep(),
-    ]
+
+    def __init__(self, **data):
+        data["steps"] = [
+            TemplateQGenStep(),
+            TemplateFullTextQAStep(),
+            TemplateSynthStep(),
+        ]
 
 
 def decontext(
     snippet: str,
     context: PaperContext,
     additional_contexts: Optional[List[PaperContext]] = None,
     pipeline: Optional[Pipeline] = None,
```

### Comparing `decontext-0.1.2/src/decontext/step/qa.py` & `decontext-0.1.3/src/decontext/step/qa.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from contextlib import ExitStack
 from importlib import resources
 
 from shadow_scholar.app import pdod
 
 from decontext.data_types import PaperSnippet, Section
 from decontext.step.step import QAStep, TemplatePipelineStep
-from decontext.utils import none_check
+from decontext.utils import none_check, unique
 
 
 class TemplateRetrievalQAStep(QAStep, TemplatePipelineStep):
     """Template step that does retrieval"""
 
     def __init__(self):
         with resources.path("decontext.templates", "qa_retrieval.yaml") as f:
@@ -100,39 +100,39 @@
             os.remove(retrieval_output_file_name)
 
         return paper_retrieval_output_file
 
     def run(self, snippet: PaperSnippet):
         self.retrieve(snippet)
         for question in snippet.qae:
-            unique_evidence = set(
-                [
-                    ev.paragraph
-                    for ev in (none_check(question.evidence, []))
-                    if (
-                        ev.paragraph != snippet.context.abstract
-                        and ev.paragraph != snippet.paragraph_with_snippet
-                    )
-                ]
-            )
+            evidence = [
+                ev.paragraph
+                for ev in (none_check(question.evidence, []))
+                if (
+                    ev.paragraph != snippet.context.abstract
+                    and ev.paragraph != snippet.paragraph_with_snippet
+                )
+            ]
+            # https://stackoverflow.com/questions/9792664/converting-a-list-to-a-set-changes-element-order
+            unique_evidence = unique(evidence)
 
             paragraph_with_snippet = snippet.paragraph_with_snippet.paragraph
             section_with_snippet = none_check(
                 snippet.paragraph_with_snippet.section, ""
             )
 
             prompt = self.template.fill(
                 {
                     "snippet": snippet.snippet,
                     "question": question.question,
                     "title": snippet.context.title,
                     "abstract": snippet.context.abstract,
                     "section_with_snippet": section_with_snippet,
                     "paragraph_with_snippet": paragraph_with_snippet,
-                    "unique_evidence": list(unique_evidence),
+                    "unique_evidence": unique_evidence,
                 }
             )
             result = self.model(prompt)
             answer = self.model.extract_text(result)
             snippet.add_answer(qid=question.qid, answer=answer)
             snippet.add_cost(result.cost)
```

### Comparing `decontext-0.1.2/src/decontext/step/qgen.py` & `decontext-0.1.3/src/decontext/step/qgen.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext/step/step.py` & `decontext-0.1.3/src/decontext/step/step.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext/step/synth.py` & `decontext-0.1.3/src/decontext/step/synth.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext/template.py` & `decontext-0.1.3/src/decontext/template.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext/templates/qa_fulltext.yaml` & `decontext-0.1.3/src/decontext/templates/qa_fulltext.yaml`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext/templates/qa_retrieval.yaml` & `decontext-0.1.3/src/decontext/templates/qa_retrieval.yaml`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext/templates/qgen.yaml` & `decontext-0.1.3/src/decontext/templates/qgen.yaml`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext/templates/synth.yaml` & `decontext-0.1.3/src/decontext/templates/synth.yaml`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/src/decontext.egg-info/PKG-INFO` & `decontext-0.1.3/src/decontext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decontext
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pipeline for decontextualization of scientific snippets.
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Benjamin Newman <bnewmancommercial@gmail.com>, Luca Soldaini <luca@soldaini.net>, Kyle Lo <kylel@allenai.org>
 Maintainer-email: Benjamin Newman <bnewmancommercial@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Repository, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Bug Tracker, https://github.com/bnewm0609/qa-decontextualization/issues
@@ -106,15 +106,15 @@
 
 The context can be loaded in using the `PaperContext.parse_raw` method:
 ```python
 PaperContext.parse_raw("""{
     "title": "<title>",
     "abstract": "<abstract>",
     "full_text": [{
-        "name" : "<section_title>",
+        "section_name" : "<section_title>",
         "paragraphs": ["<paragraph>", ...]
     }, ...]
 }""")
 ```
 
 Additionally, the `decontext` function also supports using multiple papers as context:
 ```python
```

### Comparing `decontext-0.1.2/src/decontext.egg-info/SOURCES.txt` & `decontext-0.1.3/src/decontext.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,9 +21,10 @@
 src/decontext/templates/__init__.py
 src/decontext/templates/qa_fulltext.yaml
 src/decontext/templates/qa_retrieval.yaml
 src/decontext/templates/qgen.yaml
 src/decontext/templates/synth.yaml
 tests/test_cache.py
 tests/test_data_types.py
+tests/test_model.py
 tests/test_pipeline.py
 tests/test_utils.py
```

### Comparing `decontext-0.1.2/tests/test_cache.py` & `decontext-0.1.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/tests/test_data_types.py` & `decontext-0.1.3/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.2/tests/test_pipeline.py` & `decontext-0.1.3/tests/test_pipeline.py`

 * *Files identical despite different names*

