# Comparing `tmp/fotoobo-0.9.0.tar.gz` & `tmp/fotoobo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fotoobo-0.9.0.tar", max compression
+gzip compressed data, was "fotoobo-1.0.0.tar", max compression
```

## Comparing `fotoobo-0.9.0.tar` & `fotoobo-1.0.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0     7633 2023-04-20 13:29:11.640759 fotoobo-0.9.0/LICENSE
--rw-r--r--   0        0        0     2797 2023-04-20 13:29:11.640759 fotoobo-0.9.0/README.md
--rw-r--r--   0        0        0      256 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/__init__.py
--rw-r--r--   0        0        0      206 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/__init__.py
--rw-r--r--   0        0        0     1584 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/convert.py
--rw-r--r--   0        0        0       20 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/ems/__init__.py
--rw-r--r--   0        0        0     1488 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/ems/get_commands.py
--rw-r--r--   0        0        0      784 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/ems/main.py
--rw-r--r--   0        0        0     7418 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/ems/monitor_commands.py
--rw-r--r--   0        0        0       20 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/faz/__init__.py
--rw-r--r--   0        0        0      995 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/faz/get_commands.py
--rw-r--r--   0        0        0      639 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/faz/main.py
--rw-r--r--   0        0        0       20 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/__init__.py
--rw-r--r--   0        0        0     1537 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/config_commands.py
--rw-r--r--   0        0        0     1283 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/get_commands.py
--rw-r--r--   0        0        0     1951 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/main.py
--rw-r--r--   0        0        0     1711 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/monitor_commands.py
--rw-r--r--   0        0        0       20 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fmg/__init__.py
--rw-r--r--   0        0        0     2582 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fmg/get_commands.py
--rw-r--r--   0        0        0     2368 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fmg/main.py
--rw-r--r--   0        0        0     1033 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/get.py
--rw-r--r--   0        0        0     4743 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/main.py
--rw-r--r--   0        0        0      196 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/exceptions/__init__.py
--rw-r--r--   0        0        0     1966 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/exceptions/exceptions.py
--rw-r--r--   0        0        0      190 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/__init__.py
--rw-r--r--   0        0        0    13955 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/convert.py
--rw-r--r--   0        0        0     1023 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/fortianalyzer.py
--rw-r--r--   0        0        0     5431 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/forticlientems.py
--rw-r--r--   0        0        0     2961 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/fortigate.py
--rw-r--r--   0        0        0    11342 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortigate_config.py
--rw-r--r--   0        0        0     8668 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortigate_config_check.py
--rw-r--r--   0        0        0      584 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortigate_info.py
--rw-r--r--   0        0        0    10537 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortimanager.py
--rw-r--r--   0        0        0     6523 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortinet.py
--rw-r--r--   0        0        0      322 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/cli.py
--rw-r--r--   0        0        0     3559 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/config.py
--rw-r--r--   0        0        0     6414 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/files.py
--rw-r--r--   0        0        0    11017 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/log.py
--rw-r--r--   0        0        0     9300 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/output.py
--rw-r--r--   0        0        0      128 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/inventory/__init__.py
--rw-r--r--   0        0        0      568 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/inventory/generic.py
--rw-r--r--   0        0        0     5050 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/inventory/inventory.py
--rwxr-xr-x   0        0        0     1359 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/main.py
--rw-r--r--   0        0        0      440 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/convert.py
--rw-r--r--   0        0        0       92 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/ems/__init__.py
--rw-r--r--   0        0        0     1518 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/ems/get.py
--rw-r--r--   0        0        0     7725 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/ems/monitor.py
--rw-r--r--   0        0        0       56 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/faz/__init__.py
--rw-r--r--   0        0        0      779 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/faz/get.py
--rw-r--r--   0        0        0      129 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/__init__.py
--rw-r--r--   0        0        0     3468 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/config.py
--rw-r--r--   0        0        0     1114 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/get.py
--rw-r--r--   0        0        0     3286 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/main.py
--rw-r--r--   0        0        0     4583 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/monitor.py
--rw-r--r--   0        0        0      105 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fmg/__init__.py
--rw-r--r--   0        0        0     4271 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fmg/get.py
--rw-r--r--   0        0        0     2707 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fmg/main.py
--rw-r--r--   0        0        0     2152 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/get.py
--rw-r--r--   0        0        0     1306 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/greet.py
--rw-r--r--   0        0        0     3730 2023-04-20 13:29:11.648759 fotoobo-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 fotoobo-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-08-03 09:50:30.968500 fotoobo-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2520 2023-08-03 09:50:30.968500 fotoobo-1.0.0/README.md
+-rw-r--r--   0        0        0      409 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/__init__.py
+-rw-r--r--   0        0        0      195 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/__init__.py
+-rw-r--r--   0        0        0     1817 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/convert.py
+-rw-r--r--   0        0        0       20 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/ems/__init__.py
+-rw-r--r--   0        0        0     1488 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/ems/get_commands.py
+-rw-r--r--   0        0        0      784 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/ems/main.py
+-rw-r--r--   0        0        0    11047 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/ems/monitor_commands.py
+-rw-r--r--   0        0        0       20 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/faz/__init__.py
+-rw-r--r--   0        0        0      976 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/faz/get_commands.py
+-rw-r--r--   0        0        0      639 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/faz/main.py
+-rw-r--r--   0        0        0       20 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/__init__.py
+-rw-r--r--   0        0        0     2172 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/config_commands.py
+-rw-r--r--   0        0        0     1241 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/get_commands.py
+-rw-r--r--   0        0        0     3547 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/main.py
+-rw-r--r--   0        0        0     3951 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fgt/monitor_commands.py
+-rw-r--r--   0        0        0       20 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fmg/__init__.py
+-rw-r--r--   0        0        0     2631 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fmg/get_commands.py
+-rw-r--r--   0        0        0     2394 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/fmg/main.py
+-rw-r--r--   0        0        0     1802 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/get.py
+-rw-r--r--   0        0        0     4825 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/cli/main.py
+-rw-r--r--   0        0        0      196 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/exceptions/__init__.py
+-rw-r--r--   0        0        0     1966 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/exceptions/exceptions.py
+-rw-r--r--   0        0        0      423 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/__init__.py
+-rw-r--r--   0        0        0    13927 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/convert.py
+-rw-r--r--   0        0        0     1023 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortianalyzer.py
+-rw-r--r--   0        0        0     5602 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/forticlientems.py
+-rw-r--r--   0        0        0     2961 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortigate.py
+-rw-r--r--   0        0        0    11488 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortigate_config.py
+-rw-r--r--   0        0        0     8714 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortigate_config_check.py
+-rw-r--r--   0        0        0      584 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortigate_info.py
+-rw-r--r--   0        0        0    12434 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortimanager.py
+-rw-r--r--   0        0        0     6431 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/fortinet/fortinet.py
+-rw-r--r--   0        0        0      322 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/__init__.py
+-rw-r--r--   0        0        0     1227 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/cli.py
+-rw-r--r--   0        0        0     3617 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/config.py
+-rw-r--r--   0        0        0     5408 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/files.py
+-rw-r--r--   0        0        0    10994 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/log.py
+-rw-r--r--   0        0        0     4958 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/output.py
+-rw-r--r--   0        0        0    10362 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/helpers/result.py
+-rw-r--r--   0        0        0      128 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/inventory/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-03 09:50:30.972500 fotoobo-1.0.0/fotoobo/inventory/generic.py
+-rw-r--r--   0        0        0     5203 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/inventory/inventory.py
+-rwxr-xr-x   0        0        0     1359 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/main.py
+-rw-r--r--   0        0        0      428 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/__init__.py
+-rw-r--r--   0        0        0     1284 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/convert.py
+-rw-r--r--   0        0        0       92 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/ems/__init__.py
+-rw-r--r--   0        0        0     1626 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/ems/get.py
+-rw-r--r--   0        0        0     8338 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/ems/monitor.py
+-rw-r--r--   0        0        0       56 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/faz/__init__.py
+-rw-r--r--   0        0        0      809 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/faz/get.py
+-rw-r--r--   0        0        0      129 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/__init__.py
+-rw-r--r--   0        0        0     4619 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/config.py
+-rw-r--r--   0        0        0     2377 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/get.py
+-rw-r--r--   0        0        0     2978 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/main.py
+-rw-r--r--   0        0        0     4274 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fgt/monitor.py
+-rw-r--r--   0        0        0      105 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fmg/__init__.py
+-rw-r--r--   0        0        0     4417 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fmg/get.py
+-rw-r--r--   0        0        0     2733 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/fmg/main.py
+-rw-r--r--   0        0        0     1882 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/get.py
+-rw-r--r--   0        0        0     1306 2023-08-03 09:50:30.976501 fotoobo-1.0.0/fotoobo/tools/greet.py
+-rw-r--r--   0        0        0     3711 2023-08-03 09:50:30.976501 fotoobo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 fotoobo-1.0.0/PKG-INFO
```

### Comparing `fotoobo-0.9.0/LICENSE` & `fotoobo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/README.md` & `fotoobo-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,7 @@
 clarify the following:
 
 fotoobo may be used as an imported module under the same terms that the LGPL states for dynamically
 linked (binary) libraries. So you may use fotoobo (unmodified) with code under another license (free
 or commercial).
 
 All changes to the fotoobo code itself are subject to the LGPL v3.
-
-# Legacy documentation
-
-This documentation has not yet been migrated to the Sphinx documentation.
-
-- [The FortiGate configuration structure in fotoobo](docs_legacy/fortinet/fortigate_config.md)
-- [FortiGate configuration check](docs_legacy/fortinet/fortigate_config_check.md)
```

### Comparing `fotoobo-0.9.0/fotoobo/cli/convert.py` & `fotoobo-1.0.0/fotoobo/cli/convert.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 The fotoobo convert commands
 """
 import logging
+from pathlib import Path
 
 import typer
 
 from fotoobo.helpers import cli_path
-from fotoobo.utils import convert
+from fotoobo.helpers.files import load_json_file, save_json_file
+from fotoobo.tools import convert
 
 app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
@@ -22,39 +24,43 @@
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
 @app.command(no_args_is_help=True)
 def checkpoint(
-    infile: str = typer.Argument(
+    infile: Path = typer.Argument(
         ...,
         help="The json file to read the Checkpoint objects from.",
         show_default=False,
         metavar="[infile]",
     ),
-    outfile: str = typer.Argument(
+    outfile: Path = typer.Argument(
         ...,
         help="The json file to write the converted objects to.",
         show_default=False,
         metavar="[outfile]",
     ),
     obj_type: str = typer.Argument(
         ...,
         help="The type of objects to convert.",
         show_default=False,
         metavar="[type]",
     ),
-    cache_dir: str = typer.Argument(
+    cache_dir: Path = typer.Argument(
         None,
         help="The cache directory to use.",
         show_default=False,
         metavar="[cache_dir]",
     ),
 ) -> None:
     """
     Convert Checkpoint assets into Fortinet objects.
 
     The Checkpoint objects have to be prepared in a json file. See
     https://fotoobo.readthedocs.io/en/latest/usage/convert.html for more information.
     """
-    convert.checkpoint(infile, outfile, obj_type, cache_dir)
+    checkpoint_assets = load_json_file(infile)
+
+    result = convert.checkpoint(checkpoint_assets, obj_type, outfile.name, cache_dir)
+
+    save_json_file(outfile, result.get_result("fortinet_assets"))
```

### Comparing `fotoobo-0.9.0/fotoobo/cli/ems/get_commands.py` & `fotoobo-1.0.0/fotoobo/cli/ems/get_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 The FortiClient EMS get commands
 """
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
-from fotoobo.helpers.output import print_datatable
-from fotoobo.utils import ems
+from fotoobo.tools import ems
 
 app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
