# Comparing `tmp/SQLAlchemyExample-0.0.2.tar.gz` & `tmp/SQLAlchemyExample-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemyExample-0.0.2.tar", last modified: Mon Jul 31 22:13:56 2023, max compression
+gzip compressed data, was "SQLAlchemyExample-0.1.0.tar", last modified: Thu Aug  3 01:42:08 2023, max compression
```

## Comparing `SQLAlchemyExample-0.0.2.tar` & `SQLAlchemyExample-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.926533 SQLAlchemyExample-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_otm_bi_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_otm_uni_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:08.202342 SQLAlchemyExample-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-08-03 01:42:08.202342 SQLAlchemyExample-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 01:42:08.202342 SQLAlchemyExample-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:08.194342 SQLAlchemyExample-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:08.198341 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:08.202342 SQLAlchemyExample-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/tests/test_otm_bi_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/tests/test_otm_uni_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/tests/test_simple.py
```

### Comparing `SQLAlchemyExample-0.0.2/LICENSE` & `SQLAlchemyExample-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.0.2/PKG-INFO` & `SQLAlchemyExample-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.0.2
+Version: 0.1.0
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
+Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/status/SQLAlchemyExample
     :alt: PyPI - Status
 
@@ -33,65 +37,59 @@
 .. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
     :alt: GitHub Searches
 
 .. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
     :alt: CodeCov
     :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yaml?label=pre-commit
-    :alt: GitHub Workflow Status (with event)
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yml?label=pre-commit
+    :alt: Pre-Commit
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yaml?label=ci
-    :alt: GitHub Workflow Status (with event)
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
+    :alt: ci
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
 ====================
 Exploring SQLAlchemy
 ====================
 
-    This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
+This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
 
-    Along the way some principles will be exhibited. The code should be self-explanatory.
+Along the way some principles will be exhibited. The code should be self-explanatory.
 
-    The source code in ``src`` by itself does not do much, it basically only defines the tables and some setup code.  The "examples" are in the the ``pytest's`` since we are experimenting to see howe it works and if it was successfull.
+The source code in ``src`` by itself does not do much, it basically only defines the tables and some setup code.  The "examples" are in the the ``pytest's`` since we are experimenting to see howe it works and if it was successfull.
 
+References:
 
-    References:
-
-    - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
-    - https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
-    - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
+- https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
+- https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
+- https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
 
 ==================
 Get Up-and-Running
 ==================
 
-    1. Set the following environment variables:
-    2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
-    3. dasd
-
-``pytest``
+1. Set the following environment variables:
+2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
 
 =======
 Testing
 =======
 
 This project uses ``pytest`` to run tests and also to test docstring examples.
 
 Install the test dependencies.
 
 .. code-block::bash
 
     $ pip install -r requirements_test.txt
 
 
-
-
 Run the tests.
 
 .. code-block:: bash
 
     $ pytest tests
     === XXX passed in SSS seconds ===
```

### Comparing `SQLAlchemyExample-0.0.2/README.rst` & `SQLAlchemyExample-0.1.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -19,65 +19,59 @@
 .. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
     :alt: GitHub Searches
 
 .. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
     :alt: CodeCov
     :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yaml?label=pre-commit
-    :alt: GitHub Workflow Status (with event)
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yml?label=pre-commit
+    :alt: Pre-Commit
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yaml?label=ci
-    :alt: GitHub Workflow Status (with event)
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
+    :alt: ci
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
 ====================
 Exploring SQLAlchemy
 ====================
 
-    This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
+This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
 
-    Along the way some principles will be exhibited. The code should be self-explanatory.
+Along the way some principles will be exhibited. The code should be self-explanatory.
 
-    The source code in ``src`` by itself does not do much, it basically only defines the tables and some setup code.  The "examples" are in the the ``pytest's`` since we are experimenting to see howe it works and if it was successfull.
+The source code in ``src`` by itself does not do much, it basically only defines the tables and some setup code.  The "examples" are in the the ``pytest's`` since we are experimenting to see howe it works and if it was successfull.
 
+References:
 
-    References:
-
-    - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
-    - https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
-    - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
+- https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
+- https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
+- https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
 
 ==================
 Get Up-and-Running
 ==================
 
-    1. Set the following environment variables:
-    2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
-    3. dasd
-
-``pytest``
+1. Set the following environment variables:
+2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
 
 =======
 Testing
 =======
 
 This project uses ``pytest`` to run tests and also to test docstring examples.
 
 Install the test dependencies.
 
 .. code-block::bash
 
     $ pip install -r requirements_test.txt
 
 
-
-
 Run the tests.
 
 .. code-block:: bash
 
     $ pytest tests
     === XXX passed in SSS seconds ===
```

### Comparing `SQLAlchemyExample-0.0.2/pyproject.toml` & `SQLAlchemyExample-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 [tool.black]
 skip-string-normalization = true
 extend-exclude = "/templates"
 
 
 [tool.pytest.ini_options]
