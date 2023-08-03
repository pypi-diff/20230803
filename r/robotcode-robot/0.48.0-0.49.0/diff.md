# Comparing `tmp/robotcode_robot-0.48.0.tar.gz` & `tmp/robotcode_robot-0.49.0.tar.gz`

## Comparing `robotcode_robot-0.48.0.tar` & `robotcode_robot-0.49.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/src/robotcode/robot/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    79709 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/README.md
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/pyproject.toml
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.48.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    80002 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/README.md
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/pyproject.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/PKG-INFO
```

### Comparing `robotcode_robot-0.48.0/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.49.0/src/robotcode/robot/config/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 
 
 from .model import RobotConfig
 
 PYPROJECT_TOML = "pyproject.toml"
 ROBOT_TOML = "robot.toml"
 LOCAL_ROBOT_TOML = ".robot.toml"
+USER_DEFAULT_CONFIG_TOML = "default config"
 
 
 class DiscoverdBy(str, Enum):
     GIT = ".git directory"
     HG = "hg"
-    PYPROJECT_TOML = PYPROJECT_TOML
-    ROBOT_TOML = ROBOT_TOML
-    LOCAL_ROBOT_TOML = LOCAL_ROBOT_TOML
+    PYPROJECT_TOML = "pyproject.toml (project file))"
+    ROBOT_TOML = "robot.toml (project file)"
+    LOCAL_ROBOT_TOML = ".robot.toml (local file)"
+    USER_DEFAULT_CONFIG_TOML = "robot.toml (user default config)"
     NOT_FOUND = "not found"
 
 
 class ConfigType(str, Enum):
-    PYPROJECT_TOML = PYPROJECT_TOML
-    ROBOT_TOML = ROBOT_TOML
-    LOCAL_ROBOT_TOML = LOCAL_ROBOT_TOML
-    CUSTOM_TOML = ".toml"
+    PYPROJECT_TOML = "pyproject.toml (project file))"
+    ROBOT_TOML = "robot.toml (project file)"
+    LOCAL_ROBOT_TOML = ".robot.toml (local file)"
+    USER_DEFAULT_CONFIG_TOML = "robot.toml (user default config)"
+    CUSTOM_TOML = ".toml (custom file)"
 
 
 class ConfigValueError(ValueError):
     def __init__(self, path: Path, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.path = path
 
@@ -68,14 +71,21 @@
 
     except ValueError as e:
         raise ConfigValueError(__path, f'Parsing "{__path}" failed: {e}') from e
     except TypeError as e:
         raise ConfigTypeError(__path, f'Parsing "{__path}" failed: {e}') from e
 
 
+def get_default_config() -> RobotConfig:
+    result = RobotConfig()
+    result.output_dir = "results"
+    result.python_path = ["./lib", "./resources"]
+    return result
+
+
 def load_config_from_path(*__paths: Union[Path, Tuple[Path, ConfigType]]) -> RobotConfig:
     result = RobotConfig()
 
     for __path in __paths:
         result.add_options(_load_config_data_from_path(__path if isinstance(__path, Path) else __path[0]))
 
     return result
```

### Comparing `robotcode_robot-0.48.0/src/robotcode/robot/config/model.py` & `robotcode_robot-0.49.0/src/robotcode/robot/config/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # ruff: noqa: RUF009
-
 import dataclasses
 import datetime
 import fnmatch
 import os
 import platform
 import re
 from dataclasses import dataclass
 from enum import Enum
+from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Literal,
     Optional,
     Tuple,
     Union,
     get_type_hints,
 )
 
-from robotcode.core.dataclasses import TypeValidationError, ValidateMixin, validate_types
+import tomli_w
+from robotcode.core.dataclasses import TypeValidationError, ValidateMixin, as_dict, validate_types
 from robotcode.core.utils.safe_eval import safe_eval
 from typing_extensions import Self
 
 
 class Flag(str, Enum):
     ON = "on"
     OFF = "off"
@@ -2097,14 +2098,19 @@
 
     testdoc: Optional[TestDocProfile] = field(
         description="""\
             Options to be passed to _testdoc_.
         """
     )
 
