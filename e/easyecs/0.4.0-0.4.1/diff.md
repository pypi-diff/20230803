# Comparing `tmp/easyecs-0.4.0.tar.gz` & `tmp/easyecs-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.4.0.tar", max compression
+gzip compressed data, was "easyecs-0.4.1.tar", max compression
```

## Comparing `easyecs-0.4.0.tar` & `easyecs-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2230 2023-08-03 11:19:16.925268 easyecs-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/__init__.py
--rwxr-xr-x   0        0        0     8287 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     3160 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     8573 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12418 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1356 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     3272 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2804 2023-08-03 11:19:16.945268 easyecs-0.4.0/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-03 11:19:16.945268 easyecs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-03 11:34:13.204982 easyecs-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     8332 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     3274 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     8573 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12418 2023-08-03 11:34:13.224982 easyecs-0.4.1/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1356 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     3272 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2804 2023-08-03 11:34:13.228983 easyecs-0.4.1/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-03 11:34:13.228983 easyecs-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.4.1/PKG-INFO
```

### Comparing `easyecs-0.4.0/README.md` & `easyecs-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/cli.py` & `easyecs-0.4.1/easyecs/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,28 +132,29 @@
     aws_account_id,
     aws_region,
     vpc_id,
     subnet_ids,
     azs,
     force_redeployment,
     aws_account,
+    run,
 ):
     print()
     if has_ecs_file_changed(cache_settings) or force_redeployment:
         step_import_aws_cdk()
         step_docker_build_and_push(
             no_docker_build,
             ecs_manifest,
             stack_name,
             aws_account_id,
             aws_region,
             vpc_id,
             subnet_ids,
             azs,
-            True,
+            run,
         )
         step_create_or_update_stack(stack_name, force_redeployment)
         save_hash(aws_account)
     else:
         print(f"{Color.YELLOW}No updates are to be performed.{Color.END}")
 
 
@@ -180,14 +181,15 @@
         aws_account_id,
         aws_region,
         vpc_id,
         subnet_ids,
         azs,
         force_redeployment,
         aws_account,
+        run=True,
     )
     parsed_containers = fetch_containers(user, app_name)
     print()
     create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
     step_idle_keyboard()
 
     step_clean_exit()
@@ -218,14 +220,15 @@
         aws_account_id,
         aws_region,
         vpc_id,
         subnet_ids,
         azs,
         force_redeployment,
         aws_account,
+        run=False,
     )
     parsed_containers = fetch_containers(user, app_name)
     print()
     create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
     run_nc_commands(parsed_containers, aws_region, aws_account, ecs_manifest)
     run_sync_thread(parsed_containers, ecs_manifest)
     print()
```

### Comparing `easyecs-0.4.0/easyecs/cloudformation/fetch.py` & `easyecs-0.4.1/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/cloudformation/stack/create.py` & `easyecs-0.4.1/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/cloudformation/stack/delete.py` & `easyecs-0.4.1/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/cloudformation/stack/update.py` & `easyecs-0.4.1/easyecs/cloudformation/stack/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,35 +46,42 @@
     Waits for the CloudFormation stack to be created.
     """
     client = get_client_cloudformation()
     waiter = client.get_waiter("stack_create_complete")
     waiter.wait(StackName=stack_name)
 
 
-def handle_update_error(e: ClientError, stack_name: str, force_redeployment: bool):
+def handle_update_error(
+    e: ClientError, stack_name: str, force_redeployment: bool, loader: Loader
+):
     """
     Handles a CloudFormation stack update failure.
     Depending on the error, either waits for a rollback, cancels an update,
     or prints the error and breaks the loop.
     """
     message = e.response["Error"]["Message"]
     if message == "No updates are to be performed.":
+        loader.stop()
         print(f"{Color.YELLOW}No updates are to be performed.{Color.END}")
         if force_redeployment:
             run_force_new_deployment(stack_name)
     elif "UPDATE_IN_PROGRESS" in message:
         cloudformation = boto3.resource("cloudformation")
         stack = cloudformation.Stack(stack_name)
         stack.cancel_update()
         wait_for_stack_rollback(stack_name)
+        loader.stop()
     elif "ROLLBACK_IN_PROGRESS" in message:
         wait_for_stack_rollback(stack_name)
+        loader.stop()
     elif "CREATE_IN_PROGRESS" in message:
         wait_for_stack_create(stack_name)
+        loader.stop()
     else:
+        loader.stop_error()
         print(e)
 
 
 def update_stack(stack_name: str, force_redeployment: bool):
     """
     Updates a CloudFormation stack with the given name.
     """
@@ -90,10 +97,9 @@
 
     while True:
         try:
             update_cloudformation_stack(stack_name, cloudformation_template)
             wait_for_stack_update(stack_name)
             loader.stop()
         except ClientError as e:
-            loader.stop_error()
-            handle_update_error(e, stack_name, force_redeployment)
+            handle_update_error(e, stack_name, force_redeployment, loader)
         break
```

### Comparing `easyecs-0.4.0/easyecs/cloudformation/template/__init__.py` & `easyecs-0.4.1/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/command/__init__.py` & `easyecs-0.4.1/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/docker/__init__.py` & `easyecs-0.4.1/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/helpers/common.py` & `easyecs-0.4.1/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/helpers/loader.py` & `easyecs-0.4.1/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/helpers/selector.py` & `easyecs-0.4.1/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/helpers/settings.py` & `easyecs-0.4.1/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/easyecs/model/ecs.py` & `easyecs-0.4.1/easyecs/model/ecs.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.4.0/pyproject.toml` & `easyecs-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.4.0/PKG-INFO` & `easyecs-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

