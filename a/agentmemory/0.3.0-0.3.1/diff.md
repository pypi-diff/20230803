# Comparing `tmp/agentmemory-0.3.0.tar.gz` & `tmp/agentmemory-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.3.0.tar", last modified: Thu Aug  3 07:36:11 2023, max compression
+gzip compressed data, was "agentmemory-0.3.1.tar", last modified: Thu Aug  3 07:40:31 2023, max compression
```

## Comparing `agentmemory-0.3.0.tar` & `agentmemory-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:36:11.034008 agentmemory-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 07:35:56.000000 agentmemory-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-03 07:36:11.034008 agentmemory-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-08-03 07:35:56.000000 agentmemory-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:36:11.034008 agentmemory-0.3.0/agentmemory/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:36:11.034008 agentmemory-0.3.0/agentmemory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:36:11.034008 agentmemory-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 07:35:56.000000 agentmemory-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:40:31.530713 agentmemory-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 07:40:20.000000 agentmemory-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-03 07:40:31.530713 agentmemory-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-08-03 07:40:20.000000 agentmemory-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:40:31.526713 agentmemory-0.3.1/agentmemory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:40:31.530713 agentmemory-0.3.1/agentmemory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:40:31.530713 agentmemory-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 07:40:20.000000 agentmemory-0.3.1/setup.py
```

### Comparing `agentmemory-0.3.0/LICENSE` & `agentmemory-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.0/PKG-INFO` & `agentmemory-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.3.0
+Version: 0.3.1
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/AutonomousResearchGroup/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentmemory-0.3.0/README.md` & `agentmemory-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.0/agentmemory/__init__.py` & `agentmemory-0.3.1/agentmemory/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,23 @@
     delete_memories,
     delete_similar_memories,
     count_memories,
     wipe_category,
     wipe_all_memories,
 )
 
+from .events import (
+    create_event,
+    get_epoch,
+    get_events,
+    increment_epoch,
+    reset_epoch,
+    set_epoch,
+)
+
 from .helpers import (
     chroma_collection_to_list,
     list_to_chroma_collection,
 )
 
 from .persistence import (
     export_memory_to_json,
@@ -48,8 +57,14 @@
     "export_memory_to_json",
     "export_memory_to_file",
     "import_json_to_memory",
     "import_file_to_memory",
     "get_chroma_client",
     "set_chroma_client",
     "get_persistent_directory",
+    "create_event",
+    "get_epoch",
+    "get_events",
+    "increment_epoch",
+    "reset_epoch",
+    "set_epoch",
 ]
```

### Comparing `agentmemory-0.3.0/agentmemory/client.py` & `agentmemory-0.3.1/agentmemory/client.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.0/agentmemory/events.py` & `agentmemory-0.3.1/agentmemory/events.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.0/agentmemory/helpers.py` & `agentmemory-0.3.1/agentmemory/helpers.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.0/agentmemory/main.py` & `agentmemory-0.3.1/agentmemory/main.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.0/agentmemory/persistence.py` & `agentmemory-0.3.1/agentmemory/persistence.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.0/agentmemory.egg-info/PKG-INFO` & `agentmemory-0.3.1/agentmemory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.3.0
+Version: 0.3.1
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/AutonomousResearchGroup/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentmemory-0.3.0/setup.py` & `agentmemory-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.3.0',
+    version='0.3.1',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/AutonomousResearchGroup/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

