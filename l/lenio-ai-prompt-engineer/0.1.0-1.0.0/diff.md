# Comparing `tmp/lenio-ai-prompt-engineer-0.1.0.tar.gz` & `tmp/lenio-ai-prompt-engineer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenio-ai-prompt-engineer-0.1.0.tar", last modified: Thu Aug  3 14:14:55 2023, max compression
+gzip compressed data, was "lenio-ai-prompt-engineer-1.0.0.tar", last modified: Thu Aug  3 19:29:53 2023, max compression
```

## Comparing `lenio-ai-prompt-engineer-0.1.0.tar` & `lenio-ai-prompt-engineer-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 14:14:54.998370 lenio-ai-prompt-engineer-0.1.0/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-03 14:14:54.997650 lenio-ai-prompt-engineer-0.1.0/PKG-INFO
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1808 2023-07-28 15:29:57.000000 lenio-ai-prompt-engineer-0.1.0/README.md
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 14:14:54.974177 lenio-ai-prompt-engineer-0.1.0/cli/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        0 2023-07-27 15:34:24.000000 lenio-ai-prompt-engineer-0.1.0/cli/__init__.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 14:14:54.980417 lenio-ai-prompt-engineer-0.1.0/cli/evals/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       98 2023-08-01 21:09:44.000000 lenio-ai-prompt-engineer-0.1.0/cli/evals/__init__.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3880 2023-08-03 14:02:57.000000 lenio-ai-prompt-engineer-0.1.0/cli/evals/classification.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7932 2023-08-03 14:03:13.000000 lenio-ai-prompt-engineer-0.1.0/cli/evals/elovalue.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3755 2023-08-03 14:03:27.000000 lenio-ai-prompt-engineer-0.1.0/cli/evals/equal.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3763 2023-08-03 14:03:43.000000 lenio-ai-prompt-engineer-0.1.0/cli/evals/includes.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     2622 2023-08-03 13:57:57.000000 lenio-ai-prompt-engineer-0.1.0/cli/evals/test.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1419 2023-08-03 14:14:51.000000 lenio-ai-prompt-engineer-0.1.0/cli/generation.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     6538 2023-08-03 14:10:10.000000 lenio-ai-prompt-engineer-0.1.0/cli/main.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 14:14:54.990547 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      254 2023-08-02 14:59:15.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/__init__.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1174 2023-08-02 16:07:22.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/grammatical_errors.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 23:12:10.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/lowercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:17.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/random_lowercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:27.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/random_lowercase_word.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:12.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/random_uppercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:22.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/random_uppercase_word.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1082 2023-08-02 15:26:27.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/synonymous_prompt.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 22:44:08.000000 lenio-ai-prompt-engineer-0.1.0/cli/promptChange/uppercase.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 14:14:54.996426 lenio-ai-prompt-engineer-0.1.0/lenio_ai_prompt_engineer.egg-info/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-03 14:14:54.000000 lenio-ai-prompt-engineer-0.1.0/lenio_ai_prompt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      809 2023-08-03 14:14:54.000000 lenio-ai-prompt-engineer-0.1.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        1 2023-08-03 14:14:54.000000 lenio-ai-prompt-engineer-0.1.0/lenio_ai_prompt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       59 2023-08-03 14:14:54.000000 lenio-ai-prompt-engineer-0.1.0/lenio_ai_prompt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       44 2023-08-03 14:14:54.000000 lenio-ai-prompt-engineer-0.1.0/lenio_ai_prompt_engineer.egg-info/requires.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        4 2023-08-03 14:14:54.000000 lenio-ai-prompt-engineer-0.1.0/lenio_ai_prompt_engineer.egg-info/top_level.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       38 2023-08-03 14:14:54.998803 lenio-ai-prompt-engineer-0.1.0/setup.cfg
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      403 2023-08-01 21:36:24.000000 lenio-ai-prompt-engineer-0.1.0/setup.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.029008 lenio-ai-prompt-engineer-1.0.0/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-03 19:29:53.028149 lenio-ai-prompt-engineer-1.0.0/PKG-INFO
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1808 2023-07-28 15:29:57.000000 lenio-ai-prompt-engineer-1.0.0/README.md
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.001335 lenio-ai-prompt-engineer-1.0.0/cli/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        0 2023-07-27 15:34:24.000000 lenio-ai-prompt-engineer-1.0.0/cli/__init__.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.006454 lenio-ai-prompt-engineer-1.0.0/cli/evals/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       98 2023-08-01 21:09:44.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/__init__.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3880 2023-08-03 14:02:57.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/classification.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7932 2023-08-03 14:03:13.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/elovalue.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3755 2023-08-03 14:03:27.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/equal.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3763 2023-08-03 14:03:43.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/includes.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1419 2023-08-03 14:14:51.000000 lenio-ai-prompt-engineer-1.0.0/cli/generation.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     6664 2023-08-03 19:21:25.000000 lenio-ai-prompt-engineer-1.0.0/cli/main.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.018794 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      254 2023-08-02 14:59:15.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/__init__.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1175 2023-08-03 16:41:52.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/grammatical_errors.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 23:12:10.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/lowercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:17.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/random_lowercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:27.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/random_lowercase_word.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:12.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/random_uppercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:22.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/random_uppercase_word.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1110 2023-08-03 18:30:27.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/synonymous_prompt.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 22:44:08.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/uppercase.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.025964 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      791 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        1 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       59 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       44 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/requires.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        4 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       38 2023-08-03 19:29:53.029342 lenio-ai-prompt-engineer-1.0.0/setup.cfg
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      388 2023-08-03 18:27:34.000000 lenio-ai-prompt-engineer-1.0.0/setup.py
```

### Comparing `lenio-ai-prompt-engineer-0.1.0/README.md` & `lenio-ai-prompt-engineer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-0.1.0/cli/evals/classification.py` & `lenio-ai-prompt-engineer-1.0.0/cli/evals/classification.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-0.1.0/cli/evals/elovalue.py` & `lenio-ai-prompt-engineer-1.0.0/cli/evals/elovalue.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-0.1.0/cli/evals/equal.py` & `lenio-ai-prompt-engineer-1.0.0/cli/evals/equal.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-0.1.0/cli/evals/includes.py` & `lenio-ai-prompt-engineer-1.0.0/cli/evals/includes.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-0.1.0/cli/generation.py` & `lenio-ai-prompt-engineer-1.0.0/cli/generation.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-0.1.0/cli/main.py` & `lenio-ai-prompt-engineer-1.0.0/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     candidate_model = yaml_content[block_name]['candidate_model']
     candidate_model_temperature = yaml_content[block_name]['candidate_model_temperature']
     generation_model = yaml_content[block_name]['generation_model']
     generation_model_temperature = yaml_content[block_name]['generation_model_temperature']
     generation_model_max_tokens = yaml_content[block_name]['generation_model_max_tokens']
     prompt_change = yaml_content[block_name]['prompt_change']
     method = yaml_content[block_name]['method']