@@ -32,25 +31,28 @@
         help="The FortiClientEMS hostname to access (must be defined in the inventory).",
         metavar="[host]",
     )
 ) -> None:
     """
     Get the FortiClient EMS version.
     """
-    data = ems.get.version(host)
-    print_datatable(data, title="FortiClient EMS Version", headers=["FortiClient EMS", "Version"])
+    result = ems.get.version(host)
+    result.print_result_as_table(
+        title="FortiClient EMS Version",
+        headers=["FortiClient EMS", "Version"],
+    )
 
 
 @app.command()
 def workgroups(
     host: str = typer.Argument(
         "ems",
         help="The FortiClientEMS hostname to access (must be defined in the inventory).",
         metavar="[host]",
     ),
     custom: bool = typer.Option(False, "--custom", "-c", help="Only show custom groups"),
 ) -> None:
     """
     Get the FortiClient EMS workgroups.
     """
-    data = ems.get.workgroups(host, custom)
-    print_datatable(data, title="FortiClient EMS Workgroups", auto_header=True)
+    result = ems.get.workgroups(host, custom)
+    result.print_result_as_table(title="FortiClient EMS Workgroups", headers=["Group", "Count"])
```

### Comparing `fotoobo-0.9.0/fotoobo/cli/ems/main.py` & `fotoobo-1.0.0/fotoobo/cli/ems/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/cli/faz/get_commands.py` & `fotoobo-1.0.0/fotoobo/cli/faz/get_commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 The FortiAnalyzer get commands
 """
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
-from fotoobo.helpers.output import print_datatable
-from fotoobo.utils import faz
+from fotoobo.tools import faz
 
 app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
@@ -32,9 +31,12 @@
         help="The FortiAnalyzer hostname to access (must be defined in the inventory).",
         metavar="[host]",
     )
 ) -> None:
     """
     Get the FortiAnalyzer version.
     """
-    data = faz.get.version(host)
-    print_datatable(data, title="FortiAnalyzer Version", headers=["FortiAnalyzer", "Version"])
+    result = faz.get.version(host)
+    result.print_result_as_table(
+        title="FortiAnalyzer Version",
+        headers=["FortiAnalyzer", "Version"],
+    )
```

### Comparing `fotoobo-0.9.0/fotoobo/cli/faz/main.py` & `fotoobo-1.0.0/fotoobo/cli/faz/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/cli/fgt/config_commands.py` & `fotoobo-1.0.0/fotoobo/cli/fgt/config_commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,82 @@
 """
 The FortiGate get commands
 """
 import logging
+from pathlib import Path
 
 import typer
 
-from fotoobo.helpers.output import print_datatable, print_dicttable
-from fotoobo.utils import fgt
+from fotoobo.tools import fgt
 
 app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.command(no_args_is_help=True)
 def check(
-    configuration: str = typer.Argument(
+    configuration: Path = typer.Argument(
         ...,
         help="The FortiGate configuration file or directory.",
         metavar="[config]",
         show_default=False,
     ),
-    bundles: str = typer.Argument(
+    bundles: Path = typer.Argument(
         ...,
         help="Filename of the file containing the check bundles.",
         metavar="[bundles]",
         show_default=False,
     ),
 ) -> None:
     """
     Check one or more FortiGate configuration files.
     """
-    fgt.config.check(configuration, bundles)
+    result = fgt.config.check(configuration, bundles)
+
+    result.print_messages()
+
+
+@app.command(no_args_is_help=True)
+def get(
+    configuration: Path = typer.Argument(
+        ...,
+        help="The FortiGate configuration file or directory.",
+        metavar="[config]",
+        show_default=False,
+    ),
+    scope: str = typer.Argument(
+        ..., help="Scope of the configuration ('global' or 'vdom')", metavar="[scope]"
+    ),
+    path: str = typer.Argument("/", help="Configuration path", metavar="[path]"),
+) -> None:
+    """Get configuration or parts of it from one or more FortiGate configuration files"""
+    result = fgt.config.get(configuration, scope, path)
+    result.print_raw()
 
 
 @app.command(no_args_is_help=True)
 def info(
-    configuration: str = typer.Argument(
+    configuration: Path = typer.Argument(
         ...,
         help="The FortiGate configuration file or directory.",
         metavar="[config]",
         show_default=False,
     ),
     as_list: bool = typer.Option(
         False, "--list", "-l", help="Print the result as a list instead of separate blocks."
     ),
 ) -> None:
     """
     Get the information from one or more FortiGate configuration files.
     """
-    infos = fgt.config.info(configuration)
-    info_dicts = [data.__dict__ for data in infos]
+    result = fgt.config.info(configuration)
 
     if as_list:
-        print_datatable(info_dicts, auto_header=True)
+        info_dicts = []
+
+        for _, _info in result.all_results().items():
+            info_dicts.append(_info.__dict__)
+
+        result.print_table_raw(info_dicts, [], auto_header=True)
 
     else:
-        for data in info_dicts:
-            print_dicttable(data, title=data.get("hostname", "unknown"))
+        result.print_result_as_table()
```

### Comparing `fotoobo-0.9.0/fotoobo/cli/fgt/get_commands.py` & `fotoobo-1.0.0/fotoobo/cli/fgt/get_commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 # pylint: disable=anomalous-backslash-in-string
 
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
-from fotoobo.helpers.output import print_datatable
-from fotoobo.utils import fgt
+from fotoobo.tools import fgt
 
 app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
@@ -39,9 +38,9 @@
 ) -> None:
     """
     Get the FortiGate(s) version(s).
 
     The optional argument [host] makes this command somewhat magic. If you omit \[host] it searches
     for all devices of type 'fortigate' in the inventory and tries to get their FortiOS version.
     """
-    data = fgt.get.version(host)
-    print_datatable(data, title="FortiGate Versions", headers=["FortiGate", "Version"])
+    result = fgt.get.version(host)
+    result.print_result_as_table(title="FortiGate Versions", headers=["FortiGate", "Version"])
```

### Comparing `fotoobo-0.9.0/fotoobo/cli/fgt/main.py` & `fotoobo-1.0.0/fotoobo/cli/fmg/get_commands.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,100 @@
 """
-The FortiGate commands
+The FortiManager get commands
 """
 import logging
+from pathlib import Path
 
 import typer
 
-from fotoobo import utils
-from fotoobo.cli.fgt import monitor_commands as monitor
-from fotoobo.cli.fgt import config_commands as config
-from fotoobo.cli.fgt import get_commands as get
 from fotoobo.helpers import cli_path
+from fotoobo.helpers.output import write_policy_to_html
+from fotoobo.tools import fmg
 
 app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
+HELP_TEXT_HOST = "The FortiManager to access (must be defined in the inventory)."
+
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
-    The fgt subcommand callback
+    The fmg get subcommand callback
 
     Args:
         context (Context): the context object of the typer app
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
-app.add_typer(get.app, name="get", help="FortiGate get commands.")
-app.add_typer(monitor.app, name="monitor", help="FortiGate monitor commands.")
-app.add_typer(config.app, name="config", help="FortiGate config file commands.")
+@app.command()
+def adoms(
+    host: str = typer.Argument(
+        "fmg",
+        help=HELP_TEXT_HOST,
+        metavar="[host]",
+    )
+) -> None:
+    """
+    Get the FortiManager ADOM list.
+    """
+    result = fmg.get.adoms(host)
+    result.print_result_as_table(title="FortiManager ADOMs", headers=["Name", "Version"])
 
 
 @app.command()
-def backup(
+def devices(
     host: str = typer.Argument(
-        "",
-        help="The FortiGate to backup (must be defined in the inventory). "
-        "Backups all if left empty.",
-        show_default=False,
+        "fmg",
+        help=HELP_TEXT_HOST,
         metavar="[host]",
-    ),
-    backup_dir: str = typer.Option(
-        None,
-        "--backup-dir",
-        "-b",
-        help="The directory to save the backup(s) to. Default is the current working directory.",
+    )
+) -> None:
+    """
+    Get the FortiManager logical devices list.
+
+    Be aware that if a device is a cluster only the cluster
+    device is returned, not all its physical nodes.
+    """
+    result = fmg.get.devices(host)
+    result.print_result_as_table(
+        title="Fortinet devices",
+        headers=["Device Name", "Version", "HA", "Platform", "Description"],
+    )
+
+
+@app.command(no_args_is_help=True)
+def policy(
+    adom: str = typer.Argument(
+        ...,
+        help="The FortiManager ADOM to get the firewall policy from.",
+        metavar="[adom]",
         show_default=False,
-        metavar="backup_dir",
     ),
-    ftp_server: str = typer.Option(
-        None,
-        "--ftp",
-        "-f",
-        help="The ftp configuration from the inventory to send the backup to.",
-        metavar="server",
+    policy_name: str = typer.Argument(
+        ..., help="The name of the policy to get.", metavar="[policy]", show_default=False
     ),
-    smtp_server: str = typer.Option(
-        None,
-        "--smtp",
-        "-s",
-        help="The smtp configuration from the inventory to send potential errors to.",
-        metavar="server",
+    filename: Path = typer.Argument(
+        ..., help="The filename to write the policy to.", metavar="[file]", show_default=False
+    ),
+    host: str = typer.Argument(
+        "fmg",
+        help=HELP_TEXT_HOST,
+        metavar="[host]",
     ),
 ) -> None:
     """
-    Backup one or more FortiGate(s).
+    Get a FortiManager policy.
+    """
+    result = fmg.get.policy(host, adom, policy_name)
+    write_policy_to_html(result.get_result(host), filename)
+
+
+@app.command()
+def version(host: str = typer.Argument("fmg", help=HELP_TEXT_HOST, metavar="[host]")) -> None:
+    """
+    Get the FortiManager version.
     """
-    utils.fgt.backup(host, backup_dir, ftp_server, smtp_server)
+    result = fmg.get.version(host)
+    result.print_result_as_table(title="FortiManager Version", headers=["FortiManager", "Version"])
```

### Comparing `fotoobo-0.9.0/fotoobo/cli/fgt/monitor_commands.py` & `fotoobo-1.0.0/fotoobo/cli/fmg/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,86 @@
 """
-The FortiGate check commands
+The FortiManager commands
 """
-# pylint: disable=anomalous-backslash-in-string
-
 import logging
+from pathlib import Path
 
 import typer
 
+from fotoobo.cli.fmg import get_commands as get
 from fotoobo.helpers import cli_path
-from fotoobo.helpers.output import print_datatable
-from fotoobo.utils import fgt
+from fotoobo.tools import fmg
 
 app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
-    The fgt check subcommand callback
+    The fmg subcommand callback
 
     Args:
         context (Context): the context object of the typer app
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
-@app.command()
-def hamaster(
+@app.command(no_args_is_help=True)
+def assign(
+    adoms: str = typer.Argument(
+        ...,
+        help="The ADOMs to assign the global policy/objects to. Use "
+        "'fotoobo fmg get adoms' to get a list of "
+        "available ADOMs. Separate multiple ADOMs by comma (no spaces).",
+        metavar="[adoms]",
+        show_default=False,
+    ),
+    policy: str = typer.Argument(
+        ...,
+        help="The global policy to assign",
+        metavar="[policy]",
+        show_default=False,
+    ),
     host: str = typer.Argument(
         "fmg",
-        help="The FortiManager hostname to access (must be defined in the inventory).",
+        help="The FortiManager to access (must be defined in the inventory).",
         metavar="[host]",
     ),
-    smtp_server: str = typer.Option(
-        None,
-        "--smtp",
-        help="The smtp configuration from the inventory.",
-        metavar="server",
-        show_default=False,
+    timeout: int = typer.Option(
+        60,
+        "--timeout",
+        "-t",
+        help="The timeout to wait for the FortiManager task to finish.",
+        metavar="[timeout]",
+    ),
+) -> None:
+    """
+    Assign a global policy to a specified ADOM or to a list of ADOMs.
+    """
+    fmg.assign(adoms=adoms, policy=policy, host=host, timeout=timeout)
+
+
+@app.command(no_args_is_help=True)
+def post(
+    file: Path = typer.Argument(
+        ..., help="JSON file with payload(s).", show_default=False, metavar="[file]"
+    ),
+    adom: str = typer.Argument(
+        ..., help="The ADOM to issue the set command(s).", metavar="[adom]", show_default=False
+    ),
+    host: str = typer.Argument(
+        "fmg",
+        help="The FortiManager to access (must be defined in the inventory).",
+        metavar="[host]",
     ),
 ) -> None:
     """
