# Comparing `tmp/qase-pytest-5.0.1.tar.gz` & `tmp/qase-pytest-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-pytest-5.0.1.tar", last modified: Thu Jun 15 15:49:56 2023, max compression
+gzip compressed data, was "qase-pytest-5.0.2.tar", last modified: Thu Aug  3 06:49:44 2023, max compression
```

## Comparing `qase-pytest-5.0.1.tar` & `qase-pytest-5.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.489991 qase-pytest-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/CONFIGURATION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-15 15:49:56.489991 qase-pytest-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/UPGRADE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.485991 qase-pytest-5.0.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/example/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-15 15:49:56.489991 qase-pytest-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.481991 qase-pytest-5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.485991 qase-pytest-5.0.1/src/qase_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.481991 qase-pytest-5.0.1/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.485991 qase-pytest-5.0.1/src/qaseio/pytest/
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/src/qaseio/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/src/qaseio/pytest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/src/qaseio/pytest/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/src/qaseio/pytest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.485991 qase-pytest-5.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:44.062254 qase-pytest-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/CONFIGURATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-08-03 06:49:44.062254 qase-pytest-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/UPGRADE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:44.058254 qase-pytest-5.0.2/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/example/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-03 06:49:44.062254 qase-pytest-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:44.058254 qase-pytest-5.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:44.062254 qase-pytest-5.0.2/src/qase_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-08-03 06:49:43.000000 qase-pytest-5.0.2/src/qase_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-03 06:49:44.000000 qase-pytest-5.0.2/src/qase_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:49:43.000000 qase-pytest-5.0.2/src/qase_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 06:49:43.000000 qase-pytest-5.0.2/src/qase_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 06:49:43.000000 qase-pytest-5.0.2/src/qase_pytest.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:49:43.000000 qase-pytest-5.0.2/src/qase_pytest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 06:49:43.000000 qase-pytest-5.0.2/src/qase_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 06:49:43.000000 qase-pytest-5.0.2/src/qase_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:44.058254 qase-pytest-5.0.2/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:44.062254 qase-pytest-5.0.2/src/qaseio/pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/src/qaseio/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/src/qaseio/pytest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/src/qaseio/pytest/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/src/qaseio/pytest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:44.062254 qase-pytest-5.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-03 06:49:40.000000 qase-pytest-5.0.2/tox.ini
```

### Comparing `qase-pytest-5.0.1/.coveragerc` & `qase-pytest-5.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/.gitignore` & `qase-pytest-5.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/.pre-commit-config.yaml` & `qase-pytest-5.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/CONFIGURATION.md` & `qase-pytest-5.0.2/CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/LICENSE.txt` & `qase-pytest-5.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/PKG-INFO` & `qase-pytest-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 5.0.1
+Version: 5.0.2
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qase-pytest-5.0.1/README.md` & `qase-pytest-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/UPGRADE.md` & `qase-pytest-5.0.2/UPGRADE.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/setup.cfg` & `qase-pytest-5.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Qase Team
 author-email = support@qase.io
 license = apache
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 platforms = any
-version = 5.0.1
+version = 5.0.2
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Pytest
 	Programming Language :: Python
 
 [options]
 zip_safe = False
```

### Comparing `qase-pytest-5.0.1/setup.py` & `qase-pytest-5.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
 import sys
 from pkg_resources import VersionConflict, require
 from setuptools import setup
 
-VERSION = "5.0.1"
+VERSION = "5.0.2"
 
 try:
     require("setuptools>=38.3")
 except VersionConflict:
     print("Error: version of setuptools is too old (<38.3)!")
     sys.exit(1)
```

### Comparing `qase-pytest-5.0.1/src/qase_pytest.egg-info/PKG-INFO` & `qase-pytest-5.0.2/src/qase_pytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 5.0.1
+Version: 5.0.2
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qase-pytest-5.0.1/src/qase_pytest.egg-info/SOURCES.txt` & `qase-pytest-5.0.2/src/qase_pytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/src/qaseio/pytest/__init__.py` & `qase-pytest-5.0.2/src/qaseio/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/src/qaseio/pytest/conftest.py` & `qase-pytest-5.0.2/src/qaseio/pytest/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,16 @@
                     from qaseio.commons import TestOpsPlanLoader
 
                     # Load test plan data from Qase TestOps
                     loader = TestOpsPlanLoader(
                         api_token=config.getoption("qase_testops_api_token"),
                         host=config.getoption("qase_testops_api_host", "qase.io"),
                     )
-                    execution_plan = loader.load(config.getoption("qase_testops_project"), config.getoption("qase_testops_plan_id"))
+                    execution_plan = loader.load(config.getoption("qase_testops_project"),
+                                                 int(config.getoption("qase_testops_plan_id")))
 
                 reporter = QaseTestOps(
                     api_token=config.getoption("qase_testops_api_token"),
                     project_code=config.getoption("qase_testops_project"),
                     run_id=config.getoption("qase_testops_run_id", None),
                     plan_id=config.getoption("qase_testops_plan_id", None),
                     complete_run=config.getoption("qase_testops_run_complete", False),
```

### Comparing `qase-pytest-5.0.1/src/qaseio/pytest/options.py` & `qase-pytest-5.0.2/src/qaseio/pytest/options.py`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.1/src/qaseio/pytest/plugin.py` & `qase-pytest-5.0.2/src/qaseio/pytest/plugin.py`

 * *Files identical despite different names*

