# Comparing `tmp/easyecs-0.3.0.tar.gz` & `tmp/easyecs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.3.0.tar", max compression
+gzip compressed data, was "easyecs-0.3.1.tar", max compression
```

## Comparing `easyecs-0.3.0.tar` & `easyecs-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2230 2023-08-02 20:41:14.802827 easyecs-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/__init__.py
--rwxr-xr-x   0        0        0     7304 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     2825 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     8573 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12418 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1459 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     2360 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2804 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-02 20:41:14.822827 easyecs-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-02 20:58:51.772551 easyecs-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 20:58:51.792552 easyecs-0.3.1/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     7304 2023-08-02 20:58:51.792552 easyecs-0.3.1/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-02 20:58:51.792552 easyecs-0.3.1/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     3160 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     8573 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12418 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1459 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     2360 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2804 2023-08-02 20:58:51.796552 easyecs-0.3.1/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-02 20:58:51.796552 easyecs-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.3.1/PKG-INFO
```

### Comparing `easyecs-0.3.0/README.md` & `easyecs-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/cli.py` & `easyecs-0.3.1/easyecs/cli.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/cloudformation/fetch.py` & `easyecs-0.3.1/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/cloudformation/stack/create.py` & `easyecs-0.3.1/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/cloudformation/stack/delete.py` & `easyecs-0.3.1/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/cloudformation/stack/update.py` & `easyecs-0.3.1/easyecs/cloudformation/stack/update.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,14 +37,23 @@
     Waits for the CloudFormation stack to be rolled back.
     """
     client = get_client_cloudformation()
     waiter = client.get_waiter("stack_rollback_complete")
     waiter.wait(StackName=stack_name)
 
 
+def wait_for_stack_create(stack_name: str):
+    """
+    Waits for the CloudFormation stack to be created.
+    """
+    client = get_client_cloudformation()
+    waiter = client.get_waiter("stack_create_complete")
+    waiter.wait(StackName=stack_name)
+
+
 def handle_update_error(e: ClientError, stack_name: str, force_redeployment: bool):
     """
     Handles a CloudFormation stack update failure.
     Depending on the error, either waits for a rollback, cancels an update,
     or prints the error and breaks the loop.
     """
     message = e.response["Error"]["Message"]
@@ -55,14 +64,16 @@
     elif "UPDATE_IN_PROGRESS" in message:
         cloudformation = boto3.resource("cloudformation")
         stack = cloudformation.Stack(stack_name)
         stack.cancel_update()
         wait_for_stack_rollback(stack_name)
     elif "ROLLBACK_IN_PROGRESS" in message:
         wait_for_stack_rollback(stack_name)
+    elif "CREATE_IN_PROGRESS" in message:
+        wait_for_stack_create(stack_name)
     else:
         print(e)
 
 
 def update_stack(stack_name: str, force_redeployment: bool):
     """
     Updates a CloudFormation stack with the given name.
```

### Comparing `easyecs-0.3.0/easyecs/cloudformation/template/__init__.py` & `easyecs-0.3.1/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/command/__init__.py` & `easyecs-0.3.1/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/docker/__init__.py` & `easyecs-0.3.1/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/helpers/common.py` & `easyecs-0.3.1/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/helpers/loader.py` & `easyecs-0.3.1/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/helpers/selector.py` & `easyecs-0.3.1/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/helpers/settings.py` & `easyecs-0.3.1/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/easyecs/model/ecs.py` & `easyecs-0.3.1/easyecs/model/ecs.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.0/pyproject.toml` & `easyecs-0.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.3.0/PKG-INFO` & `easyecs-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

