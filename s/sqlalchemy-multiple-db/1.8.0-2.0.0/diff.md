# Comparing `tmp/sqlalchemy-multiple-db-1.8.0.tar.gz` & `tmp/sqlalchemy-multiple-db-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-multiple-db-1.8.0.tar", last modified: Mon Jul 26 09:41:13 2021, max compression
+gzip compressed data, was "sqlalchemy-multiple-db-2.0.0.tar", last modified: Thu Aug  3 10:50:07 2023, max compression
```

## Comparing `sqlalchemy-multiple-db-1.8.0.tar` & `sqlalchemy-multiple-db-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:41:13.816032 sqlalchemy-multiple-db-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-07-26 09:41:03.000000 sqlalchemy-multiple-db-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-07-26 09:41:03.000000 sqlalchemy-multiple-db-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2021-07-26 09:41:13.816032 sqlalchemy-multiple-db-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2021-07-26 09:41:03.000000 sqlalchemy-multiple-db-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      431 2021-07-26 09:41:03.000000 sqlalchemy-multiple-db-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-26 09:41:13.816032 sqlalchemy-multiple-db-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2021-07-26 09:41:03.000000 sqlalchemy-multiple-db-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:41:13.812032 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-07-26 09:41:03.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2021-07-26 09:41:03.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-07-26 09:41:03.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:41:13.816032 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2021-07-26 09:41:13.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      429 2021-07-26 09:41:13.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:41:13.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:41:13.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-07-26 09:41:13.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-07-26 09:41:13.000000 sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:50:07.108774 sqlalchemy-multiple-db-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-03 10:49:45.000000 sqlalchemy-multiple-db-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 10:49:45.000000 sqlalchemy-multiple-db-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-03 10:50:07.108774 sqlalchemy-multiple-db-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-03 10:49:45.000000 sqlalchemy-multiple-db-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-03 10:49:45.000000 sqlalchemy-multiple-db-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:50:07.108774 sqlalchemy-multiple-db-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-03 10:49:45.000000 sqlalchemy-multiple-db-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:50:07.104774 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-03 10:49:45.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-03 10:49:45.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 10:49:45.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:50:07.108774 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-03 10:50:06.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-03 10:50:07.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:50:06.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:50:06.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 10:50:06.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 10:50:06.000000 sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db.egg-info/top_level.txt
```

### Comparing `sqlalchemy-multiple-db-1.8.0/LICENSE` & `sqlalchemy-multiple-db-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-multiple-db-1.8.0/PKG-INFO` & `sqlalchemy-multiple-db-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,49 @@
-Metadata-Version: 2.1
-Name: sqlalchemy-multiple-db
-Version: 1.8.0
-Summary: Helper for easily connect to multiple databases.
-Home-page: https://github.com/bigbag/sqlalchemy-multiple-db
-Author: Pavel Liashkov
-Author-email: pavel.liashkov@protonmail.com
-Maintainer: Pavel Liashkov
-Maintainer-email: pavel.liashkov@protonmail.com
-License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/sqlalchemy-multiple-db
-Description: # sqlalchemy-multiple-db
-        
-        [![CI](https://github.com/bigbag/sqlalchemy-multiple-db/workflows/CI/badge.svg)](https://github.com/bigbag/sqlalchemy-multiple-db/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/sqlalchemy-multiple-db/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/sqlalchemy-multiple-db)
-        [![pypi](https://img.shields.io/pypi/v/sqlalchemy-multiple-db.svg)](https://pypi.python.org/pypi/sqlalchemy-multiple-db)
-        [![downloads](https://img.shields.io/pypi/dm/sqlalchemy-multiple-db.svg)](https://pypistats.org/packages/sqlalchemy-multiple-db)
-        [![versions](https://img.shields.io/pypi/pyversions/sqlalchemy-multiple-db.svg)](https://github.com/bigbag/sqlalchemy-multiple-db)
-        [![license](https://img.shields.io/github/license/bigbag/sqlalchemy-multiple-db.svg)](https://github.com/bigbag/sqlalchemy-multiple-db/blob/master/LICENSE)
-        
-        **sqlalchemy-multiple-db** helper for easily connect to multiple databases.
-        
-        
-        ## Installation
-        
-        sqlalchemy-multiple-db is available on PyPI.
-        Use pip to install:
-        
-            $ pip install sqlalchemy-multiple-db
-        
-        ## Basic Usage
-        ```py
-        from sqlalchemy_multiple_db import DBConfig, db
-        
-        db.setup({"test1": DBConfig(dsn="sqlite://"), "test2": DBConfig(dsn="sqlite://")})
-        
-        with db.session_scope("test1") as session:
-            assert session.execute("select 1;")
-        
-        with db.session_scope("test2") as session:
-            assert session.execute("select 1;")
-        
-        db.shutdown()
-        
-        db.setup(DBConfig(dsn="sqlite://"))
-        
-        with db.session_scope() as session:
-            assert session.execute("select 1;")
-        
-        db.shutdown()
-        
-        ```
-        
-        ## License
-        
-        sqlalchemy-multiple-db is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/sqlalchemy-multiple-db/security/policy).
-        
-Platform: POSIX
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# sqlalchemy-multiple-db
+
+[![CI](https://github.com/bigbag/sqlalchemy-multiple-db/workflows/CI/badge.svg)](https://github.com/bigbag/sqlalchemy-multiple-db/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/sqlalchemy-multiple-db/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/sqlalchemy-multiple-db)
+[![pypi](https://img.shields.io/pypi/v/sqlalchemy-multiple-db.svg)](https://pypi.python.org/pypi/sqlalchemy-multiple-db)
+[![downloads](https://img.shields.io/pypi/dm/sqlalchemy-multiple-db.svg)](https://pypistats.org/packages/sqlalchemy-multiple-db)
+[![versions](https://img.shields.io/pypi/pyversions/sqlalchemy-multiple-db.svg)](https://github.com/bigbag/sqlalchemy-multiple-db)
+[![license](https://img.shields.io/github/license/bigbag/sqlalchemy-multiple-db.svg)](https://github.com/bigbag/sqlalchemy-multiple-db/blob/master/LICENSE)
+
+**sqlalchemy-multiple-db** helper for easily connect to multiple databases.
+
+
+## Installation
+
+sqlalchemy-multiple-db is available on PyPI.
+Use pip to install:
+
+    $ pip install sqlalchemy-multiple-db
+
+## Basic Usage
+```py
+from sqlalchemy_multiple_db import DBConfig, db
+
+db.setup({"test1": DBConfig(dsn="sqlite://"), "test2": DBConfig(dsn="sqlite://")})
+
+with db.session_scope("test1") as session:
+    assert session.execute("select 1;")
+
+with db.session_scope("test2") as session:
+    assert session.execute("select 1;")
+
+db.shutdown()
+
+db.setup(DBConfig(dsn="sqlite://"))
+
+with db.session_scope() as session:
+    assert session.execute("select 1;")
+
+db.shutdown()
+
+```
+
+## License
+
+sqlalchemy-multiple-db is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/sqlalchemy-multiple-db/security/policy).
```

### Comparing `sqlalchemy-multiple-db-1.8.0/setup.py` & `sqlalchemy-multiple-db-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: POSIX",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Environment :: Console",
     "Intended Audience :: Developers",
 ]
 
@@ -38,13 +40,13 @@
     maintainer="Pavel Liashkov",
     maintainer_email="pavel.liashkov@protonmail.com",
     download_url="https://pypi.python.org/pypi/sqlalchemy-multiple-db",
     url="https://github.com/bigbag/sqlalchemy-multiple-db",
     platforms=["POSIX"],
     classifiers=CLASSIFIERS,
     python_requires=">=3.7",
-    install_requires=["SQLAlchemy>=1.4,<1.5"],
+    install_requires=["SQLAlchemy>=1.4,<2.1"],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     test_suite="",
 )
```

### Comparing `sqlalchemy-multiple-db-1.8.0/sqlalchemy_multiple_db/helper.py` & `sqlalchemy-multiple-db-2.0.0/sqlalchemy_multiple_db/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from json import dumps, loads
 from typing import Any, Dict, Optional, Tuple, Union
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session, scoped_session, sessionmaker
+from sqlalchemy.sql import text
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_DB_NAME = "default"
 DEFAULT_SESSION_OPTIONS = {"autocommit": False, "autoflush": False, "expire_on_commit": False}
 DEFAULT_ENGINE_OPTIONS = {
@@ -47,20 +48,21 @@
             return object.__getattribute__(self, db_name)
         except AttributeError as exc:
             if db_name in ["sessions", "config"]:
                 print(f"DB: You need to call setup() for getting attribute {db_name}")
             raise exc
 
     def create_scoped_session(self, config: DBConfig) -> Session:
-        session: scoped_session = scoped_session(
-            sessionmaker(
-                bind=create_engine(config.dsn, **config.engine_options), **config.session_options
-            )
+        engine_options = config.engine_options or {}
+        session_options = config.session_options or {}
+
+        session = scoped_session(
+            sessionmaker(bind=create_engine(config.dsn, **engine_options), **session_options)
         )
-        return session
+        return session  # type: ignore
 
     def setup(self, config: Union[DBConfig, Dict[str, DBConfig]]):
         if isinstance(config, DBConfig):
             config = {DEFAULT_DB_NAME: config}
 
         self.config = config
 
@@ -83,15 +85,15 @@
     def get_status_info(self) -> Tuple[Dict[str, Any], bool]:
         full_status = True
         full_status_info = {}
 
         for db_name, session in self.sessions.items():
             status = True
             try:
-                session.execute("select 1;")
+                session.execute(text("select 1;"))
             except Exception as e:
                 status &= False
                 full_status &= False
                 logger.exception(e)
             finally:
                 session.close()
```

