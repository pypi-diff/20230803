# Comparing `tmp/setuptools-github-0.3.3b84.tar.gz` & `tmp/setuptools-github-0.3.3b85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.3b84.tar", last modified: Thu Aug  3 10:56:49 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.3b85.tar", last modified: Thu Aug  3 11:25:33 2023, max compression
```

## Comparing `setuptools-github-0.3.3b84.tar` & `setuptools-github-0.3.3b85.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.322698 setuptools-github-0.3.3b84/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-03 10:56:49.322698 setuptools-github-0.3.3b84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:56:49.322698 setuptools-github-0.3.3b84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.318699 setuptools-github-0.3.3b84/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.314699 setuptools-github-0.3.3b84/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.318699 setuptools-github-0.3.3b84/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.322698 setuptools-github-0.3.3b84/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:25:33.802705 setuptools-github-0.3.3b85/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-03 11:25:33.802705 setuptools-github-0.3.3b85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-03 11:25:33.000000 setuptools-github-0.3.3b85/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:25:33.802705 setuptools-github-0.3.3b85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:25:33.802705 setuptools-github-0.3.3b85/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-03 11:25:33.000000 setuptools-github-0.3.3b85/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 11:25:33.000000 setuptools-github-0.3.3b85/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:25:33.000000 setuptools-github-0.3.3b85/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 11:25:33.000000 setuptools-github-0.3.3b85/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 11:25:33.000000 setuptools-github-0.3.3b85/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 11:25:33.000000 setuptools-github-0.3.3b85/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:25:33.798705 setuptools-github-0.3.3b85/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:25:33.802705 setuptools-github-0.3.3b85/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 11:25:33.000000 setuptools-github-0.3.3b85/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:25:33.802705 setuptools-github-0.3.3b85/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-03 11:25:13.000000 setuptools-github-0.3.3b85/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.3b84/LICENSE` & `setuptools-github-0.3.3b85/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/PKG-INFO` & `setuptools-github-0.3.3b85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.3b84
+Version: 0.3.3b85
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749808935)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5750078929)
 [![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

### Comparing `setuptools-github-0.3.3b84/README.md` & `setuptools-github-0.3.3b85/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749808935)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5750078929)
 [![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

### Comparing `setuptools-github-0.3.3b84/pyproject.toml` & `setuptools-github-0.3.3b85/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/setup.py` & `setuptools-github-0.3.3b85/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.3b85/setuptools_github.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.3b84
+Version: 0.3.3b85
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749808935)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5750078929)
 [![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

### Comparing `setuptools-github-0.3.3b84/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.3b85/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/src/setuptools_github/checks.py` & `setuptools-github-0.3.3b85/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/src/setuptools_github/cli.py` & `setuptools-github-0.3.3b85/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/src/setuptools_github/scm.py` & `setuptools-github-0.3.3b85/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/src/setuptools_github/script.py` & `setuptools-github-0.3.3b85/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/src/setuptools_github/tools.py` & `setuptools-github-0.3.3b85/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/tests/conftest.py` & `setuptools-github-0.3.3b85/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/tests/test_checks.py` & `setuptools-github-0.3.3b85/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/tests/test_cli.py` & `setuptools-github-0.3.3b85/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/tests/test_conftest.py` & `setuptools-github-0.3.3b85/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/tests/test_scm.py` & `setuptools-github-0.3.3b85/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/tests/test_script.py` & `setuptools-github-0.3.3b85/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.3b84/tests/test_tools.py` & `setuptools-github-0.3.3b85/tests/test_tools.py`

 * *Files identical despite different names*

