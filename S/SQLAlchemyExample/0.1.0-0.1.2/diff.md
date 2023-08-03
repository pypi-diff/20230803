# Comparing `tmp/SQLAlchemyExample-0.1.0.tar.gz` & `tmp/SQLAlchemyExample-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemyExample-0.1.0.tar", last modified: Thu Aug  3 01:42:08 2023, max compression
+gzip compressed data, was "SQLAlchemyExample-0.1.2.tar", last modified: Thu Aug  3 15:38:03 2023, max compression
```

## Comparing `SQLAlchemyExample-0.1.0.tar` & `SQLAlchemyExample-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:08.202342 SQLAlchemyExample-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-08-03 01:42:08.202342 SQLAlchemyExample-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 01:42:08.202342 SQLAlchemyExample-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:08.194342 SQLAlchemyExample-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:08.198341 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:42:08.000000 SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:42:08.202342 SQLAlchemyExample-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/tests/test_otm_bi_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/tests/test_otm_uni_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-03 01:41:57.000000 SQLAlchemyExample-0.1.0/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:03.694403 SQLAlchemyExample-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 15:37:48.000000 SQLAlchemyExample-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 15:37:48.000000 SQLAlchemyExample-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-03 15:38:03.694403 SQLAlchemyExample-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-03 15:37:48.000000 SQLAlchemyExample-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-03 15:37:48.000000 SQLAlchemyExample-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-03 15:37:48.000000 SQLAlchemyExample-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 15:38:03.694403 SQLAlchemyExample-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:03.690402 SQLAlchemyExample-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:03.694403 SQLAlchemyExample-0.1.2/src/SQLAlchemyExample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-03 15:38:03.000000 SQLAlchemyExample-0.1.2/src/SQLAlchemyExample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-03 15:38:03.000000 SQLAlchemyExample-0.1.2/src/SQLAlchemyExample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:38:03.000000 SQLAlchemyExample-0.1.2/src/SQLAlchemyExample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 15:38:03.000000 SQLAlchemyExample-0.1.2/src/SQLAlchemyExample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:38:03.000000 SQLAlchemyExample-0.1.2/src/SQLAlchemyExample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:03.694403 SQLAlchemyExample-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-08-03 15:37:48.000000 SQLAlchemyExample-0.1.2/tests/test_otm_bi_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-03 15:37:48.000000 SQLAlchemyExample-0.1.2/tests/test_otm_uni_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-03 15:37:48.000000 SQLAlchemyExample-0.1.2/tests/test_simple.py
```

### Comparing `SQLAlchemyExample-0.1.0/LICENSE` & `SQLAlchemyExample-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.0/PKG-INFO` & `SQLAlchemyExample-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.1.0
+Version: 0.1.2
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
@@ -46,15 +46,14 @@
 
 .. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
     :alt: ci
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
-====================
 Exploring SQLAlchemy
 ====================
 
 This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
 
 Along the way some principles will be exhibited. The code should be self-explanatory.
 
@@ -62,63 +61,81 @@
 
 References:
 
 - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
 - https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
 - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
 
-==================
-Get Up-and-Running
-==================
+Installation
+============
+.. Detailed instructions on how to install, configure, and get the project running.
+
+:Status: Work In Progress
 
 1. Set the following environment variables:
 2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
 
-=======
-Testing
-=======
+
+Tests
+=====
+
+:Status: Work In Progress
 
 This project uses ``pytest`` to run tests and also to test docstring examples.
 
 Install the test dependencies.
 
-.. code-block::bash
-
-    $ pip install -r requirements_test.txt
+.. code-block:: bash
 
+    pip install -r requirements_test.txt
 
 Run the tests.
 
-.. code-block:: bash
+Instructions about how to run tests.
+
+Contributing
+============
+
+.. Guidelines on how to contribute to this project.
 
-    $ pytest tests
-    === XXX passed in SSS seconds ===
+:Status: Work In Progress
 
-==========
-Developing
-==========
-    The setup and installation is for Windows.  Feel free to add contribute to get it running on Linux as well.
+The setup and installation is for Windows.  Feel free to add contribute to get it running on Linux as well.
 
 This project uses ``black`` to format code and ``flake8`` for linting. We also support ``pre-commit`` to ensure these have been run. To configure your local environment please install these development dependencies and set up the commit hooks.
 
+
 .. code-block:: bash
 
     $ pip install black flake8 pre-commit
     $ pre-commit install
 
-=========
+
 Releasing
 =========
 
+:Status: Work In Progress
+
 Releases are published automatically when a tag is pushed to GitHub.
 
 .. code-block:: bash
 
     # Set next version number
     export RELEASE = x.x.x
 
     # Create tags
     git commit --allow -empty -m "Release $RELEASE"
     git tag -a $RELEASE -m "Version $RELEASE"
 
     # Push
     git push upstream --tags
+
+License
+=======
+
+:Status: Work In Progress
+
+.. Information about the project's license.
+
+Contact
+=======
+:Status: Work In Progress
```

### Comparing `SQLAlchemyExample-0.1.0/README.rst` & `SQLAlchemyExample-0.1.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 .. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
     :alt: ci
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
-====================
 Exploring SQLAlchemy
 ====================
 
 This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
 
 Along the way some principles will be exhibited. The code should be self-explanatory.
 
@@ -44,63 +43,81 @@
 
 References:
 
 - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
 - https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
 - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
 
-==================
-Get Up-and-Running
-==================
+Installation
+============
+.. Detailed instructions on how to install, configure, and get the project running.
+
+:Status: Work In Progress
 
 1. Set the following environment variables:
 2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
 
-=======
-Testing
-=======
+
+Tests
+=====
+
+:Status: Work In Progress
 
 This project uses ``pytest`` to run tests and also to test docstring examples.
 
 Install the test dependencies.
 
