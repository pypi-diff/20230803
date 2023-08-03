# Comparing `tmp/hydra-callbacks-0.3.0.tar.gz` & `tmp/hydra-callbacks-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-callbacks-0.3.0.tar", last modified: Sun Jul 23 12:49:06 2023, max compression
+gzip compressed data, was "hydra-callbacks-0.4.0.tar", last modified: Thu Aug  3 21:25:57 2023, max compression
```

## Comparing `hydra-callbacks-0.3.0.tar` & `hydra-callbacks-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:49:06.777284 hydra-callbacks-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:49:06.773284 hydra-callbacks-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:49:06.773284 hydra-callbacks-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-23 12:49:06.777284 hydra-callbacks-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 12:49:06.777284 hydra-callbacks-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:49:06.773284 hydra-callbacks-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:49:06.777284 hydra-callbacks-0.3.0/src/hydra_callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-23 12:49:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:49:06.777284 hydra-callbacks-0.3.0/src/hydra_callbacks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-23 12:49:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-23 12:49:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 12:49:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-23 12:49:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-23 12:49:06.000000 hydra-callbacks-0.3.0/src/hydra_callbacks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:49:06.777284 hydra-callbacks-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:49:06.777284 hydra-callbacks-0.3.0/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/dummy_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/gather_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/gather_app_conf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/git_callback.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/latest_callback.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/perf_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/resource_monitor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_app/runtime_perf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-23 12:48:06.000000 hydra-callbacks-0.3.0/tests/test_perflogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:25:57.985009 hydra-callbacks-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:25:57.981008 hydra-callbacks-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:25:57.981008 hydra-callbacks-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-03 21:25:57.985009 hydra-callbacks-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:25:57.985009 hydra-callbacks-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:25:57.981008 hydra-callbacks-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:25:57.981008 hydra-callbacks-0.4.0/src/hydra_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/src/hydra_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 21:25:57.000000 hydra-callbacks-0.4.0/src/hydra_callbacks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/src/hydra_callbacks/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/src/hydra_callbacks/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/src/hydra_callbacks/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:25:57.985009 hydra-callbacks-0.4.0/src/hydra_callbacks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-03 21:25:57.000000 hydra-callbacks-0.4.0/src/hydra_callbacks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-03 21:25:57.000000 hydra-callbacks-0.4.0/src/hydra_callbacks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:25:57.000000 hydra-callbacks-0.4.0/src/hydra_callbacks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 21:25:57.000000 hydra-callbacks-0.4.0/src/hydra_callbacks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 21:25:57.000000 hydra-callbacks-0.4.0/src/hydra_callbacks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:25:57.985009 hydra-callbacks-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:25:57.985009 hydra-callbacks-0.4.0/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/dummy_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/full_conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/gather_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/gather_app_conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/git_callback.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/latest_callback.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/perf_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/resource_monitor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_app/runtime_perf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-03 21:24:52.000000 hydra-callbacks-0.4.0/tests/test_perflogger.py
```

### Comparing `hydra-callbacks-0.3.0/.github/workflows/master-cd.yml` & `hydra-callbacks-0.4.0/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.3.0/.github/workflows/tags-release.yml` & `hydra-callbacks-0.4.0/.github/workflows/tags-release.yml`

 * *Files 26% similar despite different names*

```diff
@@ -4,45 +4,56 @@
   push:
     tags:
       - 'v[0-9]+.[0-9]+.[0-9]+'
 jobs:
   build-n-publish:
     name: Build and publish to PyPI
     runs-on: ubuntu-latest
+    environment: pypi-release
+    permissions:
+      id-token: write
     steps:
     - name: Checkout
       uses: actions/checkout@v3
     - name: Get history and tags for SCM versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python 3.10
       uses: actions/setup-python@v4
       with:
         python-version: "3.10"
 
     - name: Install dependencies
-      shell: bash -l {0}
+      shell: bash
       run: |
         python -m pip install .[test,optional]
 
     - name: Run Tests
