# Comparing `tmp/litellm-0.1.219.tar.gz` & `tmp/litellm-0.1.220.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.219.tar", last modified: Thu Aug  3 00:15:28 2023, max compression
+gzip compressed data, was "litellm-0.1.220.tar", last modified: Thu Aug  3 02:49:28 2023, max compression
```

## Comparing `litellm-0.1.219.tar` & `litellm-0.1.220.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 00:15:28.401855 litellm-0.1.219/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.219/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 00:15:28.401729 litellm-0.1.219/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.219/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 00:15:28.400778 litellm-0.1.219/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      804 2023-08-03 00:14:48.000000 litellm-0.1.219/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    10353 2023-08-02 21:49:41.000000 litellm-0.1.219/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.219/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    14200 2023-08-02 20:27:13.000000 litellm-0.1.219/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 00:15:28.401556 litellm-0.1.219/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.219/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 00:15:28.401896 litellm-0.1.219/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 00:15:26.000000 litellm-0.1.219/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 02:49:28.325632 litellm-0.1.220/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.220/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 02:49:28.325515 litellm-0.1.220/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.220/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 02:49:28.324558 litellm-0.1.220/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      935 2023-08-03 02:30:45.000000 litellm-0.1.220/litellm/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11177 2023-08-03 02:43:44.000000 litellm-0.1.220/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.220/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    14200 2023-08-02 20:27:13.000000 litellm-0.1.220/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 02:49:28.325320 litellm-0.1.220/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.220/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 02:49:28.325685 litellm-0.1.220/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 02:48:48.000000 litellm-0.1.220/setup.py
```

### Comparing `litellm-0.1.219/LICENSE` & `litellm-0.1.220/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.219/README.md` & `litellm-0.1.220/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.219/litellm/__init__.py` & `litellm-0.1.220/litellm/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 success_callback = []
 failure_callback = []
 set_verbose=False
 telemetry=True
+
+####### PROXY PARAMS ################### configurable params if you use proxy models like Helicone
+api_base = None
+headers = None
 ####### COMPLETION MODELS ###################
 open_ai_chat_completion_models = [
   'gpt-3.5-turbo', 
   'gpt-4',
   'gpt-3.5-turbo-16k-0613',
   'gpt-3.5-turbo-16k'
 ]
```

### Comparing `litellm-0.1.219/litellm/main.py` & `litellm-0.1.220/litellm/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,51 +71,74 @@
       functions=functions, function_call=function_call, 
       temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
       presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user
     )
     if azure == True:
       # azure configs
       openai.api_type = "azure"
-      openai.api_base = os.environ.get("AZURE_API_BASE")
+      openai.api_base = litellm.api_base if litellm.api_base is not None else os.environ.get("AZURE_API_BASE")
       openai.api_version = os.environ.get("AZURE_API_VERSION")
       openai.api_key = api_key if api_key is not None else os.environ.get("AZURE_API_KEY")
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
-      response = openai.ChatCompletion.create(
-        engine=model,
-        messages = messages,
-        **optional_params
-      )
+      if litellm.headers:
+         response = openai.ChatCompletion.create(
+            engine=model,
+            messages = messages,
+            headers = litellm.headers,
+            **optional_params,
+          )
+      else:
+        response = openai.ChatCompletion.create(
+          engine=model,
+          messages = messages,
+          **optional_params
+        )
     elif model in litellm.open_ai_chat_completion_models:
       openai.api_type = "openai"
-      openai.api_base = "https://api.openai.com/v1"
+      openai.api_base = litellm.api_base if litellm.api_base is not None else "https://api.openai.com/v1"
       openai.api_version = None
       openai.api_key = api_key if api_key is not None else os.environ.get("OPENAI_API_KEY")
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
-      response = openai.ChatCompletion.create(
-        model=model,
-        messages = messages,
-        **optional_params
-      )
+      if litellm.headers:
+         response = openai.ChatCompletion.create(
+          model=model,
+          messages = messages,
+          headers = litellm.headers,
+          **optional_params
+        )
+      else:
+        response = openai.ChatCompletion.create(
+          model=model,
+          messages = messages,
+          **optional_params
+        )
     elif model in litellm.open_ai_text_completion_models:
       openai.api_type = "openai"
-      openai.api_base = "https://api.openai.com/v1"
+      openai.api_base = litellm.api_base if litellm.api_base is not None else "https://api.openai.com/v1"
       openai.api_version = None
       openai.api_key = api_key if api_key is not None else os.environ.get("OPENAI_API_KEY")
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
-      response = openai.Completion.create(
+      if litellm.headers:
+        response = openai.Completion.create(
           model=model,
-          prompt = prompt
-      )
+          prompt = prompt,
+          headers = litellm.headers,
+        )
+      else:
+        response = openai.Completion.create(
+            model=model,
+            prompt = prompt
+        )
     elif "replicate" in model:
       # replicate defaults to os.environ.get("REPLICATE_API_TOKEN")
       # checking in case user set it to REPLICATE_API_KEY instead 
       if not os.environ.get("REPLICATE_API_TOKEN") and os.environ.get("REPLICATE_API_KEY"):
         replicate_api_token = os.environ.get("REPLICATE_API_KEY")
         os.environ["REPLICATE_API_TOKEN"] = replicate_api_token
       elif api_key:
@@ -167,18 +190,18 @@
         max_tokens_to_sample = max_tokens
       else:
         max_tokens_to_sample = 300 # default in Anthropic docs https://docs.anthropic.com/claude/reference/client-libraries
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
       ## COMPLETION CALL
       completion = anthropic.completions.create(
-          model=model,
-          prompt=prompt,
-          max_tokens_to_sample=max_tokens_to_sample
-      )
+            model=model,
+            prompt=prompt,
+            max_tokens_to_sample=max_tokens_to_sample
+        )
       new_response = {
         "choices": [
           {
             "finish_reason": "stop",
             "index": 0,
             "message": {
                 "content": completion.completion,
```

### Comparing `litellm-0.1.219/litellm/timeout.py` & `litellm-0.1.220/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.219/litellm/utils.py` & `litellm-0.1.220/litellm/utils.py`

 * *Files identical despite different names*

