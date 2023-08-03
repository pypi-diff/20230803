# Comparing `tmp/easycompletion-0.3.5.tar.gz` & `tmp/easycompletion-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.3.5.tar", last modified: Mon Jul 31 21:30:55 2023, max compression
+gzip compressed data, was "easycompletion-0.3.6.tar", last modified: Thu Aug  3 05:54:32 2023, max compression
```

## Comparing `easycompletion-0.3.5.tar` & `easycompletion-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:30:55.776633 easycompletion-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 21:30:45.000000 easycompletion-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 21:30:55.776633 easycompletion-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-31 21:30:45.000000 easycompletion-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:30:55.776633 easycompletion-0.3.5/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:30:55.776633 easycompletion-0.3.5/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:30:55.776633 easycompletion-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 21:30:45.000000 easycompletion-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:54:32.375574 easycompletion-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 05:54:20.000000 easycompletion-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-03 05:54:32.375574 easycompletion-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-08-03 05:54:20.000000 easycompletion-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:54:32.375574 easycompletion-0.3.6/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:54:32.375574 easycompletion-0.3.6/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 05:54:32.375574 easycompletion-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-03 05:54:20.000000 easycompletion-0.3.6/setup.py
```

### Comparing `easycompletion-0.3.5/LICENSE` & `easycompletion-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.5/PKG-INFO` & `easycompletion-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.5
+Version: 0.3.6
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.3.5/README.md` & `easycompletion-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.5/easycompletion/__init__.py` & `easycompletion-0.3.6/easycompletion/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .model import (
     function_completion,
     text_completion,
-    compose_function,
     chat_completion
 )
 
 openai_function_call = function_completion
 openai_text_call = text_completion
 
 from .prompt import (
     compose_prompt,
     trim_prompt,
     chunk_prompt,
     count_tokens,
+    compose_function,
     get_tokens,
 )
 
 from .constants import (
     DEFAULT_TEXT_MODEL,
     DEFAULT_CHUNK_LENGTH,
 )
```

### Comparing `easycompletion-0.3.5/easycompletion/constants.py` & `easycompletion-0.3.6/easycompletion/constants.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.5/easycompletion/logger.py` & `easycompletion-0.3.6/easycompletion/logger.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.5/easycompletion/model.py` & `easycompletion-0.3.6/easycompletion/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 
     Returns:
         True if function call matches with the response, False otherwise.
 
     Usage:
         isValid = validate_functions(response, functions, function_call)
     """
+    print('response')
+    print(response)
     response_function_call = response["choices"][0]["message"].get(
         "function_call", None
     )
     if response_function_call is None:
         log(f"No function call in response\n{response}", type="error", log=debug)
         return False
 
@@ -149,69 +151,28 @@
 
         return False
 
     log("Function call is valid", type="success", log=debug)
     return True
 
 
-def compose_function(name, description, properties, required_properties, debug=DEBUG):
-    """
-    Composes a function object for function calling.
-
-    Parameters:
-        name (str): The name of the function.
-        description (str): Description of the function.
-        properties (dict): Dictionary of property objects.
-        required_properties (list): List of property names that are required.
-
-    Returns:
-        A dictionary representing a function.
-
-    Usage:
-        summarization_function = compose_function(
-            name="summarize_text",
-            description="Summarize the text. Include the topic, subtopics.",
-            properties={
-                "summary": {
-                    "type": "string",
-                    "description": "Detailed summary of the text.",
-                },
-            },
-            required_properties=["summary"],
-        )
-    """
-    function = {
-        "name": name,
-        "description": description,
-        "parameters": {
-            "type": "object",
-            "properties": properties,
-            "required": required_properties,
-        },
-    }
-    log(f"Function:\n{str(function)}", type="info", log=debug)
-    return function
-
-
 def chat_completion(
     messages,
-    system_message=None,
     model_failure_retries=5,
     model=None,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     api_key=None,
     debug=DEBUG,
-    temperature=0.0
+    temperature=0.0,
 ):
     """
     Function for sending chat messages and returning a chat response.
 
     Parameters:
         messages (str): Messages to send to the model. In the form {<role>: string, <content>: string} - roles are "user" and "assistant"
-        system_message (str, optional): Message appended at the top sent by the system. Usually used to tell what the agent how to act.
         model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
         model (str, optional): The model to use. Default is the DEFAULT_TEXT_MODEL defined in constants.py.
         chunk_length (int, optional): Maximum length of text chunk to process. Default is defined in constants.py.
         api_key (str, optional): OpenAI API key. If not provided, it uses the one defined in constants.py.
 
     Returns:
         str: The response content from the model.
@@ -245,30 +206,27 @@
         return {
             "text": None,
             "usage": None,
             "finish_reason": None,
             "error": "Message too long",
         }
 
-    # Prepare messages for the API call
-    messages = [{"role": "system", "content": system_message}] + messages
-
     log(f"Prompt:\n{str(messages)}", type="prompt", log=debug)
 
     # Try to make a request for a specified number of times
     response = None
     for i in range(model_failure_retries):
         try:
