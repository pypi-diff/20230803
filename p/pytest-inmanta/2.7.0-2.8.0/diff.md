# Comparing `tmp/pytest-inmanta-2.7.0.tar.gz` & `tmp/pytest-inmanta-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-inmanta-2.7.0.tar", last modified: Thu Feb 23 12:04:48 2023, max compression
+gzip compressed data, was "pytest-inmanta-2.8.0.tar", last modified: Thu Aug  3 09:22:28 2023, max compression
```

## Comparing `pytest-inmanta-2.7.0.tar` & `pytest-inmanta-2.8.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-23 12:04:48.138089 pytest-inmanta-2.7.0/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5492 2023-02-23 12:04:41.000000 pytest-inmanta-2.7.0/CHANGELOG.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11357 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       77 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11272 2023-02-23 12:04:48.138089 pytest-inmanta-2.7.0/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10439 2023-02-23 12:04:39.000000 pytest-inmanta-2.7.0/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pyproject.toml
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-23 12:04:48.136088 pytest-inmanta-2.7.0/pytest_inmanta/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      721 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/handler.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-23 12:04:48.137089 pytest-inmanta-2.7.0/pytest_inmanta/module/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1843 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/module/init.cf
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3538 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/module/init.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6396 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/parameters.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    48495 2023-02-23 12:04:39.000000 pytest-inmanta-2.7.0/pytest_inmanta/plugin.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/py.typed
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-23 12:04:48.137089 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1139 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2983 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/boolean_parameter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2121 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/enum_parameter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1258 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/float_parameter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1259 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/integer_parameter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3314 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/list_parameter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10461 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/parameter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3269 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/path_parameter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1245 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/string_parameter.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-23 12:04:48.136088 pytest-inmanta-2.7.0/pytest_inmanta.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11272 2023-02-23 12:04:48.000000 pytest-inmanta-2.7.0/pytest_inmanta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1122 2023-02-23 12:04:48.000000 pytest-inmanta-2.7.0/pytest_inmanta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-02-23 12:04:48.000000 pytest-inmanta-2.7.0/pytest_inmanta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       43 2023-02-23 12:04:48.000000 pytest-inmanta-2.7.0/pytest_inmanta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-02-23 12:04:47.000000 pytest-inmanta-2.7.0/pytest_inmanta.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       36 2023-02-23 12:04:48.000000 pytest-inmanta-2.7.0/pytest_inmanta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       15 2023-02-23 12:04:48.000000 pytest-inmanta-2.7.0/pytest_inmanta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      561 2023-02-23 12:04:48.139089 pytest-inmanta-2.7.0/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1475 2023-02-23 12:04:41.000000 pytest-inmanta-2.7.0/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-23 12:04:48.138089 pytest-inmanta-2.7.0/tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4637 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/tests/test_basic_example.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3482 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/tests/test_basic_example_v2.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4289 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/tests/test_dependencies.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      800 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/tests/test_full_deploys.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      954 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/tests/test_handlers.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1937 2023-02-23 12:04:31.000000 pytest-inmanta-2.7.0/tests/test_options.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-08-03 09:22:28.621372 pytest-inmanta-2.8.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5839 2023-08-03 09:22:22.000000 pytest-inmanta-2.8.0/CHANGELOG.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11357 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       77 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11124 2023-08-03 09:22:28.621372 pytest-inmanta-2.8.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10291 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pyproject.toml
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-08-03 09:22:28.618372 pytest-inmanta-2.8.0/pytest_inmanta/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1323 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/pytest_inmanta/core.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      721 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/handler.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-08-03 09:22:28.619372 pytest-inmanta-2.8.0/pytest_inmanta/module/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1843 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/module/init.cf
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3538 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/module/init.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6691 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/pytest_inmanta/parameters.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    51958 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/pytest_inmanta/plugin.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/py.typed
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-08-03 09:22:28.620372 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1139 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2983 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/boolean_parameter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2121 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/enum_parameter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1258 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/float_parameter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1259 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/integer_parameter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3499 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/list_parameter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10826 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/parameter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3269 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/path_parameter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1245 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/string_parameter.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-08-03 09:22:28.619372 pytest-inmanta-2.8.0/pytest_inmanta.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11124 2023-08-03 09:22:28.000000 pytest-inmanta-2.8.0/pytest_inmanta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1145 2023-08-03 09:22:28.000000 pytest-inmanta-2.8.0/pytest_inmanta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-08-03 09:22:28.000000 pytest-inmanta-2.8.0/pytest_inmanta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       43 2023-08-03 09:22:28.000000 pytest-inmanta-2.8.0/pytest_inmanta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-08-03 09:22:28.000000 pytest-inmanta-2.8.0/pytest_inmanta.egg-info/not-zip-safe
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       36 2023-08-03 09:22:28.000000 pytest-inmanta-2.8.0/pytest_inmanta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       15 2023-08-03 09:22:28.000000 pytest-inmanta-2.8.0/pytest_inmanta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      561 2023-08-03 09:22:28.621372 pytest-inmanta-2.8.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1475 2023-08-03 09:22:22.000000 pytest-inmanta-2.8.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-08-03 09:22:28.620372 pytest-inmanta-2.8.0/tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5146 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/tests/test_basic_example.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4276 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/tests/test_basic_example_v2.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6708 2023-08-03 09:22:20.000000 pytest-inmanta-2.8.0/tests/test_dependencies.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      800 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/tests/test_full_deploys.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      954 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/tests/test_handlers.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1937 2023-08-03 09:22:11.000000 pytest-inmanta-2.8.0/tests/test_options.py
```

### Comparing `pytest-inmanta-2.7.0/CHANGELOG.md` & `pytest-inmanta-2.8.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# v 2.8.0 (2023-08-03)
+Changes in this release:
+- Log a warning when the id_attribute of a resource is called id.
+- Ignore `__pycache__` dirs when copying the current module to the test project dir
+- Introduce `--pip-index-url` option to set corresponding project config section for inmanta-core 9.0.
+- Dropped nonexistent option from the README
+
 # v 2.7.0 (2023-02-23)
 Changes in this release:
 - Introduce `project_metadata` fixture to allow modifying the `project.yml` file for the project created by the project fixture.
 
 # v 2.6.0 (2023-02-02)
 Changes in this release:
 - Add `dryrun_all` method to  the `project` fixture. Does a dryrun on every resource of a project. Also does some sanity checks.
