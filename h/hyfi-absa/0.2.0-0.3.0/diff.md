# Comparing `tmp/hyfi_absa-0.2.0.tar.gz` & `tmp/hyfi_absa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_absa-0.2.0.tar", max compression
+gzip compressed data, was "hyfi_absa-0.3.0.tar", max compression
```

## Comparing `hyfi_absa-0.2.0.tar` & `hyfi_absa-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     1071 2023-08-02 12:23:49.380314 hyfi_absa-0.2.0/LICENSE
--rw-r--r--   0        0        0     2598 2023-08-02 12:23:49.380314 hyfi_absa-0.2.0/README.md
--rw-r--r--   0        0        0     2965 2023-08-02 12:24:15.216351 hyfi_absa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      181 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/__cli__.py
--rw-r--r--   0        0        0      473 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/__init__.py
--rw-r--r--   0        0        0       22 2023-08-02 12:24:15.176351 hyfi_absa-0.2.0/src/hyabsa/_version.py
--rw-r--r--   0        0        0      157 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/agents/__init__.py
--rw-r--r--   0        0        0      641 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/agents/absa.py
--rw-r--r--   0        0        0     1458 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/agents/base.py
--rw-r--r--   0        0        0      900 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/agents/results.py
--rw-r--r--   0        0        0        0 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/__init__.py
--rw-r--r--   0        0        0      234 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/about/hyabsa.yaml
--rw-r--r--   0        0        0      158 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/agent/__init__.yaml
--rw-r--r--   0        0        0      158 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/agent/absa.yaml
--rw-r--r--   0        0        0       51 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/llm/__init__.yaml
--rw-r--r--   0        0        0       91 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/llm/gpt35.yaml
--rw-r--r--   0        0        0       80 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/llm/gpt4.yaml
--rw-r--r--   0        0        0      111 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/llm/openai.yaml
--rw-r--r--   0        0        0       64 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/prompts/__init__.yaml
--rw-r--r--   0        0        0     2975 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/prompts/default.yaml
--rw-r--r--   0        0        0      319 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/runner/absa.yaml
--rw-r--r--   0        0        0      108 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/contexts/__init__.py
--rw-r--r--   0        0        0      127 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/llms/__init__.py
--rw-r--r--   0        0        0     2949 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/llms/openai.py
--rw-r--r--   0        0        0      744 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/prompts/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/py.typed
--rw-r--r--   0        0        0       62 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/runners/__init__.py
--rw-r--r--   0        0        0     2560 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/runners/absa.py
--rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 hyfi_absa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2598 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/README.md
+-rw-r--r--   0        0        0     2965 2023-08-03 02:12:12.844527 hyfi_absa-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/__cli__.py
+-rw-r--r--   0        0        0      473 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-03 02:12:12.800525 hyfi_absa-0.3.0/src/hyabsa/_version.py
+-rw-r--r--   0        0        0      157 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/agents/__init__.py
+-rw-r--r--   0        0        0      641 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/agents/absa.py
+-rw-r--r--   0        0        0     1532 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/agents/base.py
+-rw-r--r--   0        0        0      922 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/agents/results.py
+-rw-r--r--   0        0        0        0 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/__init__.py
+-rw-r--r--   0        0        0      234 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/about/hyabsa.yaml
+-rw-r--r--   0        0        0      158 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/agent/__init__.yaml
+-rw-r--r--   0        0        0      158 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/agent/absa.yaml
+-rw-r--r--   0        0        0       64 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/agent/gpt4.yaml
+-rw-r--r--   0        0        0       51 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/llm/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/llm/gpt35.yaml
+-rw-r--r--   0        0        0       80 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/llm/gpt4.yaml
+-rw-r--r--   0        0        0      111 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/llm/openai.yaml
+-rw-r--r--   0        0        0       64 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/prompts/__init__.yaml
+-rw-r--r--   0        0        0     2975 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/prompts/default.yaml
+-rw-r--r--   0        0        0      448 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/runner/absa.yaml
+-rw-r--r--   0        0        0       51 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/conf/runner/gpt4.yaml
+-rw-r--r--   0        0        0      108 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/contexts/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-03 02:11:41.103427 hyfi_absa-0.3.0/src/hyabsa/llms/__init__.py
+-rw-r--r--   0        0        0     3041 2023-08-03 02:11:41.107427 hyfi_absa-0.3.0/src/hyabsa/llms/openai.py
+-rw-r--r--   0        0        0      744 2023-08-03 02:11:41.107427 hyfi_absa-0.3.0/src/hyabsa/prompts/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 02:11:41.107427 hyfi_absa-0.3.0/src/hyabsa/py.typed
+-rw-r--r--   0        0        0       62 2023-08-03 02:11:41.107427 hyfi_absa-0.3.0/src/hyabsa/runners/__init__.py
+-rw-r--r--   0        0        0     2990 2023-08-03 02:11:41.107427 hyfi_absa-0.3.0/src/hyabsa/runners/absa.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 hyfi_absa-0.3.0/PKG-INFO
```

### Comparing `hyfi_absa-0.2.0/LICENSE` & `hyfi_absa-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.2.0/README.md` & `hyfi_absa-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.2.0/pyproject.toml` & `hyfi_absa-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "hyfi-absa"
-version = "0.2.0"
+version = "0.3.0"
 description = "HyFI-ABSA is a Python package developed as a plugin for the Hydra Fast Interface (HyFI)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-absa.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-absa"
 readme = "README.md"
 packages = [{ include = "hyabsa", from = "src" }]
 
 [tool.poetry.scripts]
 hyabsa = 'hyabsa.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.17.0"
