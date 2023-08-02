# Comparing `tmp/SQLAlchemyExample-0.0.12.tar.gz` & `tmp/SQLAlchemyExample-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemyExample-0.0.12.tar", last modified: Wed Aug  2 12:20:57 2023, max compression
+gzip compressed data, was "SQLAlchemyExample-0.0.2.tar", last modified: Mon Jul 31 22:13:56 2023, max compression
```

## Comparing `SQLAlchemyExample-0.0.12.tar` & `SQLAlchemyExample-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:20:57.659611 SQLAlchemyExample-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 12:20:45.000000 SQLAlchemyExample-0.0.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 12:20:45.000000 SQLAlchemyExample-0.0.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-02 12:20:57.659611 SQLAlchemyExample-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-02 12:20:45.000000 SQLAlchemyExample-0.0.12/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-02 12:20:45.000000 SQLAlchemyExample-0.0.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-02 12:20:45.000000 SQLAlchemyExample-0.0.12/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 12:20:57.659611 SQLAlchemyExample-0.0.12/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:20:57.651611 SQLAlchemyExample-0.0.12/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:20:57.659611 SQLAlchemyExample-0.0.12/src/SQLAlchemyExample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-02 12:20:57.000000 SQLAlchemyExample-0.0.12/src/SQLAlchemyExample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 12:20:57.000000 SQLAlchemyExample-0.0.12/src/SQLAlchemyExample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:20:57.000000 SQLAlchemyExample-0.0.12/src/SQLAlchemyExample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 12:20:57.000000 SQLAlchemyExample-0.0.12/src/SQLAlchemyExample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:20:57.000000 SQLAlchemyExample-0.0.12/src/SQLAlchemyExample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:20:57.659611 SQLAlchemyExample-0.0.12/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-02 12:20:45.000000 SQLAlchemyExample-0.0.12/tests/test_otm_bi_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-02 12:20:45.000000 SQLAlchemyExample-0.0.12/tests/test_otm_uni_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-02 12:20:45.000000 SQLAlchemyExample-0.0.12/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.926533 SQLAlchemyExample-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:13:56.000000 SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:13:56.930533 SQLAlchemyExample-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_otm_bi_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_otm_uni_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-31 22:13:44.000000 SQLAlchemyExample-0.0.2/tests/test_simple.py
```

### Comparing `SQLAlchemyExample-0.0.12/LICENSE` & `SQLAlchemyExample-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.0.12/PKG-INFO` & `SQLAlchemyExample-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.0.12
+Version: 0.0.2
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
-Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/status/SQLAlchemyExample
     :alt: PyPI - Status
@@ -34,19 +33,19 @@
 .. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
     :alt: GitHub Searches
 
 .. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
     :alt: CodeCov
     :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yml?label=pre-commit
-    :alt: Pre-Commit
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yaml?label=pre-commit
+    :alt: GitHub Workflow Status (with event)
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
-    :alt: ci
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yaml?label=ci
+    :alt: GitHub Workflow Status (with event)
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
 ====================
 Exploring SQLAlchemy
 ====================
```

### Comparing `SQLAlchemyExample-0.0.12/README.rst` & `SQLAlchemyExample-0.0.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 .. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
     :alt: GitHub Searches
 
 .. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
     :alt: CodeCov
     :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yml?label=pre-commit
-    :alt: Pre-Commit
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yaml?label=pre-commit
+    :alt: GitHub Workflow Status (with event)
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
-    :alt: ci
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yaml?label=ci
+    :alt: GitHub Workflow Status (with event)
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
 ====================
 Exploring SQLAlchemy
 ====================
```

### Comparing `SQLAlchemyExample-0.0.12/pyproject.toml` & `SQLAlchemyExample-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.0.12/requirements.txt` & `SQLAlchemyExample-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.0.12/setup.cfg` & `SQLAlchemyExample-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [metadata]
 name = SQLAlchemyExample
-version = 0.0.12
+version = 0.0.2
 author = Hendrik du Toit
 author_email = hendrik@brightedge.co.za
 description = Exploring SQLAlchemy
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 1 - Planning
 	Intended Audience :: Developers
 	Topic :: Software Development
-	Topic :: Database
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.10
 
 [options]
 install_requires = 
 	Path
 	beetools
```

### Comparing `SQLAlchemyExample-0.0.12/src/SQLAlchemyExample.egg-info/PKG-INFO` & `SQLAlchemyExample-0.0.2/src/SQLAlchemyExample.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.0.12
+Version: 0.0.2
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
-Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/status/SQLAlchemyExample
     :alt: PyPI - Status
@@ -34,19 +33,19 @@
 .. image:: https://img.shields.io/github/search/hendrikdutoit/SQLAlchemyExample/GitHub
     :alt: GitHub Searches
 
 .. image:: https://img.shields.io/codecov/c/gh/hendrikdutoit/SQLAlchemyExample
     :alt: CodeCov
     :target: https://app.codecov.io/gh/hendrikdutoit/SQLAlchemyExample
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yml?label=pre-commit
-    :alt: Pre-Commit
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/pre-commit.yaml?label=pre-commit
+    :alt: GitHub Workflow Status (with event)
 
-.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yml?label=ci
-    :alt: ci
+.. image:: https://img.shields.io/github/actions/workflow/status/hendrikdutoit/SQLAlchemyExample/ci.yaml?label=ci
+    :alt: GitHub Workflow Status (with event)
 
 .. image:: https://img.shields.io/pypi/v/SQLAlchemyExample
     :alt: PyPi
 
 ====================
 Exploring SQLAlchemy
 ====================
```

### Comparing `SQLAlchemyExample-0.0.12/tests/test_otm_bi_single_table_inherit.py` & `SQLAlchemyExample-0.0.2/tests/test_otm_bi_single_table_inherit.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.0.12/tests/test_otm_uni_single_table_inherit.py` & `SQLAlchemyExample-0.0.2/tests/test_otm_uni_single_table_inherit.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.0.12/tests/test_simple.py` & `SQLAlchemyExample-0.0.2/tests/test_simple.py`

 * *Files identical despite different names*

