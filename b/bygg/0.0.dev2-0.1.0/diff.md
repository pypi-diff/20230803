# Comparing `tmp/bygg-0.0.dev2.tar.gz` & `tmp/bygg-0.1.0.tar.gz`

## Comparing `bygg-0.0.dev2.tar` & `bygg-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,55 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bygg-0.0.dev2/.tool-versions
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bygg-0.0.dev2/Byggfile.yml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 bygg-0.0.dev2/_version.py
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 bygg-0.0.dev2/bootstrap.sh
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 bygg-0.0.dev2/mypy.sh
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bygg-0.0.dev2/noxfile.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bygg-0.0.dev2/requirements-dev.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 bygg-0.0.dev2/requirements.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/parametric/.gitignore
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/parametric/Byggfile.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/parametric/Byggfile.yml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/parametric/README.md
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/taskrunner/Byggfile.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/Byggfile.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/Byggfile.yml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/input1.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/more_things/MoreActions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.0.dev2/examples/trivial/more_things/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/__init__.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/action.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/cache.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/configuration.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/dag.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/digest.py
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/py.typed
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/runner.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/scaffolding.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/scheduler.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/status_display.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/types.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bygg-0.0.dev2/src/bygg/util.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bygg-0.0.dev2/tests/test_action.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bygg-0.0.dev2/tests/test_cache.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 bygg-0.0.dev2/tests/test_scheduler.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 bygg-0.0.dev2/tests/test_utils.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 bygg-0.0.dev2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.0.dev2/LICENSE
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 bygg-0.0.dev2/README.md
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 bygg-0.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 bygg-0.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bygg-0.1.0/.tool-versions
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bygg-0.1.0/_version.py
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 bygg-0.1.0/bootstrap.sh
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 bygg-0.1.0/mypy.sh
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 bygg-0.1.0/noxfile.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bygg-0.1.0/requirements-dev.in
+-rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 bygg-0.1.0/requirements-dev.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 bygg-0.1.0/requirements.in
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 bygg-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bygg-0.1.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 bygg-0.1.0/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bygg-0.1.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bygg-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/Byggfile.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/Byggfile.yml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/Byggfile1.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/Byggfile2.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/requirements.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/requirements1.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/requirements2.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/parametric/.gitignore
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/parametric/Byggfile.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/parametric/Byggfile.yml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/parametric/README.md
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/taskrunner/Byggfile.yml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/Byggfile.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/Byggfile.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/input1.txt
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/more_things/MoreActions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/more_things/__init__.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 bygg-0.1.0/schemas/Byggfile_yml_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/__init__.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/action.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/apply_configuration.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/cache.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/common_types.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/configuration.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/dag.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/digest.py
+-rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/py.typed
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/runner.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/scaffolding.py
+-rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/scheduler.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/status_display.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/util.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bygg-0.1.0/tests/test_action.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bygg-0.1.0/tests/test_cache.py
+-rw-r--r--   0        0        0    11043 2020-02-02 00:00:00.000000 bygg-0.1.0/tests/test_scheduler.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 bygg-0.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bygg-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 bygg-0.1.0/README.md
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 bygg-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 bygg-0.1.0/PKG-INFO
```

### Comparing `bygg-0.0.dev2/examples/parametric/Byggfile.py` & `bygg-0.1.0/examples/parametric/Byggfile.py`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/examples/trivial/Byggfile.py` & `bygg-0.1.0/examples/trivial/Byggfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from pathlib import Path
 
-from bygg.action import Action, ActionContext
-from bygg.types import CommandStatus
+from bygg.action import Action, ActionContext, action
+from bygg.common_types import CommandStatus
 import more_things.MoreActions  # noqa: F401 (imported for side effects)
-from more_things.MoreActions import action
 
 
 @action(
     "testfile 1",
     inputs=["input1.txt"],
     outputs=["output1.txt"],
 )
```

### Comparing `bygg-0.0.dev2/examples/trivial/input1.txt` & `bygg-0.1.0/examples/trivial/input1.txt`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/examples/trivial/more_things/MoreActions.py` & `bygg-0.1.0/examples/trivial/more_things/MoreActions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from bygg.action import ActionContext, action
-from bygg.types import CommandStatus
+from bygg.common_types import CommandStatus
 
 
 @action("testfile 2", message="testfile 2", outputs=["output2.txt"])
 def write_foo_to_file(ctx: ActionContext):
     for filename in ctx.outputs:
         with open(filename, "w") as f:
             f.write("foo")