+hyfi = "^1.17.2"
 backoff = "^2.2.1"
 openai = "^0.27.8"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `hyfi_absa-0.2.0/src/hyabsa/agents/absa.py` & `hyfi_absa-0.3.0/src/hyabsa/agents/absa.py`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.2.0/src/hyabsa/agents/base.py` & `hyfi_absa-0.3.0/src/hyabsa/agents/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import json
 from typing import Optional
 
 from hyfi.composer import BaseModel
 
 from hyabsa import HyFI
 from hyabsa.contexts import ChatMessage
@@ -28,22 +29,23 @@
     @property
     def model(self) -> str:
         return self.llm.model.replace(".", "")
 
     @property
     def output_filepath(self) -> str:
         ouput_filename = (
-            self.output_filename or f"{self.task}_{self.prompt}_{self.model}.jsonl"
+            self.output_filename
+            or f"{self.task}_{self.prompt}_{self.model}_{datetime.datetime.now().strftime('%Y%m%d')}.jsonl"
         )
         HyFI.mkdir(self.output_dir)
         return f"{self.output_dir}/{ouput_filename}"
 
     def build_message(self, text: str) -> ChatMessage:
         return ChatMessage(content=self.prompts.build(text, self.task, self.prompt))
 
     def execute(self, text: str) -> str:
         result = AgentResult.from_chat_reponse(
-            self.llm.request(self.build_message(text))
+            self.llm.request(self.build_message(text)),
         )
         if self.output_filepath:
             HyFI.append_to_jsonl(result.model_dump(), self.output_filepath)
         return json.dumps(result.model_dump(), ensure_ascii=False)
```

### Comparing `hyfi_absa-0.2.0/src/hyabsa/conf/prompts/default.yaml` & `hyfi_absa-0.3.0/src/hyabsa/conf/prompts/default.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.2.0/src/hyabsa/llms/openai.py` & `hyfi_absa-0.3.0/src/hyabsa/llms/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     def initialize(self, api_key: Optional[str] = None):
         api_key = api_key or self.api_key
         denv = HyFI.dotenv()
         if not api_key and denv.OPENAI_API_KEY:
             api_key = denv.OPENAI_API_KEY.get_secret_value()
         if not api_key:
             raise ValueError("OpenAI API Key is required.")