-    Check the FortiGate HA master.
+    POST any valid JSON request to the FortiManager.
+
+    Configure the FortiManager with any valid API call(s) given within the JSON file.
+    """
+    fmg.post(file=file, adom=adom, host=host)
+
 
-    Although this command checks the HA master status of FortiGates you have to specify a
-    FortiManager to access. The command searches for all FortiGate clusters in the FortiManager
-    and checks if the designated primary node really is the HA master node.
-
-    The optional argument \[host] makes this command somewhat magic. If you omit \[host] it searches
-    for all devices in the default FortiManager (fmg) in the inventory.
-    """
-    data = fgt.monitor.hamaster(host, smtp_server)
-    print_datatable(
-        data, title="FortiGate HA master status", headers=["FortiGate Cluster", "Status"]
-    )
+app.add_typer(get.app, name="get", help="FortiManager get commands.")
```

### Comparing `fotoobo-0.9.0/fotoobo/cli/main.py` & `fotoobo-1.0.0/fotoobo/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 
 Caution: Use docstrings with care as they are used to print help texts on any command.
 """
 # pylint: disable=anomalous-backslash-in-string
 
 import logging
 import os
+from pathlib import Path
 import sys
 from typing import Optional, Union
 
 import typer
 
-from fotoobo import utils
+from fotoobo import tools
 from fotoobo.cli import convert, get
 from fotoobo.cli.ems import main as ems
 from fotoobo.cli.faz import main as faz
 from fotoobo.cli.fgt import main as fgt
 from fotoobo.cli.fmg import main as fmg
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.config import config
@@ -33,22 +34,25 @@
 )
 log = logging.getLogger("fotoobo")
 
 
 def version_callback(value: bool) -> None:
     """The version callback"""
     if value:
-        utils.get.version()
+        if not config.no_logo:
+            print_logo()
+
+        get.version(False)
         raise typer.Exit()
 
 
 @app.callback()
 def callback(  # pylint: disable=too-many-arguments
     context: typer.Context,
-    config_file: Union[str, None] = typer.Option(
+    config_file: Union[Path, None] = typer.Option(
         None,
         "--config",
         "-c",
         help="Set the fotoobo configuration file. \[default: fotoobo.yaml]",
         show_default=False,
         metavar="[file]",
     ),
@@ -119,15 +123,15 @@
     It allows you to greet someone with different colors in different languages.
     """
     if not name:
         try:
             name = os.getlogin().capitalize()
         except OSError:  # We need this, will fail on GitHub otherwise...
             name = ""
-    utils.greet(str(name), bye, log_enabled)
+    tools.greet(str(name), bye, log_enabled)
 
 
 # fotoobo specific commands
 app.add_typer(convert.app, name="convert", help="Convert commands for fotoobo.")
 app.add_typer(get.app, name="get", help="Get information about fotoobo or your configuration.")
 
 # commands for the Fortinet products
```

### Comparing `fotoobo-0.9.0/fotoobo/exceptions/exceptions.py` & `fotoobo-1.0.0/fotoobo/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/convert.py` & `fotoobo-1.0.0/fotoobo/fortinet/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """The powerful convert module
 
 Please refer to docs_legacy/convert_checkpoint_mappings.drawio.svg to see how a Checkpoint asset is
 going to be converted into a Fortinet asset.
 
-The Fortinet assets are referenced by their names. Even if we set a uuid we cannot use the uuid to
+The Fortinet assets are referenced by their names. Even if we set an uuid we cannot use the uuid to
 access the asset. The uuid is only supported for network assets and not for service assets.
 """
 
 import copy
 import logging
-import os
+from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from fotoobo.exceptions import GeneralError
 from fotoobo.helpers.files import load_json_file, save_json_file
 
 log = logging.getLogger("fotoobo")
 
 
 class CheckpointConverter:
     """
     The Checkpoint converter class
     """
 
-    def __init__(self, assets: Any, cache_file: Optional[str] = None) -> None:
-        self.assets = assets
+    def __init__(self, assets: Any, cache_file: Optional[Path] = None) -> None:
+        self.assets = copy.deepcopy(assets)
         self.converted: List[Any] = []
         self.supported_types = [
             "hosts",
             "networks",
             "address_ranges",
             "groups",
             "services_icmp",
@@ -40,15 +40,14 @@
         self.cache_file = cache_file
 
     def convert(self, obj_type: str, bulk_size: int = 100) -> List[Any]:
         """
         Convert Checkpoint configuration objects into Fortinet syntax.
 
         Args:
-            assets (Any): the original assets
             obj_type (str): define the type of objects to convert
             bulk_size: the bulk size to generate
 
         Returns:
             List: the converted assets
         """
 
@@ -67,15 +66,15 @@
         log.debug("converting asset type '%s'", obj_type)
         log.debug("found '%s' asset(s)", len(self.assets[obj_type]))
         assets = getattr(self, "_convert_" + obj_type)()
 
         # Now do the caching if cache_file is given
         if self.cache_file:
             cache: List[Any] = []
-            if os.path.isfile(self.cache_file):
+            if self.cache_file.is_file():
                 log.debug("found cache file '%s'", self.cache_file)
                 cache = list(load_json_file(self.cache_file) or [])
 
             save_json_file(self.cache_file, assets)
             assets = [asset for asset in assets if asset not in cache]
             log.debug("found '%s' new asset(s) not in cache", len(assets))
 
@@ -270,15 +269,15 @@
 
     def _convert_services_tcp(self) -> List[Dict[str, Any]]:
         """
         Convert Checkpoint services_tcp objects
 
         Possible values for "port" in the Checkpoint assets are:
         - "2000" is a single port which will be "2000"
-        - "3000-3500" is a portrange which will be "3000-4000"
+        - "3000-3500" is a port range which will be "3000-4000"
         - ">4000" will be converted to "4001-65535"
         - "<5000" will be converted to "1-4999"
 
         Returns:
             list: converted Fortinet objects
         """
         objects = self.assets["services_tcp"]
@@ -309,15 +308,15 @@
             assets.append(param)
 
         return assets
 
     def _convert_services_udp(self) -> List[Dict[str, Any]]:
         """
         Convert Checkpoint services_udp objects
-        Even though the UDP services are almost identical to the TCP services we use it's own
+        Even though the UDP services are almost identical to the TCP services we use its own
         convert function. This adds some redundancy but removes complexity and segregates duties.
 
         For possible values for the Checkpoint "port" field and how they will get converted refer
         to the _convert_services_tcp function.
 
         Returns:
             list: converted Fortinet objects
@@ -361,15 +360,15 @@
         objects = copy.deepcopy(self.assets["service_groups"])
         assets = []
         while objects:
             obj = objects.pop(0)
             url_name = obj["name"].replace("/", "\\/")
 
             # patch for special group "gIntegrity_Server"
-            # This one is not able to be converted as the members are not supported by FortiManager.
+            # This one cannot be converted as the members are not supported by FortiManager.
             # Remove the group "gIntegrity_Server" from the Checkpoint global policy (it seems not
             # to be in use). Then this patch can be removed.
             if url_name == "gIntegrity_Server":
                 continue  # pragma: no cover
 
             forti_members = []
             for uid in obj["members"]:
```

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/fortianalyzer.py` & `fotoobo-1.0.0/fotoobo/fortinet/fortianalyzer.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/forticlientems.py` & `fotoobo-1.0.0/fotoobo/fortinet/forticlientems.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 FortiClient EMS Class
 """
 import logging
-import os
 import pickle
+from pathlib import Path
 from typing import Any, Dict, Optional
 
 import requests
 
 from fotoobo.exceptions import APIError, GeneralWarning
 
 from .fortinet import Fortinet
@@ -56,14 +56,15 @@
     ) -> requests.models.Response:
         """
         API request to a FortiClientEMS device.
 
         Args:
             method (str): request method from [get, post]
             url (str): rest API URL to request data from
+            headers (dict): additional headers (if needed)
             params (dict): dictionary with parameters (if needed)
             payload (dict): JSON body for post requests (if needed)
             timeout (float): the requests read timeout
 
         Returns:
             response: response from the request
         """
@@ -77,24 +78,23 @@
         According to Fortinet support the FortiClient EMS version may be read out of the endpoint
         /system/consts/get?system_update_time=1. This endpoint is not (yet) documented. Let's hope
         they support it in case of any issue.
 
         Returns:
             str: version
         """
-        ems_version: str = ""
         try:
             response = self.api("get", "/system/consts/get?system_update_time=1")
 
         except APIError as err:
             log.warning("%s returned: %s", self.hostname, err.message)
             raise GeneralWarning(f"{self.hostname} returned: {err.message}") from err
 
         try:
-            ems_version = response.json()["data"]["System"]["VERSION"]
+            ems_version: str = response.json()["data"]["System"]["VERSION"]
 
         except KeyError as err:
             log.warning("did not find any FortiClient EMS version number in response")
             raise GeneralWarning(
                 "did not find any FortiClient EMS version number in response"
             ) from err
 
@@ -104,21 +104,21 @@
         """
         Login to the FortiClientEMS.
 
         Returns:
             int: status code from the FortiClient EMS logon
         """
         status = 401
-        cookie_file = os.path.abspath(os.path.join(self.cookie_path, f"{self.hostname}.cookie"))
+        cookie = Path(self.cookie_path).expanduser() / f"{self.hostname}.cookie"
         if self.cookie_path:
-            log.debug("searching cookie in %s", cookie_file)
-            if os.path.isfile(cookie_file):
+            log.debug("searching cookie in %s", cookie)
+            if cookie.is_file():
                 log.debug("cookie exists. skipping login")
-                with open(cookie_file, "rb") as cookiefile:
-                    self.session.cookies.update(pickle.load(cookiefile))  # type: ignore
+                with cookie.open("rb") as cookie_file:
+                    self.session.cookies.update(pickle.load(cookie_file))  # type: ignore
 
                 try:
                     response = self.api("get", "/system/serial_number")
                     if (
                         "retval" in response.json()["result"]
                         and int(response.json()["result"]["retval"]) == 1
                     ):
@@ -136,16 +136,21 @@
 
         if status == 401:
             log.debug("login to %s", self.hostname)
             payload = {"name": self.username, "password": self.password}
             response = self.api("post", "/auth/signin", payload=payload)
             if response.status_code == 200 and self.cookie_path:
                 log.debug("saving cookie for %s", self.hostname)
-                with open(cookie_file, "wb") as cookiefile:
-                    pickle.dump(self.session.cookies, cookiefile)
+
+                try:
+                    with cookie.open("wb") as cookie_file:
+                        pickle.dump(self.session.cookies, cookie_file)
+
+                except FileNotFoundError:
+                    log.warning("unable to save cookie file: %s", str(cookie.resolve()))
 
             status = response.status_code
 
         return status
 
     def logout(self) -> int:
         """