```

### Comparing `pytest-inmanta-2.7.0/LICENSE` & `pytest-inmanta-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/PKG-INFO` & `pytest-inmanta-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta
-Version: 2.7.0
+Version: 2.8.0
 Summary: A py.test plugin providing fixtures to simplify inmanta modules testing.
 Home-page: https://github.com/inmanta/pytest-inmanta
 Author: Inmanta NV
 Author-email: code@inmanta.com
 License: Apache License, Version 2.0
 Keywords: pytest py.test inmanta testing unit tests plugin
 Classifier: Development Status :: 5 - Production/Stable
@@ -244,15 +244,14 @@
     Multiple repos can be passed by space-separating them or by passing the parameter multiple times.
  * `--install-mode`: install mode to use for modules downloaded during this test, overrides `INMANTA_INSTALL_MODE`.
  * `--no-load-plugins`: Don't load plugins in the Project class. Overrides `INMANTA_NO_LOAD_PLUGINS`. 
  When not using this option during the testing of plugins with the `project.get_plugin_function` method, 
  it's possible that the module's `plugin/__init__.py` is loaded multiple times, 
  which can cause issues when it has side effects, as they are executed multiple times as well.
  * `--no-strict-deps-check`: option to run pytest-inmanta using the legacy check(less strict) on requirements. By default the new strict will be used.
- * `--agent-install-dependency-modules`: option to enable `agent_install_dependency_modules` option in the projects created by the project fixture.
  
  Use the generic pytest options `--log-cli-level` to show Inmanta logger to see any setup or cleanup warnings. For example,
  `--log-cli-level=INFO`
 
 ## Compatibility with pytest-cov
 
 The `--use-module-in-place` option should be set when pytest-inmanta is used in combination with the `pytest-cov` pytest plugin. Without the `--use-module-in-place` option, the reported test coverage will be incorrect.
```

### Comparing `pytest-inmanta-2.7.0/README.md` & `pytest-inmanta-2.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,14 @@
     Multiple repos can be passed by space-separating them or by passing the parameter multiple times.
  * `--install-mode`: install mode to use for modules downloaded during this test, overrides `INMANTA_INSTALL_MODE`.
  * `--no-load-plugins`: Don't load plugins in the Project class. Overrides `INMANTA_NO_LOAD_PLUGINS`. 
  When not using this option during the testing of plugins with the `project.get_plugin_function` method, 
  it's possible that the module's `plugin/__init__.py` is loaded multiple times, 
  which can cause issues when it has side effects, as they are executed multiple times as well.
  * `--no-strict-deps-check`: option to run pytest-inmanta using the legacy check(less strict) on requirements. By default the new strict will be used.