```

### Comparing `bygg-0.0.dev2/src/bygg/action.py` & `bygg-0.1.0/src/bygg/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import Callable, Iterable, Literal, Optional, Set, Tuple
 
-from bygg.types import CommandStatus
+from bygg.common_types import CommandStatus
 
 SchedulingType = Literal["in-process", "processpool"]
 
 # Function that returns a string that is included in the dependency digest. Returning
 # None causes the value to be ignored.
 DynamicDependency = Callable[[], str | None]
```

### Comparing `bygg-0.0.dev2/src/bygg/cache.py` & `bygg-0.1.0/src/bygg/cache.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 class Cache:
     data: CacheState | None
     db_file: Path
 
     def __init__(self, db_file: Path = DEFAULT_DB_FILE):
         self.data = CacheState({})
         self.db_file = db_file
-        make_sure_status_dir_exists()
 
     def load(self):
+        make_sure_status_dir_exists()
         try:
             with open(self.db_file, "rb") as f:
                 self.data = pickle.load(f)
         except (EOFError, FileNotFoundError):
             self.data = CacheState({})
 
     def save(self):
```

### Comparing `bygg-0.0.dev2/src/bygg/configuration.py` & `bygg-0.1.0/src/bygg/configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import os
 import sys
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 import msgspec
 import rich
 import rich.status
 
-from bygg.action import Action
-from bygg.util import create_shell_command
-
 PYTHON_INPUTFILE = "Byggfile.py"
 YAML_INPUTFILE = "Byggfile.yml"
 
 
 class SettingsSection(msgspec.Struct, forbid_unknown_fields=True):
     default_action: Optional[str] = None
 
@@ -33,25 +30,54 @@
     name: str
     description: Optional[str] = None
     message: Optional[str] = None
     inputs: Optional[List[str]] = None
     outputs: Optional[List[str]] = None
     dependencies: Optional[List[str]] = None
     is_entrypoint: Optional[bool] = None
+    environment: Optional[str] = "default"
     shell: Optional[str] = None
 
 
-class ByggFile(msgspec.Struct):
+class Environment(msgspec.Struct, forbid_unknown_fields=True):
+    """
+    name: The name of the environment.
+
+    description: A description of the environment. Used in e.g. help messages.
+
+    byggfiles: A list of Byggfiles that use this environment.
+
+    inputs: A list of files that are used as input to the environment. Typically pip
+    requirements files, but can be any files.
+
+    venv_directory: The directory where the virtual environment is located. Will be
+    recreated by Bygg if any of the inputs are modified.
+
+    shell: The shell command for creating the environment.
+
+    entrypoints: A list of entrypoints that use this environment.
+    """
+
+    byggfile: str
+    inputs: List[str]
+    venv_directory: str
+    shell: str
+    description: Optional[str] = None
+    message: Optional[str] = None
+
+
+class ByggFile(msgspec.Struct, forbid_unknown_fields=True):
     actions: List[ActionItem]
     settings: SettingsSection = msgspec.field(default_factory=SettingsSection)
+    environments: Dict[str, Environment] = msgspec.field(default_factory=dict)
 
 
-def load_python_build_file():
-    if os.path.isfile(PYTHON_INPUTFILE):
-        with open(PYTHON_INPUTFILE, "r") as f:
+def load_python_build_file(build_file: str):
+    if os.path.isfile(build_file):
+        with open(build_file, "r") as f:
             # modify load path to make the current directory importable
             preamble = "import sys\nsys.path.insert(0, '.')\n\n"
             exec(preamble + f.read(), globals())
 
 
 def read_config_file() -> ByggFile | None:
     if not os.path.isfile(YAML_INPUTFILE):
@@ -64,23 +90,12 @@
         rich.print(
             "[red bold]Error while reading configuration file "
             f"[yellow]{YAML_INPUTFILE}[/yellow]:[/red bold] {e}"
         )
         sys.exit(1)
 
 