+    #if 'iterations' in yaml_content[block_name]['iterations']:
+        #iterations = yaml_content[block_name]['iterations']
 
     if method == 'elovalue.Elo':
         class_method = elovalue.Elo
     elif method == 'classification.Classification':
         class_method = classification.Classification
     elif method == 'equal.Equal':
         class_method = equal.Equal
@@ -81,14 +83,15 @@
         elif change == 'grammatical_errors':
             prompts_value = grammatical_errors.convert_prompts(prompts_value)
 
     evaluable_object = class_method(description, test_cases, number_of_prompts, generation_model, generation_model_temperature, generation_model_max_tokens, candidate_model, candidate_model_temperature, prompts_value)
     
     # Evaluate the prompts
     results = evaluable_object.evaluate_optimal_prompt()
+
     
     yaml_folder = os.path.dirname(file)
     # Full path of the output.json file in the same folder as the YAML
     output_json_path = os.path.join(yaml_folder, "output.json")
     # Convert the result to JSON format and save it to the output.json file
     with open(output_json_path, "w") as json_file:
         json.dump(results, json_file)
```

### Comparing `lenio-ai-prompt-engineer-0.1.0/cli/promptChange/grammatical_errors.py` & `lenio-ai-prompt-engineer-1.0.0/cli/promptChange/grammatical_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import openai
 
 def grammatical_errors_prompt(string):
     x = openai.ChatCompletion.create(
                     model='gpt-3.5-turbo',
                     messages=[
                         {"role": "system", "content": """Your job is to generate changes to a "system prompt" for GPT. Said changes will consist of changing some words that you consider for others with grammatical errors without changing the meaning of the original prompt. 
-                         The prompt tells you to do tasks but you don't have to do the tasks, just change words from the prompt for others with misspellings. You will receive a prompt and you only have to return the content of the prompt with the changes with grammatical errors that you have made and nothing else"""},
+                         The prompt tells you to do tasks but you don't have to do the tasks, just change words from the prompt for others with misspellings. You will receive a prompt and you only have to return the content of the prompt with the changes with grammatical errors that you have made and nothing else."""},
                         {"role": "user", "content": string}
                     ],
                     max_tokens=500,
                     temperature=0.8,
                 ).choices[0].message.content
     return x
```

### Comparing `lenio-ai-prompt-engineer-0.1.0/cli/promptChange/synonymous_prompt.py` & `lenio-ai-prompt-engineer-1.0.0/cli/promptChange/synonymous_prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import openai
 
 def synonym(string):
     x = openai.ChatCompletion.create(
                     model='gpt-3.5-turbo',
                     messages=[
-                        {"role": "system", "content": """Your job is to generate changes to a system prompt for GPT. These changes will consist of changing some words that you consider synonymous without changing the meaning of the original prompt. 
-                        The prompt tells you to do tasks but you don't have to do the tasks, just change words from the prompt to synonyms. You will receive a prompt and you only have to return the content of the prompt with the synonymous changes that you have made and nothing else"""},
+                        {"role": "system", "content": """Your job is to generate changes in a system prompt for GPT. These changes will consist of changing some words that you consider synonymous without changing the meaning of the original message.
+                        The prompt prompts you to do tasks, but you don't have to do them, just change the prompt words to synonyms or rephrase without changing the original meaning. You will receive a notice and you only have to return the content of the notice with the changes you have made and nothing else."""},
                         {"role": "user", "content": string}
                     ],
                     max_tokens=500,
                     temperature=0.8,
                 ).choices[0].message.content
     return x
```

### Comparing `lenio-ai-prompt-engineer-0.1.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt` & `lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 cli/generation.py
 cli/main.py
 cli/evals/__init__.py
 cli/evals/classification.py
 cli/evals/elovalue.py
 cli/evals/equal.py
 cli/evals/includes.py
-cli/evals/test.py
 cli/promptChange/__init__.py
 cli/promptChange/grammatical_errors.py
 cli/promptChange/lowercase.py
 cli/promptChange/random_lowercase.py
 cli/promptChange/random_lowercase_word.py
 cli/promptChange/random_uppercase.py
 cli/promptChange/random_uppercase_word.py
```

