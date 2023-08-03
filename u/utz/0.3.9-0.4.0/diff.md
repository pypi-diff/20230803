# Comparing `tmp/utz-0.3.9.tar.gz` & `tmp/utz-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/utz-0.3.9.tar", last modified: Fri Dec 25 17:37:07 2020, max compression
+gzip compressed data, was "utz-0.4.0.tar", last modified: Thu Aug  3 00:21:53 2023, max compression
```

## Comparing `utz-0.3.9.tar` & `utz-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.473667 utz-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (116)     3190 2020-12-25 17:37:07.473667 utz-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2238 2020-12-25 17:36:39.000000 utz-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-25 17:37:07.473667 utz-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      552 2020-12-25 17:36:39.000000 utz-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.469667 utz-0.3.9/utz/
--rw-r--r--   0 runner    (1001) docker     (116)     3920 2020-12-25 17:36:39.000000 utz-0.3.9/utz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      929 2020-12-25 17:36:39.000000 utz-0.3.9/utz/argparse.py
--rw-r--r--   0 runner    (1001) docker     (116)     3142 2020-12-25 17:36:39.000000 utz-0.3.9/utz/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     1422 2020-12-25 17:36:39.000000 utz-0.3.9/utz/backoff.py
--rw-r--r--   0 runner    (1001) docker     (116)     1880 2020-12-25 17:36:39.000000 utz-0.3.9/utz/bases.py
--rw-r--r--   0 runner    (1001) docker     (116)      409 2020-12-25 17:36:39.000000 utz-0.3.9/utz/cd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1695 2020-12-25 17:36:39.000000 utz-0.3.9/utz/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     1873 2020-12-25 17:36:39.000000 utz-0.3.9/utz/collections.py
--rw-r--r--   0 runner    (1001) docker     (116)     2145 2020-12-25 17:36:39.000000 utz-0.3.9/utz/context.py
--rw-r--r--   0 runner    (1001) docker     (116)     1183 2020-12-25 17:36:39.000000 utz-0.3.9/utz/df_counts.py
--rw-r--r--   0 runner    (1001) docker     (116)     6177 2020-12-25 17:36:39.000000 utz-0.3.9/utz/diff_dfs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.473667 utz-0.3.9/utz/docker/
--rw-r--r--   0 runner    (1001) docker     (116)       67 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      502 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/dsl.py
--rw-r--r--   0 runner    (1001) docker     (116)     5128 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/file.py
--rw-r--r--   0 runner    (1001) docker     (116)      327 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/image.py
--rw-r--r--   0 runner    (1001) docker     (116)      396 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.473667 utz-0.3.9/utz/git/
--rw-r--r--   0 runner    (1001) docker     (116)     1722 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      973 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/_checkout.py
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/branch.py
--rw-r--r--   0 runner    (1001) docker     (116)     4857 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/clone.py
--rw-r--r--   0 runner    (1001) docker     (116)      376 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)      314 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/head.py
--rw-r--r--   0 runner    (1001) docker     (116)     3315 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/remote.py
--rw-r--r--   0 runner    (1001) docker     (116)      333 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/submodule.py
--rw-r--r--   0 runner    (1001) docker     (116)      113 2020-12-25 17:36:39.000000 utz-0.3.9/utz/imports.py
--rw-r--r--   0 runner    (1001) docker     (116)      986 2020-12-25 17:36:39.000000 utz-0.3.9/utz/methods.py
--rw-r--r--   0 runner    (1001) docker     (116)     3211 2020-12-25 17:36:39.000000 utz-0.3.9/utz/o.py
--rw-r--r--   0 runner    (1001) docker     (116)      380 2020-12-25 17:36:39.000000 utz-0.3.9/utz/path.py
--rw-r--r--   0 runner    (1001) docker     (116)     2513 2020-12-25 17:36:39.000000 utz-0.3.9/utz/pdf.py
--rw-r--r--   0 runner    (1001) docker     (116)     3201 2020-12-25 17:36:39.000000 utz-0.3.9/utz/pnds.py
--rw-r--r--   0 runner    (1001) docker     (116)     3074 2020-12-25 17:36:39.000000 utz-0.3.9/utz/process.py
--rw-r--r--   0 runner    (1001) docker     (116)     3791 2020-12-25 17:36:39.000000 utz-0.3.9/utz/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     2197 2020-12-25 17:36:39.000000 utz-0.3.9/utz/sql.py
--rw-r--r--   0 runner    (1001) docker     (116)     1853 2020-12-25 17:36:39.000000 utz-0.3.9/utz/ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)      298 2020-12-25 17:36:39.000000 utz-0.3.9/utz/test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2611 2020-12-25 17:36:39.000000 utz-0.3.9/utz/time.py
--rw-r--r--   0 runner    (1001) docker     (116)      434 2020-12-25 17:36:39.000000 utz-0.3.9/utz/tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (116)     5941 2020-12-25 17:36:39.000000 utz-0.3.9/utz/use.py
--rw-r--r--   0 runner    (1001) docker     (116)      771 2020-12-25 17:36:39.000000 utz-0.3.9/utz/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.469667 utz-0.3.9/utz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3190 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      749 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      172 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.949671 utz-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 00:21:23.000000 utz-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-03 00:21:53.949671 utz-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 00:21:23.000000 utz-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:21:53.949671 utz-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-03 00:21:23.000000 utz-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.945671 utz-0.4.0/utz/
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-03 00:21:23.000000 utz-0.4.0/utz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 00:21:23.000000 utz-0.4.0/utz/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-03 00:21:23.000000 utz-0.4.0/utz/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-03 00:21:23.000000 utz-0.4.0/utz/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-03 00:21:23.000000 utz-0.4.0/utz/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 00:21:23.000000 utz-0.4.0/utz/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 00:21:23.000000 utz-0.4.0/utz/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 00:21:23.000000 utz-0.4.0/utz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-03 00:21:23.000000 utz-0.4.0/utz/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-03 00:21:23.000000 utz-0.4.0/utz/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 00:21:23.000000 utz-0.4.0/utz/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 00:21:23.000000 utz-0.4.0/utz/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-03 00:21:23.000000 utz-0.4.0/utz/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-03 00:21:23.000000 utz-0.4.0/utz/df_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-03 00:21:23.000000 utz-0.4.0/utz/diff_dfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.945671 utz-0.4.0/utz/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-03 00:21:23.000000 utz-0.4.0/utz/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-03 00:21:23.000000 utz-0.4.0/utz/fn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.949671 utz-0.4.0/utz/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 00:21:23.000000 utz-0.4.0/utz/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 00:21:23.000000 utz-0.4.0/utz/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-03 00:21:23.000000 utz-0.4.0/utz/o.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 00:21:23.000000 utz-0.4.0/utz/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 00:21:23.000000 utz-0.4.0/utz/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-03 00:21:23.000000 utz-0.4.0/utz/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-08-03 00:21:23.000000 utz-0.4.0/utz/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-03 00:21:23.000000 utz-0.4.0/utz/pnds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.949671 utz-0.4.0/utz/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-03 00:21:23.000000 utz-0.4.0/utz/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-03 00:21:23.000000 utz-0.4.0/utz/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-03 00:21:23.000000 utz-0.4.0/utz/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 00:21:23.000000 utz-0.4.0/utz/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 00:21:23.000000 utz-0.4.0/utz/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-03 00:21:23.000000 utz-0.4.0/utz/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-03 00:21:23.000000 utz-0.4.0/utz/tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-08-03 00:21:23.000000 utz-0.4.0/utz/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-03 00:21:23.000000 utz-0.4.0/utz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-03 00:21:23.000000 utz-0.4.0/utz/ym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-08-03 00:21:23.000000 utz-0.4.0/utz/ymd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 00:21:23.000000 utz-0.4.0/utz/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.945671 utz-0.4.0/utz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/top_level.txt
```

### Comparing `utz-0.3.9/PKG-INFO` & `utz-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 Metadata-Version: 2.1
 Name: utz
