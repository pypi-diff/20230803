# Comparing `tmp/agentmemory-0.3.1.tar.gz` & `tmp/agentmemory-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.3.1.tar", last modified: Thu Aug  3 07:40:31 2023, max compression
+gzip compressed data, was "agentmemory-0.3.2.tar", last modified: Thu Aug  3 07:48:12 2023, max compression
```

## Comparing `agentmemory-0.3.1.tar` & `agentmemory-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:40:31.530713 agentmemory-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 07:40:20.000000 agentmemory-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-03 07:40:31.530713 agentmemory-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-08-03 07:40:20.000000 agentmemory-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:40:31.526713 agentmemory-0.3.1/agentmemory/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-08-03 07:40:20.000000 agentmemory-0.3.1/agentmemory/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:40:31.530713 agentmemory-0.3.1/agentmemory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:40:31.000000 agentmemory-0.3.1/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:40:31.530713 agentmemory-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 07:40:20.000000 agentmemory-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:48:12.768981 agentmemory-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 07:48:03.000000 agentmemory-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-08-03 07:48:12.768981 agentmemory-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-08-03 07:48:03.000000 agentmemory-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:48:12.768981 agentmemory-0.3.2/agentmemory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-08-03 07:48:03.000000 agentmemory-0.3.2/agentmemory/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:48:12.768981 agentmemory-0.3.2/agentmemory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:48:12.000000 agentmemory-0.3.2/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:48:12.768981 agentmemory-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 07:48:03.000000 agentmemory-0.3.2/setup.py
```

### Comparing `agentmemory-0.3.1/LICENSE` & `agentmemory-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.1/PKG-INFO` & `agentmemory-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.3.1
+Version: 0.3.2
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/AutonomousResearchGroup/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -640,15 +640,15 @@
 
 ```python
 create_event("This is a test event", metadata={"test": "test"})
 ```
 
 ---
 
-## `get_events(epoch=None)`
+## `get_events(epoch=None, filter_metadata=None, n_results=10)`
 
 The `get_events` function retrieves events from the agent's memory.
 
 **Arguments:**
 
 - `epoch` (int, optional): If specified, only retrieve events from this epoch.
```

### Comparing `agentmemory-0.3.1/README.md` & `agentmemory-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -624,15 +624,15 @@
 
 ```python
 create_event("This is a test event", metadata={"test": "test"})
 ```
 
 ---
 
-## `get_events(epoch=None)`
+## `get_events(epoch=None, filter_metadata=None, n_results=10)`
 
 The `get_events` function retrieves events from the agent's memory.
 
 **Arguments:**
 
 - `epoch` (int, optional): If specified, only retrieve events from this epoch.
```

#### html2text {}

```diff
@@ -173,16 +173,16 @@
 (current_epoch) ``` --- ## `create_event(text, metadata={}, embedding=None)`
 The `create_event` function creates a new event in the agent's memory.
 **Arguments:** - `text` (str): The text content of the event. - `metadata`
 (dict, optional): Additional metadata for the event. Defaults to {}. -
 `embedding` (object, optional): An optional embedding for the event. **Usage:**
 ```python create_event(text, metadata={}, embedding=None) ``` **Example:**
 ```python create_event("This is a test event", metadata={"test": "test"}) ``` -
--- ## `get_events(epoch=None)` The `get_events` function retrieves events from
-the agent's memory. **Arguments:** - `epoch` (int, optional): If specified,
-only retrieve events from this epoch. **Usage:** ```python get_events
-(epoch=None) ``` **Example:** ```python events = get_events(1) for event in
-events: print(event["document"]) ``` # Contributions Welcome If you like this
-library and want to contribute in any way, please feel free to submit a PR and
-I will review it. Please note that the goal here is simplicity and
-accesibility, using common language and few dependencies. [resources/
-youcreatethefuture.jpg]
+-- ## `get_events(epoch=None, filter_metadata=None, n_results=10)` The
+`get_events` function retrieves events from the agent's memory. **Arguments:**
+- `epoch` (int, optional): If specified, only retrieve events from this epoch.
+**Usage:** ```python get_events(epoch=None) ``` **Example:** ```python events =
+get_events(1) for event in events: print(event["document"]) ``` # Contributions
+Welcome If you like this library and want to contribute in any way, please feel
+free to submit a PR and I will review it. Please note that the goal here is
+simplicity and accesibility, using common language and few dependencies.
+[resources/youcreatethefuture.jpg]
```

### Comparing `agentmemory-0.3.1/agentmemory/__init__.py` & `agentmemory-0.3.2/agentmemory/__init__.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.1/agentmemory/client.py` & `agentmemory-0.3.2/agentmemory/client.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.1/agentmemory/events.py` & `agentmemory-0.3.2/agentmemory/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,20 +64,31 @@
     Returns:
         object: The memory object created for this event.
     """
     metadata["epoch"] = get_epoch()
     return create_memory("events", text, metadata=metadata, embedding=embedding)
 
 
-def get_events(epoch=None):
+def get_events(epoch=None, n_results=10, filter_metadata=None):
     """
     Retrieves events from the agent's memory.
 
     Args:
         epoch (int, optional): If specified, only retrieve events from this epoch.
 
     Returns:
         list: A list of memory objects for the retrieved events.
     """
     if epoch is not None:
-        return get_memories("events", filter_metadata={"epoch": epoch})
-    return get_memories("events")
+        if filter_metadata is None:
+            filter_metadata = {}
+        filter_metadata["epoch"] = epoch
+        return get_memories(
+            "events", filter_metadata=filter_metadata, n_results=n_results
+        )
+    else:
+        if filter_metadata is None:
+            return get_memories("events", n_results=n_results)
+        else:
+            return get_memories(
+                "events", filter_metadata=filter_metadata, n_results=n_results
+            )
```

### Comparing `agentmemory-0.3.1/agentmemory/helpers.py` & `agentmemory-0.3.2/agentmemory/helpers.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.1/agentmemory/main.py` & `agentmemory-0.3.2/agentmemory/main.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.1/agentmemory/persistence.py` & `agentmemory-0.3.2/agentmemory/persistence.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.3.1/agentmemory.egg-info/PKG-INFO` & `agentmemory-0.3.2/agentmemory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.3.1
+Version: 0.3.2
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/AutonomousResearchGroup/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -640,15 +640,15 @@
 
 ```python
 create_event("This is a test event", metadata={"test": "test"})
 ```
 
 ---
 
-## `get_events(epoch=None)`
+## `get_events(epoch=None, filter_metadata=None, n_results=10)`
 
 The `get_events` function retrieves events from the agent's memory.
 
 **Arguments:**
 
 - `epoch` (int, optional): If specified, only retrieve events from this epoch.
```

### Comparing `agentmemory-0.3.1/setup.py` & `agentmemory-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.3.1',
+    version='0.3.2',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/AutonomousResearchGroup/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

