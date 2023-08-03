# Comparing `tmp/satori_ci-1.3.3.tar.gz` & `tmp/satori_ci-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.3.3.tar", last modified: Tue Aug  1 21:01:39 2023, max compression
+gzip compressed data, was "satori_ci-1.3.4.tar", last modified: Thu Aug  3 11:56:21 2023, max compression
```

## Comparing `satori_ci-1.3.3.tar` & `satori_ci-1.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-08-01 21:01:19.555182 satori_ci-1.3.3/LICENSE
--rw-r--r--   0        0        0     7140 2023-08-01 21:01:19.555182 satori_ci-1.3.3/README.md
--rw-r--r--   0        0        0      755 2023-08-01 21:01:39.360215 satori_ci-1.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/__init__.py
--rw-r--r--   0        0        0       37 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/__main__.py
--rw-r--r--   0        0        0     4558 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/api.py
--rw-r--r--   0        0        0     1633 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/bundler.py
--rw-r--r--   0        0        0      484 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/models.py
--rw-r--r--   0        0        0     3345 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/playbooks.py
--rw-r--r--   0        0        0    28045 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/satori.py
--rw-r--r--   0        0        0    12410 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/utils.py
--rw-r--r--   0        0        0     1194 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/classes/validations.py
--rwxr-xr-x   0        0        0     8991 2023-08-01 21:01:19.555182 satori_ci-1.3.3/src/satoricli/cli/parser.py
--rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-03 11:56:06.359856 satori_ci-1.3.4/LICENSE
+-rw-r--r--   0        0        0     7140 2023-08-03 11:56:06.359856 satori_ci-1.3.4/README.md
+-rw-r--r--   0        0        0      755 2023-08-03 11:56:21.688043 satori_ci-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/__main__.py
+-rw-r--r--   0        0        0     4551 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/api.py
+-rw-r--r--   0        0        0     1633 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/bundler.py
+-rw-r--r--   0        0        0      484 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/models.py
+-rw-r--r--   0        0        0     3345 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/playbooks.py
+-rw-r--r--   0        0        0    27448 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/satori.py
+-rw-r--r--   0        0        0    13678 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/utils.py
+-rw-r--r--   0        0        0     1194 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/validations.py
+-rwxr-xr-x   0        0        0     9827 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/cli/parser.py
+-rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.4/PKG-INFO
```

### Comparing `satori_ci-1.3.3/LICENSE` & `satori_ci-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.3/README.md` & `satori_ci-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.3/pyproject.toml` & `satori_ci-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.3.3"
+version = "1.3.4"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.3.3/src/satoricli/classes/api.py` & `satori_ci-1.3.4/src/satoricli/classes/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         report = res.json()
         if isinstance(report, dict) and report.get("json"):
             for e in report["json"]:
                 e.pop("gfx", None)
         return report
 
     def get_report_output(self, report_id: str):
-        r = self.request("GET", f"reports/{report_id}/output", stream=True)
+        r = self.request("GET", f"outputs/{report_id}", stream=True)
         return r.iter_lines()
 
     def get_report_files(self, report_id: str):
         return self.request("GET", f"reports/{report_id}/files", stream=True)
 
     def report_delete(self, parameters: dict) -> None:
         self.request("DELETE", f"reports/{parameters['id']}")
```

### Comparing `satori_ci-1.3.3/src/satoricli/classes/bundler.py` & `satori_ci-1.3.4/src/satoricli/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.3/src/satoricli/classes/playbooks.py` & `satori_ci-1.3.4/src/satoricli/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.3/src/satoricli/classes/satori.py` & `satori_ci-1.3.4/src/satoricli/classes/satori.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import ast
-import json
+from datetime import date
 import os
 import shutil
 import sys
 import tempfile
 import time
+from typing import Optional
 import uuid
 import warnings
 from argparse import Namespace
-from base64 import b64decode
 from pathlib import Path
 
 import requests
 import yaml
 from colorama import Fore
 from rich.progress import open as progress_open, Progress
-from rich.table import Table
 from satorici.validator import validate_playbook
 from satorici.validator.exceptions import PlaybookValidationError, PlaybookVariableError
 from satorici.validator.warnings import NoLogMonitorWarning
 
 from .api import SatoriAPI
 from .bundler import get_local_files, make_bundle
 from .models import arguments
@@ -32,14 +31,15 @@
     VALUE_COLOR,
     autocolor,
     autoformat,
     autotable,
     check_monitor,
     console,
     filter_params,
+    format_outputs,
     log,
     puts,
 )
 from .validations import get_parameters, validate_parameters
 
 
 class Satori:
@@ -501,52 +501,44 @@
                 console.rule("[b red]Pending actions", style="red")
                 autotable(info["pending"], "b red")
             console.rule("[b blue]Monitors", style="blue")
             autotable(info["list"], "b blue")
 
     def output(self, report_id: str):
         """Returns commands output"""
-        current_path = ""
+        format_outputs(self.api.get_report_output(report_id))
 
-        for line in self.api.get_report_output(report_id):
-            output = json.loads(line)
-
-            if current_path != output["path"]:
-                console.rule(f"[b]{output['path']}[/b]")
-                current_path = output["path"]
-
-            console.print(f"[b][green]Command:[/green] {output['original']}[/b]")
-
-            if output["testcase"]:
-                testcase = Table(show_header=False, show_edge=False)
-
-                testcase.add_column(style="b")
-                testcase.add_column()
+    def get_outputs(
+        self,
+        from_date: Optional[date] = None,
+        to_date: Optional[date] = None,
+        name: Optional[str] = None,
+        failed: Optional[bool] = None,
+        **kwargs,
+    ):
+        res = self.api.request(
+            "GET",
+            "/outputs",
+            params={
+                "from_date": from_date,
+                "to_date": to_date,
+                "name": name,
+                "failed": failed,
+            },
+        )
 
