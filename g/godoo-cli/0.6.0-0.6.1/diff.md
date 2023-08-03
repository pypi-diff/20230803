# Comparing `tmp/godoo_cli-0.6.0.tar.gz` & `tmp/godoo_cli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godoo_cli-0.6.0.tar", max compression
+gzip compressed data, was "godoo_cli-0.6.1.tar", max compression
```

## Comparing `godoo_cli-0.6.0.tar` & `godoo_cli-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     7633 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/LICENSE
--rw-r--r--   0        0        0     7297 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/README.md
--rw-r--r--   0        0        0     5070 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       61 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/__init__.py
--rw-r--r--   0        0        0       88 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/__main__.py
--rw-r--r--   0        0        0     1963 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/cli.py
--rw-r--r--   0        0        0     5397 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/cli_common.py
--rw-r--r--   0        0        0      293 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/__init__.py
--rw-r--r--   0        0        0     5811 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/bootstrap.py
--rw-r--r--   0        0        0     1173 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/config.py
--rw-r--r--   0        0        0       28 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/db/__init__.py
--rw-r--r--   0        0        0      311 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/db/cli.py
--rw-r--r--   0        0        0     1801 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/db/connection.py
--rw-r--r--   0        0        0     1325 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/db/passwords.py
--rw-r--r--   0        0        0    10339 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/launch.py
--rw-r--r--   0        0        0      177 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/__init__.py
--rw-r--r--   0        0        0      897 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/cli.py
--rw-r--r--   0        0        0     1484 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/config_parameters.py
--rw-r--r--   0        0        0     2278 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/importer.py
--rw-r--r--   0        0        0     4828 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/modules.py
--rw-r--r--   0        0        0     4000 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/translations.py
--rw-r--r--   0        0        0     1619 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/shell.py
--rw-r--r--   0        0        0     8544 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/source_get.py
--rw-r--r--   0        0        0     4437 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/test.py
--rw-r--r--   0        0        0      161 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/__init__.py
--rw-r--r--   0        0        0     2688 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/git_odoo.py
--rw-r--r--   0        0        0     3296 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/git_odoo_addons.py
--rw-r--r--   0        0        0     6460 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/git_repo.py
--rw-r--r--   0        0        0     4585 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/git_url.py
--rw-r--r--   0        0        0     1575 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/zip_download.py
--rw-r--r--   0        0        0       49 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/__init__.py
--rw-r--r--   0        0        0     2225 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/bootstrap.py
--rw-r--r--   0        0        0      386 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/cli.py
--rw-r--r--   0        0        0     8895 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/odoo_files.py
--rw-r--r--   0        0        0     3277 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/odoo_manifest.py
--rw-r--r--   0        0        0     2766 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/system.py
--rw-r--r--   0        0        0       22 2023-07-17 10:33:31.704929 godoo_cli-0.6.0/src/godoo_cli/version.py
--rw-r--r--   0        0        0     9387 1970-01-01 00:00:00.000000 godoo_cli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/LICENSE
+-rw-r--r--   0        0        0     7297 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/README.md
+-rw-r--r--   0        0        0     5070 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/__init__.py
+-rw-r--r--   0        0        0       88 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/__main__.py
+-rw-r--r--   0        0        0     1963 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/cli.py
+-rw-r--r--   0        0        0     5397 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/cli_common.py
+-rw-r--r--   0        0        0      293 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/__init__.py
+-rw-r--r--   0        0        0     5811 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/bootstrap.py
+-rw-r--r--   0        0        0     1173 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/config.py
+-rw-r--r--   0        0        0       28 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/db/__init__.py
+-rw-r--r--   0        0        0      311 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/db/cli.py
+-rw-r--r--   0        0        0     1801 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/db/connection.py
+-rw-r--r--   0        0        0     1325 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/db/passwords.py
+-rw-r--r--   0        0        0    10424 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/launch.py
+-rw-r--r--   0        0        0      177 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/rpc/__init__.py
+-rw-r--r--   0        0        0      897 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/rpc/cli.py
+-rw-r--r--   0        0        0     1484 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/rpc/config_parameters.py
+-rw-r--r--   0        0        0     2278 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/rpc/importer.py
+-rw-r--r--   0        0        0     4828 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/rpc/modules.py
+-rw-r--r--   0        0        0     4000 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/rpc/translations.py
+-rw-r--r--   0        0        0     1619 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/shell.py
+-rw-r--r--   0        0        0     8544 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/source_get.py
+-rw-r--r--   0        0        0     4572 2023-08-03 12:31:05.804569 godoo_cli-0.6.1/src/godoo_cli/commands/test.py
+-rw-r--r--   0        0        0      161 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/git/__init__.py
+-rw-r--r--   0        0        0     2688 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/git/git_odoo.py
+-rw-r--r--   0        0        0     3296 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/git/git_odoo_addons.py
+-rw-r--r--   0        0        0     6460 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/git/git_repo.py
+-rw-r--r--   0        0        0     4585 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/git/git_url.py
+-rw-r--r--   0        0        0     1575 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/git/zip_download.py
+-rw-r--r--   0        0        0       49 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     2225 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/helpers/bootstrap.py
+-rw-r--r--   0        0        0      386 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/helpers/cli.py
+-rw-r--r--   0        0        0     8895 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/helpers/odoo_files.py
+-rw-r--r--   0        0        0     3277 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/helpers/odoo_manifest.py
+-rw-r--r--   0        0        0     2766 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/helpers/system.py
+-rw-r--r--   0        0        0       22 2023-08-03 12:31:05.808569 godoo_cli-0.6.1/src/godoo_cli/version.py
+-rw-r--r--   0        0        0     9387 1970-01-01 00:00:00.000000 godoo_cli-0.6.1/PKG-INFO
```

### Comparing `godoo_cli-0.6.0/LICENSE` & `godoo_cli-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/README.md` & `godoo_cli-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/pyproject.toml` & `godoo_cli-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gOdoo-cli"
-version = "0.6.0"
+version = "0.6.1"
 description = "Wrapper around Odoo-Bin with some convinience RPC functions."
 authors = ["Joshua Kreuder <Joshua_Kreuder@outlook.com>"]
 license = "LGPL-3"
 readme = "README.md"
 packages = [{include = "godoo_cli",  from = "src"}]
 repository = "https://github.com/OpenJKSoftware/gOdoo"
 keywords = ["odoo", "godoo","devcontainer"]