```

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/fortigate.py` & `fotoobo-1.0.0/fotoobo/fortinet/fortigate.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/fortigate_config.py` & `fotoobo-1.0.0/fotoobo/fortinet/fortigate_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 The FortiGate configuration class represents the whole or parts of a FortiGate configuration
 """
 import logging
+from pathlib import Path
 from typing import IO, Any, Dict, List, Optional
 
 from fotoobo.exceptions import GeneralWarning
 from fotoobo.helpers.files import load_json_file, save_json_file
 
 from .fortigate_info import FortiGateInfo
 
@@ -38,17 +39,17 @@
         Return a config snippet from the given configuration path.
 
         Args:
             scope (str) : the configuration part to get the configuration from (global|vdom)
             path (str)  : from where should the configuration come?
             Examples:
             /                           : the whole configuration (default)
-            /system/global/...          : subpath in global configuration
+            /system/global/...          : sub-path in global configuration
             /system/global/admin-scp    : exact configuration option
-            /root/firewall/address/...  : subpath in root vdom
+            /root/firewall/address/...  : sub-path in root vdom
 
         Returns:
             any: FortiGateConfig configuration value or snippet from the given path.
             If the path or value does not exist None is returned.
         """
         log.debug("getting configuration from scope: '%s'", scope)
         log.debug("getting configuration from path: '%s'", path)
@@ -80,46 +81,46 @@
             List: List of VDOMs
         """
         vdoms: List[str] = []
         if self.info.vdom == "1":
             vdoms = list(self.vdom_config.keys())
         return vdoms
 
-    def save_configuration_file(self, filename: str) -> None:
+    def save_configuration_file(self, configuration_file: Path) -> None:
         """
         Save the configuration to a json configuration file.
 
         Args:
-            filename (str): The json file to load the FortiGate configuration from
+            configuration_file (Path): The json file to load the FortiGate configuration from
         """
         save_json_file(
-            filename,
+            configuration_file,
             {"global": self.global_config, "vdom": self.vdom_config, "info": self.info.__dict__},
         )
 
     @staticmethod
-    def parse_configuration_file(filename: str) -> "FortiGateConfig":
+    def parse_configuration_file(configuration_file: Path) -> "FortiGateConfig":
         """
         Parse the FortiGate configuration from a file into a python object
 
         Args:
-            filename (str): the filename of the FortiGate configuration file
+            configuration_file (Path): the filename of the FortiGate configuration file
 
         Returns:
             FortiGateConfig: the parsed FortiGate configuration object
         """
-        log.debug("start configuration parser with file '%s'", filename)
+        log.debug("start configuration parser with file '%s'", configuration_file)
         FortiGateConfig._config_path = []
-        with open(filename, "r", encoding="UTF-8") as forti_file:
+        with configuration_file.open(encoding="UTF-8") as forti_file:
             parsed_config = FortiGateConfig._parse_to_dict(forti_file)
 
         global_config: Dict[str, Any] = {}
         vdom_config: Dict[str, Any] = {}
-        if not "info" in parsed_config:
-            raise GeneralWarning(f"There is no info in {filename}")
+        if "info" not in parsed_config:
+            raise GeneralWarning(f"There is no info in {configuration_file}")
         info = parsed_config["info"]
         parsed_config.pop("info")
 
         if info["vdom"] == "0":
             global_config["system"] = {}
             global_config["system"] = parsed_config["system"]
             parsed_config.pop("system")
@@ -129,46 +130,46 @@
         else:
             global_config = parsed_config["global"]
             vdom_config = parsed_config["vdom"]
 
         return FortiGateConfig(global_config, vdom_config, info)
 
     @staticmethod
-    def load_configuration_file(filename: str) -> "FortiGateConfig":
+    def load_configuration_file(configuration_file: Path) -> "FortiGateConfig":
         """
         Create a FortiGateConfig object from a json configuration file.
 
         Args:
-            filename (str): The json file to load the FortiGate configuration from
+            configuration_file (Path): The json file to load the FortiGate configuration from
 
         Returns:
             FortiGateConfig: FortiGate configuration object
         """
-        data = load_json_file(filename)
+        data = load_json_file(configuration_file)
         return FortiGateConfig(data["global"], data["vdom"], data["info"])  # type: ignore
 
     @staticmethod
     def _config_convert_dict_to_list(config: Dict[str, Any]) -> List[Any]:
         """
         Convert a FortiGate configuration list like part to a configuration list.
 
         Args:
             config (dict): a FortiGate configuration list like part from a dict
 
         Returns:
             list: configuration list as list
         """
-        conflist: List[str] = []
+        configs: List[str] = []
 
         for key, value in config.items():
-            newconf = value
-            newconf["id"] = int(key)
-            conflist.append(newconf)
+            new_config = value
+            new_config["id"] = int(key)
+            configs.append(new_config)
 
-        return conflist
+        return configs
 
     @staticmethod
     def _config_is_list(config: Dict[str, Any]) -> bool:
         """
         Check if a FortiGate configuration part contains a list of elements.
 
         Args:
@@ -184,34 +185,34 @@
         for key in config.keys():
             if not key.isnumeric():
                 is_list = False
 
         return is_list
 
     @staticmethod
-    def _get_nested_dict(configs: List[str], newdata: Any) -> Dict[str, Any]:
+    def _get_nested_dict(configs: List[str], new_data: Any) -> Dict[str, Any]:
         """
-        Create a nested configuration dict from a list of strings and add newdata to the last key.
+        Create a nested configuration dict from a list of strings and add new data to the last key.
 
         Args:
             configs (list): configuration leafs to process
-            newdata (any): data to add to the last key
+            new_data (any): data to add to the last key
 
         Returns:
             dict: the nested configuration
         """
-        newdict = {}
+        out_dict = {}
         key = configs.pop(0)
         if len(configs) > 0:
-            newdict[key] = FortiGateConfig._get_nested_dict(configs, newdata)
+            out_dict[key] = FortiGateConfig._get_nested_dict(configs, new_data)
 
         else:
-            newdict[key] = newdata
+            out_dict[key] = new_data
 
-        return dict(newdict)
+        return dict(out_dict)
 
     @staticmethod
     def _parse_config_comment(info: Dict[str, Any], line: str) -> Dict[str, str]:
         """
         Parses a comment line in a FortiGate configuration and extracts interesting values.
         The values are then written to an info dict as meta-information.
 
@@ -247,14 +248,15 @@
 
         Returns:
             dict: A dict which contains the parsed FortiGate configuration
         """
         config: Any = {}
         info: Dict[str, str] = {}
         multiline: str = ""
+        multiline_key: str = ""
 
         for line in config_file:
             line = line.strip()
 
             # handle empty lines
             if not line:
                 continue
@@ -267,15 +269,14 @@
             if multiline:
                 multiline += f"\n{line}"
                 if line.endswith('"'):
                     config[multiline_key], multiline = multiline.strip('"'), ""
                 continue
             # check if a multiline string starts. begin with "set" and uneven amount of quotes (")
             if line.startswith("set ") and line.count('"') % 2 == 1 and not line.endswith('"'):
-                multiline_key: str = ""
                 _, multiline_key, value = line.split(maxsplit=2)  # first part is always "set"
                 multiline += value
                 continue
 
             # handle configuration option
             if line.startswith("set "):
                 _, key, value = line.split(maxsplit=2)  # first part ist always "set"
@@ -289,21 +290,21 @@
                 if len(line[7:].split(" ")) == 1:
                     FortiGateConfig._config_path.append(line[7:])
                     config[line[7:].strip('"')] = FortiGateConfig._parse_to_dict(config_file)
 
                 else:
                     FortiGateConfig._config_path.append(line[7:])
                     config_path = [word.strip('"') for word in line[7:].split()]
-                    tempconfig = FortiGateConfig._get_nested_dict(
+                    temp_config = FortiGateConfig._get_nested_dict(
                         config_path[1:], FortiGateConfig._parse_to_dict(config_file)
                     )
 
                     if config_path[0] not in config:
                         config[config_path[0]] = {}
-                    config[config_path[0]] = {**config[config_path[0]], **tempconfig}
+                    config[config_path[0]] = {**config[config_path[0]], **temp_config}
 
             if line.startswith("edit "):
                 FortiGateConfig._config_path.append(line[5:])
                 config[line[5:].strip('"')] = FortiGateConfig._parse_to_dict(config_file)
 
             # handle section ends
             if line == "end":
```

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/fortigate_config_check.py` & `fotoobo-1.0.0/fotoobo/fortinet/fortigate_config_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 """
 FortiGate configuration checker
 """
 import logging
 from typing import Any, Dict, List
 
 from fotoobo.exceptions import GeneralError
+from fotoobo.helpers.result import Result
 from fotoobo.fortinet.fortigate_config import FortiGateConfig
 
 log = logging.getLogger("fotoobo")
 
 
 class FortiGateConfigCheck:
     """The FortiGate configuration check class"""
 
-    def __init__(self, config: FortiGateConfig, checks: Any) -> None:
+    def __init__(self, config: FortiGateConfig, checks: Any, result: Result[Any]) -> None:
         """
         Initialize the configuration checker.
 
         Args:
             config (FortiGateConfig): the FortiGate configuration
             checks (dict): the checks to do against the FortiGate configuration
         """
         self.allowed_checks: List[str] = ["count", "exist", "value", "value_in_list"]
         self.config = config
         self.checks = checks
-        self.results: List[str] = []
+        self.result = result
 
     def add_message(self, chk: Dict[str, Any], msg: str) -> None:
         """
         Generates a styled message and appends it to the results.
 
         Args:
             chk (Dict[str, any]): the check which generated the message
             msg (str): the message to sent to the messages list
         """
         check_name = f" (check_name: [var]{chk['name']}[/])" if "name" in chk else ""
         message = f"[chk]{chk['type']}[/]: {msg}{check_name}"
-        self.results.append(message)
+        log.info(message)
+        self.result.push_message(self.config.info.hostname, message)
 
-    def execute_checks(self) -> None:  # pylint: disable=too-many-branches
+    def execute_checks(self) -> Result[Any]:  # pylint: disable=too-many-branches
         """
         Execute the FortiGate configuration checks.
 
         After initializing a FortiGateConfigCheck object you can run this method to actually run
         the checks and write the results into the results object.
         """
         if not self.checks:
@@ -117,15 +119,15 @@
                 elif self.config.info.vdom == "1":
                     for vdom in self.config.get_vdoms():
                         config = self.config.get_configuration(
                             check["scope"], vdom + "/" + check["path"]
                         )
                         getattr(self, "_check_" + check["type"])(config, check)
 
-        self.results = [f"[hst]{self.config.info.hostname}[/]: {result}" for result in self.results]
+        return self.result
 
     def _check_count(self, config: Any, chk: Dict[str, Any]) -> None:
         """
         Check the configuration list count.
 
         Args:
             config: FortiGate configuration part to check
```

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/fortigate_info.py` & `fotoobo-1.0.0/fotoobo/fortinet/fortigate_info.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/fortimanager.py` & `fotoobo-1.0.0/fotoobo/fortinet/fortimanager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 FortiManager Class
 """
 import logging
 import re
+from pathlib import Path
 from time import sleep
 from typing import Any, Dict, List, Optional
 
 import requests
 
 from .fortinet import Fortinet
 
@@ -19,25 +20,28 @@
     """
 
     def __init__(self, hostname: str, username: str, password: str, **kwargs: Any) -> None:
         """
         Set some initial parameters.
 
         Args:
-            hostname (str): the hostname of the FortiGate to connect to
-            username (str): username
-            password (str): password
-            **kwargs (dict): see Fortinet class for available arguments
+            hostname:       The hostname of the FortiGate to connect to
+            username:       The Username
+            password:       The password
+
+        Keyword Args:
+            session_dir:    The path where to load/save the FortiManager session key
+            **kwargs:       See Fortinet class for more available arguments
         """
         super().__init__(hostname, **kwargs)
         self.api_url = f"https://{self.hostname}:{self.https_port}/jsonrpc"
         self.password = password
-        self.sessionkey: str = ""
         self.username = username
-        # self.login()
+        self.session_key: str = ""
+        self.session_path: str = kwargs.get("session_path", "")
         self.type = "fortimanager"
         self.ignored_adoms = [
             "FortiAnalyzer",
             "FortiAuthenticator",
             "FortiCache",
             "FortiCarrier",
             "FortiClient",
@@ -54,42 +58,49 @@
             "Syslog",
             "Unmanaged_Devices",
             "others",
             "root",
             "rootp",
         ]
 
+    def __del__(self) -> None:
+        """The destructor"""
+        if self.session_key and not self.session_path:
+            self.logout()
+
     def api(  # pylint: disable=too-many-arguments
         self,
         method: str,
         url: str = "",
         headers: Optional[Dict[str, str]] = None,
         params: Optional[Dict[str, str]] = None,
         payload: Optional[Dict[str, Any]] = None,
         timeout: Optional[float] = None,
     ) -> requests.models.Response:
         """
         API request to a FortiManager device.
 
         It uses the super.api method but it has to enrich the payload in post requests with the