-.. code-block::bash
-
-    $ pip install -r requirements_test.txt
+.. code-block:: bash
 
+    pip install -r requirements_test.txt
 
 Run the tests.
 
-.. code-block:: bash
+Instructions about how to run tests.
+
+Contributing
+============
+
+.. Guidelines on how to contribute to this project.
 
-    $ pytest tests
-    === XXX passed in SSS seconds ===
+:Status: Work In Progress
 
-==========
-Developing
-==========
-    The setup and installation is for Windows.  Feel free to add contribute to get it running on Linux as well.
+The setup and installation is for Windows.  Feel free to add contribute to get it running on Linux as well.
 
 This project uses ``black`` to format code and ``flake8`` for linting. We also support ``pre-commit`` to ensure these have been run. To configure your local environment please install these development dependencies and set up the commit hooks.
 
+
 .. code-block:: bash
 
     $ pip install black flake8 pre-commit
     $ pre-commit install
 
-=========
+
 Releasing
 =========
 
+:Status: Work In Progress
+
 Releases are published automatically when a tag is pushed to GitHub.
 
 .. code-block:: bash
 
     # Set next version number
     export RELEASE = x.x.x
 
     # Create tags
     git commit --allow -empty -m "Release $RELEASE"
     git tag -a $RELEASE -m "Version $RELEASE"
 
     # Push
     git push upstream --tags
+
+License
+=======
+
+:Status: Work In Progress
+
+.. Information about the project's license.
+
+Contact
+=======
+:Status: Work In Progress
```

### Comparing `SQLAlchemyExample-0.1.0/pyproject.toml` & `SQLAlchemyExample-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.0/requirements.txt` & `SQLAlchemyExample-0.1.2/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 git-it
 mysql-connector-python
 pytest
 pytest-cov
 codecov
 sqlalchemy < 2.0.0
 sqlalchemy_utils
+Pygments
```

### Comparing `SQLAlchemyExample-0.1.0/setup.cfg` & `SQLAlchemyExample-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SQLAlchemyExample
-version = 0.1.0
+version = 0.1.2
 author = Hendrik du Toit
 author_email = hendrik@brightedge.co.za
 description = Exploring SQLAlchemy
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `SQLAlchemyExample-0.1.0/src/SQLAlchemyExample.egg-info/PKG-INFO` & `SQLAlchemyExample-0.1.2/src/SQLAlchemyExample.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.1.0
+Version: 0.1.2
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
@@ -46,15 +46,14 @@
 
 .. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
     :alt: ci
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
-====================
 Exploring SQLAlchemy
 ====================
 
 This project provide a sandbox to experiment with SQLAlchemy. This idea is to build an example sequentially in steps to give new users the idea on where to start and how to progress.
 
 Along the way some principles will be exhibited. The code should be self-explanatory.
 
@@ -62,63 +61,81 @@
 
 References:
 
 - https://www.tutorialspoint.com/sqlalchemy/sqlalchemy_orm_many_to_many_relationships.htm
 - https://docs.sqlalchemy.org/en/14/orm/tutorial.html#building-a-relationship
 - https://cyruslab.net/2020/07/16/pythoncreate-database-if-not-exists-with-sqlalchemy/
 
-==================
-Get Up-and-Running
-==================
+Installation
+============
+.. Detailed instructions on how to install, configure, and get the project running.
+
+:Status: Work In Progress
 
 1. Set the following environment variables:
 2. Start Docker.  The ``docker-rebuild.bat`` script will git docker up and running.
 
-=======
-Testing
-=======
+
+Tests
+=====
+
+:Status: Work In Progress
 
 This project uses ``pytest`` to run tests and also to test docstring examples.
 
 Install the test dependencies.
 
-.. code-block::bash
-
-    $ pip install -r requirements_test.txt
+.. code-block:: bash
 
+    pip install -r requirements_test.txt
 
 Run the tests.
 
-.. code-block:: bash
+Instructions about how to run tests.
+
+Contributing
+============
+
+.. Guidelines on how to contribute to this project.
 
-    $ pytest tests
-    === XXX passed in SSS seconds ===
+:Status: Work In Progress
 
-==========
-Developing
-==========
-    The setup and installation is for Windows.  Feel free to add contribute to get it running on Linux as well.
+The setup and installation is for Windows.  Feel free to add contribute to get it running on Linux as well.
 
 This project uses ``black`` to format code and ``flake8`` for linting. We also support ``pre-commit`` to ensure these have been run. To configure your local environment please install these development dependencies and set up the commit hooks.
 
+
 .. code-block:: bash
 
     $ pip install black flake8 pre-commit
     $ pre-commit install
 
-=========
+
 Releasing
 =========
 
+:Status: Work In Progress
+
 Releases are published automatically when a tag is pushed to GitHub.
 
 .. code-block:: bash
 
     # Set next version number
     export RELEASE = x.x.x
 
     # Create tags
     git commit --allow -empty -m "Release $RELEASE"
     git tag -a $RELEASE -m "Version $RELEASE"
 
     # Push
     git push upstream --tags
+
+License
+=======
+
+:Status: Work In Progress
+
+.. Information about the project's license.
+
+Contact
+=======
+:Status: Work In Progress
```

### Comparing `SQLAlchemyExample-0.1.0/tests/test_otm_bi_single_table_inherit.py` & `SQLAlchemyExample-0.1.2/tests/test_otm_bi_single_table_inherit.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.0/tests/test_otm_uni_single_table_inherit.py` & `SQLAlchemyExample-0.1.2/tests/test_otm_uni_single_table_inherit.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.0/tests/test_simple.py` & `SQLAlchemyExample-0.1.2/tests/test_simple.py`

 * *Files identical despite different names*