- * `--agent-install-dependency-modules`: option to enable `agent_install_dependency_modules` option in the projects created by the project fixture.
  
  Use the generic pytest options `--log-cli-level` to show Inmanta logger to see any setup or cleanup warnings. For example,
  `--log-cli-level=INFO`
 
 ## Compatibility with pytest-cov
 
 The `--use-module-in-place` option should be set when pytest-inmanta is used in combination with the `pytest-cov` pytest plugin. Without the `--use-module-in-place` option, the reported test coverage will be incorrect.
```

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/__init__.py` & `pytest-inmanta-2.8.0/pytest_inmanta/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/handler.py` & `pytest-inmanta-2.8.0/pytest_inmanta/handler.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/module/init.cf` & `pytest-inmanta-2.8.0/pytest_inmanta/module/init.cf`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/module/init.py` & `pytest-inmanta-2.8.0/pytest_inmanta/module/init.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/parameters.py` & `pytest-inmanta-2.8.0/pytest_inmanta/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,25 @@
     environment_variable=inm_mod_repo_legacy.environment_variable,
     usage=inm_mod_repo_legacy.usage,
     default=["https://github.com/inmanta/"],
     group=param_group,
     legacy=inm_mod_repo_legacy,
 )
 
+pip_index_url = ListTestParameter(
+    argument="--pip-index-url",
+    environment_variable="INMANTA_PIP_INDEX_URL",
+    usage=(
+        "Pip index to install dependencies from."
+        "Can be specified multiple times to add multiple indexes."
+    ),
+    group=param_group,
+    default=[],
+)
+
 
 # This is the legacy install mode option
 # TODO remove this in next major version bump
 inm_install_mode_legacy = EnumTestParameter(
     argument="--install_mode",
     environment_variable="INMANTA_INSTALL_MODE",
     usage="Install mode for modules downloaded during this test",
```

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/plugin.py` & `pytest-inmanta-2.8.0/pytest_inmanta/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,32 +14,32 @@
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 import collections
 import importlib
 import inspect
+import itertools
 import json
 import logging
 import math
 import os
 import re
 import shutil
 import sys
 import tempfile
 import typing
 import warnings
 from collections import defaultdict
 from dataclasses import dataclass
-from distutils import dir_util
 from itertools import chain
 from pathlib import Path
 from textwrap import dedent
 from types import FunctionType, ModuleType
-from typing import Dict, Iterator, List, Optional, Set, Tuple
+from typing import Dict, Iterator, List, Optional, Sequence, Set, Tuple
 
 import pydantic
 import pytest
 import yaml
 from tornado import ioloop
 
 import inmanta.ast
@@ -52,34 +52,41 @@
 from inmanta.const import ResourceState
 from inmanta.data import LogLine
 from inmanta.data.model import AttributeStateChange, ResourceIdStr
 from inmanta.execute.proxy import DynamicProxy
 from inmanta.export import Exporter, ResourceDict, cfg_env
 from inmanta.protocol import json_encode
 from inmanta.resources import Resource
+from pytest_inmanta.core import SUPPORTS_PROJECT_PIP_INDEX
+
+from .test_parameter.parameter import ValueSetBy
 
 if typing.TYPE_CHECKING:
     # Local type stub for mypy that works with both pytest < 7 and pytest >=7
     # https://docs.pytest.org/en/7.1.x/_modules/_pytest/legacypath.html#TempdirFactory
     import py
     from inmanta.agent.io.local import IOBase
 
     class TempdirFactory:
         def mktemp(self, path: str) -> py.path.local:
             ...
 
 
+if SUPPORTS_PROJECT_PIP_INDEX:
+    from inmanta.module import ProjectPipConfig
+
 from .handler import DATA
 from .parameters import (
     inm_install_mode,
     inm_mod_in_place,
     inm_mod_repo,
     inm_no_load_plugins,
     inm_no_strict_deps_check,
     inm_venv,
+    pip_index_url,
 )
 from .test_parameter import ParameterNotSetException, TestParameterRegistry
 
 try:
     """
     Those classes are only used in type annotation, but the import doesn't work
     in python 3.6.  So we simply catch the error and ignore it.
@@ -215,14 +222,34 @@
         else:
             repo_info: module.ModuleRepoInfo
             try:
                 repo_info = module.ModuleRepoInfo(url=parts[1], type=parts[0])
             # there might be only one part or part might be just "https"
             except (IndexError, pydantic.ValidationError):
                 repo_info = module.ModuleRepoInfo(url=repo_str)
+            if SUPPORTS_PROJECT_PIP_INDEX:
+                if repo_info.type == module.ModuleRepoType.package:
+                    alternative_text: str = (
+                        "is now deprecated and will raise a warning during compilation."
+                        " Use the --pip-index-url <index_url> pytest option instead or set"
+                        " the %s environment variable to address these warnings. "
+                    )
+                    if inm_mod_repo._value_set_using == ValueSetBy.ENV_VARIABLE:
+                        LOGGER.warning(
+                            "Setting a package source through the %s environment variable "
+                            + alternative_text,
+                            inm_mod_repo.environment_variable,
+                            pip_index_url.environment_variable,
+                        )
+                    elif inm_mod_repo._value_set_using == ValueSetBy.CLI:
+                        LOGGER.warning(
+                            "Setting a package source through the --module-repo <index_url> cli option with type `package` "
+                            + alternative_text,
+                            pip_index_url.environment_variable,
+                        )
             return json.loads(repo_info.json())
 
     return [parse_repo(repo) for repo in repo_options]
 
 
 @pytest.fixture(scope="session")
 def project_dir() -> str:
@@ -258,27 +285,60 @@
             repo.split(" ")
             for repo in (
                 repo_options if isinstance(repo_options, list) else [repo_options]
             )
         )
     )
 
+    index_urls: Sequence[str] = pip_index_url.resolve(request.config)
     modulepath = ["libs"]
     in_place = inm_mod_in_place.resolve(request.config)
     if in_place:
         modulepath.append(str(Path(CURDIR).parent))
 
-    return module.ProjectMetadata(
-        name="testcase",
-        description="Project for testcase",
-        repo=repos,
-        modulepath=modulepath,
-        downloadpath="libs",
-        install_mode=inm_install_mode.resolve(request.config).value,
-    )
+    if SUPPORTS_PROJECT_PIP_INDEX:
+        # On newer versions of core we set the pip.index_url of the project.yml file
+        repos_urls: List[str] = [
+            repo["url"]
+            for repo in repos
+            if repo["type"] == module.ModuleRepoType.package
+        ]
+        pip_config: ProjectPipConfig = ProjectPipConfig(
+            # This ensures no duplicates are returned and insertion order is preserved.
+            # i.e. the left-most index will be passed to pip as --index-url and the others as --extra-index-url
+            index_urls=list(
+                {value: None for value in itertools.chain(index_urls, repos_urls)}
+            )
+        )
+        return module.ProjectMetadata(
+            name="testcase",
+            description="Project for testcase",
+            repo=repos,
+            modulepath=modulepath,
+            downloadpath="libs",
+            install_mode=inm_install_mode.resolve(request.config).value,
+            pip=pip_config,
+        )
+    else:
+        if index_urls:
+            LOGGER.warning(
+                "Setting a project-wide pip index is not supported on this version of inmanta-core. "
+                "The provided index will be used as a v2 package source"
+            )
+        v2_source_repos = [
+            {"url": index_url, "type": "package"} for index_url in index_urls
+        ]
+        return module.ProjectMetadata(
+            name="testcase",
+            description="Project for testcase",
+            repo=list(repos) + v2_source_repos,
+            modulepath=modulepath,
+            downloadpath="libs",
+            install_mode=inm_install_mode.resolve(request.config).value,
+        )
 
 
 @pytest.fixture(scope="session")
 def project_factory(
     request: pytest.FixtureRequest,
     project_dir: str,
     project_metadata: module.ProjectMetadata,
@@ -349,15 +409,19 @@
     """
     # copy the current module in
     mod: module.Module
     path: str
     mod, path = get_module()
     if not hasattr(module, "ModuleV2") or isinstance(mod, module.ModuleV1):
         if not in_place:
-            dir_util.copy_tree(path, os.path.join(v1_modules_dir, mod.name))
+            shutil.copytree(
+                path,
+                os.path.join(v1_modules_dir, mod.name),
+                ignore=shutil.ignore_patterns("__pycache__"),
+            )
     else:
         installed: typing.Optional[module.ModuleV2] = module.ModuleV2Source(
             urls=[]
         ).get_installed_module(None, mod.name)
         if installed is None:
             raise Exception(
                 "The module being tested is not installed in the current Python environment. Please install it with"
@@ -1133,14 +1197,23 @@
         exporter = Exporter()
 
         version, resources = exporter.run(types, scopes, no_commit=not export)
 
         for key, blob in exporter._file_store.items():
             self.add_blob(key, blob)
 
+        for cls_name, value in inmanta.resources.resource._resources.items():
+            name_id_attribute = value[1]["name"]
+            if name_id_attribute == "id":
+                warnings.warn(
+                    "In one of the next major releases of inmanta-core it will not be possible "
+                    f"anymore to use an id_attribute called id for {cls_name}",
+                    DeprecationWarning,
+                )
+
         self._root_scope = scopes
         self.version = version
         self.resources = resources
         self.types = types
         self._exporter = exporter
 
         captured = self._capsys.readouterr()
```

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/__init__.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/boolean_parameter.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/boolean_parameter.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/enum_parameter.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/enum_parameter.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/float_parameter.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/float_parameter.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/integer_parameter.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/integer_parameter.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/list_parameter.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/list_parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Those classes are only used in type annotation, but the import doesn't work
     in python 3.6.  So we simply catch the error and ignore it.
     """
     from pytest import Config
 except ImportError:
     pass
 
-from .parameter import ParameterNotSetException, TestParameter
+from .parameter import ParameterNotSetException, TestParameter, ValueSetBy
 
 
 class ListTestParameter(TestParameter[Sequence[str]]):
     """
     A test parameter that should contain a list of string.  For each mention of the option, the value
     will be added to the string.  If the value is passed as an environment variable, the string will
     be splitted in each space.
@@ -83,23 +83,27 @@
                 f"Type of {raw_value} is {type(raw_value)}, expected sequence"
             )
 
         return [str(item) for item in raw_value]
 
     def resolve(self, config: "Config") -> Sequence[str]:
         option = config.getoption(self.argument, default=self.default)
