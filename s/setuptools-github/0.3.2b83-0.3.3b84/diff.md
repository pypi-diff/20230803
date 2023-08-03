# Comparing `tmp/setuptools-github-0.3.2b83.tar.gz` & `tmp/setuptools-github-0.3.3b84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.2b83.tar", last modified: Thu Aug  3 09:44:36 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.3b84.tar", last modified: Thu Aug  3 10:56:49 2023, max compression
```

## Comparing `setuptools-github-0.3.2b83.tar` & `setuptools-github-0.3.3b84.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:36.649708 setuptools-github-0.3.2b83/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-03 09:44:36.649708 setuptools-github-0.3.2b83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-08-03 09:44:36.000000 setuptools-github-0.3.2b83/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:44:36.649708 setuptools-github-0.3.2b83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:36.649708 setuptools-github-0.3.2b83/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-03 09:44:36.000000 setuptools-github-0.3.2b83/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 09:44:36.000000 setuptools-github-0.3.2b83/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:44:36.000000 setuptools-github-0.3.2b83/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 09:44:36.000000 setuptools-github-0.3.2b83/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 09:44:36.000000 setuptools-github-0.3.2b83/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 09:44:36.000000 setuptools-github-0.3.2b83/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:36.645708 setuptools-github-0.3.2b83/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:36.649708 setuptools-github-0.3.2b83/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 09:44:36.000000 setuptools-github-0.3.2b83/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:36.649708 setuptools-github-0.3.2b83/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-03 09:44:19.000000 setuptools-github-0.3.2b83/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.322698 setuptools-github-0.3.3b84/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-03 10:56:49.322698 setuptools-github-0.3.3b84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:56:49.322698 setuptools-github-0.3.3b84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.318699 setuptools-github-0.3.3b84/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.314699 setuptools-github-0.3.3b84/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.318699 setuptools-github-0.3.3b84/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 10:56:49.000000 setuptools-github-0.3.3b84/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:56:49.322698 setuptools-github-0.3.3b84/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-03 10:56:30.000000 setuptools-github-0.3.3b84/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.2b83/LICENSE` & `setuptools-github-0.3.3b84/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/PKG-INFO` & `setuptools-github-0.3.3b84/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.2b83
+Version: 0.3.3b84
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,127 +19,98 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749138038)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.2/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.2)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749808935)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
-aimed at delivering packages into [PyPI](https://pypi.org). Basically:
-- beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
-- tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
-
-This integrates well with the standard release logic in PyPI (see [example](https://pypi.org/project/setuptools-github/#history))
-
-> **NOTE** for a pyproject.tom / hatch enabled version of this, please use
-> [hatch-ci plugin](https://pypi.org/project/hatch-ci)
-
-**Table of Contents**
-
-- [Prerequisites](#prerequisites)
-  - [Install](#install-setuptools-github)
-  - [Add secrets](#add-secrets)
-- [Project setup](#project-setup)
-
-
-## Prerequisites
-
-We make few assumption in the rest of this document:
-
-- the project is hosted under https://www.github.com/<username>/<project-name>
-- the github project is named <**project-name**>
-- the main project branch is <**master**>
-- you have coverage.io account https://app.codecov.io/gh/<username>/<project-name>
-
-> **NOTE**: Please change **project-name**, **username** and **master** according to your project.
-
-### Install setuptools-github
-
-Install the package with:
-```bash
-pip install setuptools-github
- or
-conda install -c conda-forge setuptools-github
-```
-
-### Add secrets
-
-Github stores secrets for the <**project-name**> repository under:
-
-https://github.com/<username>/<project-name>/settings/secrets/actions
-
-These are the needed secrets for the PyPI index and codecov services:
-- TWINE_PASSWORD
-- TWINE_USERNAME
-- CODECOV_TOKEN
-
-## Project setup
-
-### Layout
+aimed at delivering packages into [PyPI](https://pypi.org) from a hosted project at
+[Github](https://www.gitgub.com). 
 We assume this layout:
 ```python
   project-name/
-  ├── .github
-  │   └── workflows
-  │       ├── beta.yml
-  │       ├── master.yml
-  │       └── tags.yml
+  ├── setup.py
   ├── pyproject.toml
+  ├── .github
+  │   └── workflows           <- workflow files for
+  │       ├── beta.yml             * beta/N.M.O branches
+  │       ├── master.yml           * master branch
+  │       └── tags.yml             * release/N.M.O tags
   ├── src
   │   └── project_name        <- project name
   │       └── __init__.py     <- initfile
   └── tests                   <- tests (pytest)
       ├── conftest.py
       └── requirements.txt    <- requirement file for tests
 ```
 
-- it is rooted under <**project-name**>/**src** directory
-- the python package is **project_name**
-- an **initfile** is stored under **project-name**/**src**/**project_name**/__init__.py
-- **tests** are stored under **project-name**/**tests**
-- a **requirements.txt* file for tests is under **project-name**/**tests**/requirements.txt
+> **NOTE** for a pyproject.toml / hatch enabled version of this, please use
+> [hatch-ci plugin](https://pypi.org/project/hatch-ci)
 
-> **NOTE**: You need to change these values to match your project
 
-### Setup the initfile
+#### install the package
+```bash
+pip install setuptools-github
+ or
+conda install -c conda-forge setuptools-github
+```
 
+#### put the initial version info in the initfile
 Create a new `src/project_name/__init__.py` file to store the package information:
 ```
 __version__ = "N.M.O"  # replace N, M and O with numerical values (eg. 0.0.0)
 __hash__ = ""  # leave this empty
 ```
 
-Fix the setup.py file:
+#### Fix the setup.py file
 ```
 from setuptools_github import tools
-initfile = pathlib.Path(__file__).parent / "project_name/__init__.py"
+
 setup(
   name="project-name",
   version=tools.update_version(initfile, os.getenv("GITHUB_DUMP")),
   ...
 ```
-Copy over the github workflow files:
+> **NOTE**: there's an advanced function `tools.process` that can update 
+> and process files like the readmes (see an example in [setup.py](https://raw.githubusercontent.com/cav71/setuptools-github/master/setup.py))
+
+#### Add the github workflow files
 - [github/workflows/master.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/master.yml)
 - [github/workflows/beta.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/beta.yml)
 - [github/workflows/tags.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/tags.yml)
 
-Most likely you might need to change `tests/requirements.txt` file.
+> **NOTE**: Most likely you might need to change `tests/requirements.txt` file.
 
+#### Add secrets
+In order to publish to codecov the coveragen info and to PyPI the wheels,
+you need to set the github secrets under:
+
+https://github.com/<span style="color: red">username</span>/<span style="color: green">project-name</span>/settings/secrets/actions
+
+These are the needed secrets for the PyPI index and codecov services:
+- TWINE_PASSWORD
+- TWINE_USERNAME
+- CODECOV_TOKEN
+
+---
 THAT IS ALL! Now when commit to the master branch, this will trigger the 
 github action to run tests and quality checks on the code 
-(see the Rationale section below).
+---
+
+## Working with branches
 
 ### Working with the master branch
 
 Every time there's a commit on the **master** branch, this will trigger
 the workflow under ./github/workflows/master.yml:
 - Runs mypy on src/
 - Runs ruff on src/
@@ -153,15 +124,15 @@
 ```python
 
 python -m setuptools_github.script make-beta src/project_name/__init__.py 
 or
 setuptools-github make-beta src/project_name/__init__.py
 ```
 
-Every commit on **beta/N.M.O** branch ASSUMING [Secrets](#add-secrets) have been set
+Every commit on **beta/N.M.O** branch if [Secrets](#add-secrets) have been set
 properly:
 - Runs mypy on src/
 - Runs ruff on src/
 - Run all tests under tests/
 - Run coverage on tests/
 - Send the coverage result into [coverage](https://coverage.io)
 - Create a new wheel package under dist/
```

### Comparing `setuptools-github-0.3.2b83/README.md` & `setuptools-github-0.3.3b84/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,126 +1,97 @@
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749138038)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.2/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.2)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749808935)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
-aimed at delivering packages into [PyPI](https://pypi.org). Basically:
-- beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
-- tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
-
-This integrates well with the standard release logic in PyPI (see [example](https://pypi.org/project/setuptools-github/#history))
-
-> **NOTE** for a pyproject.tom / hatch enabled version of this, please use
-> [hatch-ci plugin](https://pypi.org/project/hatch-ci)
-
-**Table of Contents**
-
-- [Prerequisites](#prerequisites)
-  - [Install](#install-setuptools-github)
-  - [Add secrets](#add-secrets)
-- [Project setup](#project-setup)
-
-
-## Prerequisites
-
-We make few assumption in the rest of this document:
-
-- the project is hosted under https://www.github.com/<username>/<project-name>
-- the github project is named <**project-name**>
-- the main project branch is <**master**>
-- you have coverage.io account https://app.codecov.io/gh/<username>/<project-name>
-
-> **NOTE**: Please change **project-name**, **username** and **master** according to your project.
-
-### Install setuptools-github
-
-Install the package with:
-```bash
-pip install setuptools-github
- or
-conda install -c conda-forge setuptools-github
-```
-
-### Add secrets
-
-Github stores secrets for the <**project-name**> repository under:
-
-https://github.com/<username>/<project-name>/settings/secrets/actions
-
-These are the needed secrets for the PyPI index and codecov services:
-- TWINE_PASSWORD
-- TWINE_USERNAME
-- CODECOV_TOKEN
-
-## Project setup
-
-### Layout
+aimed at delivering packages into [PyPI](https://pypi.org) from a hosted project at
+[Github](https://www.gitgub.com). 
 We assume this layout:
 ```python
   project-name/
-  ├── .github
-  │   └── workflows
-  │       ├── beta.yml
-  │       ├── master.yml
-  │       └── tags.yml
+  ├── setup.py
   ├── pyproject.toml
+  ├── .github
+  │   └── workflows           <- workflow files for
+  │       ├── beta.yml             * beta/N.M.O branches
+  │       ├── master.yml           * master branch
+  │       └── tags.yml             * release/N.M.O tags
   ├── src
   │   └── project_name        <- project name
   │       └── __init__.py     <- initfile
   └── tests                   <- tests (pytest)
       ├── conftest.py
       └── requirements.txt    <- requirement file for tests
 ```
 
-- it is rooted under <**project-name**>/**src** directory
-- the python package is **project_name**
-- an **initfile** is stored under **project-name**/**src**/**project_name**/__init__.py
-- **tests** are stored under **project-name**/**tests**
-- a **requirements.txt* file for tests is under **project-name**/**tests**/requirements.txt
+> **NOTE** for a pyproject.toml / hatch enabled version of this, please use
+> [hatch-ci plugin](https://pypi.org/project/hatch-ci)
 
-> **NOTE**: You need to change these values to match your project
 
-### Setup the initfile
+#### install the package
+```bash
+pip install setuptools-github
+ or
+conda install -c conda-forge setuptools-github
+```
 
+#### put the initial version info in the initfile
 Create a new `src/project_name/__init__.py` file to store the package information:
 ```
 __version__ = "N.M.O"  # replace N, M and O with numerical values (eg. 0.0.0)
 __hash__ = ""  # leave this empty
 ```
 
-Fix the setup.py file:
+#### Fix the setup.py file
 ```
 from setuptools_github import tools
-initfile = pathlib.Path(__file__).parent / "project_name/__init__.py"
+
 setup(
   name="project-name",
   version=tools.update_version(initfile, os.getenv("GITHUB_DUMP")),
   ...
 ```
-Copy over the github workflow files:
+> **NOTE**: there's an advanced function `tools.process` that can update 
+> and process files like the readmes (see an example in [setup.py](https://raw.githubusercontent.com/cav71/setuptools-github/master/setup.py))
+
+#### Add the github workflow files
 - [github/workflows/master.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/master.yml)
 - [github/workflows/beta.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/beta.yml)
 - [github/workflows/tags.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/tags.yml)
 
-Most likely you might need to change `tests/requirements.txt` file.
+> **NOTE**: Most likely you might need to change `tests/requirements.txt` file.
 
+#### Add secrets
+In order to publish to codecov the coveragen info and to PyPI the wheels,
+you need to set the github secrets under:
+
+https://github.com/<span style="color: red">username</span>/<span style="color: green">project-name</span>/settings/secrets/actions
+
+These are the needed secrets for the PyPI index and codecov services:
+- TWINE_PASSWORD
+- TWINE_USERNAME
+- CODECOV_TOKEN
+
+---
 THAT IS ALL! Now when commit to the master branch, this will trigger the 
 github action to run tests and quality checks on the code 
-(see the Rationale section below).
+---
+
+## Working with branches
 
 ### Working with the master branch
 
 Every time there's a commit on the **master** branch, this will trigger
 the workflow under ./github/workflows/master.yml:
 - Runs mypy on src/
 - Runs ruff on src/
@@ -134,15 +105,15 @@
 ```python
 
 python -m setuptools_github.script make-beta src/project_name/__init__.py 
 or
 setuptools-github make-beta src/project_name/__init__.py
 ```
 
-Every commit on **beta/N.M.O** branch ASSUMING [Secrets](#add-secrets) have been set
+Every commit on **beta/N.M.O** branch if [Secrets](#add-secrets) have been set
 properly:
 - Runs mypy on src/
 - Runs ruff on src/
 - Run all tests under tests/
 - Run coverage on tests/
 - Send the coverage result into [coverage](https://coverage.io)
 - Create a new wheel package under dist/
```

### Comparing `setuptools-github-0.3.2b83/pyproject.toml` & `setuptools-github-0.3.3b84/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/setup.py` & `setuptools-github-0.3.3b84/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,38 +3,48 @@
 import sys
 
 sys.path.insert(0, str(pathlib.Path(__file__).parent / "src"))
 from setuptools_github import tools  # noqa E402
 from setuptools import setup, find_namespace_packages  # noqa E402
 
 
-fixers = {
-    # for the github actions
-    "/actions/workflows/master.yml/badge.svg": "/actions/workflows/{{ ctx.workflow }}.yml/badge.svg",  # noqa: E501
-    "/actions/workflows/master.yml": "/actions/runs/{{ ctx.runid }}",
-    # for the codecov part
-    "/tree/master/graph/badge.svg?token=SIUMZ7MT5T": "/tree/{{ ctx.branch|urlquote }}/graph/badge.svg?token=SIUMZ7MT5T",  # noqa: E501
-    "/tree/master": "/tree/{{ ctx.branch|urlquote }}",
-}
-initfile = pathlib.Path(__file__).parent / "src/setuptools_github/__init__.py"
-readme = pathlib.Path(__file__).parent / "README.md"
-version = tools.process(initfile, os.getenv("GITHUB_DUMP"), readme, fixers=fixers)[
-    "version"
-]
+PROOT = pathlib.Path(__file__).parent
+
+
+GDATA = tools.process(
+    # initfile containing the __version__ / __hash__ module variables
+    # (they will be update during build)
+    initfile=PROOT / "src/setuptools_github/__init__.py",
+    # this is the github environ (the output of ${{ toJson(github) }})
+    # (see .github/workflows/master.yml)
+    github_dump=os.getenv("GITHUB_DUMP"),
+    # a list of files, processed using jinja2
+    paths=[
+        PROOT / "README.md",
+    ],
+    # fixed simply text replace {old: new} in every paths content
+    fixers={
+        # for the github actions
+        "/actions/workflows/master.yml/badge.svg": "/actions/workflows/{{ ctx.workflow }}.yml/badge.svg",  # noqa: E501
+        "/actions/workflows/master.yml": "/actions/runs/{{ ctx.runid }}",
+        # for the codecov part
+        "/tree/master/graph/badge.svg?token=SIUMZ7MT5T": "/tree/{{ ctx.branch|urlquote }}/graph/badge.svg?token=SIUMZ7MT5T",  # noqa: E501
+        "/tree/master": "/tree/{{ ctx.branch|urlquote }}",
+    },
+)
 
-packages = find_namespace_packages(where="src")
 
 setup(
     name="setuptools-github",
-    version=version,
+    version=GDATA["version"],
     url="https://github.com/cav71/setuptools-github",
-    packages=packages,
+    packages=find_namespace_packages(where="src"),
     package_dir={"setuptools_github": "src/setuptools_github"},
     description="supports github releases",
-    long_description=readme.read_text(),
+    long_description=(PROOT / "README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=[
         "setuptools",
         "typing-extensions",
         "jinja2",
     ],
     entry_points={
```

### Comparing `setuptools-github-0.3.2b83/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.3b84/setuptools_github.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.2b83
+Version: 0.3.3b84
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,127 +19,98 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749138038)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.2/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.2)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5749808935)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.3)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
-aimed at delivering packages into [PyPI](https://pypi.org). Basically:
-- beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
-- tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
-
-This integrates well with the standard release logic in PyPI (see [example](https://pypi.org/project/setuptools-github/#history))
-
-> **NOTE** for a pyproject.tom / hatch enabled version of this, please use
-> [hatch-ci plugin](https://pypi.org/project/hatch-ci)
-
-**Table of Contents**
-
-- [Prerequisites](#prerequisites)
-  - [Install](#install-setuptools-github)
-  - [Add secrets](#add-secrets)
-- [Project setup](#project-setup)
-
-
-## Prerequisites
-
-We make few assumption in the rest of this document:
-
-- the project is hosted under https://www.github.com/<username>/<project-name>
-- the github project is named <**project-name**>
-- the main project branch is <**master**>
-- you have coverage.io account https://app.codecov.io/gh/<username>/<project-name>
-
-> **NOTE**: Please change **project-name**, **username** and **master** according to your project.
-
-### Install setuptools-github
-
-Install the package with:
-```bash
-pip install setuptools-github
- or
-conda install -c conda-forge setuptools-github
-```
-
-### Add secrets
-
-Github stores secrets for the <**project-name**> repository under:
-
-https://github.com/<username>/<project-name>/settings/secrets/actions
-
-These are the needed secrets for the PyPI index and codecov services:
-- TWINE_PASSWORD
-- TWINE_USERNAME
-- CODECOV_TOKEN
-
-## Project setup
-
-### Layout
+aimed at delivering packages into [PyPI](https://pypi.org) from a hosted project at
+[Github](https://www.gitgub.com). 
 We assume this layout:
 ```python
   project-name/
-  ├── .github
-  │   └── workflows
-  │       ├── beta.yml
-  │       ├── master.yml
-  │       └── tags.yml
+  ├── setup.py
   ├── pyproject.toml
+  ├── .github
+  │   └── workflows           <- workflow files for
+  │       ├── beta.yml             * beta/N.M.O branches
+  │       ├── master.yml           * master branch
+  │       └── tags.yml             * release/N.M.O tags
   ├── src
   │   └── project_name        <- project name
   │       └── __init__.py     <- initfile
   └── tests                   <- tests (pytest)
       ├── conftest.py
       └── requirements.txt    <- requirement file for tests
 ```
 
-- it is rooted under <**project-name**>/**src** directory
-- the python package is **project_name**
-- an **initfile** is stored under **project-name**/**src**/**project_name**/__init__.py
-- **tests** are stored under **project-name**/**tests**
-- a **requirements.txt* file for tests is under **project-name**/**tests**/requirements.txt
+> **NOTE** for a pyproject.toml / hatch enabled version of this, please use
+> [hatch-ci plugin](https://pypi.org/project/hatch-ci)
 
-> **NOTE**: You need to change these values to match your project
 
-### Setup the initfile
+#### install the package
+```bash
+pip install setuptools-github
+ or
+conda install -c conda-forge setuptools-github
+```
 
+#### put the initial version info in the initfile
 Create a new `src/project_name/__init__.py` file to store the package information:
 ```
 __version__ = "N.M.O"  # replace N, M and O with numerical values (eg. 0.0.0)
 __hash__ = ""  # leave this empty
 ```
 
-Fix the setup.py file:
+#### Fix the setup.py file
 ```
 from setuptools_github import tools
-initfile = pathlib.Path(__file__).parent / "project_name/__init__.py"
+
 setup(
   name="project-name",
   version=tools.update_version(initfile, os.getenv("GITHUB_DUMP")),
   ...
 ```
-Copy over the github workflow files:
+> **NOTE**: there's an advanced function `tools.process` that can update 
+> and process files like the readmes (see an example in [setup.py](https://raw.githubusercontent.com/cav71/setuptools-github/master/setup.py))
+
+#### Add the github workflow files
 - [github/workflows/master.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/master.yml)
 - [github/workflows/beta.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/beta.yml)
 - [github/workflows/tags.yml](https://github.com/cav71/setuptools-github/blob/master/.github/workflows/tags.yml)
 
-Most likely you might need to change `tests/requirements.txt` file.
+> **NOTE**: Most likely you might need to change `tests/requirements.txt` file.
 
+#### Add secrets
+In order to publish to codecov the coveragen info and to PyPI the wheels,
+you need to set the github secrets under:
+
+https://github.com/<span style="color: red">username</span>/<span style="color: green">project-name</span>/settings/secrets/actions
+
+These are the needed secrets for the PyPI index and codecov services:
+- TWINE_PASSWORD
+- TWINE_USERNAME
+- CODECOV_TOKEN
+
+---
 THAT IS ALL! Now when commit to the master branch, this will trigger the 
 github action to run tests and quality checks on the code 
-(see the Rationale section below).
+---
+
+## Working with branches
 
 ### Working with the master branch
 
 Every time there's a commit on the **master** branch, this will trigger
 the workflow under ./github/workflows/master.yml:
 - Runs mypy on src/
 - Runs ruff on src/
@@ -153,15 +124,15 @@
 ```python
 
 python -m setuptools_github.script make-beta src/project_name/__init__.py 
 or
 setuptools-github make-beta src/project_name/__init__.py
 ```
 
-Every commit on **beta/N.M.O** branch ASSUMING [Secrets](#add-secrets) have been set
+Every commit on **beta/N.M.O** branch if [Secrets](#add-secrets) have been set
 properly:
 - Runs mypy on src/
 - Runs ruff on src/
 - Run all tests under tests/
 - Run coverage on tests/
 - Send the coverage result into [coverage](https://coverage.io)
 - Create a new wheel package under dist/
```

### Comparing `setuptools-github-0.3.2b83/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.3b84/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/src/setuptools_github/checks.py` & `setuptools-github-0.3.3b84/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/src/setuptools_github/cli.py` & `setuptools-github-0.3.3b84/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/src/setuptools_github/scm.py` & `setuptools-github-0.3.3b84/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/src/setuptools_github/script.py` & `setuptools-github-0.3.3b84/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/src/setuptools_github/tools.py` & `setuptools-github-0.3.3b84/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/tests/conftest.py` & `setuptools-github-0.3.3b84/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/tests/test_checks.py` & `setuptools-github-0.3.3b84/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/tests/test_cli.py` & `setuptools-github-0.3.3b84/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/tests/test_conftest.py` & `setuptools-github-0.3.3b84/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/tests/test_scm.py` & `setuptools-github-0.3.3b84/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/tests/test_script.py` & `setuptools-github-0.3.3b84/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.2b83/tests/test_tools.py` & `setuptools-github-0.3.3b84/tests/test_tools.py`

 * *Files identical despite different names*

