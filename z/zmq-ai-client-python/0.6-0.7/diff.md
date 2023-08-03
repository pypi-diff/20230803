# Comparing `tmp/zmq_ai_client_python-0.6.tar.gz` & `tmp/zmq_ai_client_python-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmq_ai_client_python-0.6.tar", last modified: Wed Aug  2 14:47:31 2023, max compression
+gzip compressed data, was "zmq_ai_client_python-0.7.tar", last modified: Wed Aug  2 14:54:25 2023, max compression
```

## Comparing `zmq_ai_client_python-0.6.tar` & `zmq_ai_client_python-0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:47:31.320721 zmq_ai_client_python-0.6/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      252 2023-08-02 14:47:31.320721 zmq_ai_client_python-0.6/PKG-INFO
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      429 2023-08-02 08:28:16.000000 zmq_ai_client_python-0.6/README.md
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       38 2023-08-02 14:47:31.320721 zmq_ai_client_python-0.6/setup.cfg
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      493 2023-08-02 14:47:10.000000 zmq_ai_client_python-0.6/setup.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:47:31.320721 zmq_ai_client_python-0.6/zmq_ai_client_python/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      184 2023-08-02 10:27:31.000000 zmq_ai_client_python-0.6/zmq_ai_client_python/__init__.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)     1081 2023-08-02 07:19:04.000000 zmq_ai_client_python-0.6/zmq_ai_client_python/client.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      548 2023-08-02 07:19:19.000000 zmq_ai_client_python-0.6/zmq_ai_client_python/client_test.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:47:31.320721 zmq_ai_client_python-0.6/zmq_ai_client_python/schema/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      716 2023-08-02 07:22:19.000000 zmq_ai_client_python-0.6/zmq_ai_client_python/schema/completion.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      830 2023-08-01 14:14:59.000000 zmq_ai_client_python-0.6/zmq_ai_client_python/schema/request.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:47:31.320721 zmq_ai_client_python-0.6/zmq_ai_client_python.egg-info/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      252 2023-08-02 14:47:31.000000 zmq_ai_client_python-0.6/zmq_ai_client_python.egg-info/PKG-INFO
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      418 2023-08-02 14:47:31.000000 zmq_ai_client_python-0.6/zmq_ai_client_python.egg-info/SOURCES.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)        1 2023-08-02 14:47:31.000000 zmq_ai_client_python-0.6/zmq_ai_client_python.egg-info/dependency_links.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       14 2023-08-02 14:47:31.000000 zmq_ai_client_python-0.6/zmq_ai_client_python.egg-info/requires.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       21 2023-08-02 14:47:31.000000 zmq_ai_client_python-0.6/zmq_ai_client_python.egg-info/top_level.txt
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:54:25.795780 zmq_ai_client_python-0.7/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      252 2023-08-02 14:54:25.795780 zmq_ai_client_python-0.7/PKG-INFO
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      429 2023-08-02 08:28:16.000000 zmq_ai_client_python-0.7/README.md
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       38 2023-08-02 14:54:25.795780 zmq_ai_client_python-0.7/setup.cfg
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      493 2023-08-02 14:54:22.000000 zmq_ai_client_python-0.7/setup.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:54:25.795780 zmq_ai_client_python-0.7/zmq_ai_client_python/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      187 2023-08-02 14:53:16.000000 zmq_ai_client_python-0.7/zmq_ai_client_python/__init__.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)     1083 2023-08-02 14:52:57.000000 zmq_ai_client_python-0.7/zmq_ai_client_python/client.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      551 2023-08-02 14:48:52.000000 zmq_ai_client_python-0.7/zmq_ai_client_python/client_test.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:54:25.795780 zmq_ai_client_python-0.7/zmq_ai_client_python/schema/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      711 2023-08-02 14:52:33.000000 zmq_ai_client_python-0.7/zmq_ai_client_python/schema/completion.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      830 2023-08-02 14:52:45.000000 zmq_ai_client_python-0.7/zmq_ai_client_python/schema/request.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:54:25.795780 zmq_ai_client_python-0.7/zmq_ai_client_python.egg-info/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      252 2023-08-02 14:54:25.000000 zmq_ai_client_python-0.7/zmq_ai_client_python.egg-info/PKG-INFO
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      418 2023-08-02 14:54:25.000000 zmq_ai_client_python-0.7/zmq_ai_client_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)        1 2023-08-02 14:54:25.000000 zmq_ai_client_python-0.7/zmq_ai_client_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       14 2023-08-02 14:54:25.000000 zmq_ai_client_python-0.7/zmq_ai_client_python.egg-info/requires.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       21 2023-08-02 14:54:25.000000 zmq_ai_client_python-0.7/zmq_ai_client_python.egg-info/top_level.txt
```

### Comparing `zmq_ai_client_python-0.6/zmq_ai_client_python/client.py` & `zmq_ai_client_python-0.7/zmq_ai_client_python/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import msgpack
 import zmq
 from dataclasses import asdict
-from schema.completion import Completion, CompletionChoice
-from schema.request import Request
+from .schema.completion import Completion, CompletionChoice
+from .schema.request import Request
 
 
 
 class LlamaClient:
 
     def __init__(self, host: str):
         self.context = zmq.Context()
```

### Comparing `zmq_ai_client_python-0.6/zmq_ai_client_python/client_test.py` & `zmq_ai_client_python-0.7/zmq_ai_client_python/client_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from client import LlamaClient
-from schema.completion import Completion
-from schema.request import Message,Request
+from .client import LlamaClient
+from .schema.completion import Completion
+from .schema.request import Message,Request
 
 def main():
     client = LlamaClient('tcp://localhost:5555')
 
     messages = [
         Message(role='system', content='You are a helpful assistant.'),
         Message(role='user', content='What is the capital of france?'),
```

### Comparing `zmq_ai_client_python-0.6/zmq_ai_client_python/schema/completion.py` & `zmq_ai_client_python-0.7/zmq_ai_client_python/schema/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import List, Optional, Dict, Literal
-from schema.request import Message
+from .request import Message
+
 
 @dataclass
 class CompletionLogprobs:
     text_offset: List[int]
     token_logprobs: List[Optional[float]]
     tokens: List[str]
     top_logprobs: List[Optional[Dict[str, float]]]
```

### Comparing `zmq_ai_client_python-0.6/zmq_ai_client_python/schema/request.py` & `zmq_ai_client_python-0.7/zmq_ai_client_python/schema/request.py`

 * *Files identical despite different names*