-Version: 0.3.9
-Summary: ("yoots"): common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
+Version: 0.4.0
+Summary: *("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
 Home-page: https://github.com/runsascoded/utz
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
-Description: # utz
-        *("yoots")*: common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
-        
-        ## Install
-        ```bash
-        pip install utz
-        ```
-        
-        ## Use
-        Import the whole kitchen sink:
-        ```python
-        from utz import *
-        ```
-        
-        See [__init__.py](utz/__init__.py), which imports many of the modules below, as well as a bevy of handy stdlib methods and objects.
-        
-        ## Features
-        Some noteworthy modules:
-        - [cd](utz/cd.py): "change directory" contextmanager
-        - [o](utz/o.py): `dict` wrapper exposing keys as attrs (e.g.: `o({'a':1}).a == 1`)
-        - [process](utz/process.py): subprocess wrappers for more easily shelling out to commands and parsing their stdout
-        - [docker](docker/): DSL for programmatically creating Dockerfiles (and building images from them)
-        - [ssh](utz/ssh.py): SSH tunnel wrapped in a context manager
-        - [time](utz/time.py): `now()`/`today()` helpers with convenient / no-nonsense ISO string serialization and UTC bias
-        - [bases](utz/bases.py): `int`⟺`str` codecs with improvements over standard base64 et al.
-        - [tmpdir](utz/tmpdir.py): make temporary directories with a specific basename
-        - [context](utz/context.py): context-manager helpers, including `ctxs` for composing multiple context managers
-        - [backoff](utz/backoff.py): simple exponential-backoff utility
-        - [git](utz/git): git helpers / wrappers around [GitPython](https://gitpython.readthedocs.io/en/stable/)
-        - [pnds](utz/pnds.py): common [pandas](https://pandas.pydata.org/) imports and helpers
-        - [collections](utz/collections.py): collection/list helpers
-        
-        ### auto-`setup.py`
-        [`utz/setup.py`](utz/setup.py) provides defaults for various `setuptools.setup()` params:
-        - `name`: use parent directory name
-        - `version`: parse from git tag (otherwise from `git describe --tags`)
-        - `author_{name,email}`: infer from last commit
-        - `long_description`: parse `README.md` (and set `long_description_content_type)
-        - `description`: parse first `<p>` under opening `<h1>` from `README.md`
-        - `license`: parse from `LICENSE` file (MIT and Apache v2 supported)
-        
-        For an example, see [`gsmo==0.0.1`](https://github.com/runsascoded/gsmo/blob/v0.0.1/setup.py) ([and corresponding release](https://pypi.org/project/gsmo/)).
-        
-        It can be installed via a pip extra:
-        ```bash
-        pip install utz[setup]
-        ``` 
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pdf
-Provides-Extra: setup
 Provides-Extra: test
+License-File: LICENSE
+
+# utz
+*("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
+
+## Install
+```bash
+pip install utz
+```
+
+## Use
+Import everything:
+```python
+from utz import *
+```
+
+See [`__init__.py`](utz/__init__.py), which imports many of the modules below, as well as a many standard-library methods and objects.
+
+## Features
+Some noteworthy modules:
+- [cd](utz/cd.py): "change directory" contextmanager
+- [o](utz/o.py): `dict` wrapper exposing keys as attrs (e.g.: `o({'a':1}).a == 1`)
+- [process](utz/process.py): subprocess wrappers for more easily shelling out to commands and parsing their stdout
+- [docker](docker/): DSL for programmatically creating Dockerfiles (and building images from them)
+- [ssh](utz/ssh.py): SSH tunnel wrapped in a context manager
+- [time](utz/time.py): `now()`/`today()` helpers with convenient / no-nonsense ISO string serialization and UTC bias
+- [bases](utz/bases.py): `int`⟺`str` codecs with improvements over standard base64 et al.
+- [tmpdir](utz/tmpdir.py): make temporary directories with a specific basename
+- [context](utz/context.py): contextmanager helpers, including `ctxs` for composing multiple context managers
+- [escape](utz/escape.py): escaping split/join helpers
+- [backoff](utz/backoff.py): simple exponential-backoff utility
+- [git](utz/git): git helpers / wrappers around [GitPython](https://gitpython.readthedocs.io/en/stable/)
+- [pnds](utz/pnds.py): common [pandas](https://pandas.pydata.org/) imports and helpers
+- [collections](utz/collections.py): collection/list helpers
+
+### auto-`setup.py`
+[`utz/setup.py`](utz/setup.py) provides defaults for various `setuptools.setup()` params:
+- `name`: use parent directory name
+- `version`: parse from git tag (otherwise from `git describe --tags`)
+- `author_{name,email}`: infer from last commit
+- `long_description`: parse `README.md` (and set `long_description_content_type)
+- `description`: parse first `<p>` under opening `<h1>` from `README.md`
+- `license`: parse from `LICENSE` file (MIT and Apache v2 supported)
+
+For an example, see [`gsmo==0.0.1`](https://github.com/runsascoded/gsmo/blob/v0.0.1/setup.py) ([and corresponding release](https://pypi.org/project/gsmo/)).
+
+It can be installed via a pip extra:
+```bash
+pip install utz[setup]
+``` 
+
+
```

### Comparing `utz-0.3.9/README.md` & `utz-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # utz
-*("yoots")*: common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
+*("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
 
 ## Install
 ```bash
 pip install utz
 ```
 
 ## Use
-Import the whole kitchen sink:
+Import everything:
 ```python
 from utz import *
 ```
 
-See [__init__.py](utz/__init__.py), which imports many of the modules below, as well as a bevy of handy stdlib methods and objects.
+See [`__init__.py`](utz/__init__.py), which imports many of the modules below, as well as a many standard-library methods and objects.
 
 ## Features
 Some noteworthy modules:
 - [cd](utz/cd.py): "change directory" contextmanager
 - [o](utz/o.py): `dict` wrapper exposing keys as attrs (e.g.: `o({'a':1}).a == 1`)
 - [process](utz/process.py): subprocess wrappers for more easily shelling out to commands and parsing their stdout
 - [docker](docker/): DSL for programmatically creating Dockerfiles (and building images from them)
 - [ssh](utz/ssh.py): SSH tunnel wrapped in a context manager
 - [time](utz/time.py): `now()`/`today()` helpers with convenient / no-nonsense ISO string serialization and UTC bias
 - [bases](utz/bases.py): `int`⟺`str` codecs with improvements over standard base64 et al.
 - [tmpdir](utz/tmpdir.py): make temporary directories with a specific basename
-- [context](utz/context.py): context-manager helpers, including `ctxs` for composing multiple context managers
+- [context](utz/context.py): contextmanager helpers, including `ctxs` for composing multiple context managers
+- [escape](utz/escape.py): escaping split/join helpers
 - [backoff](utz/backoff.py): simple exponential-backoff utility
 - [git](utz/git): git helpers / wrappers around [GitPython](https://gitpython.readthedocs.io/en/stable/)
 - [pnds](utz/pnds.py): common [pandas](https://pandas.pydata.org/) imports and helpers
 - [collections](utz/collections.py): collection/list helpers
 
 ### auto-`setup.py`
 [`utz/setup.py`](utz/setup.py) provides defaults for various `setuptools.setup()` params:
```

### Comparing `utz-0.3.9/utz/__init__.py` & `utz-0.4.0/utz/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 except ImportError:
     try:
         # Python ≤3.7; pip install cached-property
         from cached_property import cached_property
     except ImportError as e:
         pass
 
-import functools
-from functools import partial, lru_cache, namedtuple, reduce, singledispatch
+from functools import partial, lru_cache, namedtuple, reduce, singledispatch, wraps
 
 from glob import glob
 
 import hashlib
 from hashlib import md5, sha256
 
 import io
@@ -109,58 +108,76 @@
 
 from .backoff import backoff
 from .tmpdir import tmpdir
 
 from . import process
 from .process import *
 
+from . import fn
+from .fn import decos, args
+
 with _try:
     from . import pnds
     from .pnds import *
 
+from .cached_property import cached_property
+
 from .cd import cd
 
 from . import docker
 from .docker.dsl import *
 
 from .o import o
 from .use import use
+with _try:
+    from .ym import YM
+    from .ymd import YMD
 
 with _try:
-    from .git import Git, Repo, make_repo
+    from git import Git, Repo
+    from .git import make_repo
 
-from .args_parser import *
+from .git import github
 
 from .context import *
 
 with _try:
-    from .collections import coerce, singleton
+    from .collections import coerce, singleton, only, is_subsequence
 
+from .defaultdict import DefaultDict, Unset
 
 # ## Optional Modules
 
 # joblib: easy parallelization
 with _try:
     from joblib import Parallel, delayed
-    parallel = Parallel(n_jobs=cpu_count())
+from .parallel import parallel
 
 # yaml
 with _try:
     import yaml
     # Fix a bad default in PyYAML (cf. https://github.com/yaml/pyyaml/issues/110)
     yaml.dump = partial(yaml.dump, sort_keys=False)
     yaml.safe_dump = partial(yaml.safe_dump, sort_keys=False)
 
 # requests
 with _try:
-    from requests import           get as   GET,          post as  POST,           put as   PUT,         patch as PATCH
+    from requests import \
+        get as   GET, \
+        post as  POST, \
+        put as   PUT, \
+        patch as PATCH
 
 
 # ## PyData / Scientific Python
 
 with _try:
     import numpy as np
     from numpy import concatenate, array, ndarray, matrix, nan
 
 with _try: import seaborn as sns
 with _try: import matplotlib.pyplot as plt
 with _try: from scipy.sparse import spmatrix, coo_matrix, csr_matrix, csc_matrix
+
+from .version import git_version, pkg_version
+
+__version__ = pkg_version('utz')
```

### Comparing `utz-0.3.9/utz/argparse.py` & `utz-0.4.0/utz/argparse.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/backoff.py` & `utz-0.4.0/utz/backoff.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/bases.py` & `utz-0.4.0/utz/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     - 0 ⟺ ''
     - [1,N) ⟺ <1-char strings>
     - [N, N²+N) ⟺ <2-char strings>
     - [N²+N, N³+N²+N) ⟺ <3-char strings>
     - etc.
     '''
     I2S = None
+
     def __init__(self):
         self.S2I = {ch:i for i, ch in enumerate(self.I2S)}
 
     def __call__(self, v):
         if isinstance(v, str):
             return s2i(v, self.S2I)
         elif isinstance(v, int):
```

### Comparing `utz-0.3.9/utz/cli.py` & `utz-0.4.0/utz/cli.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/context.py` & `utz-0.4.0/utz/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,29 +42,30 @@
 
 
 # ## `no`: context manager for verifying `NameError`s (undefined variable names)
 no = catch(NameError)
 
 
 def run_then_raise(fns, vals=None):
-    '''Run multiple functions, catching all Exceptions and raise-chaining them at the end'''
+    """Run multiple functions, catching all Exceptions and raise-chaining them at the end"""
     if not fns: return vals
     if not vals: vals = []
     (fn, *fns) = fns
     try:
         vals.append(fn())
     except Exception as e:
         run_then_raise(fns, vals=vals)
         raise e
     else:
         return run_then_raise(fns, vals=vals)
 
 
 def bind_exit(ctx): return lambda: ctx.__exit__(None, None, None)
 
+
 @contextmanager
 def ctxs(ctxs):
     vals = []
     try:
         for ctx in ctxs:
             val = ctx.__enter__()
             vals.append(val)
@@ -77,7 +78,18 @@
             ])
         )
         raise e
     else:
         fns = [ bind_exit(ctx) for ctx in reversed(ctxs) ]
         run_then_raise(fns)
 
+
+def contexts(ctxs):
+    @contextmanager
+    def fn(ctxs):
+        if not ctxs:
+            yield
+        else:
+            [ ctx, *rest ] = ctxs
+            with ctx as v, fn(rest) as vs:
+                yield [ v, *vs ]
+    return fn(ctxs)
```

### Comparing `utz-0.3.9/utz/df_counts.py` & `utz-0.4.0/utz/df_counts.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/diff_dfs.py` & `utz-0.4.0/utz/diff_dfs.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/docker/file.py` & `utz-0.4.0/utz/docker/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from contextlib import AbstractContextManager
 import json
 from os.path import exists, join
 from os import getcwd, remove
 import shlex
 from tempfile import NamedTemporaryFile
 from types import TracebackType
@@ -37,30 +36,30 @@
         self.path = path
         self.fd = None
         self.tag = tag
         self.dir = dir
         self.copy_dir = copy_dir
 
         if extend:
-            with open(extend,'r') as f:
-                self.lines = [ line.rstrip('\n') for line in f.readlines() ]
+            with open(extend, 'r') as f:
+                self.lines = [line.rstrip('\n') for line in f.readlines()]
         else:
             self.lines = []
 
     def __enter__(self):
         if File._file:
             raise RuntimeError(f"Can't enter {self}, already entered {File._file}")
         File._file = self
         return self
 
     def __exit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType]
+            self,
+            exc_type: Optional[Type[BaseException]],
+            exc_value: Optional[BaseException],
+            traceback: Optional[TracebackType]
     ):
         File._file = None
         if self.tag:
             self.build(self.tag)
         if self.path and exists(self.path) and self.rm:
             remove(self.path)
 
@@ -87,18 +86,18 @@
             path = ctx.name
 
         with ctx:
             with open(path, mode) as fd:
                 fd.writelines('%s\n' % l for l in self.lines)
 
             sh(
-                'docker','build',
-                '-f',path,
-                '-t',tag,
-                [ ['--build-arg',f'{k}={v}'] for k,v in build_args.items() ],
+                'docker', 'build',
+                '-f', path,
+                '-t', tag,
+                [['--build-arg', f'{k}={v}'] for k, v in build_args.items()],
                 dir
             )
 
             if rm:
                 remove(path)
 
         return Image(tag, self)
@@ -108,35 +107,35 @@
         if 'dir' in kwargs:
             dir = kwargs.pop('dir')
             if kwargs:
                 raise ValueError(f'Unexpected kwargs: {",".join(kwargs)}')
         else:
             dir = self.copy_dir
         if dir:
-            srcs = [ join(dir, src) for src in srcs ]
+            srcs = [join(dir, src) for src in srcs]
         self.write(f'COPY {" ".join([*srcs, dst])}')
 
     def kvs(self, cmd, *args, **kwargs):
         flattened = []
         for arg in args:
             if isinstance(arg, str):
                 flattened.append(arg)
             elif isinstance(arg, tuple):
                 if len(arg) != 2:
                     raise RuntimeError(f'Invalid tuple arg (required len 2): %s' % str(arg))
-                k,v = arg
+                k, v = arg
                 k = escape(str(k))
                 v = escape(str(v))
                 flattened.append(f'"{k}"="{v}"')
             elif isinstance(arg, dict):
-                for k,v in arg.items():
+                for k, v in arg.items():
                     flattened.append(f'"{escape(k)}"="{escape(v)}"')
             else:
                 raise ValueError(f'Unrecognized argument to {cmd}: {arg}')
-        for k,v in kwargs.items():
+        for k, v in kwargs.items():
             flattened.append(f'"{escape(k)}"="{escape(v)}"')
         if flattened:
             self.write(f'{cmd} {" ".join(flattened)}')
 
     def NOTE(self, *lines):
         self.write(*[f'# {line}' for line in lines])
 
@@ -159,17 +158,19 @@
     def FROM(self, repo, tag=None, registry=None):
         if registry:
             repo = f'{registry}/{repo}'
         if tag:
             repo = f'{repo}:{tag}'
         self.write(f'FROM {repo}')
 
-    def LN(self): self.write('')
+    def LN(self):
+        self.write('')
 
-    def WORKDIR(self, dst='/'): self.write(f'WORKDIR {dst}')
+    def WORKDIR(self, dst='/'):
+        self.write(f'WORKDIR {dst}')
 
     def ENTRYPOINT(self, *args, shell=False):
         if shell:
             self.write(f'ENTRYPOINT {shlex.join(args)}')
         else:
             self.write(f'ENTRYPOINT {json.dumps(args)}')
```

### Comparing `utz-0.3.9/utz/git/__init__.py` & `utz-0.4.0/utz/git/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from utz import process
+
 try:
     from git import Repo, Git, InvalidGitRepositoryError
     from functools import partial
     import os
+
     def make_repo(*args, exist_ok=False, search_parent_directories=True, gitignore=None, msg=None, **kwargs):
         load_kwargs = kwargs.copy()
         load_kwargs['search_parent_directories'] = search_parent_directories
         if exist_ok:
             try:
                 return Repo(*args, **load_kwargs)
             except InvalidGitRepositoryError:
@@ -23,35 +26,41 @@
         else:
             return Repo(*args, **load_kwargs)
 except ImportError:
     pass
 
 
 from . import branch, clone, diff, head, remote, submodule
+from .ctx import txn
 from .head import fmt, sha
-from .remote import push, ls_remote
-from ..process import run
+from .log import msg
+from .remote import push, ls_remote, git_remote_sha
+from .repo import git_repo
+from .submodule import git_submodules
 
 
 from ._checkout import Checkout
 checkout = Checkout()
 
 
 def merge(ref, msg=None, ff=None):
-    cmd = ['git','merge','--no-edit']
+    cmd = ['git', 'merge', '--no-edit']
 
-    if ff == True: cmd += ['--ff-only']
-    elif ff == False: cmd += ['--no-ff']
+    if ff is True:
+        cmd += ['--ff-only']
+    elif ff is False:
+        cmd += ['--no-ff']
 
-    if msg: cmd += ['-m',msg]
+    if msg:
+        cmd += ['-m', msg]
 
     cmd += [ref]
 
-    run(cmd)
+    process.run(cmd)
 
 
 def commit(msg=None, all=False, amend=False):
-    cmd = ['git','commit']
+    cmd = ['git', 'commit']
     if amend: cmd += ['--amend']
     if all: cmd += ['-a']
-    if msg: cmd += ['-m',msg]
-    run(cmd)
+    if msg: cmd += ['-m', msg]
+    process.run(cmd)
```

### Comparing `utz-0.3.9/utz/git/_checkout.py` & `utz-0.4.0/utz/git/_checkout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-# In[ ]:
-
-
 from contextlib import contextmanager
 from ..process import run
 from . import branch as _branch
 
 class Checkout:
     def __call__(checkout, branch, ref=None, create_ok=False, ctx=True, sha_ok=True):
         prev = _branch.current(sha_ok=sha_ok)
```

### Comparing `utz-0.3.9/utz/git/branch.py` & `utz-0.4.0/utz/git/branch.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/git/clone.py` & `utz-0.4.0/utz/git/clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 
 from contextlib import contextmanager
 from os.path import basename
 from sys import stderr
 from typing import Iterable
 
 import utz
-from utz import check, git, line, match, now, print_exc, run, tmpdir, uuid1
+from utz import check, git, line, match, now, print_exc, run, tmpdir
 
 
 @contextmanager
 def tmp(
     url,
     *clone_args,
     branch=None,
     ref=None,
     submodules=True,
     push=False,
     pull=False,
     cd=True,
     name=None,
     bare=False,
+    dir=None,
     **run_kwargs,
 ):
     '''contextmanager for creating a Git repo in a temporary directory, and optionally cd'ing into it and upstreaming
     commits from it
 
     - `url`: local or remote path to Git repository to be cloned
     - `clone_args` (List[str]): passed directly to `git clone`
@@ -38,15 +39,15 @@
     - `cd` (bool): move into the temporary clone dir before `yield`ing
     - `name`: basename for the temporary clone directory (defaults to basename of `url`)
     - `bare`: clone a bare repository
     '''
 
     name = name or basename(url)
     if name.endswith('.git'): name = name[:-len('.git')]
-    with tmpdir(name) as repo_dir:
+    with tmpdir(name, dir=dir) as repo_dir:
         cmd = ['git','clone']
         if submodules: cmd += ['--recurse-submodules']
         if bare: cmd += ['--bare']
         if branch and not ref:
             # branch must already exist and we want to clone and work on it
             cmd += ['-b',branch]
         cmd += clone_args
```

### Comparing `utz-0.3.9/utz/git/remote.py` & `utz-0.4.0/utz/git/remote.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+import re
 from re import match
+from subprocess import CalledProcessError
+
+from utz import process
 
 from ..process import *
 
 
-def ls(): return lines('git','remote')
+def ls(): return lines('git', 'remote')
+
+
+LS_REMOTE_LINE_REGEX = r'(?P<sha>[0-9a-f]{40})\s+(?:refs/(?P<type>[^/]+)/(?P<name>.*)|(?P<head>HEAD))'
 
 
-LS_REMOTE_LINE_REGEX = '(?P<sha>[0-9a-f]{40})\s+(?:refs/(?P<type>[^/]+)/(?P<name>.*)|(?P<head>HEAD))'
 def parse_ls_remote_lines(lns, head=None, tag=None, sha=None, heads=False, tags=False):
     d = {}
     for ln in lns:
         m = match(LS_REMOTE_LINE_REGEX, ln)
         typ = m['type']
         if typ:
             name = m['name']
@@ -26,34 +32,34 @@
 
     if head:
         return d.get('heads', {}).get(head)
     if tag:
         return d.get('tags', {}).get(tag)
     if sha:
         r = {}
-        for k,v in d.items():
+        for k, v in d.items():
             if k == 'head':
                 if v.startswith(sha):
                     r[k] = v
             else:
-                typ = { name:id for name,id in v.items() if id.startswith(sha) }
+                typ = { name: id for name, id in v.items() if id.startswith(sha) }
                 if typ:
                     r[k] = typ
         d = r
     if heads or tags:
         if heads and tags: return { 'heads': d.get('heads'), 'tags': d.get('tags') }
         elif heads: return d.get('heads')
         elif tags: return d.get('tags')
         else: raise
 
     return d
 
 
 def ls_remote(remote, *args, head=None, tag=None, sha=None, heads=False, tags=False):
-    cmd = ['git','ls-remote']
+    cmd = ['git', 'ls-remote']
     if head or heads: cmd += ['--heads']
     if tag or tags: cmd += ['--tags']
     cmd += (remote,) + args
     lns = lines(cmd)
     return parse_ls_remote_lines(lns, head=head, tag=tag, sha=sha, heads=heads, tags=tags)
 
 
@@ -67,48 +73,53 @@
         elif 'default' in kwargs:
             default = kwargs.pop('default')
         else:
             raise ValueError(f"Remote {name} doesn't exist")
 
         return default
     
-    return line('git','remote','get-url',name)
+    return line('git', 'remote', 'get-url', name)
 _url = url
 
 
 def init(name, url, branch=None, remote_branch=None, fetch=True, checkout=True, push=True):
     if exists(name):
         existing_url = _url(name)
         if existing_url != url:
-            run('git','remote','set-url',name,url)
+            run('git', 'remote', 'set-url', name, url)
     else:
-        run('git','remote','add',name,url)
+        run('git', 'remote', 'add', name, url)
     
     if fetch:
-        run('git','fetch',name)
+        run('git', 'fetch', name)
     
     if branch:
         remote_branch = remote_branch or 'master'
         upstream = f'{name}/{remote_branch}'
         try:
-            run('git','branch','-u',upstream,branch)
+            run('git', 'branch', '-u', upstream, branch)
         except CalledProcessError as e:
             if push:
                 print(f'Failed to track upstream branch {upstream}; attempting to push {branch}:{remote_branch}')
-                run('git','push',name,f'{branch}:{remote_branch}')
-                run('git','branch','-u',upstream,branch)
+                run('git', 'push', name, f'{branch}:{remote_branch}')
+                run('git', 'branch', '-u', upstream, branch)
             else:
                 raise e
         if checkout:
-            run('git','checkout',branch)
+            run('git', 'checkout', branch)
 
 
 def push(name=None, local=None, remote=None):
     refspec = None
     if local:
         if remote:
             refspec = f'{local}:{remote}'
         else:
             refspec = f'{local}:{local}'
     
-    run('git','push',name,refspec)
+    run('git', 'push', name, refspec)
+
 
+def git_remote_sha(url: str, ref: str, **kwargs):
+    line = process.line('git', 'ls-remote', url, ref, **kwargs)
+    new_sha, _ = re.split(r'\s+', line, 1)
+    return new_sha
```

### Comparing `utz-0.3.9/utz/methods.py` & `utz-0.4.0/utz/methods.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/o.py` & `utz-0.4.0/utz/o.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,43 +33,49 @@
         K = '_data'
         if K in data:
             raise ValueError(f"Reserved key '{K}' found in 'data' dict: {data}")
 
         super().__init__(**data)
 
         for k, v in data.items():
-            if isinstance(v, dict) and not isinstance(v, o): v = o(v)
+            if type(v) is dict and not isinstance(v, o): v = o(v)
             super(o, self).__setattr__(k, v)
 
         super(o, self).__setattr__(K, data)
 
-    def merge(self, *args, **kwargs): return merge(self, *args, **kwargs)
+    def merge(self, *args, **kwargs):
+        return merge(self, *args, **kwargs)
 
     def update(self, *args, **kwargs):
         for arg in args:
             self.update(**arg)
-        for k,v in kwargs.items():
+        for k, v in kwargs.items():
             setattr(self, k, v)
 
-    def __dict__(self): return dict(self._data)
+    def __items__(self):
+        for k, v in self._data.items():
+            yield k, v
 
     def __setattr__(self, k, v):
         if isinstance(v, dict) and not isinstance(v, o): v = o(v)
         self._data[k] = v
 
     def __getattr__(self, k):
         try:
             v = self._data[k]
             if isinstance(v, dict) and not isinstance(v, o): v = o(v)
             return v
         except KeyError:
             raise AttributeError(f'Key {k}')
 
-    def __len__(self): return len(self._data)
-    def __delitem__(self, k): del self._data[k]
+    def __len__(self):
+        return len(self._data)
+
+    def __delitem__(self, k):
+        del self._data[k]
 
     def get(self, k, default=None):
         if k in self:
             return self[k]
         else:
             return default
 
@@ -83,24 +89,35 @@
             else:
                 return default
 
         return obj
 
     def __getitem__(self, k):
         v = self._data[k]
-        if isinstance(v, dict) and not isinstance(v, o): v = o(v)
+        if type(v) is dict:
+            v = o(v)
         return v
-    def __setitem__(self, k, v): self._data[k] = v
-    def __contains__(self, k): return k in self._data
+
+    def __setitem__(self, k, v):
+        self._data[k] = v
+
+    def __contains__(self, k):
+        return k in self._data
     
-    def __str__(self): return str(self._data)
-    def __repr__(self): return repr(self._data)
+    def __str__(self):
+        return str(self._data)
+
+    def __repr__(self):
+        return repr(self._data)
+
+    def __iter__(self):
+        return iter(self._data)
 
-    def __iter__(self): return iter(self._data)
-    def items(self): return self._data.items()
+    def items(self):
+        return self._data.items()
 
     def __eq__(self, r):
         if isinstance(r, o):
             return self._data == r._data
         if isinstance(r, dict):
             return self._data == r
         return NotImplemented
@@ -108,8 +125,9 @@
     def __ne__(self, r):
         if isinstance(r, o):
             return self._data != r._data
         if isinstance(r, dict):
             return self._data != r
         return NotImplemented
 
-    def __hash__(self): return hash(self._data)
+    def __hash__(self):
+        return hash(self._data)
```

### Comparing `utz-0.3.9/utz/pdf.py` & `utz-0.4.0/utz/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 #!/usr/bin/env python
 
+from pathlib import Path
 from PyPDF2 import PdfFileWriter, PdfFileReader
 from io import BytesIO
 from reportlab.pdfgen import canvas
 from reportlab.lib.pagesizes import letter
 from subprocess import check_output
 
 
 def maybe_open_pdf(path, open_pdf):
     if open_pdf:
-        check_output(['open',path])
+        check_output(['open', path])
 
 
-def write(path, out, *args, page=0, open_pdf=False):
+def write(path, out, *args, page=0, font_size=None, open_pdf=False):
     path = str(path)
     out = str(out)
-    page_idx=page
+    page_idx = page
 
     if isinstance(args[0], int) and isinstance(args[1], int) and isinstance(args[2], str):
         args = [args]
     
     packet = BytesIO()
     # create a new PDF with Reportlab
     can = canvas.Canvas(packet, pagesize=letter)
+    if font_size:
+        can.setFontSize(font_size)
     
     for x, y, s in args:
         can.drawString(x, y, s)
     
     can.save()
 
-    #move to the beginning of the StringIO buffer
+    # move to the beginning of the StringIO buffer
     packet.seek(0)
     new_pdf = PdfFileReader(packet)
     # read your existing PDF
     existing_pdf = PdfFileReader(open(path, "rb"))
     output = PdfFileWriter()
     
     # add the "watermark" (which is the new pdf) on the existing page
     page = existing_pdf.getPage(page_idx)
     page.mergePage(new_pdf.getPage(page_idx))
     output.addPage(page)
 
     # finally, write "output" to a real file
-    outputStream = open(out, "wb")
-    output.write(outputStream)
-    outputStream.close()
-    
+    with open(out, "wb") as f:
+        output.write(f)
+
     maybe_open_pdf(out, open_pdf)
 
 
-from pathlib import Path
 def cat(inputs, output, open_pdf=False):
-    '''https://stackoverflow.com/a/3444735'''
+    """https://stackoverflow.com/a/3444735"""
     input_streams = []
     try:
         # First open all the files, then produce the output file, and
         # finally close the input files. This is necessary because
         # the data isn't read from the input files until the write
         # operation. Thanks to
         # https://stackoverflow.com/questions/6773631/problem-with-closing-python-pypdf-writing-getting-a-valueerror-i-o-operation/6773733#6773733
@@ -76,8 +77,7 @@
         else:
             writer.write(output)
     finally:
         for f in input_streams:
             f.close()
     
     maybe_open_pdf(output, open_pdf)
-
```

### Comparing `utz-0.3.9/utz/pnds.py` & `utz-0.4.0/utz/pnds.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/process.py` & `utz-0.4.0/utz/process/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 #!/usr/bin/env python
 
+from json import loads
 import shlex
 from subprocess import check_call, check_output, CalledProcessError, DEVNULL
+from sys import stderr
+
+
+def err(msg):
+    stderr.write(msg)
+    stderr.write('\n')
 
 
 def parse_cmd(cmd):
-    '''Stringify and potentially unwrap a command'''
+    """Stringify and potentially unwrap a command"""
+
     def flatten(args):
         if isinstance(args, list) or isinstance(args, tuple):
             return tuple(
                 a
                 for arg in args
                 for a in flatten(arg)
             )
@@ -20,15 +28,15 @@
         str(arg)
         for arg in flatten(cmd)
         if arg is not None
     ]
 
 
 def lines(*cmd, keep_trailing_newline=False, dry_run=False, err_ok=False, **kwargs):
-    '''Return the lines written to stdout by a command'''
+    """Return the lines written to stdout by a command"""
     out = output(*cmd, dry_run=dry_run, err_ok=err_ok, **kwargs)
     if err_ok and out is None:
         return None
 
     lines = [
         line.rstrip('\n')
         for line in
@@ -38,74 +46,84 @@
     if not keep_trailing_newline and lines and not lines[-1]:
         lines = lines[:-1]
 
     return lines
 
 
 def line(*cmd, empty_ok=False, err_ok=False, **kwargs):
-    '''Run a command, verify that it returns a single line of output, and return that line'''
+    """Run a command, verify that it returns a single line of output, and return that line"""
     _lines = lines(*cmd, err_ok=err_ok, **kwargs)
     if (empty_ok or err_ok) and not _lines:
         return None
     elif len(_lines) == 1:
         return _lines[0]
     else:
         raise ValueError(f'Expected 1 line, found {len(_lines)}:\n\t%s' % '\n\t'.join(_lines))
 
+
 ELIDED = '****'
 
+
 def mk_cmd_str(cmd, elide=None):
     shlex_join = getattr(shlex, 'join', ' '.join)  # shlex.join only exists in Python ≥3.8
     cmd_str = shlex_join(cmd)
     if elide:
         if isinstance(elide, str): elide = [elide]
         for s in elide:
             cmd_str = cmd_str.replace(s, ELIDED)
     return cmd_str
 
-def run(*cmd, dry_run=False, elide=None, **kwargs):
-    '''Convenience wrapper for check_call'''
+
+def run(*cmd, dry_run=False, elide=None, log=err, **kwargs):
+    """Convenience wrapper for check_call"""
     cmd = parse_cmd(cmd)
     cmd_str = mk_cmd_str(cmd, elide)
     if dry_run:
-        print(f'Would run: {cmd_str}')
+        if log:
+            log(f'Would run: {cmd_str}')
     else:
-        print(f'Running: {cmd_str}')
+        if log:
+            log(f'Running: {cmd_str}')
         check_call(cmd, **kwargs)
 
+
 sh = run
 
-def output(*cmd, dry_run=False, err_ok=False, elide=None, **kwargs):
-    '''Convenience wrapper for check_output'''
+
+def output(*cmd, dry_run=False, err_ok=False, elide=None, log=err, **kwargs):
+    """Convenience wrapper for check_output"""
     cmd = parse_cmd(cmd)
     cmd_str = mk_cmd_str(cmd, elide)
     if dry_run:
-        print(f'Would run: {cmd_str}')
-        return b''
+        if log:
+            log(f'Would run: {cmd_str}')
+        return None
     else:
-        print(f'Running: {cmd_str}')
+        if log:
+            log(f'Running: {cmd_str}')
         try:
             return check_output(cmd, **kwargs)
         except CalledProcessError as e:
             if err_ok:
                 return None
             else:
                 raise e
 
 
-from json import loads
-def json(*cmd, **kwargs):
-    '''Run a command, parse the output as JSON, and return the parsed object'''
-    out = output(*cmd, **kwargs)
+def json(*cmd, dry_run=False, **kwargs):
+    """Run a command, parse the output as JSON, and return the parsed object"""
+    out = output(*cmd, dry_run=dry_run, **kwargs)
     if out is None:
         return None
     return loads(out.decode())
 
 
 def check(*cmd, stdout=DEVNULL, stderr=DEVNULL, **kwargs):
-    '''Return True iff a command run successfully (i.e. exits with code 0)'''
+    """Return True iff a command run successfully (i.e. exits with code 0)"""
     try:
         run(*cmd, stdout=stdout, stderr=stderr, **kwargs)
         return True
     except CalledProcessError:
         return False
 
+
+__all__ = ['check', 'err', 'line', 'lines', 'output', 'run', 'sh', ]
```

### Comparing `utz-0.3.9/utz/setup.py` & `utz-0.4.0/utz/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,61 @@
 import setuptools
 from setuptools import find_packages
 
 from utz import *
 
 
 class Compute:
-    '''Container for computing fallback values to pass to setup()'''
+    """Container for computing fallback values to pass to setup()"""
 
     def long_description(self):
-        '''Read in README.md as the `long_description`'''
+        """Read in README.md as the `long_description`"""
         if exists('README.md'):
             with open('README.md', "r") as fh:
                 return fh.read()
 
     def long_description_content_type(self):
-        '''Default to markdown format for `long_description`'''
+        """Default to markdown format for `long_description`"""
         return "text/markdown"
 
-    VERSION_TAG_REGEX = r'v?(?P<version>(?P<base>\d+\.\d+\.\d+)(?P<rc>(?:r|c|rc|a|b)\d+)?(?:-(?P<commits_ahead>\d+)-g(?P<sha>[0-9a-f]{6,}))?)'
     def version(self):
-        '''Infer version from git tag of the form "v_._._" (which must be present)'''
-        try:
-            tag = line('git','describe','--tags','HEAD')
-            m = match(self.VERSION_TAG_REGEX, tag)
-            if not m:
-                raise ValueError('Unrecognized tag: %s' % tag)
-            version = m['version']
-        except CalledProcessError:
-            version = line('git','log','--format=%h','-n1')
-
-        return version
+        return git_version()
 
     def name(self):
-        '''`name` defaults to the name of the containing directory'''
+        """`name` defaults to the name of the containing directory"""
         return basename(getcwd())
 
     def author(self):
-        '''Infer author name from most recent commit'''
-        return line('git','log','-n1','--format=%an')
+        """Infer author name from most recent commit"""
+        return line('git', 'log', '-n1', '--format=%an')
 
     def author_email(self):
-        '''Infer author email from most recent commit'''
-        return line('git','log','-n1','--format=%ae')
+        """Infer author email from most recent commit"""
+        return line('git', 'log', '-n1', '--format=%ae')
 
     def description(self):
-        '''Set `description` to the contents of a <p> first-child of an initial <h1>'''
+        """Set `description` to the contents of a <p> first-child of an initial <h1>"""
         try:
+            import lxml
             import mistune
-        except ImportError:
-            import pip
-            pip.main(['install','mistune>=0.8.1,<2'])  # match nbconvert
-            import mistune
+            html = mistune.html(self.long_description())
 
-        html = mistune.Markdown()(self.long_description())
+            from lxml.html import fragments_fromstring
+            [ h1, p, *_ ] = fragments_fromstring(html)
+            if h1.tag != 'h1' or p.tag != 'p':
+                raise ValueError('Expected initial <h1> followed by <p> while parsing `description` from README.md')
 
-        try:
-            import lxml
+            return p.text_content()
         except ImportError:
-            import pip
-            pip.main(['install','lxml'])
-            import lxml
-
-        from lxml.html import fragments_fromstring
-        [ h1, p, *_ ] = fragments_fromstring(html)
-        if h1.tag != 'h1' or p.tag != 'p':
-            raise ValueError('Expected initial <h1> followed by <p> while parsing `description` from README.md')
-
-        return p.text_content()
+            md = self.long_description()
+            md_lines = md.split('\n')
+            for line in md_lines:
+                if not re.match(r'[#\[!\-|<]', line):
+                    return line
+            return None
 
     def packages(self):
         return find_packages()
 
     def classifiers(self):
         classifiers = [
             "Programming Language :: Python :: 3",
@@ -83,23 +68,24 @@
 
         return classifiers
 
     def python_requires(self): return '>=3.6'
 
     def license(self):
         if exists('LICENSE'):
-            with open('LICENSE','r') as f:
+            with open('LICENSE', 'r') as f:
                 lines = f.readlines()
                 first_lines = [ line.strip() for line in lines[:2] ]
-                if first_lines == ['Apache License','Version 2.0, January 2004',]: return 'Apache v2'
-                if first_lines == ['MIT License','',]: return 'MIT'
+                if first_lines == ['Apache License', 'Version 2.0, January 2004',]: return 'Apache v2'
+                if first_lines == ['MIT License', '',]: return 'MIT'
 
 
 def setup(**kwargs):
     c = Compute()
+
     def compute(*keys):
         for k in keys:
             if k not in kwargs:
                 fn = getattr(c, k)
                 v = fn()
                 s = str(v)
                 s = s[:100] + '…' if len(s) > 100 else s
```

### Comparing `utz-0.3.9/utz/sql.py` & `utz-0.4.0/utz/sql.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/ssh.py` & `utz-0.4.0/utz/ssh.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/time.py` & `utz-0.4.0/utz/time.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/use.py` & `utz-0.4.0/utz/use.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz/zip.py` & `utz-0.4.0/utz/zip.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.9/utz.egg-info/PKG-INFO` & `utz-0.4.0/utz.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 Metadata-Version: 2.1
 Name: utz
-Version: 0.3.9
-Summary: ("yoots"): common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
+Version: 0.4.0
+Summary: *("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
 Home-page: https://github.com/runsascoded/utz
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
-Description: # utz
-        *("yoots")*: common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
-        
-        ## Install
-        ```bash
-        pip install utz
-        ```
-        
-        ## Use
-        Import the whole kitchen sink:
-        ```python
-        from utz import *
-        ```
-        
-        See [__init__.py](utz/__init__.py), which imports many of the modules below, as well as a bevy of handy stdlib methods and objects.
-        
-        ## Features
-        Some noteworthy modules:
-        - [cd](utz/cd.py): "change directory" contextmanager
-        - [o](utz/o.py): `dict` wrapper exposing keys as attrs (e.g.: `o({'a':1}).a == 1`)
-        - [process](utz/process.py): subprocess wrappers for more easily shelling out to commands and parsing their stdout
-        - [docker](docker/): DSL for programmatically creating Dockerfiles (and building images from them)
-        - [ssh](utz/ssh.py): SSH tunnel wrapped in a context manager
-        - [time](utz/time.py): `now()`/`today()` helpers with convenient / no-nonsense ISO string serialization and UTC bias
-        - [bases](utz/bases.py): `int`⟺`str` codecs with improvements over standard base64 et al.
-        - [tmpdir](utz/tmpdir.py): make temporary directories with a specific basename
-        - [context](utz/context.py): context-manager helpers, including `ctxs` for composing multiple context managers
-        - [backoff](utz/backoff.py): simple exponential-backoff utility
-        - [git](utz/git): git helpers / wrappers around [GitPython](https://gitpython.readthedocs.io/en/stable/)
-        - [pnds](utz/pnds.py): common [pandas](https://pandas.pydata.org/) imports and helpers
-        - [collections](utz/collections.py): collection/list helpers
-        
-        ### auto-`setup.py`
-        [`utz/setup.py`](utz/setup.py) provides defaults for various `setuptools.setup()` params:
-        - `name`: use parent directory name
-        - `version`: parse from git tag (otherwise from `git describe --tags`)
-        - `author_{name,email}`: infer from last commit
-        - `long_description`: parse `README.md` (and set `long_description_content_type)
-        - `description`: parse first `<p>` under opening `<h1>` from `README.md`
-        - `license`: parse from `LICENSE` file (MIT and Apache v2 supported)
-        
-        For an example, see [`gsmo==0.0.1`](https://github.com/runsascoded/gsmo/blob/v0.0.1/setup.py) ([and corresponding release](https://pypi.org/project/gsmo/)).
-        
-        It can be installed via a pip extra:
-        ```bash
-        pip install utz[setup]
-        ``` 
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pdf
-Provides-Extra: setup
 Provides-Extra: test
+License-File: LICENSE
+
+# utz
+*("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
+
+## Install
+```bash
+pip install utz
+```
+
+## Use
+Import everything:
+```python
+from utz import *
+```
+
+See [`__init__.py`](utz/__init__.py), which imports many of the modules below, as well as a many standard-library methods and objects.
+
+## Features
+Some noteworthy modules:
+- [cd](utz/cd.py): "change directory" contextmanager
+- [o](utz/o.py): `dict` wrapper exposing keys as attrs (e.g.: `o({'a':1}).a == 1`)
+- [process](utz/process.py): subprocess wrappers for more easily shelling out to commands and parsing their stdout
+- [docker](docker/): DSL for programmatically creating Dockerfiles (and building images from them)
+- [ssh](utz/ssh.py): SSH tunnel wrapped in a context manager
+- [time](utz/time.py): `now()`/`today()` helpers with convenient / no-nonsense ISO string serialization and UTC bias
+- [bases](utz/bases.py): `int`⟺`str` codecs with improvements over standard base64 et al.
+- [tmpdir](utz/tmpdir.py): make temporary directories with a specific basename
+- [context](utz/context.py): contextmanager helpers, including `ctxs` for composing multiple context managers
+- [escape](utz/escape.py): escaping split/join helpers
+- [backoff](utz/backoff.py): simple exponential-backoff utility
+- [git](utz/git): git helpers / wrappers around [GitPython](https://gitpython.readthedocs.io/en/stable/)
+- [pnds](utz/pnds.py): common [pandas](https://pandas.pydata.org/) imports and helpers
+- [collections](utz/collections.py): collection/list helpers
+
+### auto-`setup.py`
+[`utz/setup.py`](utz/setup.py) provides defaults for various `setuptools.setup()` params:
+- `name`: use parent directory name
+- `version`: parse from git tag (otherwise from `git describe --tags`)
+- `author_{name,email}`: infer from last commit
+- `long_description`: parse `README.md` (and set `long_description_content_type)
+- `description`: parse first `<p>` under opening `<h1>` from `README.md`
+- `license`: parse from `LICENSE` file (MIT and Apache v2 supported)
+
+For an example, see [`gsmo==0.0.1`](https://github.com/runsascoded/gsmo/blob/v0.0.1/setup.py) ([and corresponding release](https://pypi.org/project/gsmo/)).
+
+It can be installed via a pip extra:
+```bash
+pip install utz[setup]
+``` 
+
+
```

### Comparing `utz-0.3.9/utz.egg-info/SOURCES.txt` & `utz-0.4.0/utz.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,45 @@
+LICENSE
 README.md
 setup.py
 utz/__init__.py
 utz/argparse.py
-utz/args_parser.py
 utz/backoff.py
 utz/bases.py
+utz/cached_property.py
+utz/case.py
 utz/cd.py
 utz/cli.py
 utz/collections.py
+utz/colors.py
 utz/context.py
+utz/dataclasses.py
+utz/defaultdict.py
 utz/df_counts.py
 utz/diff_dfs.py
+utz/escape.py
+utz/fn.py
 utz/imports.py
 utz/methods.py
 utz/o.py
+utz/parallel.py
 utz/path.py
 utz/pdf.py
+utz/plots.py
 utz/pnds.py
-utz/process.py
 utz/setup.py
 utz/sql.py
 utz/ssh.py
 utz/test.py
 utz/time.py
 utz/tmpdir.py
 utz/use.py
+utz/version.py
+utz/ym.py
+utz/ymd.py
 utz/zip.py
 utz.egg-info/PKG-INFO
 utz.egg-info/SOURCES.txt
 utz.egg-info/dependency_links.txt
 utz.egg-info/requires.txt
 utz.egg-info/top_level.txt
 utz/docker/__init__.py
@@ -36,11 +47,16 @@
 utz/docker/file.py
 utz/docker/image.py
 utz/docker/util.py
 utz/git/__init__.py
 utz/git/_checkout.py
 utz/git/branch.py
 utz/git/clone.py
+utz/git/ctx.py
 utz/git/diff.py
+utz/git/github.py
 utz/git/head.py
+utz/git/log.py
 utz/git/remote.py
-utz/git/submodule.py
+utz/git/repo.py
+utz/git/submodule.py
+utz/process/__init__.py
```

