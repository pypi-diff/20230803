# Comparing `tmp/agentloop-0.2.1.tar.gz` & `tmp/agentloop-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentloop-0.2.1.tar", last modified: Sun Jul 30 03:33:13 2023, max compression
+gzip compressed data, was "agentloop-0.2.2.tar", last modified: Thu Aug  3 16:44:48 2023, max compression
```

## Comparing `agentloop-0.2.1.tar` & `agentloop-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:33:13.322184 agentloop-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-30 03:33:04.000000 agentloop-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 03:33:13.322184 agentloop-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-30 03:33:04.000000 agentloop-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:33:13.322184 agentloop-0.2.1/agentloop/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 03:33:04.000000 agentloop-0.2.1/agentloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-30 03:33:04.000000 agentloop-0.2.1/agentloop/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-30 03:33:04.000000 agentloop-0.2.1/agentloop/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:33:13.322184 agentloop-0.2.1/agentloop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:33:13.322184 agentloop-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-30 03:33:04.000000 agentloop-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:44:48.958942 agentloop-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 16:44:37.000000 agentloop-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-08-03 16:44:48.958942 agentloop-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-08-03 16:44:37.000000 agentloop-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:44:48.954941 agentloop-0.2.2/agentloop/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-03 16:44:37.000000 agentloop-0.2.2/agentloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-03 16:44:37.000000 agentloop-0.2.2/agentloop/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-08-03 16:44:37.000000 agentloop-0.2.2/agentloop/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:44:48.958942 agentloop-0.2.2/agentloop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-08-03 16:44:48.000000 agentloop-0.2.2/agentloop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 16:44:48.000000 agentloop-0.2.2/agentloop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:44:48.000000 agentloop-0.2.2/agentloop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 16:44:48.000000 agentloop-0.2.2/agentloop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:44:48.000000 agentloop-0.2.2/agentloop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:44:48.958942 agentloop-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-03 16:44:37.000000 agentloop-0.2.2/setup.py
```

### Comparing `agentloop-0.2.1/LICENSE` & `agentloop-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentloop-0.2.1/PKG-INFO` & `agentloop-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -76,26 +76,28 @@
 
 steps = [step_one, step_two]
 ```
 
 ## Function `start`
 
 ```python
-start(steps, stepped=False)
+start(steps, stepped=False, step_interval=0.0)
 ```
 
 ### Description
 
 Starts the main loop in a separate thread. This loop will run the steps given, in a continuous or stepped manner.
 
 ### Parameters
 
 - `steps` : a list of functions that should be executed in the loop. Each function should accept a single argument and return a single value which will be passed as an argument to the next function. The first function will receive `None` as an argument.
 
-- `stepped` (optional): a boolean value that determines whether the loop should run in stepped mode or not. Defaults to `False`.
+- `paused` (optional): a boolean value that determines whether the loop should run in paused step mode or not. Defaults to `False`.
+
+- `step_interval` (optional): a float value that determines the time interval between steps in seconds. Defaults to `0.0`.
 
 ### Returns
 
 A dictionary containing
 
 - `stop_event`: an instance of `threading.Event` that's used to control stopping of the loop.
 - `step_event`: an instance of `threading.Event` that's used to control stepping.
@@ -185,29 +187,31 @@
 None
 
 ---
 
 ## Function `loop`
 
 ```python
-loop(steps, stepped=False, loop_data=None)
+loop(steps, paused=False, loop_data=None, step_interval=0.0)
 ```
 
 ### Description
 
 Runs the step array in a loop until stopped.
 
 ### Parameters
 
 - `steps`: a list of functions that should be executed in the loop. Each function should accept a single argument and return a single value which will be passed as an argument to the next function. The first function will receive `None` as an argument.
 
-- `stepped` (optional): a boolean value that determines whether the loop should run in stepped mode or not. Defaults to `False`.
+- `paused` (optional): a boolean value that determines whether the loop should run in paused / stepped mode or not. Defaults to `False`.
 
 - `loop_data` (optional): a dictionary containing `stop_event` and `step_event` instances. If not provided, new events will be created.
 
+- `step_interval` (optional): a float value that determines the time interval between steps in seconds. Defaults to `0.0`.
+
 ### Returns
 
 None
 
 ## Function `use_keyboard`
 
 ```python
```

### Comparing `agentloop-0.2.1/README.md` & `agentloop-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -60,26 +60,28 @@
 
 steps = [step_one, step_two]
 ```
 
 ## Function `start`
 
 ```python
-start(steps, stepped=False)
+start(steps, stepped=False, step_interval=0.0)
 ```
 
 ### Description
 
 Starts the main loop in a separate thread. This loop will run the steps given, in a continuous or stepped manner.
 
 ### Parameters
 
 - `steps` : a list of functions that should be executed in the loop. Each function should accept a single argument and return a single value which will be passed as an argument to the next function. The first function will receive `None` as an argument.
 
-- `stepped` (optional): a boolean value that determines whether the loop should run in stepped mode or not. Defaults to `False`.
+- `paused` (optional): a boolean value that determines whether the loop should run in paused step mode or not. Defaults to `False`.
+
+- `step_interval` (optional): a float value that determines the time interval between steps in seconds. Defaults to `0.0`.
 
 ### Returns
 
 A dictionary containing
 
 - `stop_event`: an instance of `threading.Event` that's used to control stopping of the loop.
 - `step_event`: an instance of `threading.Event` that's used to control stepping.
@@ -169,29 +171,31 @@
 None
 
 ---
 
 ## Function `loop`
 
 ```python