-      shell: bash -l {0}
+      shell: bash
       run: |
         pytest -n auto --cov-report xml:coverage.xml
 
     - name: Install pypa/build
       run: |
         python -m pip install build
         python -m pip install .
 
     - name: Build a binary wheel and a source tarball
       run: |
         python -m build --sdist --wheel --outdir dist/ .
 
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        password: ${{ secrets.PYPI_TOKEN_RESTRICTED }}
-    
-    - name: Create release
-      uses: softprops/action-gh-release@v1
+
+  gh-release:
+     name: Create release
+     env:
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+     runs-on: ubuntu-latest
+     steps:
+     - name: Checkout
+       uses: actions/checkout@v3
+       with:
+        fetch-depth: 100
+     - name: Create Relase
+       run: gh release create "$GITHUB_REF_NAME"  --generate-notes -d
```

### Comparing `hydra-callbacks-0.3.0/.github/workflows/test-ci.yml` & `hydra-callbacks-0.4.0/.github/workflows/test-ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -16,21 +16,25 @@
         uses: actions/checkout@v3
       - name: Set up Python "3.10"
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - name: Black setup
         shell: bash
-        run: pip install black ruff
+        run: pip install black ruff mypy
+
       - name: Black Check
         shell: bash
         run: black . --diff --color
       - name: ruff Check
         shell: bash
         run: ruff src
+      - name: mypy Check
+        shell: bash
+        run: mypy --install-types --non-interactive --ignore-missing-imports src
         
   test-suite:
     runs-on: ${{ matrix.os }}
     needs: linter-check
     strategy:
       fail-fast: true
       matrix:
```

### Comparing `hydra-callbacks-0.3.0/LICENSE` & `hydra-callbacks-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.3.0/PKG-INFO` & `hydra-callbacks-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-callbacks
-Version: 0.3.0
+Version: 0.4.0
 Summary: A collection of usefull hydra callbacks for hydra configuration
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>
 Project-URL: Homepage, https://github.com/paquiteau/hydra-callbacks
 Project-URL: Bug Reports, https://github.com/paquiteau/hydra-callbacks/issues
 Project-URL: Sources, https://github.com/paquiteau/hydra-callbacks
 Keywords: hydra,configuration,callback
 Classifier: Development Status :: 3 - Alpha