-def apply_configuration(configuration: ByggFile | None):
-    if not configuration:
-        return
-
-    for action in configuration.actions:
-        shell_command = (
-            create_shell_command(action.shell, action.message) if action.shell else None
-        )
-        Action(
-            action.name,
-            is_entrypoint=bool(action.is_entrypoint),
-            inputs=action.inputs,
-            outputs=action.outputs,
-            dependencies=action.dependencies,
-            command=shell_command,
-        )
+def dump_schema():
+    import json
+
+    schema = msgspec.json.schema(ByggFile)
+    print(json.dumps(schema, indent=2))
```

### Comparing `bygg-0.0.dev2/src/bygg/dag.py` & `bygg-0.1.0/src/bygg/dag.py`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/src/bygg/digest.py` & `bygg-0.1.0/src/bygg/digest.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,7 +74,16 @@
     Returns: The digest of the function as a hex string.
     """
     # Just looking at the code object is not enough, so let's disassemble it.
     out = io.StringIO()
     dis.dis(fn, file=out)
     function_dis_string = out.getvalue()
     return hashlib.new(DIGEST_TYPE, function_dis_string.encode()).hexdigest()
+
+
+def calculate_string_digest(s: str) -> str:
+    """
+    Calculate the digest of a string.
+    s: The string to calculate the digest of.
+    Returns: The digest of the string as a hex string.
+    """
+    return hashlib.new(DIGEST_TYPE, s.encode()).hexdigest()
```

### Comparing `bygg-0.0.dev2/src/bygg/main.py` & `bygg-0.1.0/src/bygg/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import argparse
+from dataclasses import dataclass
 from multiprocessing import cpu_count
 import os
 import shutil
 import stat
+import subprocess
 import sys
 import time
-from typing import List, Optional
+from typing import List
 
 import rich
 import rich.status
 
+from bygg.apply_configuration import apply_configuration
 from bygg.configuration import (
     PYTHON_INPUTFILE,
     YAML_INPUTFILE,
     ByggFile,
-    apply_configuration,
-    load_python_build_file,
+    dump_schema,
     read_config_file,
 )
 from bygg.runner import runner
 from bygg.scheduler import scheduler
 from bygg.status_display import on_job_status, on_runner_status, progress
 
 
@@ -32,24 +34,16 @@
     """
     Set up status listeners.
     """
     runner.job_status_listener = on_job_status
     runner.runner_status_listener = on_runner_status
 
 
-loading_python_build_file = rich.status.Status(
-    "[cyan]Executing Python build file", spinner="dots"
-)
-
-
 def build(actions: List[str], job_count: int | None, always_make: bool) -> bool:
     try:
-        with loading_python_build_file:
-            load_python_build_file()
-
         init_status_listeners()
 
         max_workers = get_job_count_limit() if job_count is None else job_count
 
         for action in actions:
             t1 = time.time()
             rich.print(f"Building action '{action}':")
@@ -90,17 +84,14 @@
         scheduler.shutdown()
 
     return True
 
 
 def clean(actions: List[str]):
     try:
-        with loading_python_build_file:
-            load_python_build_file()
-
         init_status_listeners()
 
         for action in actions:
             rich.print(f"Cleaning action '{action}':")
             scheduler.prepare_run(action)
             for job_name in scheduler.job_graph.get_all_jobs():
                 job = scheduler.build_actions.get(job_name, None)
@@ -129,38 +120,27 @@
 
     return True
 
 
 def check(actions: List[str]):
     print("check")
     t0 = time.time()
-    action_count = len(scheduler.build_actions)
-
-    with loading_python_build_file:
-        load_python_build_file()
-    rich.print(
-        f"{len(scheduler.build_actions) - action_count} actions registered in "
-        f"{time.time() - t0:.2f} seconds."
-    )
     init_status_listeners()
 
     for action in actions:
         t1 = time.time()
         with rich.status.Status(f"Preparing action '{action}':"):
             scheduler.prepare_run(action)
         rich.print(f"Action '{action}' prepared in {time.time() - t1:.2f} s.")
 
     rich.print(f"Total time for --check was {time.time() - t0:.2f} s.")
     return True
 
 
 def list_actions() -> bool:
-    with loading_python_build_file:
-        load_python_build_file()
-
     entrypoints = [x for x in scheduler.build_actions.values() if x.is_entrypoint]
 
     if entrypoints:
         rich.print("Available actions:")
         for action in sorted(entrypoints, key=lambda x: x.name):
             rich.print(f"  {action.name}")
         return True