```

### Comparing `godoo_cli-0.6.0/src/godoo_cli/cli.py` & `godoo_cli-0.6.1/src/godoo_cli/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/cli_common.py` & `godoo_cli-0.6.1/src/godoo_cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/bootstrap.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/config.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/db/connection.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/db/connection.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/db/passwords.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/db/passwords.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/launch.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,17 @@
     odoo_version = odoo_bin_get_version(odoo_main_path)
 
     if dev_mode:
         extra_odoo_args.append("--dev xml,qweb,reload")
         if "16.0" in odoo_version:
             extra_odoo_args[-1] += ",werkzeug"
 
+    if multithread_worker_count == 0:
+        extra_odoo_args.append("--workers 0")
+
     return _launch_command(
         odoo_path=odoo_main_path,
         odoo_conf_path=odoo_conf_path,
         extra_cmd_args=extra_odoo_args,
         workspace_addon_path=workspace_addon_path,
         upgrade_workspace_modules=install_workspace_addons,
     )
```

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/cli.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/rpc/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/config_parameters.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/rpc/config_parameters.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/importer.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/rpc/importer.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/modules.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/translations.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/rpc/translations.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/shell.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/source_get.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/source_get.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/commands/test.py` & `godoo_cli-0.6.1/src/godoo_cli/commands/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         ...,
         help="Modules to install and test (Use 'all' for all Workspace modules), ('changes:<branch> to compare git changes)",
     ),
     odoo_main_path=CLI.odoo_paths.bin_path,
     workspace_addon_path=CLI.odoo_paths.workspace_addon_path,
     thirdparty_addon_path=CLI.odoo_paths.thirdparty_addon_path,
     odoo_conf_path=CLI.odoo_paths.conf_path,
+    extra_launch_args=CLI.odoo_launch.extra_cmd_args,
     db_filter=CLI.database.db_filter,
     db_host=CLI.database.db_host,
     db_port=CLI.database.db_port,
     db_name=CLI.database.db_name,
     db_user=CLI.database.db_user,
     db_password=CLI.database.db_password,
     skip_test_modules: List[str] = typer.Option(
@@ -91,14 +92,17 @@
         "--test-enable",
         f"--log-level {odoo_log_level}",
         "--stop-after-init",
         "--no-http",
         f"--test-tags {test_module_list}",
     ]
 
+    if extra_launch_args:
+        launch_args = extra_launch_args + launch_args
+
     launch_cmd = pre_launch(
         odoo_main_path=odoo_main_path,
         workspace_addon_path=workspace_addon_path,
         thirdparty_addon_path=thirdparty_addon_path,
         odoo_conf_path=odoo_conf_path,
         db_filter=db_filter,
         db_host=db_host,
```

### Comparing `godoo_cli-0.6.0/src/godoo_cli/git/git_odoo.py` & `godoo_cli-0.6.1/src/godoo_cli/git/git_odoo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/git/git_odoo_addons.py` & `godoo_cli-0.6.1/src/godoo_cli/git/git_odoo_addons.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/git/git_repo.py` & `godoo_cli-0.6.1/src/godoo_cli/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/git/git_url.py` & `godoo_cli-0.6.1/src/godoo_cli/git/git_url.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/git/zip_download.py` & `godoo_cli-0.6.1/src/godoo_cli/git/zip_download.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/helpers/bootstrap.py` & `godoo_cli-0.6.1/src/godoo_cli/helpers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/helpers/odoo_files.py` & `godoo_cli-0.6.1/src/godoo_cli/helpers/odoo_files.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/helpers/odoo_manifest.py` & `godoo_cli-0.6.1/src/godoo_cli/helpers/odoo_manifest.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/src/godoo_cli/helpers/system.py` & `godoo_cli-0.6.1/src/godoo_cli/helpers/system.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.6.0/PKG-INFO` & `godoo_cli-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godoo-cli
-Version: 0.6.0
+Version: 0.6.1
 Summary: Wrapper around Odoo-Bin with some convinience RPC functions.
 Home-page: https://github.com/OpenJKSoftware/gOdoo
 License: LGPL-3
 Keywords: odoo,godoo,devcontainer
 Author: Joshua Kreuder
 Author-email: Joshua_Kreuder@outlook.com
 Requires-Python: >=3.8.1,<3.12
```