@@ -25,15 +25,15 @@
 [![style](https://img.shields.io/badge/style-black-black)](https://github.com/psf/black)
 [![framework](https://img.shields.io/badge/framework-hydra-blue)](https://hydra.cc)
 [![codecov](https://codecov.io/gh/paquiteau/hydra-callbacks/branch/master/graph/badge.svg?token=NEV7SY24YB)](https://codecov.io/gh/paquiteau/hydra-callbacks)
 [![CD](https://github.com/paquiteau/hydra-callbacks/actions/workflows/master-cd.yml/badge.svg)](https://github.com/paquiteau/hydra-callbacks/actions/workflows/master-cd.yml)
 [![CI](https://github.com/paquiteau/hydra-callbacks/actions/workflows/test-ci.yml/badge.svg)](https://github.com/paquiteau/hydra-callbacks/actions/workflows/test-ci.yml)
 [![Release](https://img.shields.io/github/v/release/paquiteau/hydra-callbacks)](https://github.com/paquiteau/hydra-callbacks/releases/latest)
 
-A collection of usefulls callbacks for the [https://hydra.cc/](hydra) configuration framework.
+A collection of usefulls and simple to use callbacks for the [https://hydra.cc/](hydra) configuration framework.
 
 
 ## Installation 
 ``` shell 
 pip install hydra-callbacks
 ```
 
@@ -111,7 +111,11 @@
 
 ## You too, have cool Callbacks, or idea for one ? 
 
 Open a PR or an issue !
 
 ### Possible Ideas
 - A callback that summarize log from multiple runs
+- Monitoring of GPU  using nvitop
+  
+<p align=center> :star2: If you like this work, don't forget to star it and share it 🌟 </p>
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydra-callbacks-0.3.0/README.md` & `hydra-callbacks-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![style](https://img.shields.io/badge/style-black-black)](https://github.com/psf/black)
 [![framework](https://img.shields.io/badge/framework-hydra-blue)](https://hydra.cc)
 [![codecov](https://codecov.io/gh/paquiteau/hydra-callbacks/branch/master/graph/badge.svg?token=NEV7SY24YB)](https://codecov.io/gh/paquiteau/hydra-callbacks)
 [![CD](https://github.com/paquiteau/hydra-callbacks/actions/workflows/master-cd.yml/badge.svg)](https://github.com/paquiteau/hydra-callbacks/actions/workflows/master-cd.yml)
 [![CI](https://github.com/paquiteau/hydra-callbacks/actions/workflows/test-ci.yml/badge.svg)](https://github.com/paquiteau/hydra-callbacks/actions/workflows/test-ci.yml)
 [![Release](https://img.shields.io/github/v/release/paquiteau/hydra-callbacks)](https://github.com/paquiteau/hydra-callbacks/releases/latest)
 
-A collection of usefulls callbacks for the [https://hydra.cc/](hydra) configuration framework.
+A collection of usefulls and simple to use callbacks for the [https://hydra.cc/](hydra) configuration framework.
 
 
 ## Installation 
 ``` shell 
 pip install hydra-callbacks
 ```
 
@@ -90,7 +90,11 @@
 
 ## You too, have cool Callbacks, or idea for one ? 
 
 Open a PR or an issue !
 
 ### Possible Ideas
 - A callback that summarize log from multiple runs
+- Monitoring of GPU  using nvitop
+  
+<p align=center> :star2: If you like this work, don't forget to star it and share it 🌟 </p>
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydra-callbacks-0.3.0/pyproject.toml` & `hydra-callbacks-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.3.0/src/hydra_callbacks/__init__.py` & `hydra-callbacks-0.4.0/src/hydra_callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.3.0/src/hydra_callbacks/callbacks.py` & `hydra-callbacks-0.4.0/src/hydra_callbacks/callbacks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Callback mechanism for hydra  jobs."""
 from __future__ import annotations
-from typing import Callable
+from typing import Callable, Any
 import errno
 import glob
 import json
 import logging
 import os
 from pathlib import Path
 import time
@@ -12,33 +12,37 @@
 import pandas as pd
 from hydra.core.hydra_config import HydraConfig
 from hydra.core.utils import JobReturn
 from hydra.experimental.callback import Callback
 from hydra.types import TaskFunction
 from hydra.utils import to_absolute_path
 from omegaconf import DictConfig, open_dict
+import omegaconf
 
 from .monitor import ResourceMonitorService
 
 callback_logger = logging.getLogger("hydra.callbacks")
 
 
+def dummy_run(config: DictConfig, **kwargs: None) -> None:
+    """Do nothing."""
+    pass
+
+
 class AnyRunCallback(Callback):
     """Abstract Callback that execute on any run."""
 
     def __init__(self, enabled: bool = True):
         callback_logger.debug("Init %s", self.__class__.__name__)
 
         self.enabled = enabled
         if not self.enabled:
             # don't do anything if not enabled
-            self.on_job_start = lambda *args, **kwargs: None
-            self.on_job_end = lambda *args, **kwargs: None
-            self._on_anyrun_start = lambda *args, **kwargs: None
-            self._on_anyrun_end = lambda *args, **kwargs: None
+            self._on_anyrun_start = dummy_run  # type: ignore
+            self._on_anyrun_end = dummy_run  # type: ignore
 
     def on_run_start(self, config: DictConfig, **kwargs: None) -> None:
         """Execute before a single run."""
         callback_logger.debug("run start callback %s", self.__class__.__name__)
         self._on_anyrun_start(config, **kwargs)
 
     def on_multirun_start(self, config: DictConfig, **kwargs: None) -> None:
@@ -132,30 +136,34 @@
     aggregator: Callable
         function to aggregate the results. This function should take a list of
         filepath as input and process them. By default this assume that each
         result file is a json file, and will load them as a list of dict, and
         save them as a csv file.
     """
 
-    def __init__(self, result_file: str = "results.json", aggregator: Callable = None):
+    def __init__(
+        self,
+        result_file: str = "results.json",
+        aggregator: Callable[[list[str]], os.PathLike] | None = None,
+    ):
         callback_logger.debug("Init %s", self.__class__.__name__)
         self.result_file = result_file
 
         self.aggregator = aggregator or self._default_aggregator
 
     def on_multirun_end(self, config: DictConfig, **kwargs: None) -> None:
         """Run after all job have ended.
 
         Will write a DataFrame from all the results. at the run location.
         """
         save_dir = config.hydra.sweep.dir
         os.chdir(save_dir)
         self.aggregator(glob.glob(f"*/{self.result_file}"))
 
-    def _default_aggregator(self, files: list[os.PathLike]) -> os.PathLike:
+    def _default_aggregator(self, files: list[str]) -> os.PathLike:
         """Aggregat the results as a dataframe and save it as csv."""
         results = []
         for filename in files:
             with open(filename) as f:
                 loaded = json.load(f)
                 if isinstance(loaded, list):
                     results.extend(loaded)
@@ -226,34 +234,36 @@
         if True, will log the total runtime.
     sample_interval : float or int
         The time interval at wat which to sample the process, in seconds.
     monitoring_file : str
         The file to write the monitoring data to.
     """
 
+    _monitor: dict[tuple[str, str], Any]
+
     def __init__(
         self,
         enabled: bool = True,
         sample_interval: float = 1,
         monitoring_file: str = "resource_monitoring.csv",
     ):
         super().__init__(enabled)
 
         self.sample_interval = sample_interval
         self.monitoring_file = monitoring_file
 
     def on_run_start(self, config: DictConfig, **kwargs: None) -> None:
         """Execute after a single run."""
-        self._on_anyrun_start(config.hydra.run.dir)
+        self._set_monit_file(config.hydra.run.dir)
 
     def on_multirun_start(self, config: DictConfig, **kwargs: None) -> None:
         """Execute after a multi run."""
-        self._on_anyrun_start(config.hydra.sweep.dir)
+        self._set_monit_file(config.hydra.sweep.dir)
 
-    def _on_anyrun_start(self, run_dir: str) -> None:
+    def _set_monit_file(self, run_dir: str) -> None:
         """Configure the path for the monitoring file."""
         self.monitoring_file = os.path.join(
             to_absolute_path(run_dir), self.monitoring_file
         )
         self._monitor = {}
 
     def _on_anyrun_end(self, config: DictConfig, **kwargs: None) -> None:
@@ -279,23 +289,30 @@
         **kwargs: None,
     ) -> None:
         """Execute after a single job."""
         job_full_id = self._get_job_info()
         sampled_data = self._monitor[job_full_id].stop()
 
         del self._monitor[job_full_id]
-        sampled_data["prof_dict"]["job_name"] = job_full_id[0]
-        sampled_data["prof_dict"]["job_id"] = job_full_id[1]
-
-        df = pd.DataFrame(sampled_data["prof_dict"])
-        df.to_csv(
-            self.monitoring_file,
-            mode="a",
-            header=not os.path.exists(self.monitoring_file),
-        )
+        if sampled_data:
+            df = pd.DataFrame(sampled_data)
+            df.to_csv(
+                self.monitoring_file,
+                mode="a",
+                header=not os.path.exists(self.monitoring_file),
+            )
+            max_cpu = sampled_data["cpus"].max()
+            max_mem = sampled_data["rss_GiB"].max()
+            callback_logger.debug(
+                f"{job_full_id[0]}(#{job_full_id[1]}): max cpu: {max_cpu:.2f}%,"
+                f"max mem: {max_mem:.2f} GiB"
+            )
 
-    def _get_job_info(self) -> str:
+    def _get_job_info(self) -> tuple[str, str]:
         """Get the job id."""
         hconf = HydraConfig.get()
         name = hconf.job.name
-        id = hconf.job.get("id", 0)
+        try:
+            id = hconf.job.id
+        except omegaconf.errors.MissingMandatoryValue:
+            id = "0"
         return name, id
```

### Comparing `hydra-callbacks-0.3.0/src/hydra_callbacks/logger.py` & `hydra-callbacks-0.4.0/src/hydra_callbacks/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 
     Example
     -------
     >>> with PerfLogger(print) as pfl:
             time.sleep(1)
     """
 
-    timers = {}
+    timers: dict[str, float] = {}
+    timers_stack: list[str] = []
+    _stop_time: float
+    _start_time: float
 
     def __init__(
         self,
         logger: Logger | Callable,
         level: int = logging.INFO,
         name: str = "default",
         time_format: str = "{name} duration: {:.2f}s",
@@ -39,28 +42,29 @@
         if isinstance(logger, Logger):
             self.logger = lambda msg: logger.log(self._log_level, msg)
         elif callable(logger):
             self.logger = logger
         else:
             raise ValueError("logger must be a Logger or a callable")
 
-        self._start_time = None
-        self._stop_time = None
         self._format = time_format
 
     def __enter__(self):
         self.logger(f"Starting {self._name}...")
+        self.current_timer = self._name
         self._start_time = perf_counter()
+        self.timers_stack.append(self._name)
         return self
 
     def __exit__(self, *exc_info: tuple):
         self._stop_time = perf_counter()
         elapsed = self._stop_time - self._start_time
         formatted = self._format.format(elapsed, name=self._name)
-        self.timers[self._name] = elapsed
+        self.timers["/".join(self.timers_stack)] = elapsed
+        self.timers_stack.pop(-1)
         self.logger(formatted)
 
     @classmethod
     def recap(cls) -> str:
         """Return a string summarizing all the registered timers."""
         cls.timers["Total"] = sum(cls.timers.values())
         return ", ".join([f"{name}: {t:.2f}s" for name, t in cls.timers.items()])
```

### Comparing `hydra-callbacks-0.3.0/src/hydra_callbacks/monitor.py` & `hydra-callbacks-0.4.0/src/hydra_callbacks/monitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Resource Monitor Utilities."""
 import multiprocessing
 import os
 import time
-from typing import Callable
-
+from typing import Callable, Mapping
+from numpy.typing import ArrayLike
 import numpy as np
 import psutil
 
 _MB = 1024.0**2
 
 
 class ProcessTimer(multiprocessing.Process):
@@ -65,15 +65,15 @@
         The backend to use. Can be either "threading" or "process"
     """
 
     def __init__(
         self,
         pid: int,
         interval: int | float = 1,
-        base_name: str = None,
+        base_name: str = "",
     ):
         # Make sure psutil is imported
         import psutil
 
         if interval < 0.2:
             raise RuntimeError(
                 f"Sampling interval ({interval:0.2f}s) cannot be lower than 0.2s"
@@ -89,15 +89,15 @@
         # Leave process initialized and make first sample
         self._process = psutil.Process(pid)
         self._sample(cpu_interval=0.2)
 
         # Start thread
         self._timer = ProcessTimer(self._interval, self._sample)
 
-    def _sample(self, cpu_interval: float = None) -> None:
+    def _sample(self, cpu_interval: float | None = None) -> None:
         cpu = 0.0
         rss = 0.0
         vms = 0.0
         try:
             with self._process.oneshot():
                 cpu += self._process.cpu_percent(interval=cpu_interval)
                 mem_info = self._process.memory_info()
@@ -126,30 +126,22 @@
         self._logfile.flush()
 
     def start(self) -> None:
         """Start monitoring."""
         self._sample(cpu_interval=0.2)
         self._timer.start()
 
-    def stop(self) -> dict[str, float | None]:
+    def stop(self) -> Mapping[str, ArrayLike] | None:
         """Stop monitoring."""
         self._timer.cancel()
         del self._timer
-
-        retval = {
-            "mem_peak_gb": None,
-            "cpu_percent": None,
-        }
-
         # Read .prof file in and set runtime values
         vals = np.loadtxt(self._fname, delimiter=",")
         if vals.size:
             vals = np.atleast_2d(vals)
-            retval["mem_peak_gb"] = vals[:, 2].max() / 1024
-            retval["cpu_peak_percent"] = vals[:, 1].max()
-            retval["prof_dict"] = {
+            return {
                 "time": vals[:, 0],
                 "cpus": vals[:, 1],
                 "rss_GiB": vals[:, 2] / 1024,
                 "vms_GiB": vals[:, 3] / 1024,
             }
-        return retval
+        return None
```

### Comparing `hydra-callbacks-0.3.0/src/hydra_callbacks.egg-info/PKG-INFO` & `hydra-callbacks-0.4.0/src/hydra_callbacks.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-callbacks
-Version: 0.3.0
+Version: 0.4.0
 Summary: A collection of usefull hydra callbacks for hydra configuration
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>
 Project-URL: Homepage, https://github.com/paquiteau/hydra-callbacks
 Project-URL: Bug Reports, https://github.com/paquiteau/hydra-callbacks/issues
 Project-URL: Sources, https://github.com/paquiteau/hydra-callbacks
 Keywords: hydra,configuration,callback
 Classifier: Development Status :: 3 - Alpha
@@ -25,15 +25,15 @@
 [![style](https://img.shields.io/badge/style-black-black)](https://github.com/psf/black)
 [![framework](https://img.shields.io/badge/framework-hydra-blue)](https://hydra.cc)
 [![codecov](https://codecov.io/gh/paquiteau/hydra-callbacks/branch/master/graph/badge.svg?token=NEV7SY24YB)](https://codecov.io/gh/paquiteau/hydra-callbacks)
 [![CD](https://github.com/paquiteau/hydra-callbacks/actions/workflows/master-cd.yml/badge.svg)](https://github.com/paquiteau/hydra-callbacks/actions/workflows/master-cd.yml)
 [![CI](https://github.com/paquiteau/hydra-callbacks/actions/workflows/test-ci.yml/badge.svg)](https://github.com/paquiteau/hydra-callbacks/actions/workflows/test-ci.yml)
 [![Release](https://img.shields.io/github/v/release/paquiteau/hydra-callbacks)](https://github.com/paquiteau/hydra-callbacks/releases/latest)
 
-A collection of usefulls callbacks for the [https://hydra.cc/](hydra) configuration framework.
+A collection of usefulls and simple to use callbacks for the [https://hydra.cc/](hydra) configuration framework.
 
 
 ## Installation 
 ``` shell 
 pip install hydra-callbacks
 ```
 
@@ -111,7 +111,11 @@
 
 ## You too, have cool Callbacks, or idea for one ? 
 
 Open a PR or an issue !
 
 ### Possible Ideas
 - A callback that summarize log from multiple runs
+- Monitoring of GPU  using nvitop
+  
+<p align=center> :star2: If you like this work, don't forget to star it and share it 🌟 </p>
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydra-callbacks-0.3.0/src/hydra_callbacks.egg-info/SOURCES.txt` & `hydra-callbacks-0.4.0/src/hydra_callbacks.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/hydra_callbacks.egg-info/requires.txt
 src/hydra_callbacks.egg-info/top_level.txt
 tests/test_callbacks.py
 tests/test_perflogger.py
 tests/test_app/config.yaml
 tests/test_app/dummy.txt
 tests/test_app/dummy_app.py
+tests/test_app/full_conf.yaml
 tests/test_app/gather_app.py
 tests/test_app/gather_app_conf.yaml
 tests/test_app/git_callback.yaml
 tests/test_app/latest_callback.yaml
 tests/test_app/perf_app.py
 tests/test_app/resource_monitor.yaml
 tests/test_app/runtime_perf.yaml
```

### Comparing `hydra-callbacks-0.3.0/tests/test_app/gather_app.py` & `hydra-callbacks-0.4.0/tests/test_app/gather_app.py`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.3.0/tests/test_app/perf_app.py` & `hydra-callbacks-0.4.0/tests/test_app/perf_app.py`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.3.0/tests/test_callbacks.py` & `hydra-callbacks-0.4.0/tests/test_callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import pandas as pd
 import numpy as np
 
 _chdir_to_dir_containing("pyproject.toml")
 
 
-@contextlib.contextmanager
+@contextlib.contextmanager  # type: ignore
 def chdirto(new_dir) -> None:
     """Very simple context manager to change directory temporarly.
 
     https://stackoverflow.com/a/75049063
     """
     d = os.getcwd()
     os.chdir(new_dir)
@@ -231,15 +231,14 @@
         "hydra.job.chdir=True",
         "hydra.hydra_logging.formatters.simple.format='[HYDRA] %(message)s'",
         "hydra.job_logging.formatters.simple.format='[JOB] %(message)s'",
     ]
     result, _err = run_python_script(cmd)
     assert _err == ""
     assert_regex_match(
-        result,
         dedent(
             """\
             [HYDRA] Launching 3 jobs locally
             [HYDRA] 	#0 : +a=1
             [JOB] foo: bar
             a: 1
 
@@ -252,14 +251,15 @@
             a: 3
 
             [HYDRA] Gathered results in {tmpdir}/agg_results.csv
             """.format(
                 tmpdir=tmpdir
             )
         ),
+        result,
     )
     with open(tmpdir / "agg_results.csv") as f:
         assert len(f.readlines()) == 4
 
 
 def test_dirty_git_repo_error(tmpdir: Path) -> None:
     """Test for dirty git repo error."""
@@ -283,23 +283,23 @@
         # make the repo dirty
         with open("dummy.txt", "w") as f:
             f.write("Dummy has changed.")
         # run the test app.
         result, _err = run_python_script(cmd, raise_exception=False)
     assert _err == ""
     assert_regex_match(
-        result,
         dedent(
             """\
                 [HYDRA] Git sha: {sha}, dirty: True
                 [HYDRA] Repo is dirty, aborting
                 """.format(
                 sha=sha,
             )
         ),
+        result,
     )
 
 
 @pytest.mark.parametrize("multirun", [True, False])
 def test_resource_monitor(tmpdir: Path, multirun) -> None:
     """Test for resource monitor callback."""
 
@@ -312,25 +312,25 @@
         "hydra.hydra_logging.formatters.simple.format='[HYDRA] %(message)s'",
         "hydra.job_logging.formatters.simple.format='[JOB] %(message)s'",
     ]
     if multirun:
         cmd.insert(2, "--multirun")
     result, _err = run_python_script(cmd)
     assert_regex_match(
-        result,
         (HYDRA_LAUNCH_LOG if multirun else "")
         + dedent(
             """\
         [JOB] foo: bar
 
         [{logger}] Writing monitoring data to {tmpdir}/resource_monitoring.csv
         """.format(
                 tmpdir=tmpdir, logger="HYDRA" if multirun else "JOB"
             )
         ),
+        result,
     )
 
 
 def test_resource_monitor_disabled(tmpdir):
     cmd = [
         "tests/test_app/dummy_app.py",
         "--config-name=resource_monitor.yaml",
```

### Comparing `hydra-callbacks-0.3.0/tests/test_perflogger.py` & `hydra-callbacks-0.4.0/tests/test_perflogger.py`

 * *Files identical despite different names*