@@ -171,67 +151,157 @@
         return False
 
 
 def print_no_actions_text(configuration: ByggFile | None):
     return list_actions()
 
 
+def print_version():
+    import importlib.metadata
+
+    print(f"{__package__} {importlib.metadata.version(__package__)}")
+
+
 MAKE_COMPATIBLE_PANEL = "(Roughly) Make-compatible options"
 
 
-def dispatcher(
-    actions: Optional[List[str]],
-    directory_arg: Optional[str],
-    jobs_arg: Optional[int],
-    always_make_arg: bool,
-    check_arg: bool,
-    clean_arg: bool,
-    list_arg: bool,
-):
+def dispatcher(args: argparse.Namespace):
     """
     A build tool written in Python, where all actions can be written in Python.
     """
-    if directory_arg:
+    if args.dump_schema:
+        dump_schema()
+        sys.exit(0)
+
+    if args.version:
+        print_version()
+        sys.exit(0)
+
+    directory = args.directory[0] if args.directory else None
+    is_restarted_with_env = (
+        args.is_restarted_with_env[0] if args.is_restarted_with_env else None
+    )
+
+    if directory and not is_restarted_with_env:
+        directory_arg = args.directory[0]
         rich.print(f"Entering directory '{directory_arg}'")
         os.chdir(directory_arg)
 
     if not os.path.isfile(PYTHON_INPUTFILE) and not os.path.isfile(YAML_INPUTFILE):
         rich.print("No build files found.")
         sys.exit(1)
 
     configuration = read_config_file()
-    apply_configuration(configuration)
+    action_partitions = partition_actions(configuration, args.actions)
 
-    resolved_actions = actions if actions else []
+    if not action_partitions:
+        status = print_no_actions_text(configuration)
+        if status:
+            sys.exit(0)
+        sys.exit(1)
 
-    if (
-        configuration is not None
-        and not actions
-        and configuration.settings.default_action is not None
-    ):
-        resolved_actions += [configuration.settings.default_action]
+    for partition in action_partitions:
+        env = partition.environment_name
+        # Check if we should restart with another Python interpreter (e.g. from a
+        # virtualenv):
+        restart_with = apply_configuration(configuration, env, is_restarted_with_env)
+
+        if restart_with is not None and not is_restarted_with_env:
+            exec_list = construct_exec_list(args, restart_with, partition)
+            try:
+                process = subprocess.run(exec_list, encoding="utf-8")
+                if process.returncode != 0:
+                    sys.exit(process.returncode)
+            except FileNotFoundError:
+                rich.print(
+                    f"[red]Error: Could not restart with '{restart_with}'.[/red]\n"
+                    f"[yellow]Please make sure that bygg is in your pip requirements list for this environment.[/yellow]"
+                )
+                sys.exit(1)
+        else:
+            if args.check:
+                status = check(args.actions)
+            elif args.clean:
+                status = clean(args.actions)
+            elif args.list:
+                status = list_actions()
+            else:
+                jobs = int(args.jobs) if args.jobs else None
+                status = build(partition.actions, jobs, args.always_make)
 
-    status = None
+            if not status:
+                sys.exit(1)
 
-    if not resolved_actions:
-        status = print_no_actions_text(configuration)
-    elif check_arg:
-        status = check(resolved_actions)
-    elif clean_arg:
-        status = clean(resolved_actions)
-    elif list_arg:
-        status = list_actions()
-    else:
-        status = build(resolved_actions, jobs_arg, always_make_arg)
 
-    if not status:
-        sys.exit(1)
+@dataclass
+class ActionPartition:
+    """
+    environment_name: The name of the environment that the actions should be run in.
+    None means the implicit default environment, i.e. typically the base process.
 
+    actions: The actions that should be run in the environment.
+    """
 
