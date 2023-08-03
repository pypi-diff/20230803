# Comparing `tmp/setuptools-github-0.3.5b89.tar.gz` & `tmp/setuptools-github-0.3.6b90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.5b89.tar", last modified: Thu Aug  3 14:17:00 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.6b90.tar", last modified: Thu Aug  3 14:47:36 2023, max compression
```

## Comparing `setuptools-github-0.3.5b89.tar` & `setuptools-github-0.3.6b90.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:17:00.759405 setuptools-github-0.3.5b89/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-08-03 14:17:00.759405 setuptools-github-0.3.5b89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-08-03 14:17:00.000000 setuptools-github-0.3.5b89/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:17:00.759405 setuptools-github-0.3.5b89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:17:00.755405 setuptools-github-0.3.5b89/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-08-03 14:17:00.000000 setuptools-github-0.3.5b89/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 14:17:00.000000 setuptools-github-0.3.5b89/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:17:00.000000 setuptools-github-0.3.5b89/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 14:17:00.000000 setuptools-github-0.3.5b89/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 14:17:00.000000 setuptools-github-0.3.5b89/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 14:17:00.000000 setuptools-github-0.3.5b89/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:17:00.755405 setuptools-github-0.3.5b89/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:17:00.759405 setuptools-github-0.3.5b89/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 14:17:00.000000 setuptools-github-0.3.5b89/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:17:00.759405 setuptools-github-0.3.5b89/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-03 14:16:40.000000 setuptools-github-0.3.5b89/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.243119 setuptools-github-0.3.6b90/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-08-03 14:47:36.243119 setuptools-github-0.3.6b90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:47:36.243119 setuptools-github-0.3.6b90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.239119 setuptools-github-0.3.6b90/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.239119 setuptools-github-0.3.6b90/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.239119 setuptools-github-0.3.6b90/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 14:47:36.000000 setuptools-github-0.3.6b90/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:47:36.243119 setuptools-github-0.3.6b90/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-03 14:47:16.000000 setuptools-github-0.3.6b90/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.5b89/LICENSE` & `setuptools-github-0.3.6b90/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/PKG-INFO` & `setuptools-github-0.3.6b90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.5b89
+Version: 0.3.6b90
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5751859971)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.5/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.5)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5752209245)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.5b89/README.md` & `setuptools-github-0.3.6b90/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5751859971)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.5/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.5)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5752209245)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.5b89/pyproject.toml` & `setuptools-github-0.3.6b90/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/setup.py` & `setuptools-github-0.3.6b90/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.6b90/setuptools_github.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.5b89
+Version: 0.3.6b90
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5751859971)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.5/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.5)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5752209245)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.6)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.5b89/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.6b90/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/src/setuptools_github/checks.py` & `setuptools-github-0.3.6b90/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/src/setuptools_github/cli.py` & `setuptools-github-0.3.6b90/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/src/setuptools_github/scm.py` & `setuptools-github-0.3.6b90/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/src/setuptools_github/script.py` & `setuptools-github-0.3.6b90/src/setuptools_github/script.py`

 * *Files 10% similar despite different names*

```diff
@@ -123,19 +123,23 @@
                 f"git checkout beta/{version}",
             )
             return
         local = match.group("beta")
         if local != version:
             options.error(f"wrong version file {version=} != {local}")
 
+        # create an empty commit to mark the release
+        options.repo(["commit", "--allow-empty", "-m", f"released {version}"])
+
         # tag
         options.repo(["tag", "-a", f"release/{version}", "-m", f"released {version}"])
 
-        # switch to master
+        # switch to master (and incorporate the commit message)
         options.repo(["checkout", master])
+        options.repo(["merge", f"beta/{version}"])
 
         # bump version
         new_version = tools.bump_version(version, options.mode)
         tools.set_module_var(options.initfile, "__version__", new_version)
 
         # commit
         options.repo.commit(
```

### Comparing `setuptools-github-0.3.5b89/src/setuptools_github/tools.py` & `setuptools-github-0.3.6b90/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/tests/conftest.py` & `setuptools-github-0.3.6b90/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/tests/test_checks.py` & `setuptools-github-0.3.6b90/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/tests/test_cli.py` & `setuptools-github-0.3.6b90/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/tests/test_conftest.py` & `setuptools-github-0.3.6b90/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/tests/test_scm.py` & `setuptools-github-0.3.6b90/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/tests/test_script.py` & `setuptools-github-0.3.6b90/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.5b89/tests/test_tools.py` & `setuptools-github-0.3.6b90/tests/test_tools.py`

 * *Files identical despite different names*