-            response = openai.ChatCompletion.create(model=model, messages=messages, temperature=temperature)
+            response = openai.ChatCompletion.create(
+                model=model, messages=messages, temperature=temperature
+            )
             break
         except Exception as e:
             log(f"OpenAI Error: {e}", type="error", log=debug)
             continue
-        # wait 1 second
-        time.sleep(1)
 
     # If response is not valid, print an error message and return None
     if (
         response is None
         or response["choices"] is None
         or response["choices"][0] is None
     ):
@@ -295,15 +253,15 @@
 def text_completion(
     text,
     model_failure_retries=5,
     model=None,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     api_key=None,
     debug=DEBUG,
-    temperature=0.0
+    temperature=0.0,
 ):
     """
     Function for sending text and returning a text completion response.
 
     Parameters:
         text (str): Text to send to the model.
         model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
@@ -352,15 +310,17 @@
 
     log(f"Prompt:\n{text}", type="prompt", log=debug)
 
     # Try to make a request for a specified number of times
     response = None
     for i in range(model_failure_retries):
         try:
-            response = openai.ChatCompletion.create(model=model, messages=messages, temperature=temperature)
+            response = openai.ChatCompletion.create(
+                model=model, messages=messages, temperature=temperature
+            )
             break
         except Exception as e:
             log(f"OpenAI Error: {e}", type="error", log=debug)
             continue
         # wait 1 second
         time.sleep(1)
 
@@ -387,26 +347,26 @@
         "usage": usage,
         "finish_reason": finish_reason,
         "error": None,
     }
 
 
 def function_completion(
-    text,
-    system_message=None,
+    text=None,
     messages=None,
+    system_message=None,
     functions=None,
     model_failure_retries=5,
     function_call=None,
     function_failure_retries=10,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     model=None,
     api_key=None,
     debug=DEBUG,
-    temperature=0.0
+    temperature=0.0,
 ):
     """
     Send text and a list of functions to the model and return optional text and a function call.
     The function call is validated against the functions array.
     The input text is sent to the chat model and is treated as a user message.
 
     Args:
@@ -520,15 +480,16 @@
     if system_message is not None:
         all_messages.append({"role": "system", "content": system_message})
 
     if messages is not None:
         all_messages += messages
 
     # Prepare the messages to be sent to the API
-    all_messages.append({"role": "user", "content": text})
+    if text is not None and text != "":
+        all_messages.append({"role": "user", "content": text})
 
     log(
         f"Prompt:\n{text}\n\nFunctions:\n{json.dumps(functions, indent=4)}",
         type="prompt",
         log=debug,
     )
 
@@ -539,23 +500,34 @@
             try:
                 # If there are function(s) to call
                 response = openai.ChatCompletion.create(
                     model=model,
                     messages=all_messages,
                     functions=functions,
                     function_call=function_call,
-                    temperature=temperature
+                    temperature=temperature,
                 )
+                print('***** openai response')
+                print(response)
                 if not response.get("choices") or response["choices"][0] is None:
                     log("No choices in response", type="error", log=debug)
                     continue
                 break
             except Exception as e:
+                print('**** ERROR')
+                print(e)
                 log(f"OpenAI Error: {e}", type="error", log=debug)
             time.sleep(1)
+        # Check if we have a valid response from the model
+        print('***** response')
+        print(response)
+        print('***** functions')
+        print(functions)
+        print('***** function_call')
+        print(function_call)
         if validate_functions(response, functions, function_call):
             break
         time.sleep(1)
 
     # Check if we have a valid response from the model
     if response is None:
         error = "Could not get a successful response from the model. Check your API key and arguments."
```

### Comparing `easycompletion-0.3.5/easycompletion/prompt.py` & `easycompletion-0.3.6/easycompletion/prompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -180,7 +180,47 @@
                 raise Exception(f"ERROR PARSING:\n{key}\n{value}")
         except:
             raise Exception(f"ERROR PARSING:\n{key}\n{value}")
 
     log(f"Composed prompt:\n{prompt}", log=debug)
 
     return prompt
+
+
+def compose_function(name, description, properties, required_properties, debug=DEBUG):
+    """
+    Composes a function object for function calling.
+
+    Parameters:
+        name (str): The name of the function.
+        description (str): Description of the function.
+        properties (dict): Dictionary of property objects.
+        required_properties (list): List of property names that are required.
+
+    Returns:
+        A dictionary representing a function.
+
+    Usage:
+        summarization_function = compose_function(
+            name="summarize_text",
+            description="Summarize the text. Include the topic, subtopics.",
+            properties={
+                "summary": {
+                    "type": "string",
+                    "description": "Detailed summary of the text.",
+                },
+            },
+            required_properties=["summary"],
+        )
+    """
+    function = {
+        "name": name,
+        "description": description,
+        "parameters": {
+            "type": "object",
+            "properties": properties,
+            "required": required_properties,
+        },
+    }
+    log(f"Function:\n{str(function)}", type="info", log=debug)
+    return function
+
```

### Comparing `easycompletion-0.3.5/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.3.6/easycompletion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.5
+Version: 0.3.6
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.3.5/setup.py` & `easycompletion-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.3.5',
+    version='0.3.6',
     description="Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