-        needed sessionkey.
+        needed session key.
 
         Args:
-            method (str): request method from [get, post]
-            url (str): rest API URL to request data from
-            params (dict): dictionary with parameters (if needed)
-            payload (dict): JSON body for post requests (if needed)
-            timeout (float): the requests read timeout in seconds
+            method:     Request method from [get, post]
+            url:        Rest API URL to request data from
+            params:     Dictionary with parameters (if needed)
+            payload:    JSON body for post requests (if needed)
+            timeout:    The requests read timeout in seconds
 
         Returns:
-            response: response from the request
+            Response from the request
         """
+        if not self.session_key:
+            self.login()
         payload = payload or {}
         if method.lower() == "post":
-            payload["session"] = self.sessionkey
+            payload["session"] = self.session_key
 
         return super().api(
             method, url, headers=headers, payload=payload, params=params, timeout=timeout
         )
 
     def assign_all_objects(self, adoms: str, policy: str) -> int:
         """
@@ -179,37 +190,67 @@
 
         return fmg_version
 
     def login(self) -> int:
         """
         Login to the FortiManager.
 
-        If the login to the FortiManager was successful it stores the session key in rhe object
+        If the login to the FortiManager was successful it stores the session key in the object.
         We do not use requests.session as the session key is just a string which is saved directly.
 
         Returns:
             int: status code from the FortiManager login
         """
         status: int = 401
-        if self.username and self.password:
+
+        if self.session_path:
+            session_file = Path(self.session_path).expanduser() / f"{self.hostname}.key"
+            if session_file.exists():
+                log.debug("loading session key from file %s", session_file)
+                with session_file.open(encoding="UTF-8") as file:
+                    self.session_key = file.read()
+                    payload = {
+                        "method": "get",
+                        "params": [{"url": "/sys/status"}],
+                        "session": self.session_key,
+                    }
+                    response = super().api("post", payload=payload)
+                    status = response.status_code
+                    if (
+                        response.status_code == 200
+                        and response.json()["result"][0]["status"]["code"] == 0
+                    ):
+                        log.debug("Session key is still valid")
+                    else:
+                        log.debug("Session key is invalid")
+                        self.session_key = ""
+
+            else:
+                log.debug("session file %s does ot exist", session_file)
+
+        if not self.session_key and self.username and self.password:
+            log.debug("login to %s", self.hostname)
             payload = {
                 "method": "exec",
                 "params": [
                     {
                         "data": {"passwd": self.password, "user": self.username},
                         "url": "/sys/login/user",
                     }
                 ],
             }
-            response = self.api("post", payload=payload)
-
+            response = super().api("post", payload=payload)
             if response.status_code == 200:
                 if "session" in response.json():
-                    log.debug("save session key")
-                    self.sessionkey = response.json()["session"]
+                    log.debug("store session key")
+                    self.session_key = response.json()["session"]
+                    if self.session_path:
+                        log.debug("saving session key into file %s", session_file)
+                        with session_file.open("w", encoding="UTF-8") as file:
+                            file.write(self.session_key)
 
             status = response.status_code
 
         return status
 
     def logout(self) -> int:
         """
@@ -217,41 +258,41 @@
 
         Returns:
             int: status code from the FortiManager logout
         """
         payload: Dict[str, Any] = {
             "method": "exec",
             "params": [{"url": "/sys/logout"}],
-            "session": self.sessionkey,
+            "session": self.session_key,
         }
         response = self.api("post", payload=payload)
+        self.session_key = ""
         return response.status_code
 
     def post(self, adom: str, payloads: Any) -> int:
         """
         POST method to FortiManager.
 
         You can pass a single payload (Dict) or a list of payloads (List of Dict).
 
         Args:
             adom (str): the ADOM name to issue the set commands to. If you wish to update the
-            Global ADOM specify 'global' as ADOM.
+                        Global ADOM specify 'global' as ADOM.
 
             payload(s) (Any): one payload (Dict) or a list of payloads (List of Dict)
 
         Returns:
             int: amount of errors ocurred during the set command
         """
         # if payload is a dict convert it to a list with one dict in it.
         if isinstance(payloads, dict):
             payloads = [payloads]
         errors = 0
         for payload in payloads:
             for i, _ in enumerate(payload["params"]):
