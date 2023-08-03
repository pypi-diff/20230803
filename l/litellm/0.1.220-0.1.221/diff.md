# Comparing `tmp/litellm-0.1.220.tar.gz` & `tmp/litellm-0.1.221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.220.tar", last modified: Thu Aug  3 02:49:28 2023, max compression
+gzip compressed data, was "litellm-0.1.221.tar", last modified: Thu Aug  3 05:26:24 2023, max compression
```

## Comparing `litellm-0.1.220.tar` & `litellm-0.1.221.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 02:49:28.325632 litellm-0.1.220/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.220/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 02:49:28.325515 litellm-0.1.220/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.220/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 02:49:28.324558 litellm-0.1.220/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      935 2023-08-03 02:30:45.000000 litellm-0.1.220/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11177 2023-08-03 02:43:44.000000 litellm-0.1.220/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.220/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    14200 2023-08-02 20:27:13.000000 litellm-0.1.220/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 02:49:28.325320 litellm-0.1.220/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 02:49:28.000000 litellm-0.1.220/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.220/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 02:49:28.325685 litellm-0.1.220/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 02:48:48.000000 litellm-0.1.220/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 05:26:24.034352 litellm-0.1.221/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-03 05:26:12.000000 litellm-0.1.221/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 05:26:24.034352 litellm-0.1.221/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-08-03 05:26:12.000000 litellm-0.1.221/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 05:26:24.030351 litellm-0.1.221/litellm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      969 2023-08-03 05:26:12.000000 litellm-0.1.221/litellm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11192 2023-08-03 05:26:12.000000 litellm-0.1.221/litellm/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2546 2023-08-03 05:26:12.000000 litellm-0.1.221/litellm/timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14924 2023-08-03 05:26:12.000000 litellm-0.1.221/litellm/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 05:26:24.034352 litellm-0.1.221/litellm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 05:26:23.000000 litellm-0.1.221/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-08-03 05:26:24.000000 litellm-0.1.221/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 05:26:23.000000 litellm-0.1.221/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-08-03 05:26:23.000000 litellm-0.1.221/litellm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-03 05:26:23.000000 litellm-0.1.221/litellm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-03 05:26:12.000000 litellm-0.1.221/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-03 05:26:24.034352 litellm-0.1.221/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      407 2023-08-03 05:26:12.000000 litellm-0.1.221/setup.py
```

### Comparing `litellm-0.1.220/LICENSE` & `litellm-0.1.221/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.220/README.md` & `litellm-0.1.221/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.220/litellm/__init__.py` & `litellm-0.1.221/litellm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 success_callback = []
 failure_callback = []
 set_verbose=False
 telemetry=True