+
         if option is not None and option is not self.default:
             # A value is set, and it is not the default one
+            self._value_set_using = ValueSetBy.CLI
             if isinstance(option, collections.abc.Sequence):
                 return self.validate(option)
             else:
                 return self.validate([option])
 
         env_var = os.getenv(self.environment_variable)
         if env_var is not None:
             # A value is set
+            self._value_set_using = ValueSetBy.ENV_VARIABLE
             return self.validate(env_var.split(" "))
 
         if self.default is not None:
+            self._value_set_using = ValueSetBy.DEFAULT_VALUE
             return self.default
 
         raise ParameterNotSetException(self)
```

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/parameter.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Contact: code@inmanta.com
 """
 import logging
 import os
 import uuid
 from abc import abstractmethod
 from collections import defaultdict
+from enum import Enum
 from typing import Container, Dict, Generic, List, Optional, Set, TypeVar, Union
 
 try:
     """
     Those classes are only used in type annotation, but the import doesn't work
     in python 3.6.  So we simply catch the error and ignore it.
     """
@@ -161,14 +162,24 @@
 
         # We setup all the options that are already registered
         for group_name, parameters in cls.test_parameter_groups().items():
             for param in parameters:
                 TestParameterRegistry.add_option(parser, group_name, param)
 
 
+class ValueSetBy(Enum):
+    """
+    This class is used to record how the value was provided for a test parameter.
+    """
+
+    DEFAULT_VALUE: str = "DEFAULT_VALUE"
+    CLI: str = "CLI"
+    ENV_VARIABLE: str = "ENV_VARIABLE"
+
+
 class TestParameter(Generic[ParameterType]):
     """
     This class represents a parameter that can be passed to the tests, either via a pytest
     argument, or via an environment variable.
     """
 
     def __init__(
@@ -200,14 +211,16 @@
             its deprecation.
         """
         self.argument = argument
         self.environment_variable = environment_variable
         self.usage = usage
         self.default = default
         self.legacy = legacy
+        # Track how the value was set when it is being resolved:
+        self._value_set_using: Optional[str] = None
 
         TestParameterRegistry.register(key, self, group)
 
     @property
     def help(self) -> str:
         """
         Build up a help message, based on the usage, default value and environment variable name.
```

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/path_parameter.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/path_parameter.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta/test_parameter/string_parameter.py` & `pytest-inmanta-2.8.0/pytest_inmanta/test_parameter/string_parameter.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta.egg-info/PKG-INFO` & `pytest-inmanta-2.8.0/pytest_inmanta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta
-Version: 2.7.0
+Version: 2.8.0
 Summary: A py.test plugin providing fixtures to simplify inmanta modules testing.
 Home-page: https://github.com/inmanta/pytest-inmanta
 Author: Inmanta NV
 Author-email: code@inmanta.com
 License: Apache License, Version 2.0
 Keywords: pytest py.test inmanta testing unit tests plugin
 Classifier: Development Status :: 5 - Production/Stable
