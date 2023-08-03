# Comparing `tmp/beanclerk-0.0.5.tar.gz` & `tmp/beanclerk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanclerk-0.0.5.tar", last modified: Sat Jul 29 11:17:41 2023, max compression
+gzip compressed data, was "beanclerk-0.0.6.tar", last modified: Thu Aug  3 15:38:39 2023, max compression
```

## Comparing `beanclerk-0.0.5.tar` & `beanclerk-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.968478 beanclerk-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.960477 beanclerk-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.960477 beanclerk-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-29 11:17:29.000000 beanclerk-0.0.5/.github/workflows/publishing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-29 11:17:29.000000 beanclerk-0.0.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-29 11:17:29.000000 beanclerk-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-29 11:17:29.000000 beanclerk-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-07-29 11:17:29.000000 beanclerk-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-07-29 11:17:41.968478 beanclerk-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-29 11:17:29.000000 beanclerk-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.964477 beanclerk-0.0.5/beanclerk/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/bean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/clerk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.964477 beanclerk-0.0.5/beanclerk/importers/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/importers/banka_creditas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/importers/fio_banka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.964477 beanclerk-0.0.5/beanclerk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      259 2023-07-29 11:17:29.000000 beanclerk-0.0.5/build_venv
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-29 11:17:29.000000 beanclerk-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 11:17:41.968478 beanclerk-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.964477 beanclerk-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/beanclerk-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.968478 beanclerk-0.0.5/tests/importers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/banka_creditas_transactions.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/fio_banka_transactions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/test_banka_creditas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/test_fio_banka.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/ledger.beancount
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/test_clerk.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:39.933011 beanclerk-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:39.929011 beanclerk-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:39.929011 beanclerk-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 15:38:29.000000 beanclerk-0.0.6/.github/workflows/publishing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 15:38:29.000000 beanclerk-0.0.6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-08-03 15:38:29.000000 beanclerk-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 15:38:29.000000 beanclerk-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-08-03 15:38:29.000000 beanclerk-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-08-03 15:38:39.933011 beanclerk-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-08-03 15:38:29.000000 beanclerk-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:39.929011 beanclerk-0.0.6/beanclerk/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/bean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/clerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:39.933011 beanclerk-0.0.6/beanclerk/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/importers/banka_creditas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-03 15:38:29.000000 beanclerk-0.0.6/beanclerk/importers/fio_banka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:39.929011 beanclerk-0.0.6/beanclerk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-08-03 15:38:39.000000 beanclerk-0.0.6/beanclerk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-03 15:38:39.000000 beanclerk-0.0.6/beanclerk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:38:39.000000 beanclerk-0.0.6/beanclerk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 15:38:39.000000 beanclerk-0.0.6/beanclerk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-03 15:38:39.000000 beanclerk-0.0.6/beanclerk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 15:38:39.000000 beanclerk-0.0.6/beanclerk.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      259 2023-08-03 15:38:29.000000 beanclerk-0.0.6/build_venv
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-03 15:38:29.000000 beanclerk-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:38:39.933011 beanclerk-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:39.933011 beanclerk-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/beanclerk-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:39.933011 beanclerk-0.0.6/tests/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/importers/banka_creditas_transactions.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/importers/fio_banka_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/importers/test_banka_creditas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/importers/test_fio_banka.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/ledger.beancount
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/test_clerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-03 15:38:29.000000 beanclerk-0.0.6/tests/test_config.py
```

### Comparing `beanclerk-0.0.5/.github/workflows/publishing.yml` & `beanclerk-0.0.6/.github/workflows/publishing.yml`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.5/.gitignore` & `beanclerk-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.5/.pre-commit-config.yaml` & `beanclerk-0.0.6/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       - id: check-xml
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-added-large-files
       - id: check-merge-conflict
       - id: detect-private-key
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.280
+    rev: v0.0.281
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
     rev: 23.7.0
     hooks:
       - id: black
```

### Comparing `beanclerk-0.0.5/LICENSE` & `beanclerk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.5/PKG-INFO` & `beanclerk-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanclerk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automation for Beancount
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -371,43 +371,43 @@
 [![license](https://img.shields.io/pypi/l/beanclerk)](https://pypi.org/project/beanclerk/)
 [![python versions](https://img.shields.io/pypi/pyversions/beanclerk)](https://pypi.org/project/beanclerk/)
 [![ci tests](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml/badge.svg)](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/beanclerk/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/beanclerk/main)
 
 ## Description
 
-Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance), automating some areas not addressed by Beancount itself, namely:
+Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance). It automates some areas not addressed by Beancount itself, namely:
 
-1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As some financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import process from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) that aims to support any compatible API.
+1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) to support any compatible API.
 1. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
     * As the first step, Beanclerk provides a way to define rules for automated categorization.
     * The future step is to augment it by machine-learning capabilities (e.g. via integration of the [Smart Importer](https://github.com/beancount/smart_importer)). (Btw, it might be also interesting to use machine-learning to discover hidden patterns or to provide predictions about our financial behavior.)
-1. _Automatic insertion of new transactions_: Beanclerk _appends_ new transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about the precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) can sort them out anyway.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes transparent and easy to review.
+1. _Automatic insertion of new transactions_: Beanclerk _appends_ transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about a precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) sort and filter them effectively.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes easy to review.
 
 **Beanclerk is still a rather 'rough' prototype.** You may encounter some unhandled exceptions and the API may change significantly in the future.
 
 **Beanclerk is currently tested on Linux only.**
 
 ### Existing importers
 
