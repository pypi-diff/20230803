# Comparing `tmp/sqlalchemy-state-machine-1.8.0.tar.gz` & `tmp/sqlalchemy-state-machine-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-state-machine-1.8.0.tar", last modified: Mon Jul 26 09:39:45 2021, max compression
+gzip compressed data, was "sqlalchemy-state-machine-1.9.0.tar", last modified: Thu Jan 19 08:51:51 2023, max compression
```

## Comparing `sqlalchemy-state-machine-1.8.0.tar` & `sqlalchemy-state-machine-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:39:45.011368 sqlalchemy-state-machine-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-07-26 09:39:36.000000 sqlalchemy-state-machine-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-07-26 09:39:36.000000 sqlalchemy-state-machine-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2021-07-26 09:39:45.011368 sqlalchemy-state-machine-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2021-07-26 09:39:36.000000 sqlalchemy-state-machine-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      433 2021-07-26 09:39:36.000000 sqlalchemy-state-machine-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-26 09:39:45.011368 sqlalchemy-state-machine-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-07-26 09:39:36.000000 sqlalchemy-state-machine-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:39:45.007370 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-07-26 09:39:36.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-07-26 09:39:36.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine/state_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-07-26 09:39:36.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:39:45.011368 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2021-07-26 09:39:44.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      452 2021-07-26 09:39:44.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:39:44.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:39:44.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-07-26 09:39:44.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-07-26 09:39:44.000000 sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 08:51:51.199470 sqlalchemy-state-machine-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-01-19 08:51:38.000000 sqlalchemy-state-machine-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-19 08:51:38.000000 sqlalchemy-state-machine-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-01-19 08:51:51.195470 sqlalchemy-state-machine-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-01-19 08:51:38.000000 sqlalchemy-state-machine-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-19 08:51:38.000000 sqlalchemy-state-machine-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 08:51:51.199470 sqlalchemy-state-machine-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-01-19 08:51:38.000000 sqlalchemy-state-machine-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 08:51:51.195470 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-19 08:51:38.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-01-19 08:51:38.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine/state_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-19 08:51:38.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 08:51:51.195470 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-01-19 08:51:50.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-19 08:51:51.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 08:51:50.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 08:51:50.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-19 08:51:50.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-19 08:51:50.000000 sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine.egg-info/top_level.txt
```

### Comparing `sqlalchemy-state-machine-1.8.0/LICENSE` & `sqlalchemy-state-machine-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-state-machine-1.8.0/PKG-INFO` & `sqlalchemy-state-machine-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-state-machine
-Version: 1.8.0
+Version: 1.9.0
 Summary: Helper for add transitions functionality in sqlalchemy
 Home-page: https://github.com/bigbag/sqlalchemy-state-machine
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
```

### Comparing `sqlalchemy-state-machine-1.8.0/README.md` & `sqlalchemy-state-machine-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-state-machine-1.8.0/setup.py` & `sqlalchemy-state-machine-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,13 +37,13 @@
     maintainer="Pavel Liashkov",
     maintainer_email="pavel.liashkov@protonmail.com",
     download_url="https://pypi.python.org/pypi/sqlalchemy-state-machine",
     url="https://github.com/bigbag/sqlalchemy-state-machine",
     platforms=["POSIX"],
     classifiers=CLASSIFIERS,
     python_requires=">=3.7",
-    install_requires=["SQLAlchemy>=1.4,<1.5", "transitions>=0.8,<0.9"],
+    install_requires=["SQLAlchemy>=1.4,<1.5", "transitions>=0.8,<0.10"],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     test_suite="",
 )
```

### Comparing `sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine/state_mixin.py` & `sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine/state_mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-state-machine-1.8.0/sqlalchemy_state_machine.egg-info/PKG-INFO` & `sqlalchemy-state-machine-1.9.0/sqlalchemy_state_machine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-state-machine
-Version: 1.8.0
+Version: 1.9.0
 Summary: Helper for add transitions functionality in sqlalchemy
 Home-page: https://github.com/bigbag/sqlalchemy-state-machine
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
```

