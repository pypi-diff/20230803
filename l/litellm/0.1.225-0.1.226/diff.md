# Comparing `tmp/litellm-0.1.225.tar.gz` & `tmp/litellm-0.1.226.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.225.tar", last modified: Thu Aug  3 15:24:08 2023, max compression
+gzip compressed data, was "litellm-0.1.226.tar", last modified: Thu Aug  3 15:34:11 2023, max compression
```

## Comparing `litellm-0.1.225.tar` & `litellm-0.1.226.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:24:08.596813 litellm-0.1.225/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.225/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:24:08.596684 litellm-0.1.225/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.225/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:24:08.595636 litellm-0.1.225/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      969 2023-08-03 02:58:58.000000 litellm-0.1.225/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11192 2023-08-03 02:58:28.000000 litellm-0.1.225/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.225/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    15073 2023-08-03 15:17:43.000000 litellm-0.1.225/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:24:08.596494 litellm-0.1.225/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:24:08.000000 litellm-0.1.225/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 15:24:08.000000 litellm-0.1.225/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 15:24:08.000000 litellm-0.1.225/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 15:24:08.000000 litellm-0.1.225/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 15:24:08.000000 litellm-0.1.225/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.225/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 15:24:08.596869 litellm-0.1.225/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 15:23:59.000000 litellm-0.1.225/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:34:11.016290 litellm-0.1.226/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.226/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:34:11.016167 litellm-0.1.226/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.226/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:34:11.014765 litellm-0.1.226/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      995 2023-08-03 15:30:01.000000 litellm-0.1.226/litellm/__init__.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:34:11.015846 litellm-0.1.226/litellm/integrations/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       15 2023-08-03 15:30:17.000000 litellm-0.1.226/litellm/integrations/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3548 2023-08-03 15:22:44.000000 litellm-0.1.226/litellm/integrations/helicone.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11192 2023-08-03 02:58:28.000000 litellm-0.1.226/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.226/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    15221 2023-08-03 15:33:53.000000 litellm-0.1.226/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 15:34:11.015480 litellm-0.1.226/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      333 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 15:34:10.000000 litellm-0.1.226/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.226/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 15:34:11.016343 litellm-0.1.226/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      527 2023-08-03 15:34:08.000000 litellm-0.1.226/setup.py
```

### Comparing `litellm-0.1.225/LICENSE` & `litellm-0.1.226/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.225/README.md` & `litellm-0.1.226/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.225/litellm/__init__.py` & `litellm-0.1.226/litellm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 open_ai_embedding_models = [
     'text-embedding-ada-002'
 ]
 
 from .timeout import timeout
 from .utils import client, logging, exception_type  # Import all the symbols from main.py
 from .main import *  # Import all the symbols from main.py
-
+from .integrations import *
```

### Comparing `litellm-0.1.225/litellm/main.py` & `litellm-0.1.226/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.225/litellm/timeout.py` & `litellm-0.1.226/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.225/litellm/utils.py` & `litellm-0.1.226/litellm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,20 +235,22 @@
           slack_app.client.chat_postMessage(channel=alerts_channel, text=slack_msg)
         elif callback == "helicone":
           print_verbose("reaches helicone for logging!")
           model = args[0] if len(args) > 0 else kwargs["model"]
           messages = args[1] if len(args) > 1 else kwargs["messages"]
           heliconeLogger.log_success(model=model, messages=messages, response_obj=result, start_time=start_time, end_time=end_time, print_verbose=print_verbose)
       except:
+        print_verbose(f"Success Callback Error - {traceback.format_exc()}")
         pass
 
     if success_handler and callable(success_handler):
       success_handler(args, kwargs)
     pass
   except:
+    print_verbose(f"Success Callback Error - {traceback.format_exc()}")
     pass
 
 
 def exception_type(model, original_exception):
     try:
       if isinstance(original_exception, OpenAIError):
           # Handle the OpenAIError
```