@@ -244,15 +244,14 @@
     Multiple repos can be passed by space-separating them or by passing the parameter multiple times.
  * `--install-mode`: install mode to use for modules downloaded during this test, overrides `INMANTA_INSTALL_MODE`.
  * `--no-load-plugins`: Don't load plugins in the Project class. Overrides `INMANTA_NO_LOAD_PLUGINS`. 
  When not using this option during the testing of plugins with the `project.get_plugin_function` method, 
  it's possible that the module's `plugin/__init__.py` is loaded multiple times, 
  which can cause issues when it has side effects, as they are executed multiple times as well.
  * `--no-strict-deps-check`: option to run pytest-inmanta using the legacy check(less strict) on requirements. By default the new strict will be used.
- * `--agent-install-dependency-modules`: option to enable `agent_install_dependency_modules` option in the projects created by the project fixture.
  
  Use the generic pytest options `--log-cli-level` to show Inmanta logger to see any setup or cleanup warnings. For example,
  `--log-cli-level=INFO`
 
 ## Compatibility with pytest-cov
 
 The `--use-module-in-place` option should be set when pytest-inmanta is used in combination with the `pytest-cov` pytest plugin. Without the `--use-module-in-place` option, the reported test coverage will be incorrect.
```

### Comparing `pytest-inmanta-2.7.0/pytest_inmanta.egg-info/SOURCES.txt` & `pytest-inmanta-2.8.0/pytest_inmanta.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 pytest_inmanta/__init__.py
+pytest_inmanta/core.py
 pytest_inmanta/handler.py
 pytest_inmanta/parameters.py
 pytest_inmanta/plugin.py
 pytest_inmanta/py.typed
 pytest_inmanta.egg-info/PKG-INFO
 pytest_inmanta.egg-info/SOURCES.txt
 pytest_inmanta.egg-info/dependency_links.txt
