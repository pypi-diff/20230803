# Comparing `tmp/lenio-ai-prompt-engineer-1.0.0.tar.gz` & `tmp/lenio-ai-prompt-engineer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenio-ai-prompt-engineer-1.0.0.tar", last modified: Thu Aug  3 19:29:53 2023, max compression
+gzip compressed data, was "lenio-ai-prompt-engineer-1.0.1.tar", last modified: Thu Aug  3 20:10:07 2023, max compression
```

## Comparing `lenio-ai-prompt-engineer-1.0.0.tar` & `lenio-ai-prompt-engineer-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.029008 lenio-ai-prompt-engineer-1.0.0/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-03 19:29:53.028149 lenio-ai-prompt-engineer-1.0.0/PKG-INFO
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1808 2023-07-28 15:29:57.000000 lenio-ai-prompt-engineer-1.0.0/README.md
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.001335 lenio-ai-prompt-engineer-1.0.0/cli/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        0 2023-07-27 15:34:24.000000 lenio-ai-prompt-engineer-1.0.0/cli/__init__.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.006454 lenio-ai-prompt-engineer-1.0.0/cli/evals/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       98 2023-08-01 21:09:44.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/__init__.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3880 2023-08-03 14:02:57.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/classification.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7932 2023-08-03 14:03:13.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/elovalue.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3755 2023-08-03 14:03:27.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/equal.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3763 2023-08-03 14:03:43.000000 lenio-ai-prompt-engineer-1.0.0/cli/evals/includes.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1419 2023-08-03 14:14:51.000000 lenio-ai-prompt-engineer-1.0.0/cli/generation.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     6664 2023-08-03 19:21:25.000000 lenio-ai-prompt-engineer-1.0.0/cli/main.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.018794 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      254 2023-08-02 14:59:15.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/__init__.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1175 2023-08-03 16:41:52.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/grammatical_errors.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 23:12:10.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/lowercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:17.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/random_lowercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:27.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/random_lowercase_word.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:12.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/random_uppercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:22.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/random_uppercase_word.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1110 2023-08-03 18:30:27.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/synonymous_prompt.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 22:44:08.000000 lenio-ai-prompt-engineer-1.0.0/cli/promptChange/uppercase.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 19:29:53.025964 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      791 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        1 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       59 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       44 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/requires.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        4 2023-08-03 19:29:52.000000 lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/top_level.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       38 2023-08-03 19:29:53.029342 lenio-ai-prompt-engineer-1.0.0/setup.cfg
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      388 2023-08-03 18:27:34.000000 lenio-ai-prompt-engineer-1.0.0/setup.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 20:10:07.717607 lenio-ai-prompt-engineer-1.0.1/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-03 20:10:07.717020 lenio-ai-prompt-engineer-1.0.1/PKG-INFO
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1808 2023-07-28 15:29:57.000000 lenio-ai-prompt-engineer-1.0.1/README.md
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 20:10:07.696162 lenio-ai-prompt-engineer-1.0.1/cli/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        0 2023-07-27 15:34:24.000000 lenio-ai-prompt-engineer-1.0.1/cli/__init__.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 20:10:07.700287 lenio-ai-prompt-engineer-1.0.1/cli/evals/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       98 2023-08-01 21:09:44.000000 lenio-ai-prompt-engineer-1.0.1/cli/evals/__init__.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3880 2023-08-03 14:02:57.000000 lenio-ai-prompt-engineer-1.0.1/cli/evals/classification.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7932 2023-08-03 14:03:13.000000 lenio-ai-prompt-engineer-1.0.1/cli/evals/elovalue.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3755 2023-08-03 14:03:27.000000 lenio-ai-prompt-engineer-1.0.1/cli/evals/equal.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3763 2023-08-03 14:03:43.000000 lenio-ai-prompt-engineer-1.0.1/cli/evals/includes.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1396 2023-08-03 19:35:10.000000 lenio-ai-prompt-engineer-1.0.1/cli/generation.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     6664 2023-08-03 19:21:25.000000 lenio-ai-prompt-engineer-1.0.1/cli/main.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 20:10:07.708378 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      254 2023-08-02 14:59:15.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/__init__.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1175 2023-08-03 16:41:52.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/grammatical_errors.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 23:12:10.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/lowercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:17.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/random_lowercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:27.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/random_lowercase_word.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:12.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/random_uppercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:22.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/random_uppercase_word.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1110 2023-08-03 18:30:27.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/synonymous_prompt.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 22:44:08.000000 lenio-ai-prompt-engineer-1.0.1/cli/promptChange/uppercase.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-03 20:10:07.715901 lenio-ai-prompt-engineer-1.0.1/lenio_ai_prompt_engineer.egg-info/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-03 20:10:07.000000 lenio-ai-prompt-engineer-1.0.1/lenio_ai_prompt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      791 2023-08-03 20:10:07.000000 lenio-ai-prompt-engineer-1.0.1/lenio_ai_prompt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        1 2023-08-03 20:10:07.000000 lenio-ai-prompt-engineer-1.0.1/lenio_ai_prompt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       59 2023-08-03 20:10:07.000000 lenio-ai-prompt-engineer-1.0.1/lenio_ai_prompt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       44 2023-08-03 20:10:07.000000 lenio-ai-prompt-engineer-1.0.1/lenio_ai_prompt_engineer.egg-info/requires.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        4 2023-08-03 20:10:07.000000 lenio-ai-prompt-engineer-1.0.1/lenio_ai_prompt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       38 2023-08-03 20:10:07.717929 lenio-ai-prompt-engineer-1.0.1/setup.cfg
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      388 2023-08-03 20:10:05.000000 lenio-ai-prompt-engineer-1.0.1/setup.py
```

### Comparing `lenio-ai-prompt-engineer-1.0.0/README.md` & `lenio-ai-prompt-engineer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.0.0/cli/evals/classification.py` & `lenio-ai-prompt-engineer-1.0.1/cli/evals/classification.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.0.0/cli/evals/elovalue.py` & `lenio-ai-prompt-engineer-1.0.1/cli/evals/elovalue.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.0.0/cli/evals/equal.py` & `lenio-ai-prompt-engineer-1.0.1/cli/evals/equal.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.0.0/cli/evals/includes.py` & `lenio-ai-prompt-engineer-1.0.1/cli/evals/includes.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.0.0/cli/generation.py` & `lenio-ai-prompt-engineer-1.0.1/cli/generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,8 @@
                 ],
             temperature=candidate_model_temperature,
             n=number_of_prompts)
 
         prompts = []
         for i in outputs.choices:
             prompts.append(i.message.content)
-        print(prompts)
         return prompts
```

### Comparing `lenio-ai-prompt-engineer-1.0.0/cli/main.py` & `lenio-ai-prompt-engineer-1.0.1/cli/main.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.0.0/cli/promptChange/grammatical_errors.py` & `lenio-ai-prompt-engineer-1.0.1/cli/promptChange/grammatical_errors.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.0.0/cli/promptChange/synonymous_prompt.py` & `lenio-ai-prompt-engineer-1.0.1/cli/promptChange/synonymous_prompt.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.0.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt` & `lenio-ai-prompt-engineer-1.0.1/lenio_ai_prompt_engineer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

