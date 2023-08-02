# Comparing `tmp/run_one-1.0.8.tar.gz` & `tmp/run_one-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.0.8.tar", max compression
+gzip compressed data, was "run_one-1.0.9.tar", max compression
```

## Comparing `run_one-1.0.8.tar` & `run_one-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-26 13:54:21.921189 run_one-1.0.8/LICENSE
--rw-r--r--   0        0        0     1708 2023-07-26 13:54:21.921189 run_one-1.0.8/README.md
--rw-r--r--   0        0        0      740 2023-07-26 13:54:21.921189 run_one-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      345 2023-07-26 13:54:21.921189 run_one-1.0.8/run_one/__init__.py
--rw-r--r--   0        0        0      282 2023-07-26 13:54:21.921189 run_one-1.0.8/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     1916 2023-07-26 13:54:21.921189 run_one-1.0.8/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1182 2023-07-26 13:54:21.921189 run_one-1.0.8/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     3391 2023-07-26 13:54:21.921189 run_one-1.0.8/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0        0 2023-07-26 13:54:21.921189 run_one-1.0.8/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2023-07-26 13:54:21.925189 run_one-1.0.8/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2023-07-26 13:54:21.925189 run_one-1.0.8/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2023-07-26 13:54:21.925189 run_one-1.0.8/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-26 13:54:21.925189 run_one-1.0.8/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     5608 2023-07-26 13:54:21.925189 run_one-1.0.8/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2023-07-26 13:54:21.925189 run_one-1.0.8/run_one/util/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-26 13:54:21.925189 run_one-1.0.8/run_one/util/config.py
--rw-r--r--   0        0        0     3474 2023-07-26 13:54:21.925189 run_one-1.0.8/run_one/util/util.py
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 run_one-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-27 20:18:40.668017 run_one-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1708 2023-07-27 20:18:40.668017 run_one-1.0.9/README.md
+-rw-r--r--   0        0        0      740 2023-07-27 20:18:40.668017 run_one-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      345 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     1916 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1182 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     3391 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0        0 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     5608 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/util/config.py
+-rw-r--r--   0        0        0     3461 2023-07-27 20:18:40.668017 run_one-1.0.9/run_one/util/util.py
+-rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 run_one-1.0.9/PKG-INFO
```

### Comparing `run_one-1.0.8/LICENSE` & `run_one-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.0.8/README.md` & `run_one-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `run_one-1.0.8/pyproject.toml` & `run_one-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.0.8"
+version = "1.0.9"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
```

### Comparing `run_one-1.0.8/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.0.9/run_one/action_handlers/TH2ActHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.8/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.0.9/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.8/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.0.9/run_one/action_handlers/TH2Check1Handler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.8/run_one/processors/abstract_processor.py` & `run_one-1.0.9/run_one/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.8/run_one/processors/th2_processor.py` & `run_one-1.0.9/run_one/processors/th2_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.8/run_one/util/config.py` & `run_one-1.0.9/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.8/run_one/util/util.py` & `run_one-1.0.9/run_one/util/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import ast
 from collections import defaultdict
 from datetime import datetime
 from itertools import tee
-import json
 from typing import Callable
 import uuid
 
 import pandas as pd
 
 from run_one.util.config import Config
 
@@ -72,15 +72,15 @@
             row.dropna(inplace=True)
             extracted_fields = row.get([field for field in config.fields_to_extract if field in row], [])
             row.drop(config.fields_to_drop + config.fields_to_extract, errors='ignore', inplace=True)
             row.rename(config.field_mapping, inplace=True)
 
             for field in config.nested_fields:
                 if field in row and row[field] != '*':
-                    row[field] = json.loads(row[field].replace("'", '"'))
+                    row[field] = ast.literal_eval(row[field])
 
             if id_function is not None:
                 for field in config.regenerate_id_fields:
                     if field in row and row[field] != '*':
                         field_value = row[field]
                         if field_value.startswith('!='):
                             key = field_value[2:]
```

### Comparing `run_one-1.0.8/PKG-INFO` & `run_one-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

