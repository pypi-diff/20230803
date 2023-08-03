# Comparing `tmp/easyecs-0.3.2.tar.gz` & `tmp/easyecs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.3.2.tar", max compression
+gzip compressed data, was "easyecs-0.4.0.tar", max compression
```

## Comparing `easyecs-0.3.2.tar` & `easyecs-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2230 2023-08-03 10:50:03.766339 easyecs-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/__init__.py
--rwxr-xr-x   0        0        0     7304 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     3160 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     8573 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12418 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1356 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     2360 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2804 2023-08-03 10:50:03.786339 easyecs-0.3.2/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-03 10:50:03.786339 easyecs-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-03 11:19:16.925268 easyecs-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     8287 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     3160 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     8573 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12418 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1356 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     3272 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-03 11:19:16.941268 easyecs-0.4.0/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2804 2023-08-03 11:19:16.945268 easyecs-0.4.0/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-03 11:19:16.945268 easyecs-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.4.0/PKG-INFO
```

### Comparing `easyecs-0.3.2/README.md` & `easyecs-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/cli.py` & `easyecs-0.4.0/easyecs/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,25 @@
     execute_command,
     run_sync_thread,
     popen_procs_port_forward,
     popen_procs_exec_command,
     threads,
 )
 from easyecs.docker import build_docker_image
+from easyecs.helpers.color import Color
 from easyecs.helpers.common import check_credentials
 from easyecs.helpers.loader import Loader
 