-def main():
+    environment_name: str | None
+    actions: List[str]
+
+
+def construct_exec_list(
+    args: argparse.Namespace, restart_with: str, partition: ActionPartition
+):
+    exec_list = [restart_with, *partition.actions]
+    for k, v in vars(args).items():
+        if k == "actions":
+            continue
+        elif v is True:
+            exec_list.append(f"--{k}")
+        elif v:
+            exec_list.append(f"--{k} {v}")
+    if partition.environment_name:
+        exec_list.append("--is_restarted_with_env")
+        exec_list.append(partition.environment_name)
+    return exec_list
+
+
+def partition_actions(
+    configuration: ByggFile | None,
+    actions: List[str] | None,
+) -> List[ActionPartition] | None:
+    """
+    Partition the actions into groups that should be run in the same environment.
+    """
+
+    # TODO: Implement this.
+
+    resolved_actions = actions if actions else []
+
+    if configuration:
+        if not actions and configuration.settings.default_action is not None:
+            # Resolve to default action:
+            resolved_actions += [configuration.settings.default_action]
+            return [ActionPartition("default", resolved_actions)]
+
+        # Put consecutive actions with the same environment in the same partition:
+        action_partitions = []
+        action_dict = {a.name: a for a in configuration.actions}
+        current_partition: ActionPartition | None = None
+        for action in [action_dict[a] for a in resolved_actions]:
+            if (
+                current_partition is None
+                or current_partition.environment_name != action.environment
+            ):
+                current_partition = ActionPartition(action.environment, [action.name])
+                action_partitions.append(current_partition)
+            else:
+                current_partition.actions.append(action.name)
+
+        return action_partitions
+
+
+def create_argument_parser():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="""
 A build tool written in Python, where all actions can be written in Python.
 
 Build the default action:
  %(prog)s
@@ -248,18 +318,29 @@
     )
     parser.add_argument(
         "actions",
         nargs="*",
         default=None,
         help="Entrypoint actions to operate on.",
     )
+    parser.add_argument(
+        "-v", "--version", action="store_true", help="Show version string and exit."
+    )
+    parser.add_argument(
+        "--is_restarted_with_env",
+        nargs=1,
+        type=str,
+        default=None,
+        help=argparse.SUPPRESS,
+    )
     # Commands that operate on the build setup:
-    build_setup_group = parser.add_argument_group(
+    build_setup_wrapper_group = parser.add_argument_group(
         "Commands that operate on the build setup"
-    )
+    )  # add_mutually_exclusive_group doesn't accept a title, so wrap it in a regular group.
+    build_setup_group = build_setup_wrapper_group.add_mutually_exclusive_group()
     build_setup_group.add_argument(
         "-c",
         "--check",
         action="store_true",
         help="Check the specified actions.",
     )
     build_setup_group.add_argument(
@@ -293,27 +374,30 @@
     )
     make_group.add_argument(
         "-B",
         "--always-make",
         action="store_true",
         help="Always build all actions.",
     )
+    # Meta arguments:
+    meta_group = parser.add_argument_group("Meta arguments")
+    meta_group.add_argument(
+        "--dump-schema",
+        action="store_true",
+        help="Generate a JSON Schema for the Byggfile.yml files. The schema will be printed to stdout.",
+    )
+    return parser
+
 
+def main():
+    parser = create_argument_parser()
     args = parser.parse_args()
 
     try:
-        return dispatcher(
-            args.actions,
-            args.directory[0] if args.directory else None,
-            int(args.jobs) if args.jobs else None,
-            args.always_make,
-            args.check,
-            args.clean,
-            args.list,
-        )
+        return dispatcher(args)
     except KeyboardInterrupt:
         rich.print("[red]Interrupted by user. Aborting.[/red]")
         return 1
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bygg-0.0.dev2/src/bygg/runner.py` & `bygg-0.1.0/src/bygg/runner.py`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/src/bygg/scheduler.py` & `bygg-0.1.0/src/bygg/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,23 @@
         if self.always_make:
             return True
 
         action = self.build_actions[job_name]
         cached_digests = self.cache.get_digests(job_name)
 
         if (
+            len(action.inputs) == 0
+            and len(action.outputs) == 0
+            and not action.dynamic_dependency
+        ):
+            # An action with neither inputs nor outputs will always be built
+            # print(f"Job {job_name} is dirty (no inputs or outputs)")
+            return True
+
+        if (
             not cached_digests
             or not cached_digests.outputs_digest
             or not cached_digests.inputs_digest
         ):
             # No previous result, so we need to build
             # print(f"Job {job_name} is dirty (no previous result)")
             return True
@@ -141,29 +150,34 @@
                 return True
 
             dd_result = action.dynamic_dependency()
             if (
                 dd_result is None
                 or calculate_digest([dd_result]) != cached_digests.dynamic_digest
             ):
+                # print(f"Job {job_name} is dirty (dynamic dependency changed)")
                 return True
 
         # TODO handle files_were_missing here? abort?
         if cached_digests.inputs_digest != inputs_digest:
             # The inputs have changed, so we need to rebuild
             # print(f"Job {job_name} is dirty (inputs changed)")
             return True
 
         # print(f"Job {job_name} is clean")
         return False
 
     def get_ready_jobs(self, batch_size: int = 0) -> List[Job]:
         """