+    def save(self, path: "os.PathLike[str]") -> None:
+        Path(path).parent.mkdir(parents=True, exist_ok=True)
+        with Path(path).open("w", encoding="utf-8") as f:
+            f.write(tomli_w.dumps(as_dict(self, remove_defaults=True)))
+
 
 @dataclass
 class RobotExtraBaseProfile(RobotBaseProfile):
     """Base profile for Robot Framework with Extras."""
 
     extra_args: Optional[List[str]] = field(
         description="""\
@@ -2134,15 +2140,15 @@
 class RobotProfile(RobotExtraBaseProfile):
     """Robot Framework configuration profile."""
 
     description: Optional[str] = field(description="Description of the profile.")
 
     detached: Optional[bool] = field(
         description="""\
-            The profile should be detached."
+            The profile should be detached.
             Detached means it is not inherited from the main profile.
             """,
     )
 
     enabled: Union[bool, Condition, None] = field(
         description="""\
             If enabled the profile is used. You can also use and `if` condition
```

### Comparing `robotcode_robot-0.48.0/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.49.0/src/robotcode/robot/config/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,35 @@
 from pathlib import Path
 from typing import Callable, Optional, Sequence, Tuple, Union
 
-from .loader import (
-    ConfigType,
-    DiscoverdBy,
-    find_project_root,
-    get_config_files_from_folder,
-)
+import platformdirs
+
+from .loader import ConfigType, DiscoverdBy, find_project_root, get_config_files_from_folder, get_default_config
+
+
+def get_user_config_file(
+    create: bool = True, verbose_callback: Optional[Callable[[str], None]] = None
+) -> Optional[Path]:
+    result = Path(platformdirs.user_config_dir("robotcode", appauthor=False), "robot.toml")
+    if result.is_file():
+        if verbose_callback:
+            verbose_callback(f"Found user configuration file:\n    {result}")
+        return result
+
+    if not create:
+        if verbose_callback:
+            verbose_callback("User configuration file not found, but create is set to False.")
+        return None
+
+    if verbose_callback:
+        verbose_callback(f"User configuration file not found, try to create it at:\n    {result}")
+
+    get_default_config().save(result)
+
+    return result
 
 
 def get_config_files(
     paths: Optional[Sequence[Union[str, Path]]] = None,
     config_files: Optional[Sequence[Path]] = None,
     *,
     raise_on_error: bool = True,
@@ -26,25 +45,31 @@
         return [], None, DiscoverdBy.NOT_FOUND
 
     if verbose_callback:
         verbose_callback(f"Found root at:\n    {root_folder} ({discovered_by.value})")
 
     if config_files:
         if verbose_callback:
-            verbose_callback("Using config file:" + "\n    ".join(str(config_files)))
-
-        return [(f, ConfigType.CUSTOM_TOML) for f in config_files], root_folder, discovered_by
+            verbose_callback("Using config file:" + "\n    ".join([str(f) for f in config_files]))
 
-    result = get_config_files_from_folder(root_folder)
+        result: Sequence[Tuple[Path, ConfigType]] = [(f, ConfigType.CUSTOM_TOML) for f in config_files]
+    else:
+        result = get_config_files_from_folder(root_folder)
 
-    if not result and raise_on_error:
-        raise FileNotFoundError("Cannot find any configuration file. 😥")
+        if not result and raise_on_error:
+            raise FileNotFoundError("Cannot find any configuration file. 😥")
 
-    if verbose_callback:
-        if result:
-            verbose_callback(
-                "Found configuration files:\n    " + "\n    ".join(str(f[0]) for f in result),
-            )
-        else:
-            verbose_callback("No configuration files found.")
-
-    return result, root_folder, discovered_by
+        if verbose_callback:
+            if result:
+                verbose_callback(
+                    "Found configuration files:\n    " + "\n    ".join(str(f[0]) for f in result),
+                )
+            else:
+                verbose_callback("No configuration files found.")
+
+    user_config = get_user_config_file(verbose_callback=verbose_callback)
+
+    return (
+        [*([(user_config, ConfigType.USER_DEFAULT_CONFIG_TOML)] if user_config else []), *result],
+        root_folder,
+        discovered_by,
+    )
```

### Comparing `robotcode_robot-0.48.0/.gitignore` & `robotcode_robot-0.49.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.48.0/LICENSE.txt` & `robotcode_robot-0.49.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.48.0/README.md` & `robotcode_robot-0.49.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.48.0/pyproject.toml` & `robotcode_robot-0.49.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
-  "robotcode-core==0.48.0",
+  "platformdirs<3.9.0,>=3.2.0",
+  "robotcode-core==0.49.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.48.0/PKG-INFO` & `robotcode_robot-0.49.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.48.0
+Version: 0.49.0
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.48.0
+Requires-Dist: platformdirs<3.9.0,>=3.2.0
+Requires-Dist: robotcode-core==0.49.0
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

