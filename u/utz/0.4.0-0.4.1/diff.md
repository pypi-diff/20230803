# Comparing `tmp/utz-0.4.0.tar.gz` & `tmp/utz-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utz-0.4.0.tar", last modified: Thu Aug  3 00:21:53 2023, max compression
+gzip compressed data, was "utz-0.4.1.tar", last modified: Thu Aug  3 15:59:17 2023, max compression
```

## Comparing `utz-0.4.0.tar` & `utz-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.949671 utz-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 00:21:23.000000 utz-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-03 00:21:53.949671 utz-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 00:21:23.000000 utz-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:21:53.949671 utz-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-03 00:21:23.000000 utz-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.945671 utz-0.4.0/utz/
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-03 00:21:23.000000 utz-0.4.0/utz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 00:21:23.000000 utz-0.4.0/utz/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-03 00:21:23.000000 utz-0.4.0/utz/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-03 00:21:23.000000 utz-0.4.0/utz/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-03 00:21:23.000000 utz-0.4.0/utz/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 00:21:23.000000 utz-0.4.0/utz/case.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 00:21:23.000000 utz-0.4.0/utz/cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 00:21:23.000000 utz-0.4.0/utz/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-03 00:21:23.000000 utz-0.4.0/utz/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-03 00:21:23.000000 utz-0.4.0/utz/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 00:21:23.000000 utz-0.4.0/utz/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 00:21:23.000000 utz-0.4.0/utz/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-03 00:21:23.000000 utz-0.4.0/utz/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-03 00:21:23.000000 utz-0.4.0/utz/df_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-03 00:21:23.000000 utz-0.4.0/utz/diff_dfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.945671 utz-0.4.0/utz/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-03 00:21:23.000000 utz-0.4.0/utz/docker/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-03 00:21:23.000000 utz-0.4.0/utz/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-03 00:21:23.000000 utz-0.4.0/utz/fn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.949671 utz-0.4.0/utz/git/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/head.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 00:21:23.000000 utz-0.4.0/utz/git/submodule.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 00:21:23.000000 utz-0.4.0/utz/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 00:21:23.000000 utz-0.4.0/utz/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-03 00:21:23.000000 utz-0.4.0/utz/o.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 00:21:23.000000 utz-0.4.0/utz/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 00:21:23.000000 utz-0.4.0/utz/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-03 00:21:23.000000 utz-0.4.0/utz/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-08-03 00:21:23.000000 utz-0.4.0/utz/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-03 00:21:23.000000 utz-0.4.0/utz/pnds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.949671 utz-0.4.0/utz/process/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-03 00:21:23.000000 utz-0.4.0/utz/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-03 00:21:23.000000 utz-0.4.0/utz/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-03 00:21:23.000000 utz-0.4.0/utz/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 00:21:23.000000 utz-0.4.0/utz/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 00:21:23.000000 utz-0.4.0/utz/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-03 00:21:23.000000 utz-0.4.0/utz/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-03 00:21:23.000000 utz-0.4.0/utz/tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-08-03 00:21:23.000000 utz-0.4.0/utz/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-03 00:21:23.000000 utz-0.4.0/utz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-03 00:21:23.000000 utz-0.4.0/utz/ym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-08-03 00:21:23.000000 utz-0.4.0/utz/ymd.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 00:21:23.000000 utz-0.4.0/utz/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:21:53.945671 utz-0.4.0/utz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 00:21:53.000000 utz-0.4.0/utz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.878284 utz-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 15:57:40.000000 utz-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-03 15:59:17.878284 utz-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 15:57:40.000000 utz-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:59:17.878284 utz-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-03 15:57:40.000000 utz-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.874284 utz-0.4.1/utz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-03 15:57:40.000000 utz-0.4.1/utz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 15:57:40.000000 utz-0.4.1/utz/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-03 15:57:40.000000 utz-0.4.1/utz/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-03 15:57:40.000000 utz-0.4.1/utz/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 15:57:40.000000 utz-0.4.1/utz/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 15:57:40.000000 utz-0.4.1/utz/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 15:57:40.000000 utz-0.4.1/utz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-03 15:57:40.000000 utz-0.4.1/utz/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-03 15:57:40.000000 utz-0.4.1/utz/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 15:57:40.000000 utz-0.4.1/utz/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 15:57:40.000000 utz-0.4.1/utz/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-03 15:57:40.000000 utz-0.4.1/utz/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-03 15:57:40.000000 utz-0.4.1/utz/df_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-08-03 15:57:40.000000 utz-0.4.1/utz/diff_dfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.874284 utz-0.4.1/utz/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-03 15:57:40.000000 utz-0.4.1/utz/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-03 15:57:40.000000 utz-0.4.1/utz/fn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.878284 utz-0.4.1/utz/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 15:57:40.000000 utz-0.4.1/utz/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 15:57:40.000000 utz-0.4.1/utz/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-03 15:57:40.000000 utz-0.4.1/utz/o.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 15:57:40.000000 utz-0.4.1/utz/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 15:57:40.000000 utz-0.4.1/utz/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-03 15:57:40.000000 utz-0.4.1/utz/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-08-03 15:57:40.000000 utz-0.4.1/utz/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-03 15:57:40.000000 utz-0.4.1/utz/pnds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.878284 utz-0.4.1/utz/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-03 15:57:40.000000 utz-0.4.1/utz/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-03 15:57:40.000000 utz-0.4.1/utz/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-03 15:57:40.000000 utz-0.4.1/utz/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 15:57:40.000000 utz-0.4.1/utz/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 15:57:40.000000 utz-0.4.1/utz/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-03 15:57:40.000000 utz-0.4.1/utz/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-03 15:57:40.000000 utz-0.4.1/utz/tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-08-03 15:57:40.000000 utz-0.4.1/utz/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-03 15:57:40.000000 utz-0.4.1/utz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-03 15:57:40.000000 utz-0.4.1/utz/ym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-08-03 15:57:40.000000 utz-0.4.1/utz/ymd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 15:57:40.000000 utz-0.4.1/utz/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.874284 utz-0.4.1/utz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/top_level.txt
```

### Comparing `utz-0.4.0/LICENSE` & `utz-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/PKG-INFO` & `utz-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: utz
-Version: 0.4.0
-Summary: *("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
+Version: 0.4.1
+Summary: ("oots"): imports and utilities for easy wildcard-importing + boilerplate-reduction
 Home-page: https://github.com/runsascoded/utz
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dt
+Provides-Extra: git
+Provides-Extra: pd
 Provides-Extra: pdf
+Provides-Extra: setup
 Provides-Extra: test
+Provides-Extra: all
 License-File: LICENSE
 
 # utz
 *("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
 
 ## Install
 ```bash
```

### Comparing `utz-0.4.0/README.md` & `utz-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/argparse.py` & `utz-0.4.1/utz/argparse.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/backoff.py` & `utz-0.4.1/utz/backoff.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/bases.py` & `utz-0.4.1/utz/bases.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/cli.py` & `utz-0.4.1/utz/cli.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/collections.py` & `utz-0.4.1/utz/collections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python
 
-from pandas import Series
+try:
+    from pandas import Series
+except ImportError:
+    Series = None
 from math import exp, log
-from numpy import nan
 from sys import stderr
 
 
 class Expected1Found0(ValueError): pass
 
 
 class Expected1FoundN(ValueError):
@@ -31,15 +33,15 @@
         self.missing = set(expected).difference(actual)
         self.extra = set(actual).difference(expected)
         self.msg = f'Expected {expected}, actual {actual}. Extra: {self.extra}, missing: {self.missing}'
         super().__init__()
 
 
 def singleton(elems, fn=None, empty_ok=False, name='elems', dedupe=True, key=None):
-    if isinstance(elems, Series):
+    if Series and isinstance(elems, Series):
         elems = elems.unique().tolist()
     elif isinstance(elems, dict):
         if key:
             keys = list(elems.keys())
             actual_key = singleton(keys)
             if actual_key != key:
                 raise WrongKey(key, actual_key)
@@ -98,14 +100,18 @@
     if not valids:
         msg = f'Best choice {choice} for value {value} has error {exp(best["ratio"]) - 1} > {ε}'
         if errors == 'raise':
             raise ValueError(msg)
         if warn:
             stderr.write(msg + '\n')
         if errors == 'coerce':
+            try:
+                from numpy import nan
+            except ImportError:
+                nan = None
             return nan
         else:
             return value
     if len(valids) > 1 and not multi_ok:
         raise ValueError(
             '%d choices passed ε<%f filter:\n\t%s' % (
                 len(valids),
```

### Comparing `utz-0.4.0/utz/colors.py` & `utz-0.4.1/utz/colors.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/context.py` & `utz-0.4.1/utz/context.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/dataclasses.py` & `utz-0.4.1/utz/dataclasses.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/defaultdict.py` & `utz-0.4.1/utz/defaultdict.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/df_counts.py` & `utz-0.4.1/utz/df_counts.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/docker/dsl.py` & `utz-0.4.1/utz/docker/dsl.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/docker/file.py` & `utz-0.4.1/utz/docker/file.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/escape.py` & `utz-0.4.1/utz/escape.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/git/__init__.py` & `utz-0.4.1/utz/git/__init__.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/git/_checkout.py` & `utz-0.4.1/utz/git/_checkout.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/git/branch.py` & `utz-0.4.1/utz/git/branch.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/git/clone.py` & `utz-0.4.1/utz/git/clone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
 from contextlib import contextmanager
 from os.path import basename
+from re import match
 from sys import stderr
+from traceback import print_exc
 from typing import Iterable
 
-import utz
-from utz import check, git, line, match, now, print_exc, run, tmpdir
-
+from utz import now, tmpdir
+from utz.cd import cd
+from utz.process import check, line, run
 
 @contextmanager
 def tmp(
     url,
     *clone_args,
     branch=None,
     ref=None,
@@ -36,15 +38,16 @@
         `git push`
     - `pull` (bool): upstream changes post-`yield` by `cd`ing into the origin directory (must be a local dir, otherwise
         use `push`) and running a `git pull` from this temporary clone
     - `cd` (bool): move into the temporary clone dir before `yield`ing
     - `name`: basename for the temporary clone directory (defaults to basename of `url`)
     - `bare`: clone a bare repository
     '''
-
+    import utz
+    from utz import git
     name = name or basename(url)
     if name.endswith('.git'): name = name[:-len('.git')]
     with tmpdir(name, dir=dir) as repo_dir:
         cmd = ['git','clone']
         if submodules: cmd += ['--recurse-submodules']
         if bare: cmd += ['--bare']
         if branch and not ref:
```

### Comparing `utz-0.4.0/utz/git/ctx.py` & `utz-0.4.1/utz/git/ctx.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/git/github.py` & `utz-0.4.1/utz/git/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import click
 from functools import wraps
 from os import environ
 import re
 from sys import stderr
 from typing import Optional, Literal
 from utz import process
 
@@ -32,14 +31,15 @@
         env=GITHUB_REPOSITORY,
         help='Repository name with owner, e.g. "owner/repo"', **flag_kwargs,
 ):
     if not flag_args:
         flag_args = ('-R', '--repository')
 
     def option(fn):
+        import click
         @click.option(*flag_args, help=help, **flag_kwargs)
         @wraps(fn)
         def _fn(*args, repository=None, **kwargs):
             if not repository:
                 repository = environ.get(env)
                 if not repository:
                     verbose = kwargs.get('verbose', 0)
```

### Comparing `utz-0.4.0/utz/git/remote.py` & `utz-0.4.1/utz/git/remote.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/git/submodule.py` & `utz-0.4.1/utz/git/submodule.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/methods.py` & `utz-0.4.1/utz/methods.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/o.py` & `utz-0.4.1/utz/o.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/pdf.py` & `utz-0.4.1/utz/pdf.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/plots.py` & `utz-0.4.1/utz/plots.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/pnds.py` & `utz-0.4.1/utz/pnds.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 #!/usr/bin/env python
 
 # # Pandas imports / aliases / helpers
 
-try:
-    from dateutil.parser import parse
-except ImportError:
-    pass
-
 from pathlib import Path
 
-from numpy import nan, array, ndarray
 from os import remove
 from os.path import exists, isdir, splitext
 
-import pandas as pd
-from pandas import \
-    concat, \
-    DataFrame as DF, \
-    Series, \
-    isna, \
-    read_csv, read_excel, read_json, read_parquet, read_sql, read_sql_query, read_sql_table, \
-    date_range, to_datetime as to_dt, Timedelta as Δ, NaT, \
-    get_option, set_option
-
-from shutil import rmtree
+from utz.imports import _try
+with _try:
+    from dateutil.parser import parse
+with _try:
+    from numpy import nan, array, ndarray
+    import pandas as pd
+    from pandas import \
+        concat, \
+        DataFrame as DF, \
+        Series, \
+        isna, \
+        read_csv, read_excel, read_json, read_parquet, read_sql, read_sql_query, read_sql_table, \
+        date_range, to_datetime as to_dt, Timedelta as Δ, NaT, \
+        get_option, set_option
+    def display(r=None, c=None):
+        '''Set the default number of rows and columns for Pandas to display'''
+        if r:
+            pd.options.display.max_rows = r
+        if c:
+            pd.options.display.max_columns = c
 
-# ## Config
+    display(100, 100)
 
-def display(r=None, c=None):
-    '''Set the default number of rows and columns for Pandas to display'''
-    if r:
-        pd.options.display.max_rows = r
-    if c:
-        pd.options.display.max_columns = c
 
-display(100, 100)
+from shutil import rmtree
 
 
 # ## Concat / Creation
 
 def sxs(*dfs, **kwargs):
     '''Concat some DataFrames "side by side"'''
     return concat(dfs, axis=1, **kwargs)
```

### Comparing `utz-0.4.0/utz/process/__init__.py` & `utz-0.4.1/utz/process/__init__.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/setup.py` & `utz-0.4.1/utz/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from os import getcwd
+from os.path import basename, exists
+import re
 import setuptools
 from setuptools import find_packages
 
-from utz import *
+from utz.process import line
+from utz.version import git_version
 
 
 class Compute:
     """Container for computing fallback values to pass to setup()"""
 
     def long_description(self):
         """Read in README.md as the `long_description`"""
```

### Comparing `utz-0.4.0/utz/sql.py` & `utz-0.4.1/utz/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 #!/usr/bin/env python
-# coding: utf-8
-
-# In[ ]:
-
 
 import dask.dataframe as dd
 import pandas as pd
-from sqlalchemy import create_engine
 from os import cpu_count
 
 
-# In[ ]:
-
-
 def to_sql(
     table, name, db_path, force=False,
 ):
     if_exists = 'replace' if force else 'fail'
     table.to_sql(name, db_path, if_exists=if_exists)
     if isinstance(table, dd.DataFrame):
         divisions = pd.Series(table.divisions, name='divisions')
         divisions.to_sql(f'{name}/divisions', db_path, if_exists=if_exists)
 
-        
+
 def from_sql(
     name, db_path, index_col=None, dask=True,
 ):
     if index_col is None:
         index_col = 'index'
 
     if dask:
@@ -34,27 +26,25 @@
         table = dd.read_sql_table(name, db_path, index_col=index_col, divisions=divisions)
     else:
         table = pd.read_sql_table(name, db_path, index_col=index_col)
 
     return table
 
 
-# In[ ]:
-
-
 def table_to_sql(
     table_name,
     db_path,
     index_col=None,
     dask=True,
     npartitions=-1,
     table_path=None,
     force_db_refresh=False,
     **kwargs
 ):
+    from sqlalchemy import create_engine
     engine = create_engine(db_path)
 
     if npartitions is not None:
         if npartitions <= 0:
             npartitions = cpu_count()
 
     if force_db_refresh or not engine.has_table(table_name):
@@ -74,8 +64,7 @@
         
         if index_col is not None:
             csv = csv.set_index(index_col)
 
         to_sql(csv, table_name, db_path, force=force_db_refresh)
 
     return from_sql(table_name, db_path, index_col=index_col, dask=dask)
-
```

### Comparing `utz-0.4.0/utz/ssh.py` & `utz-0.4.1/utz/ssh.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/time.py` & `utz-0.4.1/utz/time.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/use.py` & `utz-0.4.1/utz/use.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/version.py` & `utz-0.4.1/utz/version.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz/ym.py` & `utz-0.4.1/utz/ym.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 from dataclasses import dataclass
 from datetime import datetime as dt, date
 from functools import wraps
 import re
 from math import ceil
 from typing import Tuple, Union, Generator
 
-import pandas as pd
-from click import option
-from pandas.core.tools.datetimes import DatetimeScalar
-
 
 # Types that can be passed to the Month constructor
 Monthy = Union['YM', str, int, None]
 
 
 @dataclass(init=False, order=True, eq=True, unsafe_hash=True)
 class YM:
@@ -96,15 +92,16 @@
     def __int__(self):
         return int(str(self))
 
     def format(self, url, **kwargs):
         return url.format(ym=str(self), y=str(self.y), m=str(self.m), **kwargs)
 
     @property
-    def dt(self) -> DatetimeScalar:
+    def dt(self):
+        import pandas as pd
         return pd.to_datetime('%d-%02d' % (self.y, self.m))
 
     @property
     def date(self) -> date:
         return self.dt.date()
 
     @property
@@ -143,14 +140,15 @@
 
 
 def dates(*flags, default_start=None, default_end=None, help=None):
     if not flags:
         flags = ('-d', '--dates')
 
     def _dates(fn):
+        from click import option
         @option('-d', '--dates', help=help)
         @wraps(fn)
         def _fn(*args, dates=None, **kwargs):
             if dates:
                 pcs = dates.split('-')
                 if len(pcs) == 2:
                     [ start, end ] = pcs
```

### Comparing `utz-0.4.0/utz/ymd.py` & `utz-0.4.1/utz/ymd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import re
 from dataclasses import dataclass
 from datetime import datetime as dt, date, timedelta
 from functools import wraps
 from typing import Union, Generator
+from utz.imports import _try
 
-import pandas as pd
-from click import option
-from pandas.core.tools.datetimes import DatetimeScalar
 
 # Types that can be passed to the Month constructor
 Monthy = Union['YMD', str, int, None]
 
 
 @dataclass(init=False, order=True, eq=True, unsafe_hash=True)
 class YMD:
@@ -105,15 +103,16 @@
     def __int__(self):
         return int(str(self))
 
     def format(self, url, **kwargs):
         return url.format(ymd=str(self), y=str(self.y), m=str(self.m), d=str(self.d), **kwargs)
 
     @property
-    def dt(self) -> DatetimeScalar:
+    def dt(self):
+        import pandas as pd
         return pd.to_datetime('%d-%02d-%02d' % (self.y, self.m, self.d))
 
     @property
     def date(self) -> date:
         return self.dt.date()
 
     def __add__(self, n: int) -> 'YMD':
@@ -135,14 +134,15 @@
             cur = cur + step
 
 
 def dates(*flags, default_start=None, default_end=None, help=None):
     if not flags:
         flags = ('-d', '--dates')
 
+    from click import option
     def _dates(fn):
         @option(*flags, help=help)
         @wraps(fn)
         def _fn(*args, dates=None, **kwargs):
             if dates:
                 pcs = dates.split('-')
                 if len(pcs) == 2:
```

### Comparing `utz-0.4.0/utz/zip.py` & `utz-0.4.1/utz/zip.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.0/utz.egg-info/PKG-INFO` & `utz-0.4.1/utz.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: utz
-Version: 0.4.0
-Summary: *("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
+Version: 0.4.1
+Summary: ("oots"): imports and utilities for easy wildcard-importing + boilerplate-reduction
 Home-page: https://github.com/runsascoded/utz
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dt
+Provides-Extra: git
+Provides-Extra: pd
 Provides-Extra: pdf
+Provides-Extra: setup
 Provides-Extra: test
+Provides-Extra: all
 License-File: LICENSE
 
 # utz
 *("oots")*: imports and utilities for easy wildcard-importing + boilerplate-reduction
 
 ## Install
 ```bash
```

### Comparing `utz-0.4.0/utz.egg-info/SOURCES.txt` & `utz-0.4.1/utz.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 setup.py
 utz/__init__.py
 utz/argparse.py
 utz/backoff.py
 utz/bases.py
-utz/cached_property.py
 utz/case.py
 utz/cd.py
 utz/cli.py
 utz/collections.py
 utz/colors.py
 utz/context.py
 utz/dataclasses.py
```