-Currently, there is 1 built-in importer for [Fio banka](https://www.fio.cz/). I plan to add another for [Banka Creditas](https://www.creditas.cz/), and, maybe, for some crypto exchanges. (All importers may move into separate repos in the future so the user may install only those they actually need).
+Beanclerk provides 2 built-in importers for [Fio banka](https://www.fio.cz/) and for [Banka Creditas](https://www.creditas.cz/). I plan to add another for some crypto exchanges. (All importers may move into separate repos in the future so you can install only those you actually need). Moreover, Beanclerk is designed in such a way to import importers (Python classes) from your working directory (this feature is not enabled yet).
 
 ### Notes
 
-I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
+I started Beanclerk primarily to try out some Python packages and to get better in programming by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
 
 * [beancount-import](https://github.com/jbms/beancount-import): Web UI for semi-automatically importing external data into beancount.
 * [finance-dl](https://github.com/jbms/finance-dl): Tools for automatically downloading/scraping personal financial data.
 * [beancount_reds_importers](https://github.com/redstreet/beancount_reds_importers): Simple ingesting tools for Beancount (plain text, double entry accounting software). More importantly, a framework to allow you to easily write your own importers.
 * [smart_importer](https://github.com/beancount/smart_importer): Augment Beancount importers with machine learning functionality.
 * [autobean](https://github.com/SEIAROTg/autobean): A collection of plugins and scripts that help automating bookkeeping with beancount.
 
 ## Installation
 
-Beanclerk requires Beancount, that may need some additional steps for its installation. See [Beancount Download & Installation](https://github.com/beancount/beancount#download--installation). Then, install Beanclerk via pip:
+Beanclerk requires Beancount, that may need some additional steps for its build and installation. See [Beancount Download & Installation](https://github.com/beancount/beancount#download--installation). Then, install Beanclerk via pip:
 
 ```
 pip install beanclerk
 ```
 
 Or, you may use [pipx](https://github.com/pypa/pipx) to install Beanclerk in an isolated environment:
 ```
@@ -423,23 +423,24 @@
 
 ### Configuration
 
 Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory. Or, set a path to the config file via the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
 
 ### Running the import
 
-Beanclerk currently implements a single command `import`. When running it for the first time, it is necessary to use at least the `--from-date` option to set the date to start the import from. (At the moment, Beanclerk runs import for all configured accounts.)
+Beanclerk implements a single command `import`. When running it for the first time, it is necessary to use the `--from-date` option to set the date to start the import from. (Beanclerk runs import for all configured accounts.)
 
 ```
 bean-clerk import --from-date 2023-01-01
 ```
 
-Once Beanclerk encounters a transaction without a matching categorization rule, it prompts the user to resolve the situation:
+Once Beanclerk encounters a transaction without a matching categorization rule, it prompts you to resolve the situation:
 
 ```
+Importing transactions for account: 'Assets:Banks:Fio:Checking'
 ...
 No categorization rule matches the following transaction:
 Transaction(
     meta={
         'id': '10000000002',
         'account_id': '2345678901',
         'account_name': 'Pavel, Žák',
@@ -470,17 +471,23 @@
 )
 Available actions:
 'r': reload config (you should add a new rule first)
 'i': import as-is (transaction remains unbalanced)
 ...
 ```
 
+After all new transactions from an account are imported, Beanclerk prints the import status:
+```
+...
+New transactions: 3, balance OK: 2000.10
+```
+
 ## Contributing
 
-Contributions are welcome. Make sure to create an issue first so we can discuss it.
+Contributions are welcome. As changes to the project are still rather dynamic, make sure to create an issue first so we can discuss it.
 
 Set up a development environment for playing with the source code:
 ```bash
 ./build_venv
 source venv/bin/activate
 pre-commit install  # https://pre-commit.com/
 ```
```

### Comparing `beanclerk-0.0.5/README.md` & `beanclerk-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 [![license](https://img.shields.io/pypi/l/beanclerk)](https://pypi.org/project/beanclerk/)
 [![python versions](https://img.shields.io/pypi/pyversions/beanclerk)](https://pypi.org/project/beanclerk/)
 [![ci tests](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml/badge.svg)](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/beanclerk/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/beanclerk/main)
 
 ## Description
 
-Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance), automating some areas not addressed by Beancount itself, namely:
+Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance). It automates some areas not addressed by Beancount itself, namely:
 
-1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As some financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import process from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) that aims to support any compatible API.
+1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) to support any compatible API.
 1. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
     * As the first step, Beanclerk provides a way to define rules for automated categorization.
     * The future step is to augment it by machine-learning capabilities (e.g. via integration of the [Smart Importer](https://github.com/beancount/smart_importer)). (Btw, it might be also interesting to use machine-learning to discover hidden patterns or to provide predictions about our financial behavior.)
-1. _Automatic insertion of new transactions_: Beanclerk _appends_ new transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about the precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) can sort them out anyway.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes transparent and easy to review.
+1. _Automatic insertion of new transactions_: Beanclerk _appends_ transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about a precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) sort and filter them effectively.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes easy to review.
 
 **Beanclerk is still a rather 'rough' prototype.** You may encounter some unhandled exceptions and the API may change significantly in the future.
 
 **Beanclerk is currently tested on Linux only.**
 
 ### Existing importers
 
-Currently, there is 1 built-in importer for [Fio banka](https://www.fio.cz/). I plan to add another for [Banka Creditas](https://www.creditas.cz/), and, maybe, for some crypto exchanges. (All importers may move into separate repos in the future so the user may install only those they actually need).
+Beanclerk provides 2 built-in importers for [Fio banka](https://www.fio.cz/) and for [Banka Creditas](https://www.creditas.cz/). I plan to add another for some crypto exchanges. (All importers may move into separate repos in the future so you can install only those you actually need). Moreover, Beanclerk is designed in such a way to import importers (Python classes) from your working directory (this feature is not enabled yet).
 
 ### Notes
 
-I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
+I started Beanclerk primarily to try out some Python packages and to get better in programming by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
 
 * [beancount-import](https://github.com/jbms/beancount-import): Web UI for semi-automatically importing external data into beancount.
 * [finance-dl](https://github.com/jbms/finance-dl): Tools for automatically downloading/scraping personal financial data.
 * [beancount_reds_importers](https://github.com/redstreet/beancount_reds_importers): Simple ingesting tools for Beancount (plain text, double entry accounting software). More importantly, a framework to allow you to easily write your own importers.
 * [smart_importer](https://github.com/beancount/smart_importer): Augment Beancount importers with machine learning functionality.
 * [autobean](https://github.com/SEIAROTg/autobean): A collection of plugins and scripts that help automating bookkeeping with beancount.
 
 ## Installation
 
-Beanclerk requires Beancount, that may need some additional steps for its installation. See [Beancount Download & Installation](https://github.com/beancount/beancount#download--installation). Then, install Beanclerk via pip:
+Beanclerk requires Beancount, that may need some additional steps for its build and installation. See [Beancount Download & Installation](https://github.com/beancount/beancount#download--installation). Then, install Beanclerk via pip:
 
 ```
 pip install beanclerk
 ```
 
 Or, you may use [pipx](https://github.com/pypa/pipx) to install Beanclerk in an isolated environment:
 ```
@@ -56,23 +56,24 @@
 
 ### Configuration
 
 Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory. Or, set a path to the config file via the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
 
 ### Running the import
 
-Beanclerk currently implements a single command `import`. When running it for the first time, it is necessary to use at least the `--from-date` option to set the date to start the import from. (At the moment, Beanclerk runs import for all configured accounts.)
+Beanclerk implements a single command `import`. When running it for the first time, it is necessary to use the `--from-date` option to set the date to start the import from. (Beanclerk runs import for all configured accounts.)
 
 ```
 bean-clerk import --from-date 2023-01-01
 ```
 
-Once Beanclerk encounters a transaction without a matching categorization rule, it prompts the user to resolve the situation:
+Once Beanclerk encounters a transaction without a matching categorization rule, it prompts you to resolve the situation:
 
 ```
+Importing transactions for account: 'Assets:Banks:Fio:Checking'
 ...
 No categorization rule matches the following transaction:
 Transaction(
     meta={
         'id': '10000000002',
         'account_id': '2345678901',
         'account_name': 'Pavel, Žák',
@@ -103,17 +104,23 @@
 )
 Available actions:
 'r': reload config (you should add a new rule first)
 'i': import as-is (transaction remains unbalanced)
 ...
 ```
 
+After all new transactions from an account are imported, Beanclerk prints the import status:
+```
+...
+New transactions: 3, balance OK: 2000.10
+```
+
 ## Contributing
 
-Contributions are welcome. Make sure to create an issue first so we can discuss it.
+Contributions are welcome. As changes to the project are still rather dynamic, make sure to create an issue first so we can discuss it.
 
 Set up a development environment for playing with the source code:
 ```bash
 ./build_venv
 source venv/bin/activate
 pre-commit install  # https://pre-commit.com/
 ```
```

### Comparing `beanclerk-0.0.5/beanclerk/bean_helpers.py` & `beanclerk-0.0.6/beanclerk/bean_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,16 @@
         Directive: a Beancount directive
     """
     for entry in entries:
         if isinstance(entry, cls):
             yield entry
 
 
-def check_account_name(name: str) -> None:
-    """Check a Beanount account name.
+def validate_account_name(name: str) -> None:
+    """Validate a Beanount account name.
 
     Args:
         name (str): a Beancount account name
 
     Raises:
         ValueError: if the account name is invalid
     """
```

### Comparing `beanclerk-0.0.5/beanclerk/clerk.py` & `beanclerk-0.0.6/beanclerk/clerk.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 from beancount.core.realization import compute_postings_balance, postings_by_account
 from beancount.loader import load_file
 from beancount.parser.printer import print_entry
 from rich import print as rprint
 from rich.prompt import Prompt
 
 from .bean_helpers import (
-    check_account_name,
     create_posting,
     create_transaction,
     filter_entries,
+    validate_account_name,
 )
 from .config import CategorizationRule, Config, load_config, load_importer
 from .exceptions import ClerkError
 from .importers import ApiImporterProtocol
 
 
 def find_last_import_date(entries: list[Directive], account_name: str) -> date | None:
@@ -47,15 +47,15 @@
 
     Raises:
         ValueError: if account_name is not a valid Beancount account name
 
     Returns:
         date | None
     """
-    check_account_name(account_name)
+    validate_account_name(account_name)
     txn_postings = filter_entries(
         postings_by_account(entries)[account_name],
         TxnPosting,
     )
     for txn_posting in reversed(list(txn_postings)):  # latest first
         if txn_posting.txn.meta.get("id") is not None:
             return txn_posting.txn.date
@@ -76,15 +76,15 @@
 
     Raises:
         ValueError: if account_name is not a valid Beancount account name
 
     Returns:
         bool
     """
-    check_account_name(account_name)
+    validate_account_name(account_name)
     txn_postings = filter_entries(
         postings_by_account(entries)[account_name],
         TxnPosting,
     )
     return any(txn_posting.txn.meta.get("id") == txn_id for txn_posting in txn_postings)
 
 
@@ -105,15 +105,15 @@
     Raises:
         ValueError: if account_name is not a valid Beancount account name
         ValueError: if currency is not a valid ISO code
 
     Returns:
         Amount: account balance
     """
-    check_account_name(account_name)
+    validate_account_name(account_name)
     if not re.match(r"^[A-Z]{3}$", currency):
         raise ValueError(f"'{currency}' is not a valid currency code")
     return compute_postings_balance(
         postings_by_account(entries)[account_name],
     ).get_currency_units(currency)
 
 
@@ -128,37 +128,24 @@
     to categorize the transaction, None is returned then.
 
     Args:
         transaction (Transaction): a Beancount transaction
         config (Config): Beanclerk config
 
     Raises:
-        ClerkError: if a categorization rule is invalid.
-        ClerkError: if a dangerous pattern is used in a categorization rule.
         ClerkError: if an unexpected action is chosen by the user.
 
     Returns:
         CategorizationRule | None: a matching rule, or None
     """
     while True:
         if config.categorization_rules:
             for rule in config.categorization_rules:
-                if len(rule.matches.metadata) == 0:
-                    raise ClerkError(
-                        f"Categorization rule: {rule}\n"
-                        "Sanity check failed: no patterns to match",
-                    )
                 num_matches = 0
                 for key, pattern in rule.matches.metadata.items():
-                    if pattern == "":
-                        raise ClerkError(
-                            f"Categorization rule: {rule}\n"
-                            'Dangerous pattern "" matches everything. '
-                            'Use ".*" or "^$" instead.',
-                        )
                     if (
                         key in transaction.meta
                         and re.search(pattern, transaction.meta[key]) is not None
                     ):
                         num_matches += 1
                 if num_matches == len(rule.matches.metadata):
                     return rule
```

### Comparing `beanclerk-0.0.5/beanclerk/cli.py` & `beanclerk-0.0.6/beanclerk/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,45 +34,34 @@
     ctx.obj["config_file"] = config_file
 
 
 _ISO_DATE_FMT: str = "YYYY-MM-DD"
 
 
 class Date(click.ParamType):
-    """A convenience date type for Click.
+    """A convenience date type for Click."""
 
-    Converts dates to a date (instead of datetime).
-    """
-
-    name = "date"
+    name = _ISO_DATE_FMT
 
     def convert(self, value, param, ctx):  # noqa: D102
         if isinstance(value, date):
             return value
         try:
             return date.fromisoformat(value)
         except ValueError:
             self.fail(
-                f"'{value}' is not a valid date format ({_ISO_DATE_FMT})",
+                f"'{value}' is not a valid ISO date format: {_ISO_DATE_FMT}",
                 param,
                 ctx,
             )
 
 
 @cli.command("import")
-@click.option(
-    "--from-date",
-    type=Date(),
-    help=f"The first date to import ({_ISO_DATE_FMT}).",
-)
-@click.option(
-    "--to-date",
-    type=Date(),
-    help=f"The last date to import ({_ISO_DATE_FMT}).",
-)
+@click.option("--from-date", type=Date(), help="The first date to import.")
+@click.option("--to-date", type=Date(), help="The last date to import.")
 @click.pass_context
 def import_(ctx: click.Context, from_date: Date, to_date: Date) -> None:
     """Import transactions and check the current balance."""
     try:
         import_transactions(
             config_file=ctx.obj["config_file"],
             from_date=from_date,
```

### Comparing `beanclerk-0.0.5/beanclerk/config.py` & `beanclerk-0.0.6/beanclerk/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pathlib import Path
 from typing import Any
 
 import yaml
 from pydantic import BaseModel, ConfigDict, ValidationError, field_validator
 from pydantic_settings import BaseSettings
 
-from .bean_helpers import check_account_name
+from .bean_helpers import validate_account_name
 from .exceptions import ConfigError
 from .importers import ApiImporterProtocol
 
 
 class _BaseModelStrict(BaseModel):
     model_config = ConfigDict(extra="forbid")
 
@@ -38,23 +38,35 @@
     importer: str
 
     model_config = ConfigDict(extra="allow")  # allows access to extra fields
 
     @field_validator("account")
     def name_is_valid(cls, name: str) -> str:
         """Validate account name."""
-        check_account_name(name)
+        validate_account_name(name)
         return name
 
 
 class MatchCategories(_BaseModelStrict):
     """Match categories model."""
 
     metadata: dict[str, str]
 
+    @field_validator("metadata")
+    def metadata_is_valid(cls, metadata: dict[str, str]) -> dict[str, str]:
+        """Validate metadata."""
+        if not metadata:
+            raise ValueError("No patterns in metadata")
+        for pattern in metadata.values():
+            if pattern == "":
+                raise ValueError("Dangerous pattern: empty string matches everything")
+            if pattern.startswith("|"):
+                raise ValueError("Dangerous pattern: regex '|...' matches everything")
+        return metadata
+
 
 class CategorizationRule(_BaseModelStrict):
     """Categorization rule model."""
 
     matches: MatchCategories
     account: str
     flag: str | None = None
```

### Comparing `beanclerk-0.0.5/beanclerk/exceptions.py` & `beanclerk-0.0.6/beanclerk/exceptions.py`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.5/beanclerk/importers/banka_creditas.py` & `beanclerk-0.0.6/beanclerk/importers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,54 @@
-"""Banka Creditas a.s.
+"""API Importer Protocol and utilities for custom importers."""
 
-Todo:
-    This module is a work in progress. It needs a major rework.
-
-docs:
-    https://www.creditas.cz/firma/creditas-api/
-"""
-
-import base64
+import abc
 from datetime import date
 from decimal import Decimal
+from typing import Any
 
-import creditas
 from beancount.core.data import Amount, Transaction
 from beancount.core.flags import FLAG_WARNING
 from lxml import etree
 
 from ..bean_helpers import create_posting, create_transaction
-from . import prepare_meta
 
+TransactionReport = tuple[list[Transaction], Amount]
 
-def _get_transactions(token: str, account_id: str, from_date: date) -> bytes:
-    # Creditas API v 1.0.0:
-    # Manually generated token can be used only with the following URLs (and
-    # the corresponding methods):
-    #   /account/current/get
-    #   /account/savings/get
-    #   /account/balance/get
-    #   /account/transaction/search
-    #   /account/transaction/export
-    #   /account/statement/list
-    #   /account/statement/get
-
-    config = creditas.Configuration()
-    config.access_token = token
-    api = creditas.TransactionApi(creditas.ApiClient(config))
-    body = creditas.Body8(
-        account_id=account_id,
-        format="XML",
-        filter=creditas.AccountTransactionFilter(date_from=from_date),
-    )
-    # TODO: handle creditas.rest.ApiException
-    data: creditas.InlineResponse20011 = api.d_ps_account_transaction_export_api(
-        body=body,
-    )
-    # TODO: handle other exceptions
-    return base64.b64decode(data.export)
 
+def prepare_meta(d: dict[str, Any]) -> dict[str, str]:
+    """Return a dict of metadata for a Beancount transaction.
+
+    Args:
+        d (dict[str, Any]): a dict of values
+
+    Returns:
+        dict[str, str]: a dict of metadata
+    """
+    meta = {}
+    for k, v in d.items():
+        if not (v is None or v == ""):
+            meta[k] = str(v)
+    return meta
 
-# FIXME: This function has to be turned into a class implementing ApiImporterProtocol.
-def get_transactions(  # noqa: D103
-    token: str,
-    account_id: str,
-    bean_account: str,
-    from_date: date,
-) -> tuple[list[Transaction], Amount]:
+
+def parse_camt_053_001_02(xml: bytes, bean_account: str) -> TransactionReport:
+    """Return a tuple with a list of Beancount transactions and the current balance.
+
+    Args:
+        xml (bytes): bytes with the XML data (camt.053.001.02)
+            https://cbaonline.cz/formaty-xml-pro-vzajemnou-komunikaci-bank-s-klienty
+        bean_account (str): a Beancount account name
+
+    Returns:
+        TransactionReport: A tuple with the list of transactions and
+            the current balance.
+    """
     # TODO: handle etree.XMLSyntaxError
     # TODO: handle other exceptions
-    xml_root = etree.fromstring(  # noqa: S320
-        _get_transactions(token, account_id, from_date),
-    )
+    xml_root = etree.fromstring(xml)  # noqa: S320
     nsmap = xml_root.nsmap
 
     # TODO: handle other exceptions
     # TODO: raise if not found
     def get_amount(element) -> Amount:
         amount = element.find("./Amt", nsmap)
         number = Decimal(amount.text)
@@ -87,37 +72,35 @@
         "./TxsSummry/TtlNtries/NbOfNtries",
         raise_if_none=True,
     )
     if num_entries == 0:
         return ([], balance)
     txns: list[Transaction] = []
     for entry in statement.findall("./Ntry", nsmap):
+        # Related party may be a debitor or a creditor.
         if get_text(entry, "./CdtDbtInd", raise_if_none=True) == "DBIT":
-            # Whether the related party is a debitor or a creditor.
             ind = "Cdtr"
         else:
             ind = "Dbtr"
         details = "./NtryDtls/TxDtls"
-        # TODO: change `transaction_id` to `id` and `recipient_message`
-        #   to `remittance_info`
         meta = prepare_meta(
             {
-                "transaction_id": get_text(entry, "./NtryRef", raise_if_none=True),
+                "id": get_text(entry, "./NtryRef", raise_if_none=True),
                 "account_id": get_text(
                     entry,
                     f"{details}/RltdPties/{ind}Acct/Id/Othr/Id",
                 ),
                 "bank_id": get_text(
                     entry,
                     f"{details}/RltdAgts/{ind}Agt/FinInstnId/Othr/Id",
                 ),
                 "ks": get_text(entry, f"{details}/Refs/InstrId"),
                 "vs": get_text(entry, f"{details}/Refs/EndToEndId"),
                 "ss": get_text(entry, f"{details}/Refs/PmtInfId"),
-                "recipient_message": get_text(entry, f"{details}/RmtInf/Ustrd"),
+                "remittance_info": get_text(entry, f"{details}/RmtInf/Ustrd"),
                 "executor": get_text(entry, f"{details}/RltdPties/{ind}/Nm"),
             },
         )
         txns.append(
             create_transaction(
                 _date=date.fromisoformat(
                     get_text(
@@ -132,8 +115,37 @@
                         account=bean_account,
                         units=get_amount(entry),
                     ),
                 ],
                 meta=meta,
             ),
         )
+        txns.sort(key=lambda txn: txn.date)
     return (txns, balance)
+
+
+class ApiImporterProtocol(abc.ABC):
+    """API Importer Protocol for custom importers.
+
+    All API importers must comply with this interface. Make sure to implement
+    all methods decorated with `@abc.abstractmethod`. There are no restrictions
+    on other methods, variables or properties.
+    """
+
+    @abc.abstractmethod
+    def fetch_transactions(
+        self,
+        bean_account: str,
+        from_date: date,
+        to_date: date,
+    ) -> TransactionReport:
+        """Return a tuple with a list of Beancount transactions and the current balance.
+
+        Args:
+            bean_account (str): a Beancount account name
+            from_date (date): the first date to import
+            to_date (date): the last date to import
+
+        Returns:
+            TransactionReport: A tuple with the list of transactions and
+                the current balance.
+        """
```

### Comparing `beanclerk-0.0.5/beanclerk/importers/fio_banka.py` & `beanclerk-0.0.6/beanclerk/importers/fio_banka.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,25 +19,26 @@
 class ApiImporter(ApiImporterProtocol):
     """API importer for Fio banka, a.s."""
 
     def __init__(self, token: str) -> None:
         """Initialize the importer.
 
         Args:
-            token (str): _description_
+            token (str): API token
         """
         self._token = token
 
     def fetch_transactions(  # noqa: D102
         self,
         bean_account: str,
         from_date: date,
         to_date: date,
     ) -> TransactionReport:
         client = fio_banka.Account(self._token)
+        # TODO: handle exceptions
         statement = client.periods(from_date, to_date, fio_banka.TransactionsFmt.JSON)
 
         txns: list[Transaction] = []
         for txn in fio_banka.get_transactions(statement):
             txns.append(
                 create_transaction(
                     _date=txn.date,
```

### Comparing `beanclerk-0.0.5/beanclerk.egg-info/PKG-INFO` & `beanclerk-0.0.6/beanclerk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanclerk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automation for Beancount
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -371,43 +371,43 @@
 [![license](https://img.shields.io/pypi/l/beanclerk)](https://pypi.org/project/beanclerk/)
 [![python versions](https://img.shields.io/pypi/pyversions/beanclerk)](https://pypi.org/project/beanclerk/)
 [![ci tests](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml/badge.svg)](https://github.com/peberanek/beanclerk/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/beanclerk/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/beanclerk/main)
 
 ## Description
 
-Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance), automating some areas not addressed by Beancount itself, namely:
+Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance). It automates some areas not addressed by Beancount itself, namely:
 
-1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As some financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import process from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) that aims to support any compatible API.
+1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) to support any compatible API.
 1. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
     * As the first step, Beanclerk provides a way to define rules for automated categorization.
     * The future step is to augment it by machine-learning capabilities (e.g. via integration of the [Smart Importer](https://github.com/beancount/smart_importer)). (Btw, it might be also interesting to use machine-learning to discover hidden patterns or to provide predictions about our financial behavior.)
-1. _Automatic insertion of new transactions_: Beanclerk _appends_ new transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about the precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) can sort them out anyway.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes transparent and easy to review.
+1. _Automatic insertion of new transactions_: Beanclerk _appends_ transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about a precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) sort and filter them effectively.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes easy to review.
 
 **Beanclerk is still a rather 'rough' prototype.** You may encounter some unhandled exceptions and the API may change significantly in the future.
 
 **Beanclerk is currently tested on Linux only.**
 
 ### Existing importers
 
-Currently, there is 1 built-in importer for [Fio banka](https://www.fio.cz/). I plan to add another for [Banka Creditas](https://www.creditas.cz/), and, maybe, for some crypto exchanges. (All importers may move into separate repos in the future so the user may install only those they actually need).
+Beanclerk provides 2 built-in importers for [Fio banka](https://www.fio.cz/) and for [Banka Creditas](https://www.creditas.cz/). I plan to add another for some crypto exchanges. (All importers may move into separate repos in the future so you can install only those you actually need). Moreover, Beanclerk is designed in such a way to import importers (Python classes) from your working directory (this feature is not enabled yet).
 
 ### Notes
 
-I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
+I started Beanclerk primarily to try out some Python packages and to get better in programming by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
 
 * [beancount-import](https://github.com/jbms/beancount-import): Web UI for semi-automatically importing external data into beancount.
 * [finance-dl](https://github.com/jbms/finance-dl): Tools for automatically downloading/scraping personal financial data.
 * [beancount_reds_importers](https://github.com/redstreet/beancount_reds_importers): Simple ingesting tools for Beancount (plain text, double entry accounting software). More importantly, a framework to allow you to easily write your own importers.
 * [smart_importer](https://github.com/beancount/smart_importer): Augment Beancount importers with machine learning functionality.
 * [autobean](https://github.com/SEIAROTg/autobean): A collection of plugins and scripts that help automating bookkeeping with beancount.
 
 ## Installation
 
-Beanclerk requires Beancount, that may need some additional steps for its installation. See [Beancount Download & Installation](https://github.com/beancount/beancount#download--installation). Then, install Beanclerk via pip:
+Beanclerk requires Beancount, that may need some additional steps for its build and installation. See [Beancount Download & Installation](https://github.com/beancount/beancount#download--installation). Then, install Beanclerk via pip:
 
 ```
 pip install beanclerk
 ```
 
 Or, you may use [pipx](https://github.com/pypa/pipx) to install Beanclerk in an isolated environment:
 ```
@@ -423,23 +423,24 @@
 
 ### Configuration
 
 Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory. Or, set a path to the config file via the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
 
 ### Running the import
 
-Beanclerk currently implements a single command `import`. When running it for the first time, it is necessary to use at least the `--from-date` option to set the date to start the import from. (At the moment, Beanclerk runs import for all configured accounts.)
+Beanclerk implements a single command `import`. When running it for the first time, it is necessary to use the `--from-date` option to set the date to start the import from. (Beanclerk runs import for all configured accounts.)
 
 ```
 bean-clerk import --from-date 2023-01-01
 ```
 
-Once Beanclerk encounters a transaction without a matching categorization rule, it prompts the user to resolve the situation:
+Once Beanclerk encounters a transaction without a matching categorization rule, it prompts you to resolve the situation:
 
 ```
+Importing transactions for account: 'Assets:Banks:Fio:Checking'
 ...
 No categorization rule matches the following transaction:
 Transaction(
     meta={
         'id': '10000000002',
         'account_id': '2345678901',
         'account_name': 'Pavel, Žák',
@@ -470,17 +471,23 @@
 )
 Available actions:
 'r': reload config (you should add a new rule first)
 'i': import as-is (transaction remains unbalanced)
 ...
 ```
 
+After all new transactions from an account are imported, Beanclerk prints the import status:
+```
+...
+New transactions: 3, balance OK: 2000.10
+```
+
 ## Contributing
 
-Contributions are welcome. Make sure to create an issue first so we can discuss it.
+Contributions are welcome. As changes to the project are still rather dynamic, make sure to create an issue first so we can discuss it.
 
 Set up a development environment for playing with the source code:
 ```bash
 ./build_venv
 source venv/bin/activate
 pre-commit install  # https://pre-commit.com/
 ```
```

### Comparing `beanclerk-0.0.5/beanclerk.egg-info/SOURCES.txt` & `beanclerk-0.0.6/beanclerk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.5/pyproject.toml` & `beanclerk-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.5/tests/beanclerk-config.yml` & `beanclerk-0.0.6/tests/beanclerk-config.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 ---
-# `vars` section is completely optional. It may be useful for defining YAML
-# anchors (https://support.atlassian.com/bitbucket-cloud/docs/yaml-anchors/)
+# `vars` section is optional and may define any data structure you need. It
+# may be useful for defining YAML anchors
+# (https://support.atlassian.com/bitbucket-cloud/docs/yaml-anchors/)
 # to reuse common values.
 vars:
   fio_importer: &fio_importer "beanclerk.importers.fio_banka.ApiImporter"
 
 # A Beancount ledger; path may be relative or absolute, may include ~ or env vars.
 input_file: "${TEST_DIR}/ledger.beancount"
 
-accounts: # Acounts to import data to.
+accounts: # Acounts managed by Beanclerk
   - account: "Assets:Banks:Fio:Checking" # an existing Beancount account
-    # `importer` points to an importable Python class that implements ApiImporterProtocol
+    # `importer` points to an importable class that implements ApiImporterProtocol
     importer: "beanclerk.importers.fio_banka.ApiImporter"
     # `account` and `importer` are required. All other keys provide an importer-specific
-    # configuration. (It must be described by the importer.)
+    # configuration. (It should be documented by the importer.)
     token: "testKeyFVqI4dagXgi1eB1cgLzNjwsWS36bGXZVZPOJ4pMrdnPleaUcdUlqy2LqF"
 
   - account: "Assets:Banks:Fio:Savings"
     importer: *fio_importer # YAML alias (points to a YAML anchor)
     token: "testKeyXZVZPOJ4pMrdnPleaUcdUlqy2LqFFVqI4dagXgi1eB1cgLzNjwsWS36bG"
 
-# `categorization_rules` section is optional, however, Beanclerk prompts the user
+# `categorization_rules` section is optional, however, Beanclerk prompts you
 # once it encounters an uncategorized transaction.
 categorization_rules:
   # 1 example rule
   - matches:
       # `metadata` section contains any metadata that an importer might assign
       # to a transaction (like `bank_id` etc.). All must match.
       metadata:
         ks: "05\\d{2}" # supports regex
     # Missing values to be added to the transaction:
-    account: "Expenses:Todo" # an arbitrary Beancount account (may or may not exist)
+    account: "Expenses:Todo" # an arbitrary Beancount account (it may or may not exist)
     flag: "!" # optional (https://github.com/beancount/beancount/blob/master/beancount/core/flags.py)
     payee: "My payee" # optional
     narration: "My narration" # optional
```

### Comparing `beanclerk-0.0.5/tests/conftest.py` & `beanclerk-0.0.6/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import os
 import shutil
 from pathlib import Path
 
 import fio_banka
 import pytest
 
+from beanclerk.importers.banka_creditas import ApiImporter
+
 TOP_DIR = Path(os.path.realpath(__file__)).parent
 
 
 @pytest.fixture()
 def _mock_fio_banka(monkeypatch: pytest.MonkeyPatch):
     """Mock fio_banka package."""
 
@@ -17,14 +19,31 @@
         with (TOP_DIR / "importers" / "fio_banka_transactions.json").open("r") as file:
             return file.read()
 
     monkeypatch.setattr(fio_banka.Account, "_request", mock__request)
 
 
 @pytest.fixture()
+def _mock_creditas_api_importer(monkeypatch: pytest.MonkeyPatch):
+    """Mock beanclerk.importers.banka_creditas.ApiImporter.
+
+    creditas pkg does not seem to be easy to mock, mock some of the importer
+    methods instead.
+    """
+
+    def mock__fetch_transactions(*args, **kwargs) -> bytes:
+        with (TOP_DIR / "importers" / "banka_creditas_transactions.xml").open(
+            "rb",
+        ) as file:
+            return file.read()
+
+    monkeypatch.setattr(ApiImporter, "_fetch_transactions", mock__fetch_transactions)
+
+
+@pytest.fixture()
 def config_file(tmp_path, monkeypatch: pytest.MonkeyPatch) -> Path:
     """Return path to the config file."""
     monkeypatch.setenv("TEST_DIR", str(tmp_path))
     return Path(shutil.copy(TOP_DIR / "beanclerk-config.yml", tmp_path))
 
 
 @pytest.fixture()
```

### Comparing `beanclerk-0.0.5/tests/importers/banka_creditas_transactions.xml` & `beanclerk-0.0.6/tests/importers/banka_creditas_transactions.xml`

 * *Files 0% similar despite different names*

#### Comparing `beanclerk-0.0.5/tests/importers/banka_creditas_transactions.xml` & `beanclerk-0.0.6/tests/importers/banka_creditas_transactions.xml`

```diff
@@ -43,15 +43,15 @@
       <TxsSummry>
         <TtlNtries>
           <NbOfNtries>1</NbOfNtries>
         </TtlNtries>
       </TxsSummry>
       <Ntry>
         <NtryRef>RLZ-1000000000</NtryRef>
-        <Amt Ccy="CZK">1</Amt>
+        <Amt Ccy="CZK">100.99</Amt>
         <CdtDbtInd>CRDT</CdtDbtInd>
         <RvslInd>false</RvslInd>
         <Sts>BOOK</Sts>
         <BookgDt>
           <Dt>2023-01-01</Dt>
         </BookgDt>
         <BkTxCd>
```

### Comparing `beanclerk-0.0.5/tests/importers/fio_banka_transactions.json` & `beanclerk-0.0.6/tests/importers/fio_banka_transactions.json`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.5/tests/importers/test_fio_banka.py` & `beanclerk-0.0.6/tests/importers/test_fio_banka.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,114 +5,119 @@
 from beancount.core.data import Amount, Posting, Transaction
 
 from beanclerk.importers.fio_banka import ApiImporter
 
 pytestmark = pytest.mark.usefixtures("_mock_fio_banka")
 
 
-def test_get_transactions():
-    bean_account = "Assets:Account"
-    importer = ApiImporter(
+class TestApiImporter:
+    """Test ApiImporter."""
+
+    IMPORTER = ApiImporter(
         token="testKeyXZVZPOJ4pMrdnPleaUcdUlqy2LqFFVqI4dagXgi1eB1cgLzNjwsWS36bG",
     )
-    txns, balance = importer.fetch_transactions(
-        bean_account=bean_account,
-        from_date=date(2023, 1, 1),
-        to_date=date(2023, 1, 1),
-    )
-    assert balance.number == Decimal("2000.10")
-    assert balance.currency == "CZK"
-    for txn in txns:
-        match txn.meta["id"]:
-            case "10000000000":
-                assert txn == Transaction(
-                    meta={
-                        "id": "10000000000",
-                        "vs": "1000",
-                        "user_identification": "Nákup: example.com, dne 31.12.2022, částka  20.00 USD",  # noqa: E501
-                        "remittance_info": "Nákup: example.com, dne 31.12.2022, částka  20.00 USD",  # noqa: E501
-                        "type": "Platba kartou",
-                        "executor": "Novák, Jan",
-                        "comment": "Nákup: example.com, dne 31.12.2022, částka  20.00 USD",  # noqa: E501
-                        "order_id": "30000000000",
-                    },
-                    date=date(2023, 1, 1),
-                    flag="*",
-                    payee=None,
-                    narration="",
-                    tags=frozenset(),
-                    links=frozenset(),
-                    postings=[
-                        Posting(
-                            account=bean_account,
-                            units=Amount(Decimal("2000.0"), "CZK"),
-                            cost=None,
-                            price=None,
-                            flag=None,
-                            meta={},
-                        ),
-                    ],
-                )
-            case "10000000001":
-                assert txn == Transaction(
-                    meta={
-                        "id": "10000000001",
-                        "account_id": "9876543210",
-                        "bank_id": "0800",
-                        "bank_name": "Česká spořitelna, a.s.",
-                        "ks": "0558",
-                        "vs": "0001",
-                        "ss": "0002",
-                        "type": "Okamžitá odchozí platba",
-                        "executor": "Novák, Jan",
-                        "order_id": "30000000001",
-                    },
-                    date=date(2023, 1, 2),
-                    flag="*",
-                    payee=None,
-                    narration="",
-                    tags=frozenset(),
-                    links=frozenset(),
-                    postings=[
-                        Posting(
-                            account=bean_account,
-                            units=Amount(Decimal("-1500.89"), "CZK"),
-                            cost=None,
-                            price=None,
-                            flag=None,
-                            meta={},
-                        ),
-                    ],
-                )
-            case "10000000002":
-                assert txn == Transaction(
-                    meta={
-                        "id": "10000000002",
-                        "account_id": "2345678901",
-                        "account_name": "Pavel, Žák",
-                        "bank_id": "2010",
-                        "bank_name": "Fio banka, a.s.",
-                        "type": "Příjem převodem uvnitř banky",
-                        "specification": "test specification",
-                        "bic": "TESTBICXXXX",
-                        "order_id": "30000000002",
-                        "payer_reference": "test payer reference",
-                    },
-                    date=date(2023, 1, 3),
-                    flag="*",
-                    payee=None,
-                    narration="",
-                    tags=frozenset(),
-                    links=frozenset(),
-                    postings=[
-                        Posting(
-                            account=bean_account,
-                            units=Amount(Decimal("500.0"), "CZK"),
-                            cost=None,
-                            price=None,
-                            flag=None,
-                            meta={},
-                        ),
-                    ],
-                )
-            case _ as _id:
-                pytest.fail(f"Unexpected transaction ID: {_id}")
+
+    def test_get_transactions(self):
+        """Test get_transactions."""
+        bean_account = "Assets:Account"
+        txns, balance = self.IMPORTER.fetch_transactions(
+            bean_account=bean_account,
+            from_date=date(2023, 1, 1),
+            to_date=date(2023, 1, 1),
+        )
+        assert balance.number == Decimal("2000.10")
+        assert balance.currency == "CZK"
+        for txn in txns:
+            match txn.meta["id"]:
+                case "10000000000":
+                    assert txn == Transaction(
+                        meta={
+                            "id": "10000000000",
+                            "vs": "1000",
+                            "user_identification": "Nákup: example.com, dne 31.12.2022, částka  20.00 USD",  # noqa: E501
+                            "remittance_info": "Nákup: example.com, dne 31.12.2022, částka  20.00 USD",  # noqa: E501
+                            "type": "Platba kartou",
+                            "executor": "Novák, Jan",
+                            "comment": "Nákup: example.com, dne 31.12.2022, částka  20.00 USD",  # noqa: E501
+                            "order_id": "30000000000",
+                        },
+                        date=date(2023, 1, 1),
+                        flag="*",
+                        payee=None,
+                        narration="",
+                        tags=frozenset(),
+                        links=frozenset(),
+                        postings=[
+                            Posting(
+                                account=bean_account,
+                                units=Amount(Decimal("2000.0"), "CZK"),
+                                cost=None,
+                                price=None,
+                                flag=None,
+                                meta={},
+                            ),
+                        ],
+                    )
+                case "10000000001":
+                    assert txn == Transaction(
+                        meta={
+                            "id": "10000000001",
+                            "account_id": "9876543210",
+                            "bank_id": "0800",
+                            "bank_name": "Česká spořitelna, a.s.",
+                            "ks": "0558",
+                            "vs": "0001",
+                            "ss": "0002",
+                            "type": "Okamžitá odchozí platba",
+                            "executor": "Novák, Jan",
+                            "order_id": "30000000001",
+                        },
+                        date=date(2023, 1, 2),
+                        flag="*",
+                        payee=None,
+                        narration="",
+                        tags=frozenset(),
+                        links=frozenset(),
+                        postings=[
+                            Posting(
+                                account=bean_account,
+                                units=Amount(Decimal("-1500.89"), "CZK"),
+                                cost=None,
+                                price=None,
+                                flag=None,
+                                meta={},
+                            ),
+                        ],
+                    )
+                case "10000000002":
+                    assert txn == Transaction(
+                        meta={
+                            "id": "10000000002",
+                            "account_id": "2345678901",
+                            "account_name": "Pavel, Žák",
+                            "bank_id": "2010",
+                            "bank_name": "Fio banka, a.s.",
+                            "type": "Příjem převodem uvnitř banky",
+                            "specification": "test specification",
+                            "bic": "TESTBICXXXX",
+                            "order_id": "30000000002",
+                            "payer_reference": "test payer reference",
+                        },
+                        date=date(2023, 1, 3),
+                        flag="*",
+                        payee=None,
+                        narration="",
+                        tags=frozenset(),
+                        links=frozenset(),
+                        postings=[
+                            Posting(
+                                account=bean_account,
+                                units=Amount(Decimal("500.0"), "CZK"),
+                                cost=None,
+                                price=None,
+                                flag=None,
+                                meta={},
+                            ),
+                        ],
+                    )
+                case _ as _id:
+                    pytest.fail(f"Unexpected transaction ID: {_id}")
```

### Comparing `beanclerk-0.0.5/tests/test_clerk.py` & `beanclerk-0.0.6/tests/test_clerk.py`

 * *Files identical despite different names*