-        Create a batch of jobs and put them in the running pool. Returns all ready jobs if
-        batch_size is 0.
+        Create a batch of jobs and put them in the running pool. Returns all ready jobs
+        if batch_size is 0.
+
+        An empty job list may be returned even if there are more jobs left to run if all
+        jobs in the batch were skipped. Job runners should continue polling for more
+        jobs until the scheduler status is "finished".
         """
         if batch_size == 0 or len(self.ready_jobs) < batch_size:
             new_jobs = self.job_graph.get_ready_jobs(
                 self.finished_jobs, self.running_jobs
             )
             dirty_jobs = []
             for job in new_jobs:
```

### Comparing `bygg-0.0.dev2/src/bygg/status_display.py` & `bygg-0.1.0/src/bygg/status_display.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import rich
 import rich.box
 import rich.progress
 import rich.status
 import rich.table
 
 from bygg.action import Action
+from bygg.common_types import CommandStatus
 from bygg.runner import JobStatus
-from bygg.types import CommandStatus
 
 console = rich.console.Console()
 
 progress: rich.progress.Progress = rich.progress.Progress(
     rich.progress.SpinnerColumn(
         table_column=rich.table.Column(ratio=None),
         spinner_name="bouncingBar",
```

### Comparing `bygg-0.0.dev2/src/bygg/util.py` & `bygg-0.1.0/src/bygg/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 import subprocess
 from typing import List, Optional, Set, Tuple
 
-from bygg.types import CommandStatus
+from bygg.common_types import CommandStatus
 
 
 def create_shell_command(shell_command: str, message: Optional[str] = None):
     def call_shell_command(inputs: Optional[Set[str]], outputs: Optional[Set[str]]):
         # Map stderr onto stdout and return both as the output
         process = subprocess.run(
             shell_command,
```

### Comparing `bygg-0.0.dev2/tests/test_action.py` & `bygg-0.1.0/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/tests/test_cache.py` & `bygg-0.1.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/tests/test_scheduler.py` & `bygg-0.1.0/tests/test_scheduler.py`

 * *Files 9% similar despite different names*

```diff
@@ -266,14 +266,56 @@
         name="action1",
         dependencies=["action2"],
         is_entrypoint=True,
     )
     Action(name="action2", dynamic_dependency=lambda: "foo")
 
     assert scheduler.run_status() == "not started"
+    scheduler.start_run("action1")
+    assert scheduler.run_status() == "running"
+
+    # check that the scheduler has the correct number of actions
+    assert len(scheduler.build_actions) == 2
+    assert len(scheduler.job_graph) == 2
+
+    job = scheduler.get_ready_jobs()[0]
+    assert job
+    assert job.name == "action2"
+    job.status = CommandStatus(0, "Executed successfully", None)
+    scheduler.job_finished(job)
+
+    # check again that the scheduler has the correct number of actions
+    assert len(scheduler.build_actions) == 2
+    assert len(scheduler.job_graph) == 1
+
+    job = scheduler.get_ready_jobs()[0]
+    assert job
+    assert len(scheduler.job_graph) == 1
+    job.status = CommandStatus(0, "Executed successfully", None)
+    scheduler.job_finished(job)
+
+    assert scheduler.run_status() == "finished"
+
+    assert len(scheduler.build_actions) == 2
+    assert len(scheduler.running_jobs) == 0
+
+
+def test_scheduler_dynamic_dependency_two_runs():
+    scheduler.__init__()
+    cache_file = get_closed_tmpfile()
+    scheduler.init_cache(cache_file)
+
+    Action(
+        name="action1",
+        dependencies=["action2"],
+        is_entrypoint=True,
+    )
+    Action(name="action2", dynamic_dependency=lambda: "foo")
+
+    assert scheduler.run_status() == "not started"
 
     scheduler.start_run("action1")
 
     assert scheduler.run_status() == "running"
 
     # check that the scheduler has the correct number of actions
     assert len(scheduler.build_actions) == 2
@@ -321,16 +363,22 @@
 
     # check that the scheduler has the correct number of actions
     assert len(scheduler.build_actions) == 2
     assert len(scheduler.job_graph) == 2
 
     jobs = scheduler.get_ready_jobs()
     assert len(jobs) == 0
+    assert scheduler.run_status() == "running"
+
+    # Ask again since the job should have been skipped and the scheduler is still
+    # running:
+    job = scheduler.get_ready_jobs()[0]
+    assert job
+    assert len(scheduler.job_graph) == 1
+
+    job.status = CommandStatus(0, "Executed successfully", None)
+    scheduler.job_finished(job)
 
-    # Asking again triggers the scheduler to realise whether it's done or not.
-    # TODO this behavious should probably be changeed.
-    jobs = scheduler.get_ready_jobs()
-    assert len(scheduler.job_graph) == 0
     assert scheduler.run_status() == "finished"
 
     assert len(scheduler.build_actions) == 2
     assert len(scheduler.running_jobs) == 0
```

### Comparing `bygg-0.0.dev2/tests/test_utils.py` & `bygg-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/LICENSE` & `bygg-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/README.md` & `bygg-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,33 @@
-# Bygg, a Python build system that gets out of your way
+<div align="center">
+
+# Bygg
+
+_a Python build system that gets out of your way_
+
+[![PyPI](https://img.shields.io/pypi/v/bygg?flat)](https://pypi.org/project/bygg/)
+[![GitHub Release Date](https://img.shields.io/github/release-date/rikardg/bygg)](https://github.com/rikardg/bygg/releases)
+[![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/rikardg/bygg/run_tests.yml?branch=master&flat)](https://github.com/rikardg/bygg/actions?query=branch%3Amaster+)
+[![GitHub](https://img.shields.io/github/license/rikardg/bygg)](LICENSE)
+
+[Installation](#installation) • [Usage](#usage) • [Development](#development)
+
+</div>
+
+---
 
 _Bygg is in early stage of development. It is usable and useful for its
 currently implemented use cases. Feel free to try it out, but also expect
-things to change and evolve. Comments and bug reports are welcome!_
+things to change and evolve. Feedback and bug reports are welcome!_
 
 ## Introduction
 
 Bygg is a build system implemented in and configured using Python. It is
 general-purpose, but is aimed at those that use Python to glue together other
-sytems.
+systems.
 
 Bygg tries to get out of your way and be as thin as possible, while still
 providing correctness and minimal rebuilds.
 
 ### Basics
 
 - Specify actions in pure Python.
@@ -47,43 +62,44 @@
 @action(
     "build1",
     inputs=["foo.in", "bar.in"],
     outputs=["foo.out", "bar.out"]
     is_entrypoint: True
 )
 def a_build_command(ctx: Context):
-  # do stuff
-  ...
+    # do stuff
+    ...
 
 
 # Separate function + Action constructor:
 
 def also_a_build_command(ctx: Context):
-  # do stuff
-  ...
+    # do stuff
+    ...
 
 Action(
-  "build2",
-  inputs=["foo.in", "bar.in"],
-  outputs=["foo.out", "bar.out"],
-  dependencies=["another action"],
-  command=my_python_command
-  is_entrypoint=True
+    "build2",
+    inputs=["foo.in", "bar.in"],
+    outputs=["foo.out", "bar.out"],
+    dependencies=["another action"],
+    command=also_a_build_command
+    is_entrypoint=True
 )
 ```
 
 Bygg will check for the presence of `Byggfile.py` in the current directory. The
-actions above can be built with `build bygg1` and `bygg build2`, respectively.
+actions above can be built with `bygg build1` and `bygg build2`, respectively.
 
 ### Settings file
 
 There is also experimental support for declaring actions in a settings file
 (currently YAML). This is intended primarily for configuring static settings
 like which virtual environment to use, but can also be used for declaring
-simple actions. See `examples/taskrunner/Byggfile.yml`.
+simple actions. See `examples/taskrunner/Byggfile.yml` and
+`examples/environments/Byggfile.yml`.
 
 ## Getting a local copy
 
 If you want to try out the examples or even develop Bygg itself, Bygg can be
 tried out and worked on without installing it globally:
 
 First, clone this repo and cd into it, then execute the commands below.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bygg-0.0.dev2/pyproject.toml` & `bygg-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bygg-0.0.dev2/PKG-INFO` & `bygg-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bygg
-Version: 0.0.dev2
+Version: 0.1.0
 Summary: A small build system
 Project-URL: Homepage, https://github.com/rikardg/bygg
 Project-URL: Bug Tracker, https://github.com/rikardg/bygg/issues
 Author-email: Rikard Gillemyr <rikard.gillemyr@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 rikardg
@@ -28,31 +28,49 @@
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: dill==0.3.6
-Requires-Dist: msgspec==0.13.1
+Requires-Dist: markdown-it-py==3.0.0
+Requires-Dist: mdurl==0.1.2
+Requires-Dist: msgspec==0.16.0
 Requires-Dist: multiprocess==0.70.14
+Requires-Dist: pygments==2.15.1
 Requires-Dist: pyyaml==6.0
-Requires-Dist: rich==13.3.1
+Requires-Dist: rich==13.4.2
 Description-Content-Type: text/markdown
 
-# Bygg, a Python build system that gets out of your way
+<div align="center">
+
+# Bygg
+
+_a Python build system that gets out of your way_
+
+[![PyPI](https://img.shields.io/pypi/v/bygg?flat)](https://pypi.org/project/bygg/)
+[![GitHub Release Date](https://img.shields.io/github/release-date/rikardg/bygg)](https://github.com/rikardg/bygg/releases)
+[![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/rikardg/bygg/run_tests.yml?branch=master&flat)](https://github.com/rikardg/bygg/actions?query=branch%3Amaster+)
+[![GitHub](https://img.shields.io/github/license/rikardg/bygg)](LICENSE)
+
+[Installation](#installation) • [Usage](#usage) • [Development](#development)
+
+</div>
+
+---
 
 _Bygg is in early stage of development. It is usable and useful for its
 currently implemented use cases. Feel free to try it out, but also expect
-things to change and evolve. Comments and bug reports are welcome!_
+things to change and evolve. Feedback and bug reports are welcome!_
 
 ## Introduction
 
 Bygg is a build system implemented in and configured using Python. It is
 general-purpose, but is aimed at those that use Python to glue together other
-sytems.
+systems.
 
 Bygg tries to get out of your way and be as thin as possible, while still
 providing correctness and minimal rebuilds.
 
 ### Basics
 
 - Specify actions in pure Python.
@@ -87,43 +105,44 @@
 @action(
     "build1",
     inputs=["foo.in", "bar.in"],
     outputs=["foo.out", "bar.out"]
     is_entrypoint: True
 )
 def a_build_command(ctx: Context):
-  # do stuff
-  ...
+    # do stuff
+    ...
 
 
 # Separate function + Action constructor:
 
 def also_a_build_command(ctx: Context):
-  # do stuff
-  ...
+    # do stuff
+    ...
 
 Action(
-  "build2",
-  inputs=["foo.in", "bar.in"],
-  outputs=["foo.out", "bar.out"],
-  dependencies=["another action"],
-  command=my_python_command
-  is_entrypoint=True
+    "build2",
+    inputs=["foo.in", "bar.in"],
+    outputs=["foo.out", "bar.out"],
+    dependencies=["another action"],
+    command=also_a_build_command
+    is_entrypoint=True
 )
 ```
 
 Bygg will check for the presence of `Byggfile.py` in the current directory. The
-actions above can be built with `build bygg1` and `bygg build2`, respectively.
+actions above can be built with `bygg build1` and `bygg build2`, respectively.
 
 ### Settings file
 
 There is also experimental support for declaring actions in a settings file
 (currently YAML). This is intended primarily for configuring static settings
 like which virtual environment to use, but can also be used for declaring
-simple actions. See `examples/taskrunner/Byggfile.yml`.
+simple actions. See `examples/taskrunner/Byggfile.yml` and
+`examples/environments/Byggfile.yml`.
 
 ## Getting a local copy
 
 If you want to try out the examples or even develop Bygg itself, Bygg can be
 tried out and worked on without installing it globally:
 
 First, clone this repo and cd into it, then execute the commands below.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