-loop(steps, stepped=False, loop_data=None)
+loop(steps, paused=False, loop_data=None, step_interval=0.0)
 ```
 
 ### Description
 
 Runs the step array in a loop until stopped.
 
 ### Parameters
 
 - `steps`: a list of functions that should be executed in the loop. Each function should accept a single argument and return a single value which will be passed as an argument to the next function. The first function will receive `None` as an argument.
 
-- `stepped` (optional): a boolean value that determines whether the loop should run in stepped mode or not. Defaults to `False`.
+- `paused` (optional): a boolean value that determines whether the loop should run in paused / stepped mode or not. Defaults to `False`.
 
 - `loop_data` (optional): a dictionary containing `stop_event` and `step_event` instances. If not provided, new events will be created.
 
+- `step_interval` (optional): a float value that determines the time interval between steps in seconds. Defaults to `0.0`.
+
 ### Returns
 
 None
 
 ## Function `use_keyboard`
 
 ```python
```

### Comparing `agentloop-0.2.1/agentloop/input.py` & `agentloop-0.2.2/agentloop/input.py`

 * *Files identical despite different names*

### Comparing `agentloop-0.2.1/agentloop/loop.py` & `agentloop-0.2.2/agentloop/loop.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import threading
 
 
-def start(steps, paused=False):
+def start(steps, paused=False, step_interval=0.0):
     """
     Function to start the main loop
 
     Args:
+        steps: array of functions to be run in the loop
+
         paused: boolean - whether the loop should run automatically. If paused can be stepped one-step-at-a-time.
             Defaults to False.
 
+        step_interval: float - time in seconds to wait between steps. Defaults to 0.0 (no wait)
+
+
     Returns:
         loop_data: a dictionary of loop data
     """
 
     loop_data = {
         "stop_event": threading.Event(),
         "step_event": threading.Event(),
         "started_event": threading.Event(),
         "pause_event": threading.Event(),
     }
 
     if paused:
         loop_data["pause_event"].set()
 
-    thread = threading.Thread(target=loop, args=(steps, loop_data))
+    thread = threading.Thread(target=loop, args=(steps, loop_data, step_interval))
     loop_data["thread"] = thread
 
     thread.start()
     loop_data["started_event"].wait()  # Wait here until loop is started
 
     return loop_data
 
@@ -82,28 +87,31 @@
         loop_data: loop data object, created by the start function
 
     This function does not return any value.
     """
     loop_data["pause_event"].clear()
 
 
-def loop(steps, loop_data):
+def loop(steps, loop_data, step_interval=0.0):
     """
     Run the step array in a loop until stopped
 
     Args:
         steps: array of functions to be run in the loop
         paused: boolean - whether the loop should run start up paused (can be stepped) or running
         loop_data: loop data object, created by the start function
+        step_interval: float - time in seconds to wait between steps. Defaults to 0.0 (no wait)
 
     This function does not return any value.
     """
     next_output = None
     loop_data["started_event"].set()  # Indicate that the loop has started
     while not loop_data["stop_event"].is_set():
+        if step_interval > 0:
+            loop_data["stop_event"].wait(timeout=step_interval)
         for step in steps:
             number_of_args = step.__code__.co_argcount
             if number_of_args == 1:
                 next_output = step(next_output)
             elif number_of_args == 2:
                 next_output = step(next_output, loop_data)
             else:
```

### Comparing `agentloop-0.2.1/agentloop.egg-info/PKG-INFO` & `agentloop-0.2.2/agentloop.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -76,26 +76,28 @@
 
 steps = [step_one, step_two]
 ```
 
 ## Function `start`
 
 ```python
-start(steps, stepped=False)
+start(steps, stepped=False, step_interval=0.0)
 ```
 
 ### Description
 
 Starts the main loop in a separate thread. This loop will run the steps given, in a continuous or stepped manner.
 
 ### Parameters
 
 - `steps` : a list of functions that should be executed in the loop. Each function should accept a single argument and return a single value which will be passed as an argument to the next function. The first function will receive `None` as an argument.
 
-- `stepped` (optional): a boolean value that determines whether the loop should run in stepped mode or not. Defaults to `False`.
+- `paused` (optional): a boolean value that determines whether the loop should run in paused step mode or not. Defaults to `False`.
+
+- `step_interval` (optional): a float value that determines the time interval between steps in seconds. Defaults to `0.0`.
 
 ### Returns
 
 A dictionary containing
 
 - `stop_event`: an instance of `threading.Event` that's used to control stopping of the loop.
 - `step_event`: an instance of `threading.Event` that's used to control stepping.
@@ -185,29 +187,31 @@
 None
 
 ---
 
 ## Function `loop`
 
 ```python
-loop(steps, stepped=False, loop_data=None)
+loop(steps, paused=False, loop_data=None, step_interval=0.0)
 ```
 
 ### Description
 
 Runs the step array in a loop until stopped.
 
 ### Parameters
 
 - `steps`: a list of functions that should be executed in the loop. Each function should accept a single argument and return a single value which will be passed as an argument to the next function. The first function will receive `None` as an argument.
 
-- `stepped` (optional): a boolean value that determines whether the loop should run in stepped mode or not. Defaults to `False`.
+- `paused` (optional): a boolean value that determines whether the loop should run in paused / stepped mode or not. Defaults to `False`.
 
 - `loop_data` (optional): a dictionary containing `stop_event` and `step_event` instances. If not provided, new events will be created.
 
+- `step_interval` (optional): a float value that determines the time interval between steps in seconds. Defaults to `0.0`.
+
 ### Returns
 
 None
 
 ## Function `use_keyboard`
 
 ```python
```

### Comparing `agentloop-0.2.1/setup.py` & `agentloop-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentloop",
-    version="0.2.1",
+    version="0.2.2",
     description="A simple, lightweight loop for your agent.",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentloop",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

