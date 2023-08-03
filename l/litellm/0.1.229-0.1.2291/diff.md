# Comparing `tmp/litellm-0.1.229.tar.gz` & `tmp/litellm-0.1.2291.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.229.tar", last modified: Thu Aug  3 21:02:10 2023, max compression
+gzip compressed data, was "litellm-0.1.2291.tar", last modified: Thu Aug  3 21:04:36 2023, max compression
```

## Comparing `litellm-0.1.229.tar` & `litellm-0.1.2291.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:02:10.335166 litellm-0.1.229/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.229/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 21:02:10.335052 litellm-0.1.229/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.229/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:02:10.333507 litellm-0.1.229/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1231 2023-08-03 21:01:57.000000 litellm-0.1.229/litellm/__init__.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:02:10.334757 litellm-0.1.229/litellm/integrations/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       15 2023-08-03 15:30:17.000000 litellm-0.1.229/litellm/integrations/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3548 2023-08-03 15:22:44.000000 litellm-0.1.229/litellm/integrations/helicone.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    12069 2023-08-03 20:51:32.000000 litellm-0.1.229/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2893 2023-08-03 16:40:54.000000 litellm-0.1.229/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    15221 2023-08-03 17:14:57.000000 litellm-0.1.229/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:02:10.334380 litellm-0.1.229/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 21:02:10.000000 litellm-0.1.229/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      333 2023-08-03 21:02:10.000000 litellm-0.1.229/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 21:02:10.000000 litellm-0.1.229/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       80 2023-08-03 21:02:10.000000 litellm-0.1.229/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 21:02:10.000000 litellm-0.1.229/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.229/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 21:02:10.335209 litellm-0.1.229/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      546 2023-08-03 21:02:08.000000 litellm-0.1.229/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:04:36.333102 litellm-0.1.2291/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.2291/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      152 2023-08-03 21:04:36.332961 litellm-0.1.2291/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.2291/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:04:36.331304 litellm-0.1.2291/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1201 2023-08-03 21:03:40.000000 litellm-0.1.2291/litellm/__init__.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:04:36.332623 litellm-0.1.2291/litellm/integrations/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       15 2023-08-03 15:30:17.000000 litellm-0.1.2291/litellm/integrations/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3548 2023-08-03 15:22:44.000000 litellm-0.1.2291/litellm/integrations/helicone.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    12068 2023-08-03 21:04:08.000000 litellm-0.1.2291/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2893 2023-08-03 16:40:54.000000 litellm-0.1.2291/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    15221 2023-08-03 17:14:57.000000 litellm-0.1.2291/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:04:36.332194 litellm-0.1.2291/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      152 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      333 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       80 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.2291/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 21:04:36.333147 litellm-0.1.2291/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      547 2023-08-03 21:04:34.000000 litellm-0.1.2291/setup.py
```

### Comparing `litellm-0.1.229/LICENSE` & `litellm-0.1.2291/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.229/README.md` & `litellm-0.1.2291/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.229/litellm/__init__.py` & `litellm-0.1.2291/litellm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,12 +37,11 @@
 
 model_list = open_ai_chat_completion_models + open_ai_text_completion_models + cohere_models + anthropic_models
 
 ####### EMBEDDING MODELS ###################
 open_ai_embedding_models = [
     'text-embedding-ada-002'
 ]
-from .main import acompletion
 from .timeout import timeout
 from .utils import client, logging, exception_type  # Import all the symbols from main.py
 from .main import *  # Import all the symbols from main.py
 from .integrations import *
```

### Comparing `litellm-0.1.229/litellm/integrations/helicone.py` & `litellm-0.1.2291/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.229/litellm/main.py` & `litellm-0.1.2291/litellm/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,23 @@
       optional_params["user"] = user
   if deployment_id != None:
       optional_params["deployment_id"] = user
   return optional_params
 
 ####### COMPLETION ENDPOINTS ################
 #############################################
+async def acompletion(*args, **kwargs):
+  loop = asyncio.get_event_loop()
+  
+  # Use a partial function to pass your keyword arguments
+  func = partial(completion, *args, **kwargs)
+
+  # Call the synchronous function using run_in_executor
+  return await loop.run_in_executor(None, func)
+
 @client
 @retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(2), reraise=True, retry_error_callback=lambda retry_state: setattr(retry_state.outcome, 'retry_variable', litellm.retry)) # retry call, turn this off by setting `litellm.retry = False`
 @timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
 def completion(
     model, messages, # required params
     # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
     functions=[], function_call="", # optional params
@@ -254,24 +263,14 @@
     return response
   except Exception as e:
     # log the original exception
     logging(model=model, input=messages, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn, exception=e)
     ## Map to OpenAI Exception
     raise exception_type(model=model, original_exception=e)
 
-
-async def acompletion(*args, **kwargs):
-  loop = asyncio.get_event_loop()
-  
-  # Use a partial function to pass your keyword arguments
-  func = partial(completion, *args, **kwargs)
-
-  # Call the synchronous function using run_in_executor
-  return await loop.run_in_executor(None, func)
-
 ### EMBEDDING ENDPOINTS ####################
 @client
 @timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
 def embedding(model, input=[], azure=False, force_timeout=60, logger_fn=None):
   try:
     response = None
     if azure == True:
```

### Comparing `litellm-0.1.229/litellm/timeout.py` & `litellm-0.1.2291/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.229/litellm/utils.py` & `litellm-0.1.2291/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.229/setup.py` & `litellm-0.1.2291/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='litellm',
-    version='0.1.229',
+    version='0.1.2291',
     description='Library to easily interface with LLM API providers',
     author='BerriAI',
     packages=[
         'litellm'
     ],
     package_data={
         "litellm": ["integrations/*"],  # Specify the directory path relative to your package
```

