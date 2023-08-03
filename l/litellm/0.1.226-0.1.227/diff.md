# Comparing `tmp/litellm-0.1.226.tar.gz` & `tmp/litellm-0.1.227.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.226.tar", last modified: Thu Aug  3 15:34:11 2023, max compression
+gzip compressed data, was "litellm-0.1.227.tar", last modified: Thu Aug  3 19:03:12 2023, max compression
```

## Comparing `litellm-0.1.226.tar` & `litellm-0.1.227.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:34:11.016290 litellm-0.1.226/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.226/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:34:11.016167 litellm-0.1.226/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.226/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:34:11.014765 litellm-0.1.226/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      995 2023-08-03 15:30:01.000000 litellm-0.1.226/litellm/__init__.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:34:11.015846 litellm-0.1.226/litellm/integrations/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       15 2023-08-03 15:30:17.000000 litellm-0.1.226/litellm/integrations/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3548 2023-08-03 15:22:44.000000 litellm-0.1.226/litellm/integrations/helicone.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11192 2023-08-03 02:58:28.000000 litellm-0.1.226/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.226/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    15221 2023-08-03 15:33:53.000000 litellm-0.1.226/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:34:11.015480 litellm-0.1.226/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      333 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.226/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 15:34:11.016343 litellm-0.1.226/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      527 2023-08-03 15:34:08.000000 litellm-0.1.226/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 19:03:12.662376 litellm-0.1.227/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-03 19:02:55.000000 litellm-0.1.227/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 19:03:12.662376 litellm-0.1.227/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-03 19:02:55.000000 litellm-0.1.227/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 19:03:12.662376 litellm-0.1.227/litellm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1202 2023-08-03 19:02:55.000000 litellm-0.1.227/litellm/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 19:03:12.662376 litellm-0.1.227/litellm/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-08-03 19:02:55.000000 litellm-0.1.227/litellm/integrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2023-08-03 19:02:55.000000 litellm-0.1.227/litellm/integrations/helicone.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11805 2023-08-03 19:02:55.000000 litellm-0.1.227/litellm/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-08-03 19:02:55.000000 litellm-0.1.227/litellm/timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15221 2023-08-03 19:02:55.000000 litellm-0.1.227/litellm/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 19:03:12.662376 litellm-0.1.227/litellm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 19:03:12.000000 litellm-0.1.227/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-08-03 19:03:12.000000 litellm-0.1.227/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 19:03:12.000000 litellm-0.1.227/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-08-03 19:03:12.000000 litellm-0.1.227/litellm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-03 19:03:12.000000 litellm-0.1.227/litellm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-03 19:02:55.000000 litellm-0.1.227/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-03 19:03:12.662376 litellm-0.1.227/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-08-03 19:02:55.000000 litellm-0.1.227/setup.py
```

### Comparing `litellm-0.1.226/LICENSE` & `litellm-0.1.227/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.226/README.md` & `litellm-0.1.227/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.226/litellm/integrations/helicone.py` & `litellm-0.1.227/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.226/litellm/main.py` & `litellm-0.1.227/litellm/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 import traceback
 import dotenv
 import traceback
 import litellm
 from litellm import client, logging, exception_type, timeout, success_callback, failure_callback
 import random
+import asyncio
+from tenacity import (
+    retry,
+    stop_after_attempt,
+    wait_random_exponential,
+)  # for exponential backoff
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
 def get_optional_params(
     # 12 optional params
     functions = [],
     function_call = "",
@@ -51,23 +57,24 @@
   if user != "":
       optional_params["user"] = user
   return optional_params
 
 ####### COMPLETION ENDPOINTS ################
 #############################################
 @client
+@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(2), reraise=True, retry_error_callback=lambda retry_state: setattr(retry_state.outcome, 'retry_variable', litellm.retry)) # retry call, turn this off by setting `litellm.retry = False`
 @timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
 def completion(
     model, messages, # required params
     # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
     functions=[], function_call="", # optional params
     temperature=1, top_p=1, n=1, stream=False, stop=None, max_tokens=float('inf'),
     presence_penalty=0, frequency_penalty=0, logit_bias={}, user="",
     # Optional liteLLM function params
-    *, api_key=None, force_timeout=60, azure=False, logger_fn=None, verbose=False
+    *, return_async=False, api_key=None, force_timeout=60, azure=False, logger_fn=None, verbose=False
   ):
   try:
     # check if user passed in any of the OpenAI optional params
     optional_params = get_optional_params(
       functions=functions, function_call=function_call, 
       temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
       presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user
@@ -244,14 +251,20 @@
   except Exception as e:
     # log the original exception
     logging(model=model, input=messages, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn, exception=e)
     ## Map to OpenAI Exception
     raise exception_type(model=model, original_exception=e)
 
 
+async def acompletion(*args, **kwargs):
+  loop = asyncio.get_event_loop()
+  
+  # Call the synchronous function using run_in_executor()
+  return loop.run_in_executor(None, completion, *args, **kwargs)
+
 ### EMBEDDING ENDPOINTS ####################
 @client
 @timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
 def embedding(model, input=[], azure=False, force_timeout=60, logger_fn=None):
   try:
     response = None
     if azure == True:
```

### Comparing `litellm-0.1.226/litellm/timeout.py` & `litellm-0.1.227/litellm/timeout.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,34 +33,37 @@
         def wrapper(*args, **kwargs):
             async def async_func():
                 return func(*args, **kwargs)
 
             thread = _LoopWrapper()
             thread.start()
             future = asyncio.run_coroutine_threadsafe(async_func(), thread.loop)
+            local_timeout_duration = timeout_duration
+            if "force_timeout" in kwargs:
+                local_timeout_duration = kwargs["force_timeout"]
             try:
-                local_timeout_duration = timeout_duration
-                if "force_timeout" in kwargs:
-                    local_timeout_duration = kwargs["force_timeout"]
                 result = future.result(timeout=local_timeout_duration)
             except futures.TimeoutError:
                 thread.stop_loop()
-                raise exception_to_raise()
+                raise exception_to_raise(f"A timeout error occurred. The function call took longer than {local_timeout_duration} second(s).")
             thread.stop_loop()
             return result
 
         @wraps(func)
         async def async_wrapper(*args, **kwargs):
+            local_timeout_duration = timeout_duration
+            if "force_timeout" in kwargs:
+                local_timeout_duration = kwargs["force_timeout"]
             try:
                 value = await asyncio.wait_for(
                     func(*args, **kwargs), timeout=timeout_duration
                 )
                 return value
             except asyncio.TimeoutError:
-                raise exception_to_raise()
+                raise exception_to_raise(f"A timeout error occurred. The function call took longer than {local_timeout_duration} second(s).")
 
         if iscoroutinefunction(func):
             return async_wrapper
         return wrapper
 
     return decorator
```

### Comparing `litellm-0.1.226/litellm/utils.py` & `litellm-0.1.227/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.226/setup.py` & `litellm-0.1.227/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='litellm',
-    version='0.1.226',
+    version='0.1.227',
     description='Library to easily interface with LLM API providers',
     author='BerriAI',
     packages=[
         'litellm'
     ],
     package_data={
         "litellm": ["integrations/*"],  # Specify the directory path relative to your package
@@ -15,9 +15,10 @@
         'openai',
         'cohere',
         'pytest',
         'anthropic',
         'replicate',
         'python-dotenv',
         'openai[datalib]',
+        'tenacity'
     ],
 )
```