-                for key, value in output["testcase"].items():
-                    testcase.add_row(key, b64decode(value).decode(errors="ignore"))
+        for item in res.json():
+            output = requests.get(item["url"], stream=True)
 
-                console.print("[blue]Testcase:[/blue]")
-                console.print(testcase)
+            if not output.ok:
+                continue
 
-            console.print("[blue]Return code:[/blue]", output["output"]["return_code"])
-            console.print("[blue]Stdout:[/blue]")
-            if output["output"]["stdout"]:
-                console.out(
-                    b64decode(output["output"]["stdout"])
-                    .decode(errors="ignore")
-                    .strip()
-                )
-            console.print("[blue]Stderr:[/blue]")
-            if output["output"]["stderr"]:
-                console.out(
-                    b64decode(output["output"]["stderr"])
-                    .decode(errors="ignore")
-                    .strip()
-                )
+            console.print(f"Report: {item['report_id']}")
+            format_outputs(output.iter_lines())
+            console.print()
 
     def output_files(self, report_id: str):
         r = self.api.get_report_files(report_id)
         total = int(r.headers["Content-Length"])
 
         with Progress() as progress:
             task = progress.add_task("Downloading...", total=total)
```

### Comparing `satori_ci-1.3.3/src/satoricli/classes/utils.py` & `satori_ci-1.3.4/src/satoricli/classes/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from base64 import b64decode
 from typing import Union, Optional
 import json
 import yaml
 import re
 from typing import Any
 from colorama import Fore, Style
 from rich.logging import RichHandler
@@ -397,7 +398,44 @@
 def iter_loop(data: Union[tuple[Any], list[Any]]):
     i = 0
     while True:
         yield data[i]
         i += 1
         if i >= len(data):
             i = 0
+
+
+def format_outputs(outputs):
+    current_path = ""
+
+    for line in outputs:
+        output = json.loads(line)
+
+        if current_path != output["path"]:
+            console.rule(f"[b]{output['path']}[/b]")
+            current_path = output["path"]
+
+        console.print(f"[b][green]Command:[/green] {output['original']}[/b]")
+
+        if output["testcase"]:
+            testcase = Table(show_header=False, show_edge=False)
+
+            testcase.add_column(style="b")
+            testcase.add_column()
+
+            for key, value in output["testcase"].items():
+                testcase.add_row(key, b64decode(value).decode(errors="ignore"))
+
+            console.print("[blue]Testcase:[/blue]")
+            console.print(testcase)
+
+        console.print("[blue]Return code:[/blue]", output["output"]["return_code"])
+        console.print("[blue]Stdout:[/blue]")
+        if output["output"]["stdout"]:
+            console.out(
+                b64decode(output["output"]["stdout"]).decode(errors="ignore").strip()
+            )
+        console.print("[blue]Stderr:[/blue]")
+        if output["output"]["stderr"]:
+            console.out(
+                b64decode(output["output"]["stderr"]).decode(errors="ignore").strip()
+            )
```

### Comparing `satori_ci-1.3.3/src/satoricli/classes/validations.py` & `satori_ci-1.3.4/src/satoricli/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.3/src/satoricli/cli/parser.py` & `satori_ci-1.3.4/src/satoricli/cli/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import requests  # autoupgrade
 from importlib import metadata
 from colorama import just_fix_windows_console
 from rich import print
 from pkg_resources import get_distribution, DistributionNotFound  # autoupgrade
 from packaging import version  # autoupgrade
-from datetime import datetime
+from datetime import date, datetime
 
 # from subprocess import call # autoupgrade
 from ..classes.satori import Satori
 from ..classes.utils import console
 
 VERSION = metadata.version("satori-ci")
 just_fix_windows_console()
@@ -157,14 +157,40 @@
         "--filter",
         type=str,
         default="",
         help="Filters: from,to,satori_error,status",
     )
     add_satori_arguments(report_cmd)
 
+    # outputs
+    outputs_cmd = subparsers.add_parser("outputs", parents=[baseparser])
+    output_filters = outputs_cmd.add_argument_group("filters")
+    output_filters.add_argument(
+        "--from",
+        type=date.fromisoformat,
+        help="Date in ISO format",
+        metavar="DATE",
+        dest="from_date",
+    )
+    output_filters.add_argument(
+        "--to",
+        type=date.fromisoformat,
+        help="Date in ISO format",
+        metavar="DATE",
+        dest="to_date",
+    )
+    output_filters.add_argument("-n", "--name", help="Playbook name")
+    output_filters.add_argument(
+        "-f",
+        "--failed",
+        action="store_const",
+        const=True,
+        help="Fetch only failed reports outputs",
+    )
+
     # monitor {id} <start|stop|delete>
     monitor_cmd = subparsers.add_parser("monitor", parents=[baseparser])
     monitor_cmd.add_argument(
         "--clean", default=False, action="store_true", help="Clean all report related"
     )
     monitor_cmd.add_argument(
         "--deleted", default=False, action="store_true", help="Display deleted monitors"
@@ -218,10 +244,12 @@
         elif args.subcommand in (None, "dashboard"):
             instance.dashboard(args)
         elif args.subcommand == "help":
             if args.web:
                 subprocess.run(["satori-docs", "--web"])
             else:
                 subprocess.run(["satori-docs"])
+        elif args.subcommand == "outputs":
+            instance.get_outputs(**vars(args))
     except KeyboardInterrupt:
         console.print("[critical]Interrupted by user")
         sys.exit(1)
```

### Comparing `satori_ci-1.3.3/PKG-INFO` & `satori_ci-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.3.3
+Version: 1.3.4
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

