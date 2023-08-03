# Comparing `tmp/ghastoolkit-0.7.0.tar.gz` & `tmp/ghastoolkit-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.7.0.tar", last modified: Fri Jul 28 14:57:47 2023, max compression
+gzip compressed data, was "ghastoolkit-0.7.2.tar", last modified: Thu Aug  3 14:39:46 2023, max compression
```

## Comparing `ghastoolkit-0.7.0.tar` & `ghastoolkit-0.7.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.194078 ghastoolkit-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-28 14:57:47.194078 ghastoolkit-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:57:47.194078 ghastoolkit-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.186078 ghastoolkit-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.186078 ghastoolkit-0.7.0/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/codeql/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.190078 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 14:57:47.000000 ghastoolkit-0.7.0/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:57:47.194078 ghastoolkit-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_codeql_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-28 14:57:18.000000 ghastoolkit-0.7.0/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.391044 ghastoolkit-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-03 14:39:46.391044 ghastoolkit-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:39:46.391044 ghastoolkit-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.379043 ghastoolkit-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.379043 ghastoolkit-0.7.2/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.383043 ghastoolkit-0.7.2/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.383043 ghastoolkit-0.7.2/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.383043 ghastoolkit-0.7.2/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.387044 ghastoolkit-0.7.2/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.387044 ghastoolkit-0.7.2/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.387044 ghastoolkit-0.7.2/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.387044 ghastoolkit-0.7.2/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.383043 ghastoolkit-0.7.2/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-03 14:39:46.000000 ghastoolkit-0.7.2/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-03 14:39:46.000000 ghastoolkit-0.7.2/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:39:46.000000 ghastoolkit-0.7.2/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 14:39:46.000000 ghastoolkit-0.7.2/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 14:39:46.000000 ghastoolkit-0.7.2/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:39:46.387044 ghastoolkit-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_codeql_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-03 14:39:08.000000 ghastoolkit-0.7.2/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.7.0/LICENSE` & `ghastoolkit-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/PKG-INFO` & `ghastoolkit-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.7.0
+Version: 0.7.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.7.0/README.md` & `ghastoolkit-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/pyproject.toml` & `ghastoolkit-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.7.0"
+version = "0.7.2"
 authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/__init__.py` & `ghastoolkit-0.7.2/src/ghastoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """GitHub Advanced Security Toolkit."""
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/__main__.py` & `ghastoolkit-0.7.2/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/__main__.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/packs/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/pack.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/packs/pack.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/packs/packs.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/packs/packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.7.2/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/advisories.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Dependency Graph Octokit."""
 import logging
-from typing import Any
+from typing import Any, Dict
 import urllib.parse
 
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.supplychain.advisories import Advisory
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 from ghastoolkit.supplychain.dependencies import Dependencies, Dependency
 from ghastoolkit.octokit.octokit import GraphQLRequest, Optional, RestRequest
@@ -25,14 +25,37 @@
         self.repository = repository or GitHub.repository
         self.rest = RestRequest(repository)
         self.graphql = GraphQLRequest(repository)
 
         self.enable_graphql = enable_graphql
         self.enable_clearlydefined = enable_clearlydefined
 
+    def getOrganizationDependencies(self) -> Dict[Repository, Dependencies]:
+        """Get Organization Dependencies."""
+        deps = {}
+
+        repositories = self.rest.get("/orgs/{org}/repos")
+        if not isinstance(repositories, list):
+            raise Exception("Invalid organization")
+
+        for repo in repositories:
+            repo = Repository.parseRepository(repo.get("full_name"))
+            logger.debug(f"Processing repository :: {repo}")
+            try:
+                self.rest = RestRequest(repo)
+
+                repo_deps = self.getDependenciesSbom()
+                deps[repo] = repo_deps
+            except Exception as err:
+                logger.warning(f"Failed to get dependencies :: {err}")
+                deps[repo] = Dependencies()
+
+        self.rest = RestRequest(self.repository)
+        return deps
+
     def getDependencies(self) -> Dependencies:
         """Get Dependencies."""
         deps = self.getDependenciesSbom()
 
         if self.enable_graphql:
             logger.debug("Enabled GraphQL Dependencies")
             graph_deps = self.getDependenciesGraphQL()
@@ -120,20 +143,26 @@
     def getDependenciesInPR(self, base: str, head: str) -> Dependencies:
         """Get all the dependencies from a Pull Request."""
         dependencies = Dependencies()
         base = urllib.parse.quote(base, safe="")
         head = urllib.parse.quote(head, safe="")
         basehead = f"{base}...{head}"
         logger.debug(f"PR basehead :: {basehead}")
+
         results = self.rest.get(
             "/repos/{owner}/{repo}/dependency-graph/compare/{basehead}",
             {"basehead": basehead},
             expected=200,
         )
+
         if not results:
+            logger.warning("Failed to get dependencies from Pull Request")
+            logger.warning(
+                "Make sure Advanced Security is enabled and token permissions are correct"
+            )
             return dependencies
 
         for depdata in results:
             if depdata.get("change_type") == "removed":
                 continue
 
             purl = depdata.get("package_url")
```

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.7.2/src/ghastoolkit/octokit/secretscanning.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,34 @@
 
 
 @dataclass
 class SecretAlert(OctoItem):
     """Secret Scanning Alert."""
 
     number: int
+    """Number / Identifier"""
     state: str
+    """Alert State"""
 
     created_at: str
+    """Created Timestamp"""
 
     secret_type: str
+    """Secret Scanning type"""
     secret_type_display_name: str
+    """Secret Scanning type display name"""
     secret: str
+    """Secret value (sensitive)"""
 
     _locations: list[dict] = field(default_factory=list)
     _sha: Optional[str] = None
 
     @property
     def locations(self) -> list[dict]:
-        """Get Alert locations.
-
-        Use cache or request from API."""
+        """Get Alert locations. Uses a cached version or request from API."""
         if not self._locations:
             self._locations = SecretScanning().getAlertLocations(self.number)
         return self._locations
 
     @property
     def commit_sha(self) -> Optional[str]:
         """Get commit sha if present."""
```

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.7.2/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.7.2/src/ghastoolkit/supplychain/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.7.2/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.7.2/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.7.2/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.7.2/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.7.0
+Version: 0.7.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.7.0/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.7.2/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_advisories.py` & `ghastoolkit-0.7.2/tests/test_advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_codeql_dataext.py` & `ghastoolkit-0.7.2/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_codeql_packs.py` & `ghastoolkit-0.7.2/tests/test_codeql_packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_codeqldb.py` & `ghastoolkit-0.7.2/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_codescanning.py` & `ghastoolkit-0.7.2/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_default.py` & `ghastoolkit-0.7.2/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_dependencies.py` & `ghastoolkit-0.7.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_depgraph.py` & `ghastoolkit-0.7.2/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_github.py` & `ghastoolkit-0.7.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_licenses.py` & `ghastoolkit-0.7.2/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_octokit.py` & `ghastoolkit-0.7.2/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.7.0/tests/test_secretscanning.py` & `ghastoolkit-0.7.2/tests/test_secretscanning.py`

 * *Files identical despite different names*