-from easyecs.helpers.settings import load_settings, read_ecs_file
+from easyecs.helpers.settings import (
+    compute_hash_ecs_file,
+    delete_hash,
+    load_settings,
+    read_ecs_file,
+    save_hash,
+)
 
 
 def step_import_aws_cdk():
     loader_import = Loader(
         "Importing CloudFormation:",
         "Importing CloudFormation: \u2705",
         "Importing CloudFormation: \u274c",
@@ -108,14 +115,52 @@
 
     for popen_proc in popen_procs_exec_command:
         popen_proc.stdin.write("exit\x03\x04".encode("utf8"))
         popen_proc.stdin.flush()
         popen_proc.wait()
 
 
+def has_ecs_file_changed(cache_settings):
+    hash_sha256 = compute_hash_ecs_file()
+    return hash_sha256 != cache_settings["sha256"]
+
+
+def step_bring_up_stack(
+    cache_settings,
+    no_docker_build,
+    ecs_manifest,
+    stack_name,
+    aws_account_id,
+    aws_region,
+    vpc_id,
+    subnet_ids,
+    azs,
+    force_redeployment,
+    aws_account,
+):
+    print()
+    if has_ecs_file_changed(cache_settings) or force_redeployment:
+        step_import_aws_cdk()
+        step_docker_build_and_push(
+            no_docker_build,
+            ecs_manifest,
+            stack_name,
+            aws_account_id,
+            aws_region,
+            vpc_id,
+            subnet_ids,
+            azs,
+            True,
+        )
+        step_create_or_update_stack(stack_name, force_redeployment)
+        save_hash(aws_account)
+    else:
+        print(f"{Color.YELLOW}No updates are to be performed.{Color.END}")
+
+
 def action_run(ctx):
     no_docker_build = ctx.obj["no_docker_build"]
     force_redeployment = ctx.obj["force_redeployment"]
     aws_account = fetch_aws_account()
     cache_settings = load_settings(aws_account)
     ecs_manifest = read_ecs_file()
     app_name = ecs_manifest.metadata.appname
@@ -123,28 +168,27 @@
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
     vpc_id = cache_settings["vpc_id"]
     subnet_ids = cache_settings["subnet_ids"]
     azs = cache_settings["azs"]
     stack_name = f"{user}-{app_name}"
 
-    print()
-    step_import_aws_cdk()
-    step_docker_build_and_push(
+    step_bring_up_stack(
+        cache_settings,
         no_docker_build,
         ecs_manifest,
         stack_name,
         aws_account_id,
         aws_region,
         vpc_id,
         subnet_ids,
         azs,
-        True,
+        force_redeployment,
+        aws_account,
     )
-    step_create_or_update_stack(stack_name, force_redeployment)
     parsed_containers = fetch_containers(user, app_name)
     print()
     create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
     step_idle_keyboard()
 
     step_clean_exit()
 
@@ -162,28 +206,27 @@
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
     vpc_id = cache_settings["vpc_id"]
     subnet_ids = cache_settings["subnet_ids"]
     azs = cache_settings["azs"]
     stack_name = f"{user}-{app_name}"
 
-    print()
-    step_import_aws_cdk()
-    step_docker_build_and_push(
+    step_bring_up_stack(
+        cache_settings,
         no_docker_build,
         ecs_manifest,
         stack_name,
         aws_account_id,
         aws_region,
         vpc_id,
         subnet_ids,
         azs,
-        False,
+        force_redeployment,
+        aws_account,
     )
-    step_create_or_update_stack(stack_name, force_redeployment)
     parsed_containers = fetch_containers(user, app_name)
     print()
     create_port_forwards(ecs_manifest, aws_region, aws_account, parsed_containers)
     run_nc_commands(parsed_containers, aws_region, aws_account, ecs_manifest)
     run_sync_thread(parsed_containers, ecs_manifest)
     print()
 
@@ -197,19 +240,21 @@
     if not found_tty:
         step_idle_keyboard()
     step_clean_exit()
     exit(0)
 
 
 def action_delete(_):
+    aws_account = fetch_aws_account()
     ecs_manifest = read_ecs_file()
     app_name = ecs_manifest.metadata.appname
     user = ecs_manifest.metadata.user
     stack_name = f"{user}-{app_name}"
     delete_stack(stack_name)
+    delete_hash(aws_account)
 
 
 @click.group()
 @click.pass_context
 def entrypoint(ctx):
     ctx.ensure_object(dict)
     check_credentials()
```

### Comparing `easyecs-0.3.2/easyecs/cloudformation/fetch.py` & `easyecs-0.4.0/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/cloudformation/stack/create.py` & `easyecs-0.4.0/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/cloudformation/stack/delete.py` & `easyecs-0.4.0/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/cloudformation/stack/update.py` & `easyecs-0.4.0/easyecs/cloudformation/stack/update.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/cloudformation/template/__init__.py` & `easyecs-0.4.0/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/command/__init__.py` & `easyecs-0.4.0/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/docker/__init__.py` & `easyecs-0.4.0/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/helpers/common.py` & `easyecs-0.4.0/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/helpers/loader.py` & `easyecs-0.4.0/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/helpers/selector.py` & `easyecs-0.4.0/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/easyecs/helpers/settings.py` & `easyecs-0.4.0/easyecs/helpers/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import json
 import os
 import yaml
 from yaml import SafeLoader
 
 from easyecs.cloudformation.fetch import (
     fetch_account_id,
@@ -16,14 +17,39 @@
 
 def read_ecs_file() -> EcsFileModel:
     with open("./ecs.yml") as f:
         data = yaml.load(f, Loader=SafeLoader)
     return EcsFileModel(**data)
 
 
+def compute_hash_ecs_file():
+    hash_sha256 = hashlib.sha256()
+    with open("ecs.yml", "rb") as f:
+        for chunk in iter(lambda: f.read(4096), b""):
+            hash_sha256.update(chunk)
+    return hash_sha256.hexdigest()
+
+
+def save_hash(aws_account):
+    hash_sha256 = compute_hash_ecs_file()
+    with open(".tmp/easyecs.tmp", "r") as f:
+        cache_configuration = json.load(f)
+    cache_configuration[aws_account]["sha256"] = hash_sha256
+    with open(".tmp/easyecs.tmp", "w") as f:
+        json.dump(cache_configuration, f)
+
+
+def delete_hash(aws_account):
+    with open(".tmp/easyecs.tmp", "r") as f:
+        cache_configuration = json.load(f)
+    cache_configuration[aws_account]["sha256"] = None
+    with open(".tmp/easyecs.tmp", "w") as f:
+        json.dump(cache_configuration, f)
+
+
 def load_settings(aws_account):
     try:
         os.makedirs(".tmp", exist_ok=True)
         with open(".tmp/easyecs.tmp", "r") as f:
             cache_configuration = json.load(f)
     except FileNotFoundError:
         cache_configuration = {}
@@ -42,20 +68,23 @@
     vpc_id = account_cache_configuration.get("vpc_id", None)
     if not vpc_id:
         vpc_id = fetch_vpc_id()
     subnet_ids = account_cache_configuration.get("subnet_ids", None)
     if not subnet_ids:
         subnet_ids = fetch_container_subnet_ids(vpc_id)
 
+    hash_sha256 = account_cache_configuration.get("sha256", None)
+
     cache_configuration[aws_account] = {
         "aws_region": aws_region,
         "aws_account_id": aws_account_id,
         "vpc_id": vpc_id,
         "subnet_ids": subnet_ids,
         "azs": azs,
+        "sha256": hash_sha256,
     }
 
     print(
         "Selected aws account:"
         f" {Color.BOLD}{Color.GREEN}{aws_account}{Color.END} \u2705"
     )
     print(f"Selected region: {Color.BOLD}{Color.GREEN}{aws_region}{Color.END} \u2705")
```

### Comparing `easyecs-0.3.2/easyecs/model/ecs.py` & `easyecs-0.4.0/easyecs/model/ecs.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.3.2/pyproject.toml` & `easyecs-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.3.2"
+version = "0.4.0"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.3.2/PKG-INFO` & `easyecs-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.3.2
+Version: 0.4.0
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