-
                 # Here we have to replace the {adom} in the URL entry:
                 #    for Global: /pm/config/ global      /obj/firewall/address/{address}
                 #    for ADOM:   /pm/config/ adom/{adom} /obj/firewall/address/{address}
                 #                            \_________/ --> this is the {adom} part in the payload
                 adom_str = "global" if adom.lower() == "global" else f"adom/{adom}"
                 payload["params"][i]["url"] = payload["params"][i]["url"].replace(
                     "{adom}", adom_str
```

### Comparing `fotoobo-0.9.0/fotoobo/fortinet/fortinet.py` & `fotoobo-1.0.0/fotoobo/fortinet/fortinet.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,33 +22,36 @@
     from this class. If there are methods which have to be defined in every subclass it has to be
     defined here with the abstractmethod decorator.
     """
 
     def __init__(self, hostname: str, **kwargs: Any) -> None:
         """
         Set some initial parameters for the Fortinet super class.
+
         It also initializes a requests session. If you're making several requests to the same host,
         the underlying TCP connection will be reused, which can result in a significant performance
         increase. (https://docs.python-requests.org/en/master/user/advanced/)
 
         Args:
             hostname (str): the hostname of the Fortinet device to connect to
-            **kwargs: additional arguments from the following list:
-                https_port (int): The tcp port number to connect to the https api
-                    If you do not specify a port number it is set to 443 by default.
-                proxy (str): proxy server to use to connect to the Fortinet device
-                    If you need to connect to your Fortinet device through a proxy server you can
-                    set it here as as string. If needed you may append the proxy server port with a
-                    column to the proxy server. e.g. "proxy.local:8000".
-                ssl_verify (bool): enable/disable SSL certificate check
-                    When ssl_verify is enabled you have to install a trusted SSL certificate onto
-                    the device you wish to connect to. If you set ssl_verify to false it will also
-                    disable the warnings in urllib3. This prevents unwanted SSL warnings to be
-                    logged.
-                timeout (float): connection timeout in seconds
+
+        Keyword Args:
+            https_port (int): The tcp port number to connect to the https api
+                If you do not specify a port number it is set to 443 by default.
+            proxy (str): proxy server to use to connect to the Fortinet device
+                If you need to connect to your Fortinet device through a proxy server you can
+                set it here as as string. If needed you may append the proxy server port with a
+                column to the proxy server. e.g. "proxy.local:8000".
+            ssl_verify (bool): enable/disable SSL certificate check
+                When ssl_verify is enabled you have to install a trusted SSL certificate onto
+                the device you wish to connect to. If you set ssl_verify to false it will also
+                disable the warnings in urllib3. This prevents unwanted SSL warnings to be
+                logged.
+
+            timeout (float): connection timeout in seconds
         """
         self.api_url: str = ""
         self.hostname: str = hostname
         self.https_port: int = kwargs.get("https_port", 443)
         self.session = requests.Session()
         self.session.trust_env = False
         self.session.proxies: Dict[str, Any] = {"http": None, "https": None}  # type: ignore
@@ -77,15 +80,14 @@
         Args:
             method (str): request method from [get, post]
             url (str): rest API URL to request data from
             params (dict): dictionary with parameters (if needed)
             payload (dict): JSON body for post requests (if needed)
             timeout (float): the requests read timeout
 
-
         Returns:
             response: response from the request
         """
         full_url = f"{self.api_url}/{url.strip('/')}".strip("/")
         params = params or {}
         payload = payload or {}
         timeout = timeout or self.timeout
```

### Comparing `fotoobo-0.9.0/fotoobo/helpers/cli.py` & `fotoobo-1.0.0/fotoobo/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/helpers/config.py` & `fotoobo-1.0.0/fotoobo/helpers/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 """
 The config helper is used to load and set basic configuration for fotoobo. Some configuration
 options may be set by the global configuration file which by default points to fotoobo.yaml in the
-local directory. Some configuration options may be set by command line parameters regarding to the
-cli help system.
+local directory. Some configuration options may be set by command line parameters as described in
+the cli help system.
 If there are configuration options available in the global configuration file and also as a command
 line option, the command line option takes precedence over the global configuration file option.
 """
-import os
 from dataclasses import dataclass, field
+from pathlib import Path
 from typing import Any, Dict, Union
 
 from fotoobo.helpers.files import load_yaml_file
 
 
 @dataclass(eq=False, order=False)
 class Config:
     """
     This is the configuration dataclass for the global configuration options.
     First all the configuration options must be initialized.
     If an option is not defined here it is not guaranteed that it may be used later in the code.
     """
 
     # set default values
-    inventory_file: str = "inventory.yaml"
+    inventory_file: Path = Path("inventory.yaml")
     logging: Union[Dict[str, Any], None] = None
     audit_logging: Union[Dict[str, Any], None] = None
     no_logo: bool = False
-    snmp_community: str = ""
     cli_info: Dict[str, Any] = field(default_factory=dict)
     ssl_verify: Union[str, bool] = True
 
-    def load_configuration(self, config_file: Union[str, None]) -> None:
+    def load_configuration(self, config_file: Union[Path, None]) -> None:
         """
         Load the global fotoobo configuration file. If the configuration file is not present it just
         will be ignored and all the options remain as they are.
         If a file is present it looks for configuration options to set. Keep in mind that it is not
         mandatory to define every option in the configuration file. For that case make sure that an
-        option not present in the configuration file is set with it's default.
+        option not present in the configuration file is set with its default.
 
         Args:
-            config_file (str): fotoobo configuration file to load configuration from
+            config_file (Path): fotoobo configuration file to load configuration from
         """
 
         # If no explicit config file has been given, search at the predefined places
         if config_file is None:
-            fotoobo_yaml_in_dot_config = os.path.join(
-                os.path.expanduser("~"), ".config", "fotoobo.yaml"
-            )
+            fotoobo_yaml_in_dot_config = Path("~").expanduser() / ".config" / "fotoobo.yaml"
 
             # First we check whether there is a project fotoobo.yaml in the
             # current working directory
-            if os.path.isfile("fotoobo.yaml"):
-                config_file = "fotoobo.yaml"
+            if Path("fotoobo.yaml").is_file():
+                config_file = Path("fotoobo.yaml")
 
             # Second we check whether there is a user wide fotoobo.yaml in the .config folder
-            elif os.path.isfile(fotoobo_yaml_in_dot_config):
+            elif fotoobo_yaml_in_dot_config.is_file():
                 config_file = fotoobo_yaml_in_dot_config
 
             # If no config file can be found we rest with the defaults
             else:
                 return
 
         if config_file:
             if loaded_config := load_yaml_file(config_file):
                 # We need a dict here
                 loaded_config = dict(loaded_config)
 
                 # then set the config options from file if set in file
-                self.inventory_file = loaded_config.get("inventory", self.inventory_file)
+                self.inventory_file = Path(
+                    loaded_config.get("inventory", self.inventory_file)
+                ).expanduser()
+
+                if not self.inventory_file.is_absolute():
+                    self.inventory_file = config_file.parent / self.inventory_file
 
                 if loaded_config.get("logging"):
                     self.logging = loaded_config["logging"]
 
                 if loaded_config.get("audit_logging"):
                     self.audit_logging = loaded_config["audit_logging"]
 
                 self.no_logo = loaded_config.get("no_logo", self.no_logo)
-                self.snmp_community = loaded_config.get("snmp_community", self.snmp_community)
 
                 self.ssl_verify = loaded_config.get("ssl_verify", self.ssl_verify)
 
 
 config = Config()
```

### Comparing `fotoobo-0.9.0/fotoobo/helpers/log.py` & `fotoobo-1.0.0/fotoobo/helpers/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,24 @@
 import logging
 import logging.config
 import os
 import pwd
 import socket
 from datetime import datetime
 from logging.handlers import RotatingFileHandler, SysLogHandler
+from syslog import (
+    LOG_AUTH,
+    LOG_CRIT,
+    LOG_DEBUG,
+    LOG_ERR,
+    LOG_INFO,
+    LOG_USER,
+    LOG_WARNING,
+)
 from typing import Optional, Union
-from syslog import LOG_AUTH, LOG_CRIT, LOG_DEBUG, LOG_ERR, LOG_INFO, LOG_USER, LOG_WARNING
 
 from rich.logging import RichHandler
 
 from fotoobo.exceptions import GeneralError, GeneralWarning
 from fotoobo.helpers.config import config
 from fotoobo.helpers.files import load_yaml_file
 
@@ -46,17 +54,14 @@
 
     def format(self, record: logging.LogRecord) -> str:
         """
         Format the message
 
         Args:
             record:
-
-        Returns:
-
         """
 
         if record.levelname == "DEBUG":
             level: int = LOG_DEBUG
         elif record.levelname == "INFO":
             level = LOG_INFO
         elif record.levelname == "WARNING":
@@ -103,19 +108,16 @@
         """
         This function will configure the logging for fotoobo
 
         Args:
             log_switch: Whether we globally turn logging off or on
             log_level:  The desired log_level (given by CLI argument)
 
-        Returns:
-            Nothing
-
         Raises:
-            GeneralError    On unrecoverable errors (usually on non-existing/empty or
+            GeneralError:   On unrecoverable errors (usually on non-existing/empty or
                             invalid logging configuration file
         """
         # pylint: disable=too-many-branches
         # pylint: disable=too-many-statements
 
         # Make some defaults for (some chatty) external libraries
         logging.getLogger("requests").setLevel(logging.CRITICAL)
@@ -153,15 +155,15 @@
                 "WARNING",
                 "INFO",
                 "DEBUG",
             ]:
                 raise GeneralWarning(f"Loglevel {log_level} not known")
 
             # If nothing is configured in the config file but logging is requested from
-            # the commandline use a simple basic config
+            # the command line use a simple basic config
             if not config.logging and log_switch:
                 # Configure logger "fotoobo"
                 logger.setLevel(log_level or logging.INFO)
                 console_handler = RichHandler(markup=True)
                 console_handler.setFormatter(
                     logging.Formatter(fmt="[grey37]%(name)s[/] %(message)s", datefmt="[%X]")
                 )
```

### Comparing `fotoobo-0.9.0/fotoobo/inventory/generic.py` & `fotoobo-1.0.0/fotoobo/inventory/generic.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/inventory/inventory.py` & `fotoobo-1.0.0/fotoobo/inventory/inventory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Devices class for storing device information
 """
 
 import logging
+import re
+from pathlib import Path
 from typing import Any, Dict, Optional
-import os
 
 from fotoobo.exceptions import GeneralWarning
 from fotoobo.fortinet.fortianalyzer import FortiAnalyzer
 from fotoobo.fortinet.forticlientems import FortiClientEMS
 from fotoobo.fortinet.fortigate import FortiGate
 from fotoobo.fortinet.fortimanager import FortiManager
 from fotoobo.helpers.files import load_yaml_file
@@ -21,17 +22,17 @@
 class Inventory:
     """
     Represents an inventory full of Fortinet and generic devices. Instantiate the inventory by
     providing an inventory file in yaml format as described in the documentation at
     https://fotoobo.readthedocs.io/en/latest/usage/inventory.html
     """
 
-    def __init__(self, inventory_file: str):
+    def __init__(self, inventory_file: Path):
         """Initialize the inventory"""
-        self._inventory_file: str = inventory_file
+        self._inventory_file: Path = inventory_file
         self._globals: Dict[str, Any] = {
             "fortianalyzer": {},
             "forticlientems": {},
             "fortigate": {},
             "fortimanager": {},
         }
         self.assets: Dict[str, Any] = {}
@@ -46,58 +47,61 @@
         name: Optional[str] = None,
         type: Optional[str] = None,  # pylint: disable=redefined-builtin
     ) -> Dict[str, Any]:
         """
         Get a list of assets from the inventory
 
         Args:
-            asset (str, optional): Which asset to get. If blank get every asset
-            type (str, optional) : Which asset type to get. If blank get every asset.
+            name:   Which asset to get. If blank get every asset. Wildcard * is supported in any
+                    position. E.g. "FortiGate", "*Gate", "Forti*ate", "Forti*".
+            type:   Which asset type to get. If blank get every asset.
 
         Returns:
-            Dict[str, Any]: Dict of assets with name as key
+            Dict of assets with name as key
+
+        Raises:
+            GeneralWarning if no asset was found that matches name or type
         """
         log.debug("getting assets with name '%s' and type '%s'", name, type)
-        if name and name not in self.assets:
-            raise GeneralWarning(f"asset {name} is not defined in inventory")
-
+        name_pattern = f"^{name}$".replace("*", ".*")
         assets = {}
         for _name, _asset in self.assets.items():
             if not name and not type:
                 assets[_name] = _asset
 
-            if not name and getattr(_asset, "type", None) == type:
+            elif not name and getattr(_asset, "type", None) == type:
                 assets[_name] = _asset
 
-            if name and _name == name:
+            elif name and re.match(name_pattern, _name):
                 if (type and getattr(_asset, "type", None) == type) or not type:
                     assets[_name] = _asset
 
-        if type and len(assets) == 0:
-            raise GeneralWarning(f"no asset of type '{type}' was found in the inventory")
+        if not assets:
+            raise GeneralWarning(
+                f"no asset of type '{type}' and name '{name}' was found in the inventory"
+            )
 
         return assets
 
     def _load_inventory(self) -> None:
         """
         Load the inventory from a file given
         """
         # Expand user home shortcuts in the inventory file path
-        expanded_inventory_file = os.path.expanduser(self._inventory_file)
+        expanded_inventory_file = self._inventory_file.expanduser()
         log.debug("loading assets from '%s'", expanded_inventory_file)
         inventory_raw: Dict[str, Any] = dict(load_yaml_file(expanded_inventory_file) or {})
 
         # set the globals
         # this has to be done before the looping over all inventory items so that the globals are
         # already set during looping
         if "globals" in inventory_raw:
             self._set_globals(inventory_raw["globals"])
 
         for name, asset in inventory_raw.items():
-
             # skip globals
             if name == "globals":
                 continue
 
             # enrich the raw asset data with the globals
             if asset.get("type", None) in self._globals:
                 asset = {**self._globals[asset["type"]], **asset}
@@ -134,12 +138,12 @@
     """
 
     def _set_globals(self, data: Dict[str, Any]) -> None:
         """
         Set some defaults for device types
 
         Args:
-            data (Dict[str, Any]): defaults by device where key is the device type and value defines
-            its defaults
+            data:   defaults by device where key is the device type and value defines
+                    its defaults
         """
         for key, value in data.items():
             self._globals[key] = value
```

### Comparing `fotoobo-0.9.0/fotoobo/main.py` & `fotoobo-1.0.0/fotoobo/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/fotoobo/utils/ems/get.py` & `fotoobo-1.0.0/fotoobo/tools/ems/get.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,52 +2,60 @@
 FortiClient EMS get module
 """
 import logging
 from typing import Dict, List
 
 from fotoobo.fortinet.forticlientems import FortiClientEMS
 from fotoobo.helpers.config import config
+from fotoobo.helpers.result import Result
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
 
 
-def version(host: str) -> Dict[str, str]:
+def version(host: str) -> Result[str]:
     """
     ems get version
 
     Args:
         host (str): host defined in inventory
 
     Returns:
-        Dict[str, str]: version data in a dict with keys: host, version
+        Result[Dict[str, str]]: version data in a dict with keys: host, version
     """
+    result = Result[str]()
+
     inventory = Inventory(config.inventory_file)
     ems: FortiClientEMS = inventory.get(host, "forticlientems")[host]
     log.debug("FortiClient EMS get version ...")
     ems.login()
     ems_version = ems.get_version()
 
-    return {"host": host, "version": ems_version}
+    result.push_result(host, f"v{ems_version}")
+
+    return result
 
 
-def workgroups(host: str, custom: bool = False) -> List[Dict[str, str]]:
+def workgroups(host: str, custom: bool = False) -> Result[List[Dict[str, str]]]:
     """
     ems get workgroups
 
     Args:
         host (str): host defined in inventory
         custom (bool): if true it only returns custom groups
 
     Returns:
         List[Dict[str, str]]: workgroups data in a list of dict with keys: name, id, total_devices
     """
-    groups = []
+    result = Result[List[Dict[str, str]]]()
+
     inventory = Inventory(config.inventory_file)
     ems: FortiClientEMS = inventory.get(host, "forticlientems")[host]
+
     log.debug("FortiClient EMS get workgroups ...")
     ems.login()
-    result = ems.api("get", f"/workgroups/index?custom={custom}").json()["data"]
-    for _ in result:
-        groups.append({"Name": _["name"], "id": str(_["id"]), "Count": str(_["total_devices"])})
 
-    return groups
+    raw_data = ems.api("get", f"/workgroups/index?custom={custom}").json()["data"]
+    for entry in raw_data:
+        result.push_result(entry["name"], entry["total_devices"])
+
+    return result
```

### Comparing `fotoobo-0.9.0/fotoobo/utils/ems/monitor.py` & `fotoobo-1.0.0/fotoobo/tools/ems/monitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,177 +4,194 @@
 
 import logging
 from datetime import datetime
 from typing import Any, Dict
 
 from fotoobo.fortinet.forticlientems import FortiClientEMS
 from fotoobo.helpers.config import config
+from fotoobo.helpers.result import Result
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
 
 
-def connections(host: str) -> Dict[Any, Any]:
+def connections(host: str) -> Result[Dict[str, Any]]:
     """
     Get connections information from FortiClient EMS.
 
-    The data returned is the raw data part from the EMS response. Additionally the data is enriched
+    The data returned is the raw data part from the EMS response. Additionally, the data is enriched
     with calculated and interesting values. All the enriched values are in the "fotoobo" in the
     returned dict.
 
     Args:
         host (str): FortiClient EMS host defined in the inventory
 
-    Returns: Dict[str, Any]
+    Returns: Result[Dict[str, Any]]
     """
+    result = Result[Dict[str, Any]]()
     inventory = Inventory(config.inventory_file)
+
     ems: FortiClientEMS = inventory.get(host, "forticlientems")[host]
     ems.login()
+
     response = ems.api("get", "/endpoints/connection/donut")
-    data: Dict[str, Any] = {}
-    data["data"] = list(response.json()["data"])
 
-    data["fotoobo"] = {}
+    data: Dict[str, Any] = {"data": list(response.json()["data"]), "fotoobo": {}}
+
     for item in data["data"]:
         data["fotoobo"][item["token"]] = item["value"]
 
-    return data
+    result.push_result(host, data)
+
+    return result
 
 
-def endpoint_management_status(host: str) -> Dict[str, Any]:
+def endpoint_management_status(host: str) -> Result[Dict[str, Any]]:
     """
     Get management information about endpoints registered in FortiClient EMS.
 
-    The data returned is the raw data part from the EMS response. Additionally the data is enriched
+    The data returned is the raw data part from the EMS response. Additionally, the data is enriched
     with calculated and interesting values. All the enriched values are in the key "fotoobo" in the
     returned dict:
 
         - {{ fotoobo.managed }}     Amount of managed endpoints
         - {{ fotoobo.unmanaged }}   Amount of unmanaged endpoints
 
     Args:
         host (str): FortiClient EMS host defined in the inventory
 
-    Returns: Dict[str, Any]
+    Returns: Result
     """
+    result = Result[Dict[str, Any]]()
     inventory = Inventory(config.inventory_file)
+
     ems: FortiClientEMS = inventory.get(host, "forticlientems")[host]
     ems.login()
 
     response = ems.api("get", "/endpoints/management/donut")
 
-    data = {}
-    data["data"] = dict(response.json())["data"]
+    data = {"data": dict(response.json())["data"]}
 
     managed = unmanaged = 0
     for item in data["data"]:
         if item["token"] == "managed":
             managed = item["value"]
             log.debug("management: managed: %s", managed)
 
         if item["token"] == "unmanaged":
             unmanaged = item["value"]
             log.debug("management: unmanaged: %s", unmanaged)
 
     data["fotoobo"] = {"managed": managed, "unmanaged": unmanaged}
-    return data
+
+    result.push_result(host, data)
+    return result
 
 
-def endpoint_online_outofsync(host: str) -> Dict[str, Any]:
+def endpoint_online_outofsync(host: str) -> Result[Dict[str, Any]]:
     """
     Get amount of FortiClient EMS devices which are online but policy not in sync.
 
     The data returned is a dict with a key "fotoobo" with the relevant data. In this utility only
     one key value pair is present.
 
         - {{ fotoobo.outofsync }}   Amount of managed endpoints which are online but their policy
             is not in synch with FortiClient EMS
 
     Args:
         host (str): FortiClient EMS host defined in the inventory
 
-    Returns: Dict[str, Any]
+    Returns: Result
     """
+    result = Result[Dict[str, Any]]()
     inventory = Inventory(config.inventory_file)
     ems: FortiClientEMS = inventory.get(host, "forticlientems")[host]
     ems.login()
 
     response = ems.api(
         "get", "/endpoints/index?offset=0&count=1&connection=online&status=outofsync"
     )
 
     data = {"fotoobo": {"outofsync": response.json()["data"]["total"]}}
     log.debug("endpoints outofsync: %s", data["fotoobo"]["outofsync"])
 
-    return data
+    result.push_result(host, data)
 
+    return result
 
-def endpoint_os_versions(host: str) -> Dict[str, Any]:
+
+def endpoint_os_versions(host: str) -> Result[Dict[str, Dict[str, Any]]]:
     """
     Get management information about endpoints registered in FortiClient EMS.
 
-    The data returned is the raw data part from the EMS response. Additionally the data is enriched
+    The data returned is the raw data part from the EMS response. Additionally, the data is enriched
     with calculated and interesting values. All the enriched values are in the key "fotoobo" in the
     returned dict:
 
         - {{ fotoobo.fctversionlinux }}     Amount of managed linux endpoints
         - {{ fotoobo.fctversionmac }}       Amount of managed mac endpoints
         - {{ fotoobo.fctversionwindows }}   Amount of managed windows endpoints
 
     Args:
         host (str): FortiClient EMS host defined in the inventory
 
-    Returns: Dict[str, Any]
+    Returns: Result[Dict[str, Dict[str, Any]]]
     """
+    result = Result[Dict[str, Dict[str, Any]]]()
     inventory = Inventory(config.inventory_file)
+
     ems: FortiClientEMS = inventory.get(host, "forticlientems")[host]
     ems.login()
 
-    data: Dict[str, Any] = {}
-    data["data"] = {}
-    data["fotoobo"] = {}
+    data: Dict[str, Any] = {"data": {}, "fotoobo": {}}
 
     for fctversion_os in ["fctversionwindows", "fctversionmac", "fctversionlinux"]:
         response = ems.api("get", f"/endpoints/{fctversion_os}/donut")
         data["data"][fctversion_os] = dict(response.json())["data"]
         count = sum(item["value"] for item in data["data"][fctversion_os])
         data["fotoobo"][fctversion_os] = count
 
-    return data
+    result.push_result(host, data)
+
+    return result
 
 
-def system(host: str) -> Dict[str, Any]:
+def system(host: str) -> Result[Dict[str, Any]]:
     """
     Get system information from FortiClient EMS.
 
     Args:
         host (str): FortiClient EMS host defined in inventory
 
-    Returns: Dict[str, Any]
+    Returns: Result[Dict[str, Any]]
     """
+    result = Result[Dict[str, Any]]()
     inventory = Inventory(config.inventory_file)
+
     ems: FortiClientEMS = inventory.get(host, "forticlientems")[host]
     ems.login()
 
     # get EMS serial number (just for debug logging and because it's possible)
     response = ems.api("get", "/system/serial_number")
     log.debug("serial number: %s (from /system/serial_number)", response.json()["data"])
 
     # get EMS system info
     response = ems.api("get", "/system/info/")
     log.debug("serial number: %s (from /system/info/)", response.json()["data"]["license"]["sn"])
 
-    return dict(response.json()["data"])
+    result.push_result(host, dict(response.json()["data"]))
 
+    return result
 
-def license(host: str) -> Dict[str, Any]:  # pylint: disable=redefined-builtin
+
+def license(host: str) -> Result[Dict[str, Any]]:  # pylint: disable=redefined-builtin
     """
     Get license information from FortiClient EMS.
 
-    The data returned is the raw data part from the EMS response. Additionally the data is enriched
+    The data returned is the raw data part from the EMS response. Additionally, the data is enriched
     with calculated and interesting values. All the enriched values are in the key "fotoobo" in the
     returned dict:
 
         - {{ fotoobo.[MODULE]_usage }}          License usage in percent by MODULE where MODULE is
             one of:
                 - fabric_agent
                 - ztna
@@ -184,39 +201,44 @@
                 - sase
                 - ztna_user
                 - epp_user
                 - sase_user
                 - vpn_only
         - {{ fotoobo.license_expiry_days }}     Days until your FortiClient EMS license expires.
             Be aware that it only shows the expiry of the "fabric_agent" fabric_agent as for now.
-            If you wish mor granular view this utility has to be improved accordingly.
+            If you wish more granular view this utility has to be improved accordingly.
 
     Args:
         host (str): FortiClient EMS host defined in the inventory
 
-    Returns: Dict[str, Any]
+    Returns: Result
     """
+    result = Result[Dict[str, Any]]()
     inventory = Inventory(config.inventory_file)
     ems: FortiClientEMS = inventory.get(host, "forticlientems")[host]
     ems.login()
-    response = ems.api("get", "/license/get")
-    data = dict(response.json()["data"])
 
-    for lic in data["licenses"]:
+    response = ems.api("get", "/license/get")
+    data = {}
+    data["data"] = dict(response.json()["data"])
 
+    for lic in data["data"]["licenses"]:
         if lic["type"] == "fabric_agent":
             log.debug("license expiry: %s", lic["expiry_date"])
             license_expiry = datetime.strptime(lic["expiry_date"], "%Y-%m-%dT%H:%M:%S")
             license_expiry_days = int((license_expiry - datetime.now()).days)
             log.debug("days to license expiry: %s", license_expiry_days)
 
     data["fotoobo"] = {}
     data["fotoobo"]["license_expiry_days"] = license_expiry_days
-    for key in data["seats"]:
-        if data["seats"][key] > 0:
-            log.debug(f"{key} license count: %s", data["seats"][key])
-            log.debug(f"{key} license used: %s", data["used"][key])
-            license_usage = int(100 / data["seats"][key] * data["used"][key])
+
+    for key in data["data"]["seats"]:
+        if data["data"]["seats"][key] > 0:
+            log.debug(f"{key} license count: %s", data["data"]["seats"][key])
+            log.debug(f"{key} license used: %s", data["data"]["used"][key])
+            license_usage = int(100 / data["data"]["seats"][key] * data["data"]["used"][key])
             log.debug(f"{key} license usage : %s%%", license_usage)
             data["fotoobo"][key + "_usage"] = license_usage
 
-    return data
+    result.push_result(host, data)
+
+    return result
```

### Comparing `fotoobo-0.9.0/fotoobo/utils/faz/get.py` & `fotoobo-1.0.0/fotoobo/tools/faz/get.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """
 FortiAnalyzer get version utility
 """
 
 import logging
-from typing import Dict
 
 from fotoobo.helpers.config import config
+from fotoobo.helpers.result import Result
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
 
 
-def version(host: str) -> Dict[str, str]:
+def version(host: str) -> Result[str]:
     """
     FortiAnalyzer get version
 
     Args:
         host (str): host defined in inventory
 
     Raises:
         GeneralWarning: GeneralWarning
 
     Returns:
-        Dict[str, str]: version data in a dict with keys: host, version
+        Result[str]: The version string per FAZ
     """
+    result = Result[str]()
+
     inventory = Inventory(config.inventory_file)
     assets = inventory.get(host, "fortianalyzer")
     log.debug("FortiAnalyzer get version ...")
     assets[host].login()
     faz_version = assets[host].get_version()
     assets[host].logout()
 
-    return {"host": host, "version": faz_version}
+    result.push_result(host, faz_version)
+
+    return result
```

### Comparing `fotoobo-0.9.0/fotoobo/utils/fgt/main.py` & `fotoobo-1.0.0/fotoobo/tools/fgt/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,86 @@
 """
 FortiGate backup utility
 """
-import datetime
+import concurrent.futures
 import json
 import logging
-import os
-from typing import Optional
+from typing import Tuple, Union
 
-from fotoobo.exceptions import APIError, GeneralError, GeneralWarning
+from rich.progress import Progress
+
+from fotoobo.exceptions import APIError, GeneralError
+from fotoobo.fortinet.fortigate import FortiGate
 from fotoobo.helpers.config import config
-from fotoobo.helpers.files import create_dir, file_to_ftp, file_to_zip
-from fotoobo.helpers.output import Output
+from fotoobo.helpers.result import Result
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
 
 
-def backup(  # pylint: disable=too-many-locals, too-many-branches
-    host: str,
-    backup_dir: str = "",
-    ftp_server: Optional[str] = None,
-    smtp_server: Optional[str] = None,
-) -> None:
+def backup(
+    host: Union[str, None] = None,
+) -> Result[str]:
     """
     Create a FortiGate configuration backup into a file and optionally upload it to an FTP server.
 
     Args:
-        host (str):         The host from the inventory to get the backup. If no host is given all
-                            FortiGate devices in the inventory are backed up.
-        backup_dir (str):   The directory to save tha backup(s) to
-        ftp_server (str):   The FTP server from the inventory to upload the backup to. You may omit
-                            this argument to only safe the backup to a file. This argument also
-                            compresses the configuration file into a zip file.
-        smtp_server (str):  The SMTP server from the inventory to send mail messages if errors occur
+        host:   The host from the inventory to get the backup. If no host is given all
+                FortiGate devices in the inventory are backed up.
+
+    Returns:
+        The Result object with all the results
     """
-    output = Output()
+    result = Result[str]()
     inventory = Inventory(config.inventory_file)
     fgts = inventory.get(host, "fortigate")
-    if not backup_dir:
-        backup_dir = os.getcwd()
 
-    create_dir(backup_dir)
+    def _get_single_backup(name: str, fgt: FortiGate) -> Tuple[str, str]:
+        """Get the configuration backup from a single FortiGate.
 
-    # backup every FortiGate
-    for name, fgt in fgts.items():
-        log.debug("backup FortiGate '%s'", name)
-        config_file = os.path.join(backup_dir, name + ".conf")
-
-        if os.path.isfile(config_file):
-            os.remove(config_file)
+        This private method is used for multithreading. It only queries one single FortiGate for its
+        configuration backup and returns it.
 
+        Args:
+            name:   The name of the FortiGate (as defined in the inventory)
+            fgt:    The FortiGate object to query
+
+        Returns:
+            name:   The name of the FortiGate (as defined in the inventory)
+            data:   The configuration backup of the FortiGate (fgt)
+        """
+        log.debug("backup FortiGate '%s'", name)
+        data: str = ""
         try:
-            data: str = fgt.backup()
+            data = fgt.backup()
+            if data.startswith("#config-version"):
+                message = f"config backup for '{name}' succeeded"
+                log.info(message)
+                result.push_message(name, message)
+
+            else:
+                data_json = json.loads(data)
+                message = f"backup '{name}' failed with error '{data_json['http_status']}'"
+                log.error(message)
+                result.push_message(name, message, level="error")
 
         except GeneralError as err:
-            output.add(err.message)
-            continue
+            result.push_message(name, err.message, level="error")
 
         except APIError as err:
-            output.add(f"{name} returned {err.message}")
-            continue
+            result.push_message(name, f"{name} returned {err.message}", level="error")
 
-        if data.startswith("#config-version"):
-            log.info("backup '%s' succeeded", name)
+        return name, data
 
-        else:
-            data_json = json.loads(data)
-            log.error("backup '%s' failed with error '%s'", name, data_json["http_status"])
-            continue
-
-        with open(config_file, "w", encoding="UTF-8") as file:
-            file.writelines(data)
-
-        if not os.path.isfile(config_file):
-            output.add(f"backup file for '{name}' does not exist")
-            continue
-
-        if ftp_server:
-            if ftp_server in inventory.assets:
-                server = inventory.assets[ftp_server]
-                log.debug("compressing configuration '%s'", name)
-                time: str = datetime.datetime.now().strftime("%Y%m%d-%H%M")
-                zip_file = os.path.join(backup_dir, name + "-" + time + ".conf.zip")
-                file_to_zip(config_file, zip_file)
-                file_to_ftp(zip_file, server)
-                os.remove(zip_file)
-
-            else:
-                raise GeneralWarning(f"ftp server '{ftp_server}' not found in inventory")
+    with Progress() as progress:
+        task = progress.add_task("getting FortiGate versions...", total=len(fgts))
+        with concurrent.futures.ThreadPoolExecutor(max_workers=10) as executor:
+            futures = []
+            for name, fgt in fgts.items():
+                futures.append(executor.submit(_get_single_backup, name, fgt))
+
+            for future in concurrent.futures.as_completed(futures):
+                name, configuration_backup = future.result()
+                result.push_result(name, configuration_backup)
+                progress.update(task, advance=1)
 
-    if smtp_server:
-        if smtp_server in inventory.assets:
-            output.send_mail(inventory.assets[smtp_server])
+    return result
```

### Comparing `fotoobo-0.9.0/fotoobo/utils/fmg/get.py` & `fotoobo-1.0.0/fotoobo/tools/fmg/get.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,43 +3,48 @@
 """
 
 import logging
 from typing import Any, Dict, List, Optional
 
 from fotoobo.exceptions.exceptions import GeneralError
 from fotoobo.helpers.config import config
+from fotoobo.helpers.result import Result
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
 
 
-def adoms(host: str) -> List[Dict[str, str]]:
+def adoms(host: str) -> Result[str]:
     """
     FortiManager get ADOMs
 
     Args:
         host (str): the host from the inventory to get the ADOMs list from
 
     Returns:
         list of dict: list of ADOMs where ADOM is a dict with keys: name, version
     """
     inventory = Inventory(config.inventory_file)
     fmg = inventory.get(host, "fortimanager")[host]
-    adom_list = []
+    result = Result[str]()
+
     log.debug("FortiManager get adoms ...")
+
     fmg.login()
     fmg_adoms = fmg.get_adoms()
+
     for adom in fmg_adoms:
-        adom_list.append({"name": adom["name"], "version": f"{adom['os_ver']}.{adom['mr']}"})
+        result.push_result(adom["name"], f"{adom['os_ver']}.{adom['mr']}")
 
     fmg.logout()
-    return adom_list
+
+    return result
 
 
-def devices(host: str) -> List[Dict[str, str]]:
+def devices(host: str) -> Result[Dict[str, str]]:
     """
     FortiManager get logical devices
     In a cluster only the cluster device is returned, not the physical nodes
 
     Args:
         host (str): the FortiManager from the inventory to get the Fortinet devices list from
 
@@ -59,30 +64,32 @@
                 "option": "object member",
                 "url": "/dvmdb/device",
             }
         ],
     }
     response = fmg.api("post", payload=payload)
     fmg.logout()
-    device_list = []
+    result = Result[Dict[str, str]]()
     for device in response.json()["result"][0]["data"]:
-        device_list.append(
+        result.push_result(
+            device["name"],
             {
-                "name": device["name"],
                 "version": f"{device['os_ver']}.{device['mr']}.{device['patch']}",
                 "ha_mode": str(device["ha_mode"]),
                 "platform": device["platform_str"],
                 "desc": device["desc"],
-            }
+            },
         )
 
-    return device_list
+    return result
 
 
-def policy(host: str, adom: str, policy_name: str, fields: Optional[List[str]] = None) -> List[Any]:
+def policy(
+    host: str, adom: str, policy_name: str, fields: Optional[List[str]] = None
+) -> Result[List[Dict[str, Any]]]:
     """
     FortiManager get policy
     """
     fields = fields or [
         "status",
         # "_last_hit",  # data-format not clear
         "global-label",
@@ -121,28 +128,31 @@
         raise GeneralError(f"FortiManager {host} returned {code}: {message}")
 
     policies = []
     for pol in data["result"][0]["data"]:
         policies.append({field: pol.get(field, None) for field in fields})
 
     fmg.logout()
-    return policies
+
+    out_result = Result[List[Dict[str, Any]]]()
+    out_result.push_result(host, policies)
+    return out_result
 
 
-def version(host: str) -> Dict[str, str]:
+def version(host: str) -> Result[str]:
     """
     FortiManager get version
 
     Args:
         host (str): the host from the inventory to get the version
 
     Returns:
         Dict[str, str]: version data in a dict with keys: host, version
     """
     inventory = Inventory(config.inventory_file)
     fmg = inventory.get(host, "fortimanager")[host]
     log.debug("FortiManager get version ...")
-    fmg.login()
     fmg_version = fmg.get_version()
-    fmg.logout()
+    result = Result[str]()
+    result.push_result(host, fmg_version)
 
-    return {"host": host, "version": fmg_version}
+    return result
```

### Comparing `fotoobo-0.9.0/fotoobo/utils/fmg/main.py` & `fotoobo-1.0.0/fotoobo/tools/fmg/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 FortiManager assign utility
 """
 
 import logging
+from pathlib import Path
 
 from fotoobo.exceptions.exceptions import GeneralWarning
 from fotoobo.helpers.config import config
 from fotoobo.helpers.files import load_json_file
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
@@ -49,15 +50,15 @@
             if message["history"]:
                 for line in message["history"]:
                     getattr(log, level)("- %s", line["detail"])
 
     fmg.logout()
 
 
-def post(file: str, adom: str, host: str) -> None:
+def post(file: Path, adom: str, host: str) -> None:
     """
     POST the given configuration from a JSON file to the FortiManager
 
     Args:
         file (str): The configuration file to oad the configuration from
         adom (str): The ADOM to assign the global policy to
         host (str): The FortiManager defined in inventory
```

### Comparing `fotoobo-0.9.0/fotoobo/utils/greet.py` & `fotoobo-1.0.0/fotoobo/tools/greet.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.9.0/pyproject.toml` & `fotoobo-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fotoobo"
-version = "0.9.0"
+version = "1.0.0"
 description = "The awesome Fortinet Toolbox"
 authors = ["Patrik Spiess <patrik.spiess@mgb.ch>", "Lukas Murer-Jäckle <lukas.murer@mgb.ch>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0, <3.12"
 typer = "~0.6.0"
 rich = "~12.5.1"
 PyYAML = "~6.0.0"
-requests = "~2.28.2"
+requests = "~2.31.0"
 Jinja2 = "~3.1.2"
-pysnmp = "^4.4.12"
 
 [tool.poetry.dev-dependencies]
 pytest = "~7.2.0"
 black = "~22.10.0"
 mypy = ">0.9, <1.0"
 tox = "~4.4.0"
 pylint = "~2.15.0"
 pytest-cov = "~4.0.0"
 types-requests = "~2.27.11"
 isort = "~5.10.1"
 types-PyYAML = "~6.0.5"
 pygount = "~1.5.0"
-Sphinx = "~5.3.0"
-sphinx-rtd-theme = "^1.1.1"
+Sphinx = "~6.2.0"
+sphinx-rtd-theme = "~1.2.0"
 
 [tool.poetry.scripts]
 fotoobo = "fotoobo.main:main"
 
 # isort is used to organize-imports
 [tool.isort]
 sections = ['FUTURE', 'STDLIB', 'THIRDPARTY', 'FIRSTPARTY', 'LOCALFOLDER']
@@ -97,22 +96,22 @@
 commands = pytest --basetemp=tests/temp/ {posargs}
 
 [testenv:coverage-integration]
 description = check pytest coverage for integration tests (which are under tests/cli)
 skip_install = true
 allowlist_externals = poetry, pytest
 commands_pre = poetry install
-commands = pytest --cov-report term-missing --cov-fail-under 80 --cov=fotoobo/cli tests/cli {posargs}
+commands = pytest --cov-report term-missing --cov-fail-under 90 --cov=fotoobo/cli tests/cli {posargs}
 
 [testenv:coverage]
 description = check pytest coverage for unit tests (without cli because these are unit-tests)
 skip_install = true
 allowlist_externals = poetry, pytest
 commands_pre = poetry install
-commands = pytest --cov-report term-missing --cov-fail-under 80 --cov=fotoobo --cov-config=.coverage_unittests_rc --ignore=tests/cli tests/ {posargs}
+commands = pytest --cov-report term-missing --cov-fail-under 90 --cov=fotoobo --cov-config=.coverage_unittests_rc --ignore=tests/cli tests/ {posargs}
 
 [testenv:requirements]
 description = Create a requirements.txt from the Poetry dependencies (used for readthedocs)
 skip_install = True
 allowlist_externals = poetry
 commands = poetry export --without-hashes --format=requirements.txt --output=docs/requirements.txt
```

### Comparing `fotoobo-0.9.0/PKG-INFO` & `fotoobo-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: fotoobo
-Version: 0.9.0
+Version: 1.0.0
 Summary: The awesome Fortinet Toolbox
 Author: Patrik Spiess
 Author-email: patrik.spiess@mgb.ch
 Requires-Python: >=3.8.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<3.2.0)
 Requires-Dist: PyYAML (>=6.0.0,<6.1.0)
-Requires-Dist: pysnmp (>=4.4.12,<5.0.0)
-Requires-Dist: requests (>=2.28.2,<2.29.0)
+Requires-Dist: requests (>=2.31.0,<2.32.0)
 Requires-Dist: rich (>=12.5.1,<12.6.0)
 Requires-Dist: typer (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
 <p style="text-align: right"><img src=docs/source/fotoobo.png width="200px"></p>
 
 # fotoobo | Fortinet Toolbox
@@ -55,14 +54,7 @@
 
 fotoobo may be used as an imported module under the same terms that the LGPL states for dynamically
 linked (binary) libraries. So you may use fotoobo (unmodified) with code under another license (free
 or commercial).
 
 All changes to the fotoobo code itself are subject to the LGPL v3.
 
-# Legacy documentation
-
-This documentation has not yet been migrated to the Sphinx documentation.
-
-- [The FortiGate configuration structure in fotoobo](docs_legacy/fortinet/fortigate_config.md)
-- [FortiGate configuration check](docs_legacy/fortinet/fortigate_config_check.md)
-
```