```

### Comparing `pytest-inmanta-2.7.0/setup.cfg` & `pytest-inmanta-2.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/setup.py` & `pytest-inmanta-2.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with io.open(os.path.join(cwd, "README.md"), encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="pytest-inmanta",
-    version="2.7.0",
+    version="2.8.0",
     description=(
         "A py.test plugin providing fixtures to simplify inmanta modules testing."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/inmanta/pytest-inmanta",
     author="Inmanta NV",
```

### Comparing `pytest-inmanta-2.7.0/tests/test_basic_example.py` & `pytest-inmanta-2.8.0/tests/test_basic_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,28 @@
     testdir.copy_example("testmodule")
 
     result = testdir.runpytest("tests/test_BadLog.py")
 
     result.assert_outcomes(xfailed=1)
 
 
+def test_resource_bad_id_attribute(testdir):
+    """Make sure a deprecation warning is shown if an id_attribute called 'id' is found."""
+
+    testdir.copy_example("testmodule")
+
+    result = testdir.runpytest("tests/test_resource_bad_id_attribute.py")
+
+    result.assert_outcomes(passed=1)
+    assert (
+        "In one of the next major releases of inmanta-core it will not be possible anymore "
+        "to use an id_attribute called id for testmodule::ResourceBadIdAttribute"
+    ) in result.stdout.str()
+
+
 def test_release_mode_validation(testdir):
     """Set invalid release mode"""
 
     testdir.copy_example("testmodule")
 
     result = testdir.runpytest("tests/test_resource_run.py", "--install_mode", "other")
     assert (
```

### Comparing `pytest-inmanta-2.7.0/tests/test_basic_example_v2.py` & `pytest-inmanta-2.8.0/tests/test_basic_example_v2.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,33 +18,47 @@
 import logging
 
 # Note: These tests only function when the pytest output is not modified by plugins such as pytest-sugar!
 from typing import Iterator
 
 import pytest
 
-# be careful not to import any core>=6 objects directly
-import core
 import utils
 from inmanta import env
 
-if not core.SUPPORTS_MODULES_V2:
+# be careful not to import any core>=6 objects directly
+from pytest_inmanta.core import SUPPORTS_MODULES_V2
+
+if not SUPPORTS_MODULES_V2:
     pytest.skip(
         "Skipping modules v2 tests for inmanta-core<6 (pre modules v2).",
         allow_module_level=True,
     )
 
 
-@pytest.fixture(scope="session")
-def testmodulev2_venv(pytestconfig) -> Iterator[env.VirtualEnv]:
+@pytest.fixture(scope="function")
+def testmodulev2_editable_install() -> bool:
+    raise NotImplementedError(
+        "Tests using the testmodulev2 should have a marker specifying whether the module "
+        "should be installed in editable mode or not."
+    )
+
+
+@pytest.fixture(scope="function")
+def testmodulev2_venv(
+    testdir: pytest.Testdir,
+    pytestconfig: pytest.Config,
+    testmodulev2_editable_install: bool,
+) -> Iterator[env.VirtualEnv]:
     """
     Yields a Python environment with testmodulev2 installed in it.
     """
+    module_dir = testdir.copy_example("testmodulev2")
     with utils.module_v2_venv(
-        pytestconfig.rootpath / "examples" / "testmodulev2"
+        module_dir, editable_install=testmodulev2_editable_install
     ) as venv:
         yield venv
 
 
 @pytest.fixture(scope="function")
 def testmodulev2_venv_active(
     deactive_venv: None,
@@ -53,35 +67,42 @@
     """
     Activates a Python environment with testmodulev2 installed in it for the currently running process.
     """
     with utils.activate_venv(testmodulev2_venv) as venv:
         yield venv
 
 
-def test_basic_example(testdir, caplog, testmodulev2_venv_active):
+@pytest.mark.parametrize("testmodulev2_editable_install", [False, True])
+def test_basic_example(
+    testdir: pytest.Testdir,
+    caplog: pytest.LogCaptureFixture,
+    testmodulev2_venv_active: env.VirtualEnv,
+    testmodulev2_editable_install: bool,
+) -> None:
     """
     Make sure that our plugin works for v2 modules.
     """
-    testdir.copy_example("testmodulev2")
-
     caplog.clear()
     with caplog.at_level(logging.WARNING):
         result = testdir.runpytest_inprocess("tests/test_basics.py")
         result.assert_outcomes(passed=1)
-        # The testmodulev2_venv_active fixture does not install the module in editable mode. For pytest-inmanta tests this is
-        # fine but for module testing this is likely a mistake. Verify that the plugin raises an appropriate warning.
-        assert (
-            "The module being tested is not installed in editable mode."
-            " As a result the tests will not pick up any changes to the local source files."
-            " To install it in editable mode, run `inmanta module install -e .`."
-            in caplog.messages
-        )
 
+        if not testmodulev2_editable_install:
+            # The testmodulev2_venv_active fixture does not install the module in editable mode. For pytest-inmanta tests
+            # this is fine but for module testing this is likely a mistake. Verify that the plugin raises an appropriate
+            # warning.
+            assert (
+                "The module being tested is not installed in editable mode."
+                " As a result the tests will not pick up any changes to the local source files."
+                " To install it in editable mode, run `inmanta module install -e .`."
+                in caplog.messages
+            )
 
-def test_basic_example_no_install(testdir):
+
+def test_basic_example_no_install(testdir: pytest.Testdir) -> None:
     """
     Make sure that the plugin reports an informative error if the module under test is not installed.
     """
     testdir.copy_example("testmodulev2")
 
     result = testdir.runpytest_inprocess("tests/test_basics.py::test_compile")
 
@@ -90,16 +111,17 @@
         [
             r".*Exception: The module being tested is not installed in the current Python environment\."
             r" Please install it with `inmanta module install -e \.` before running the tests\..*"
         ]
     )
 
 
-def test_import(testdir, testmodulev2_venv_active):
+@pytest.mark.parametrize("testmodulev2_editable_install", [True])
+def test_import(
+    testdir: pytest.Testdir, testmodulev2_venv_active: env.VirtualEnv
+) -> None:
     """
     Make sure that our plugin works for v2 modules.
     """
-    testdir.copy_example("testmodulev2")
-
     result = testdir.runpytest_inprocess("tests/test_import.py")
 
     result.assert_outcomes(passed=3)
```

### Comparing `pytest-inmanta-2.7.0/tests/test_dependencies.py` & `pytest-inmanta-2.8.0/tests/test_dependencies.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,54 +12,65 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 # Note: These tests only function when the pytest output is not modified by plugins such as pytest-sugar!
-
+import logging
 import os
 import tempfile
 
 import pytest
 
 import pytest_inmanta.plugin
 import utils
 from inmanta import env
+from pytest_inmanta.core import SUPPORTS_PROJECT_PIP_INDEX
+from pytest_inmanta.parameters import pip_index_url
 
 
-def test_transitive_v2_dependencies(examples_v2_package_index, pytestconfig, testdir):
+def test_transitive_v2_dependencies(
+    examples_v2_package_index, pytestconfig, testdir, caplog
+):
     # set working directory to allow in-place with all example modules
     pytest_inmanta.plugin.CURDIR = str(
         pytestconfig.rootpath / "examples" / "test_dependencies_head"
     )
 
     testdir.copy_example("test_dependencies_head")
 
-    with tempfile.TemporaryDirectory() as venv_dir:
-        # set up environment
-        venv: env.VirtualEnv = env.VirtualEnv(env_path=venv_dir)
-        try:
-            venv.use_virtual_env()
-
-            # run tests
-            result = testdir.runpytest_inprocess(
-                "tests/test_basics.py",
-                "--use-module-in-place",
-                # add pip index containing examples packages as module repo
-                "--module_repo",
-                f"package:{examples_v2_package_index}",
-                # include configured pip index for inmanta-module-std
-                "--module_repo",
-                "package:"
-                + os.environ.get("PIP_INDEX_URL", "package:https://pypi.org/simple"),
+    with caplog.at_level(logging.WARNING):
+        with tempfile.TemporaryDirectory() as venv_dir:
+            # set up environment
+            venv: env.VirtualEnv = env.VirtualEnv(env_path=venv_dir)
+            try:
+                venv.use_virtual_env()
+
+                # run tests
+                result = testdir.runpytest_inprocess(
+                    "tests/test_basics.py",
+                    "--use-module-in-place",
+                    # add pip index containing examples packages as module repo
+                    "--pip-index-url",
+                    f"{examples_v2_package_index}",
+                    # include configured pip index for inmanta-module-std
+                    "--pip-index-url",
+                    f'{os.environ.get("PIP_INDEX_URL", "https://pypi.org/simple")}',
+                )
+                result.assert_outcomes(passed=1)
+            finally:
+                utils.unload_modules_for_path(venv.site_packages_dir)
+
+        if not SUPPORTS_PROJECT_PIP_INDEX:
+            warning_msg: str = (
+                "Setting a project-wide pip index is not supported on this version of inmanta-core. "
+                "The provided index will be used as a v2 package source"
             )
-            result.assert_outcomes(passed=1)
-        finally:
-            utils.unload_modules_for_path(venv.site_packages_dir)
+            assert warning_msg in caplog.text
 
 
 @pytest.mark.parametrize(
     "no_strict_deps_check, error_msg",
     [
         (True, "CompilerException"),
         (False, "ConflictingRequirements"),
@@ -93,18 +104,62 @@
 
             # run tests
             result = testdir.runpytest_inprocess(
                 "tests/test_basics.py",
                 *(["--no-strict-deps-check"] if no_strict_deps_check else []),
                 "--use-module-in-place",
                 # add pip index containing examples packages as module repo
-                "--module_repo",
-                f"package:{examples_v2_package_index}",
+                "--pip-index-url",
+                f"{examples_v2_package_index}",
                 # include configured pip index for inmanta-module-std and lorem
-                "--module_repo",
-                "package:"
-                + os.environ.get("PIP_INDEX_URL", "package:https://pypi.org/simple"),
+                "--pip-index-url",
+                f'{os.environ.get("PIP_INDEX_URL", "https://pypi.org/simple")}',
             )
             result.assert_outcomes(errors=1)
             assert error_msg in "\n".join(result.outlines)
         finally:
             utils.unload_modules_for_path(venv.site_packages_dir)
+
+
+def test_transitive_v2_dependencies_legacy_warning(
+    examples_v2_package_index, pytestconfig, testdir, caplog
+):
+    # set working directory to allow in-place with all example modules
+    pytest_inmanta.plugin.CURDIR = str(
+        pytestconfig.rootpath / "examples" / "test_dependencies_head"
+    )
+
+    testdir.copy_example("test_dependencies_head")
+
+    with caplog.at_level(logging.WARNING):
+        with tempfile.TemporaryDirectory() as venv_dir:
+            # set up environment
+            venv: env.VirtualEnv = env.VirtualEnv(env_path=venv_dir)
+            try:
+                venv.use_virtual_env()
+
+                # run tests
+                result = testdir.runpytest_inprocess(
+                    "tests/test_basics.py",
+                    "--use-module-in-place",
+                    # add pip index containing examples packages as module repo
+                    "--module_repo",
+                    f"package:{examples_v2_package_index}",
+                    # include configured pip index for inmanta-module-std
+                    "--module_repo",
+                    "package:"
+                    + os.environ.get(
+                        "PIP_INDEX_URL", "package:https://pypi.org/simple"
+                    ),
+                )
+                result.assert_outcomes(passed=1)
+            finally:
+                utils.unload_modules_for_path(venv.site_packages_dir)
+
+        if SUPPORTS_PROJECT_PIP_INDEX:
+            warning_msg: str = (
+                "Setting a package source through the --module-repo <index_url> cli option with type `package` "
+                "is now deprecated and will raise a warning during compilation."
+                " Use the --pip-index-url <index_url> pytest option instead or set"
+                f" the {pip_index_url.environment_variable} environment variable to address these warnings. "
+            )
+            assert warning_msg in caplog.text
```

### Comparing `pytest-inmanta-2.7.0/tests/test_full_deploys.py` & `pytest-inmanta-2.8.0/tests/test_full_deploys.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/tests/test_handlers.py` & `pytest-inmanta-2.8.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-2.7.0/tests/test_options.py` & `pytest-inmanta-2.8.0/tests/test_options.py`

 * *Files identical despite different names*

