# Comparing `tmp/kotsu-0.3.2.tar.gz` & `tmp/kotsu-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kotsu-0.3.2.tar", last modified: Sun Sep 11 12:01:20 2022, max compression
+gzip compressed data, was "kotsu-0.3.3.tar", last modified: Thu Aug  3 11:33:37 2023, max compression
```

## Comparing `kotsu-0.3.2.tar` & `kotsu-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 12:01:20.400941 kotsu-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-09-11 12:00:43.000000 kotsu-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-11 12:00:43.000000 kotsu-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5985 2022-09-11 12:01:20.400941 kotsu-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4557 2022-09-11 12:00:43.000000 kotsu-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 12:01:20.404941 kotsu-0.3.2/kotsu/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-11 12:00:43.000000 kotsu-0.3.2/kotsu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-09-11 12:01:20.404941 kotsu-0.3.2/kotsu/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-09-11 12:00:43.000000 kotsu-0.3.2/kotsu/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     5773 2022-09-11 12:00:43.000000 kotsu-0.3.2/kotsu/registration.py
--rw-r--r--   0 runner    (1001) docker     (121)     6487 2022-09-11 12:00:43.000000 kotsu-0.3.2/kotsu/run.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-09-11 12:00:43.000000 kotsu-0.3.2/kotsu/store.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-09-11 12:00:43.000000 kotsu-0.3.2/kotsu/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 12:01:20.400941 kotsu-0.3.2/kotsu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5985 2022-09-11 12:01:20.000000 kotsu-0.3.2/kotsu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-11 12:01:20.000000 kotsu-0.3.2/kotsu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 12:01:20.000000 kotsu-0.3.2/kotsu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-11 12:01:20.000000 kotsu-0.3.2/kotsu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-11 12:01:20.000000 kotsu-0.3.2/kotsu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-11 12:00:43.000000 kotsu-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-09-11 12:01:20.400941 kotsu-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-09-11 12:00:43.000000 kotsu-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 12:01:20.400941 kotsu-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-11 12:00:43.000000 kotsu-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-09-11 12:00:43.000000 kotsu-0.3.2/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-09-11 12:00:43.000000 kotsu-0.3.2/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (121)     7986 2022-09-11 12:00:43.000000 kotsu-0.3.2/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-09-11 12:00:43.000000 kotsu-0.3.2/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (121)    69935 2022-09-11 12:00:43.000000 kotsu-0.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:33:37.020021 kotsu-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-03 11:32:49.000000 kotsu-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 11:32:49.000000 kotsu-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-03 11:33:37.020021 kotsu-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-08-03 11:32:49.000000 kotsu-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:33:37.020021 kotsu-0.3.3/kotsu/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-03 11:32:49.000000 kotsu-0.3.3/kotsu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-03 11:33:37.020021 kotsu-0.3.3/kotsu/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-03 11:32:49.000000 kotsu-0.3.3/kotsu/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-08-03 11:32:49.000000 kotsu-0.3.3/kotsu/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-08-03 11:32:49.000000 kotsu-0.3.3/kotsu/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-03 11:32:49.000000 kotsu-0.3.3/kotsu/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-03 11:32:49.000000 kotsu-0.3.3/kotsu/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:33:37.016021 kotsu-0.3.3/kotsu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-03 11:33:36.000000 kotsu-0.3.3/kotsu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-03 11:33:36.000000 kotsu-0.3.3/kotsu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:33:36.000000 kotsu-0.3.3/kotsu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 11:33:36.000000 kotsu-0.3.3/kotsu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 11:33:36.000000 kotsu-0.3.3/kotsu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-03 11:32:49.000000 kotsu-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-03 11:33:37.020021 kotsu-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-03 11:32:49.000000 kotsu-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:33:37.020021 kotsu-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:32:49.000000 kotsu-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-03 11:32:49.000000 kotsu-0.3.3/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-08-03 11:32:49.000000 kotsu-0.3.3/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-08-03 11:32:49.000000 kotsu-0.3.3/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 11:32:49.000000 kotsu-0.3.3/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69935 2023-08-03 11:32:49.000000 kotsu-0.3.3/versioneer.py
```

### Comparing `kotsu-0.3.2/LICENSE.txt` & `kotsu-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/PKG-INFO` & `kotsu-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kotsu
-Version: 0.3.2
+Version: 0.3.3
 Summary: Lightweight framework for structured and repeatable model validation
 Home-page: https://github.com/datavaluepeople/kotsu
 Author: datavaluepeople
 Author-email: opensource@datavaluepeople.com
 License: MIT
 Description: # kotsu: lightweight framework for structuring model validation
```

### Comparing `kotsu-0.3.2/README.md` & `kotsu-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/kotsu/registration.py` & `kotsu-0.3.3/kotsu/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     """
 
     def __init__(self):
         self.entity_specs = {}
 
     def make(self, id: str, **kwargs) -> Entity:
         """Instantiate an instance of an entity of the given ID."""
-        logging.info(f"Making new entity: {id} ({kwargs})")
+        logger.info(f"Making new entity: {id} ({kwargs})")
         try:
             return self.entity_specs[id].make(**kwargs)
         except KeyError:
             raise KeyError(f"No registered entity with ID {id}")
 
     def all(self):
         """Return all the entitys in the registry."""
```

### Comparing `kotsu-0.3.2/kotsu/run.py` & `kotsu-0.3.3/kotsu/run.py`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/kotsu/typing.py` & `kotsu-0.3.3/kotsu/typing.py`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/kotsu.egg-info/PKG-INFO` & `kotsu-0.3.3/kotsu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kotsu
-Version: 0.3.2
+Version: 0.3.3
 Summary: Lightweight framework for structured and repeatable model validation
 Home-page: https://github.com/datavaluepeople/kotsu
 Author: datavaluepeople
 Author-email: opensource@datavaluepeople.com
 License: MIT
 Description: # kotsu: lightweight framework for structuring model validation
```

### Comparing `kotsu-0.3.2/setup.cfg` & `kotsu-0.3.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 no_lines_before = KOTSU_TYPING
 sections = TYPING, KOTSU_TYPING, STDLIB, THIRDPARTY, FIRSTPARTY, LOCALFOLDER
 
 [flake8]
 exclude = .git,logs,.*/*.py,build/*.py,*.egg-info,versioneer.py,kotsu/_version.py
 max-line-length = 99
 max-complexity = 10
-ignore = W503, W391 #F405 - start with no ignored errors and add as required
+ignore = W503, W391
 
 [mypy]
 incremental = True
 warn_unused_configs = True
 warn_unused_ignores = True
 check_untyped_defs = True
 warn_redundant_casts = True
```

### Comparing `kotsu-0.3.2/setup.py` & `kotsu-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/tests/test_end_to_end.py` & `kotsu-0.3.3/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/tests/test_registration.py` & `kotsu-0.3.3/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/tests/test_run.py` & `kotsu-0.3.3/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/tests/test_store.py` & `kotsu-0.3.3/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `kotsu-0.3.2/versioneer.py` & `kotsu-0.3.3/versioneer.py`

 * *Files identical despite different names*