-
+max_tokens = 256 # OpenAI Defaults
 ####### PROXY PARAMS ################### configurable params if you use proxy models like Helicone
 api_base = None
 headers = None
 ####### COMPLETION MODELS ###################
 open_ai_chat_completion_models = [
   'gpt-3.5-turbo', 
   'gpt-4',
```

### Comparing `litellm-0.1.220/litellm/main.py` & `litellm-0.1.221/litellm/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
           prompt += f"{HUMAN_PROMPT}{message['content']}"
       prompt += f"{AI_PROMPT}"
       anthropic = Anthropic()
       # check if user passed in max_tokens != float('inf')
       if max_tokens != float('inf'):
         max_tokens_to_sample = max_tokens
       else:
-        max_tokens_to_sample = 300 # default in Anthropic docs https://docs.anthropic.com/claude/reference/client-libraries
+        max_tokens_to_sample = litellm.max_tokens # default in Anthropic docs https://docs.anthropic.com/claude/reference/client-libraries
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
       ## COMPLETION CALL
       completion = anthropic.completions.create(
             model=model,
             prompt=prompt,
             max_tokens_to_sample=max_tokens_to_sample
```

### Comparing `litellm-0.1.220/litellm/timeout.py` & `litellm-0.1.221/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.220/litellm/utils.py` & `litellm-0.1.221/litellm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import dotenv, json, traceback, threading
 import subprocess, os 
 import litellm, openai 
 import random, uuid, requests
+import datetime
 from openai.error import AuthenticationError, InvalidRequestError, RateLimitError, ServiceUnavailableError, OpenAIError
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 sentry_sdk_instance = None
 capture_exception = None
 add_breadcrumb = None
 posthog = None
 slack_app = None
 alerts_channel = None
+heliconeLogger = None
 callback_list = []
 user_logger_fn = None
 additional_details = {}
 
 def print_verbose(print_statement):
   if litellm.set_verbose:
     print(f"LiteLLM: {print_statement}")
@@ -64,44 +66,46 @@
 # make it easy to log if completion/embedding runs succeeded or failed + see what happened | Non-Blocking
 def client(original_function):
     def function_setup(*args, **kwargs): #just run once to check if user wants to send their data anywhere - PostHog/Sentry/Slack/etc.
       try: 
         global callback_list, add_breadcrumb
         if (len(litellm.success_callback) > 0 or len(litellm.failure_callback) > 0) and len(callback_list) == 0: 
           callback_list = list(set(litellm.success_callback + litellm.failure_callback))
-          set_callbacks(callback_list=callback_list)
+          set_callbacks(callback_list=callback_list,)
         if add_breadcrumb:
           add_breadcrumb(
                 category="litellm.llm_call",
                 message=f"Positional Args: {args}, Keyword Args: {kwargs}",
                 level="info",
             )
       except: # DO NOT BLOCK running the function because of this
         print_verbose(f"[Non-Blocking] {traceback.format_exc()}")
       pass
 
     def wrapper(*args, **kwargs):
         try:
           function_setup(args, kwargs)
           ## MODEL CALL
+          start_time = datetime.datetime.now()
           result = original_function(*args, **kwargs)
+          end_time = datetime.datetime.now()
           ## LOG SUCCESS 
-          my_thread = threading.Thread(target=handle_success, args=(args, kwargs)) # don't interrupt execution of main thread
+          my_thread = threading.Thread(target=handle_success, args=(args, kwargs, result, start_time, end_time)) # don't interrupt execution of main thread
           my_thread.start()
           return result
         except Exception as e:
           traceback_exception = traceback.format_exc()
           my_thread = threading.Thread(target=handle_failure, args=(e, traceback_exception, args, kwargs)) # don't interrupt execution of main thread
           my_thread.start()
           raise e
     return wrapper
 
 ####### HELPER FUNCTIONS ################
 def set_callbacks(callback_list):
-  global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel
+  global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel, heliconeLogger
   try:
     for callback in callback_list:
       if callback == "sentry":
         try:
             import sentry_sdk
         except ImportError:
             print_verbose("Package 'sentry_sdk' is missing. Installing it...")
@@ -130,14 +134,18 @@
             from slack_bolt import App
         slack_app = App(
           token=os.environ.get("SLACK_API_TOKEN"),
           signing_secret=os.environ.get("SLACK_API_SECRET")
         )
         alerts_channel = os.environ["SLACK_API_CHANNEL"]
         print_verbose(f"Initialized Slack App: {slack_app}")
+      elif callback == "helicone":
+        from .integrations.helicone import HeliconeLogger
+
+        heliconeLogger = HeliconeLogger()
   except:
     pass
 
 
 def handle_failure(exception, traceback_exception, args, kwargs):
     global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel
     try:
@@ -196,15 +204,16 @@
           "additional_details": additional_details
         }
         failure_handler(call_details)
       pass
     except:
       pass
 
-def handle_success(*args, **kwargs):
+def handle_success(args, kwargs, result, start_time, end_time):
+  global heliconeLogger
   try:
     success_handler = additional_details.pop("success_handler", None)
     failure_handler = additional_details.pop("failure_handler", None)
     additional_details["Event_Name"] = additional_details.pop("successful_event_name", "litellm.succes_query")
     for callback in litellm.success_callback:
       try:
         if callback == "posthog":
@@ -219,14 +228,19 @@
             posthog.capture(unique_id, event_name, ph_obj)
           pass
         elif callback == "slack":
           slack_msg = "" 
           for detail in additional_details: 
             slack_msg += f"{detail}: {additional_details[detail]}\n"
           slack_app.client.chat_postMessage(channel=alerts_channel, text=slack_msg)
+        elif callback == "helicone":
+          print_verbose("reaches helicone for logging!")
+          model = args[0] if len(args) > 0 else kwargs["model"]
+          messages = args[1] if len(args) > 1 else kwargs["messages"]
+          heliconeLogger.log_success(model=model, messages=messages, response_obj=result, start_time=start_time, end_time=end_time)
       except:
         pass
 
     if success_handler and callable(success_handler):
       success_handler(args, kwargs)
     pass
   except:
```

