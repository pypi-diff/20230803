# Comparing `tmp/litellm-0.1.218.tar.gz` & `tmp/litellm-0.1.219.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.218.tar", last modified: Wed Aug  2 21:55:06 2023, max compression
+gzip compressed data, was "litellm-0.1.219.tar", last modified: Thu Aug  3 00:15:28 2023, max compression
```

## Comparing `litellm-0.1.218.tar` & `litellm-0.1.219.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 21:55:06.441280 litellm-0.1.218/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.218/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 21:55:06.441156 litellm-0.1.218/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.218/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 21:55:06.440140 litellm-0.1.218/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      691 2023-08-02 20:51:39.000000 litellm-0.1.218/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    10353 2023-08-02 21:49:41.000000 litellm-0.1.218/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.218/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    14200 2023-08-02 20:27:13.000000 litellm-0.1.218/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 21:55:06.440934 litellm-0.1.218/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.218/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-02 21:55:06.441327 litellm-0.1.218/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-02 21:53:35.000000 litellm-0.1.218/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 00:15:28.401855 litellm-0.1.219/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.219/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 00:15:28.401729 litellm-0.1.219/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.219/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 00:15:28.400778 litellm-0.1.219/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      804 2023-08-03 00:14:48.000000 litellm-0.1.219/litellm/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    10353 2023-08-02 21:49:41.000000 litellm-0.1.219/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.219/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    14200 2023-08-02 20:27:13.000000 litellm-0.1.219/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 00:15:28.401556 litellm-0.1.219/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 00:15:28.000000 litellm-0.1.219/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.219/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 00:15:28.401896 litellm-0.1.219/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-03 00:15:26.000000 litellm-0.1.219/setup.py
```

### Comparing `litellm-0.1.218/LICENSE` & `litellm-0.1.219/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.218/README.md` & `litellm-0.1.219/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.218/litellm/__init__.py` & `litellm-0.1.219/litellm/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 ]
 
 anthropic_models = [
   "claude-2", 
   "claude-instant-1"
 ]
 
+model_list = open_ai_chat_completion_models + open_ai_text_completion_models + cohere_models + anthropic_models
+
 ####### EMBEDDING MODELS ###################
 open_ai_embedding_models = [
     'text-embedding-ada-002'
 ]
 
 from .timeout import timeout
 from .utils import client, logging, exception_type  # Import all the symbols from main.py
```

### Comparing `litellm-0.1.218/litellm/main.py` & `litellm-0.1.219/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.218/litellm/timeout.py` & `litellm-0.1.219/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.218/litellm/utils.py` & `litellm-0.1.219/litellm/utils.py`

 * *Files identical despite different names*