+        openai.api_key = api_key
+        logger.info("OpenAI API Key is set successfully.")
         self._engine_ = openai.ChatCompletion()
         logger.info("OpenAI ChatCompletion API is initialized.")
 
     def build_config(self, message: ChatMessage) -> Dict[str, Any]:
         return ChatCompletionConfig(
             model=self.model,
             temperature=self.temperature,
```

### Comparing `hyfi_absa-0.2.0/src/hyabsa/prompts/__init__.py` & `hyfi_absa-0.3.0/src/hyabsa/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.2.0/src/hyabsa/runners/absa.py` & `hyfi_absa-0.3.0/src/hyabsa/runners/absa.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from hyabsa import HyFI
 from hyabsa.agents import AbsaAgent
 
 logger = HyFI.getLogger(__name__)
 
 
 class AbsaRunner(BaseRunner):
-    _config_group_: str = "runner"
     _config_name_: str = "absa"
     _auto_populate_: bool = True
 
+    task_name: str = "absa"
     agent: AbsaAgent = AbsaAgent()
     tasks: Optional[List[str]] = []
     data_load: RunConfig = RunConfig(_config_name_="load_dataset")
     data_save: RunConfig = RunConfig(_config_name_="save_dataset_to_disk")
 
     text_col: str = "bodyText"
     batch_size: int = 1000
     num_workers: int = 1
     remove_columns: Optional[Union[List[str], str]] = None
     load_from_cache_file: bool = True
+    top_n: Optional[int] = None
 
     _dataset: Optional[Dataset] = None
 
     @property
     def dataset(self) -> Dataset:
         if self._dataset is None:
             self._dataset = self.load_dataset()
@@ -38,59 +39,65 @@
         return HyFI.partial(self.data_load.config)()
 
     def save_dataset(self, dataset: Dataset) -> None:
         HyFI.partial(self.data_save.config)(dataset)
 
     def run(self):
         dataset = self.load_dataset()
+        if self.top_n is not None:
+            logger.info("Selecting top %s rows...", self.top_n)
+            dataset = dataset.select(range(self.top_n))
+
         tasks = self.tasks or ["QUAD"]
         for task in tasks:
-            logger.info("Predicting %s...", task)
+            logger.info(
+                "Predicting %s with a batch size of %s and %s workers...",
+                task,
+                self.batch_size,
+                self.num_workers,
+            )
             dataset = dataset.map(
                 batch_run,
                 batched=True,
                 batch_size=self.batch_size,
                 num_proc=self.num_workers,
                 fn_kwargs={
                     "task": task,
                     "agent": self.agent.model_copy(),
                     "text_col": self.text_col,
                 },
                 remove_columns=self.remove_columns,
                 load_from_cache_file=self.load_from_cache_file,
             )
         if self.verbose:
+            logger.info("Dataset shape: %s", dataset.shape)
+            logger.info("Dataset columns: %s", dataset.column_names)
             print(dataset[0])
         self.save_dataset(dataset)
 
 
 def batch_run(
     batch,
     task: str = "QUAD",
     agent: AbsaAgent = None,
     text_col: str = "bodyText",
 ) -> dict:
     if agent is None:
-        agent = {}
-    model = agent
-    model.task = task
-    if model.verbose:
-        print(model)
+        raise ValueError("Agent must be provided")
+    agent.task = task
+    if agent.verbose:
+        HyFI.print(agent.model_dump())
 
-    res = [execute_each(text, model) for text in batch[text_col]]
+    res = [execute_each(text, agent) for text in batch[text_col]]
     return {f"{task}_pred": res}
 
 
 def execute_each(
     text: str,
     agent: AbsaAgent,
 ) -> str:
     response = agent.execute(text)
     if agent.verbose:
-        logger.info(
-            "Task: %s | Text:\n%s\n | Response:\n%s\n",
-            agent.task,
-            text,
-            response,
-        )
+        # logger.info("Text: %s", text)
+        logger.info("Response: %s", response)
 
     return response
```

### Comparing `hyfi_absa-0.2.0/PKG-INFO` & `hyfi_absa-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hyfi-absa
-Version: 0.2.0
+Version: 0.3.0
 Summary: HyFI-ABSA is a Python package developed as a plugin for the Hydra Fast Interface (HyFI).
 Home-page: https://hyfi-absa.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: hyfi (>=1.17.0,<2.0.0)
+Requires-Dist: hyfi (>=1.17.2,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-absa
 Description-Content-Type: text/markdown
 
 # HyFI-ABSA
 
 [![pypi-image]][pypi-url]
```