-addopts = ["--import-mode=importlib", '-v', '--ignore-glob=*\Archive', '--cov-report=html']
-#addopts = ["--import-mode=importlib", '-v', '--cov=./', '--ignore-glob=*\Archive', '--cov-report=html']
+#addopts = ["--import-mode=importlib", '-v', '--ignore-glob=*\Archive', '--cov-report=html']
+addopts = ["--import-mode=importlib", '-v', '--cov=./', '--ignore-glob=*\Archive', '--cov-report=html']
 #pythonpath = ["src", "tests" ]
 markers = [
     'select: Run a selection of tests',
     'otmuni: One-To-Manu Uni-direction'
 ]
```

### Comparing `SQLAlchemyExample-0.0.2/requirements.txt` & `SQLAlchemyExample-0.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/PKG-INFO` & `SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.0.2
+Version: 0.1.0
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
+Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/status/SQLAlchemyExample
     :alt: PyPI - Status
 
@@ -33,65 +37,59 @@
 .. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
     :alt: GitHub Searches
 
 .. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
     :alt: CodeCov
     :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yaml?label=pre-commit
-    :alt: GitHub Workflow Status (with event)
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yml?label=pre-commit
+    :alt: Pre-Commit
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yaml?label=ci
-    :alt: GitHub Workflow Status (with event)
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
+    :alt: ci
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
 ====================
 Exploring SQLAlchemy
 ====================
 
-    This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
+This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
 
-    Along the way some principles will be exhibited. The code should be self-explanatory.
+Along the way some principles will be exhibited. The code should be self-explanatory.
 
-    The source code in ``src`` by itself does not do much, it basically only defines the tables and some setup code.  The "examples" are in the the ``pytest's`` since we are experimenting to see howe it works and if it was successfull.
+The source code in ``src`` by itself does not do much, it basically only defines the tables and some setup code.  The "examples" are in the the ``pytest's`` since we are experimenting to see howe it works and if it was successfull.
 
+References:
 
-    References:
-
-    - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
-    - https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
-    - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
+- https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
+- https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
+- https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
 
 ==================
 Get Up-and-Running
 ==================
 
-    1. Set the following environment variables:
-    2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
-    3. dasd
-
-``pytest``
+1. Set the following environment variables:
+2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
 
 =======
 Testing
 =======
 
 This project uses ``pytest`` to run tests and also to test docstring examples.
 
 Install the test dependencies.
 
 .. code-block::bash
 
     $ pip install -r requirements_test.txt
 
 
-
-
 Run the tests.
 
 .. code-block:: bash
 
     $ pytest tests
     === XXX passed in SSS seconds ===
```

### Comparing `SQLAlchemyExample-0.0.2/tests/test_otm_bi_single_table_inherit.py` & `SQLAlchemyExample-0.1.0/tests/test_otm_bi_single_table_inherit.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,7 +69,25 @@
         pass
 
     def test_parentotmbi_table_dunder_str_ok(self, setup_db_otm_bi_sti):
         parent = tab_cfg.ParentOTMBi(name='John')
 
         assert str(parent) == 'John'
         pass
+
+    def test_childotmbi_table_dunder_repr_ok(self, setup_db_otm_bi_sti):
+        engine, session, base = setup_db_otm_bi_sti
+        child = tab_cfg.ChildOTMBi(name='John')
+        session.add_all([child])
+        session.commit()
+
+        assert repr(child) == '<ChildOTMBi(id=1 name=John)>'
+        pass
+
+    def test_childotmbisti_table_dunder_repr_ok(self, setup_db_otm_bi_sti):
+        engine, session, base = setup_db_otm_bi_sti
+        child = tab_cfg.ChildOTMBiSTI(name='John')
+        session.add_all([child])
+        session.commit()
+
+        assert repr(child) == '<ChildOTMBiSTI(id=1 name=John parent_id=None)>'
+        pass
```

### Comparing `SQLAlchemyExample-0.0.2/tests/test_otm_uni_single_table_inherit.py` & `SQLAlchemyExample-0.1.0/tests/test_otm_uni_single_table_inherit.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,7 +65,25 @@
         pass
 
     def test_parentotmbi_table_dunder_str_ok(self):
         parent = tab_cfg.ParentOTMUni(name='John')
 
         assert str(parent) == 'John'
         pass
+
+    def test_childotmuni_table_dunder_repr_ok(self, setup_db_otm_uni_sti):
+        engine, session, base = setup_db_otm_uni_sti
+        child = tab_cfg.ChildOTMUni(name='John')
+        session.add_all([child])
+        session.commit()
+
+        assert repr(child) == '<ChildOTMUni(id=1 name=John)>'
+        pass
+
+    def test_childotmbisti_table_dunder_repr_ok(self, setup_db_otm_bi_sti):
+        engine, session, base = setup_db_otm_bi_sti
+        child = tab_cfg.ChildOTMUniSTI(name='John')
+        session.add_all([child])
+        session.commit()
+
+        assert repr(child) == '<ChildOTMUniSTI(id=1 name=John parent_id=None)>'
+        pass
```

### Comparing `SQLAlchemyExample-0.0.2/tests/test_simple.py` & `SQLAlchemyExample-0.1.0/tests/test_simple.py`

 * *Files identical despite different names*

