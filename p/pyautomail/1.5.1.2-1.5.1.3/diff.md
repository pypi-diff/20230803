# Comparing `tmp/pyautomail-1.5.1.2.tar.gz` & `tmp/pyautomail-1.5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautomail-1.5.1.2.tar", last modified: Mon Jul 31 04:05:07 2023, max compression
+gzip compressed data, was "pyautomail-1.5.1.3.tar", last modified: Thu Aug  3 00:58:02 2023, max compression
```

## Comparing `pyautomail-1.5.1.2.tar` & `pyautomail-1.5.1.3.tar`

### file list

```diff
@@ -1,62 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.095667 pyautomail-1.5.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/automail/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/automail/config/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/emailsender.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/automail/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/storage/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/storage/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/contact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   191926 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/_static/automail-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.095667 pyautomail-1.5.1.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/_templates/apidoc/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/_templates/apidoc/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/_templates/apidoc/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/_templates/apidoc/toc.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/api/automail.config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/api/automail.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/api/automail.storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/document.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/examples/base-usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/pyautomail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/sending_gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/templates/body.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/templates/html.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.946076 pyautomail-1.5.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.950076 pyautomail-1.5.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.950076 pyautomail-1.5.1.3/automail/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.950076 pyautomail-1.5.1.3/automail/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/emailsender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.950076 pyautomail-1.5.1.3/automail/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/storage/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/storage/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/automail/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/contact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   191926 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/_static/automail-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.946076 pyautomail-1.5.1.3/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/_templates/apidoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/_templates/apidoc/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/_templates/apidoc/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/_templates/apidoc/toc.rst_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/api/automail.config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/api/automail.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/api/automail.storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/document.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/examples/base-usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/pyautomail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 00:58:02.000000 pyautomail-1.5.1.3/pyautomail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/sending_gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-03 00:58:02.958077 pyautomail-1.5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/templates/body.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/templates/html.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:58:02.954076 pyautomail-1.5.1.3/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_cli/test_cli_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_cli/test_cli_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-03 00:57:53.000000 pyautomail-1.5.1.3/tests/test_manager.py
```

### Comparing `pyautomail-1.5.1.2/.readthedocs.yaml` & `pyautomail-1.5.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/PKG-INFO` & `pyautomail-1.5.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pyautomail
-Version: 1.5.1.2
-Summary: A Python pkg and command-line interface for Sending email to your contact list
-Home-page: https://github.com/msinamsina/automail
+Version: 1.5.1.3
+Summary: Automated Email Sending for Large Scale Email and Gmail Automation
+Home-page: https://github.com/msinamsina/pyautomail
 Author: Mohammad sina Allahkaram
 Author-email: msinamsina@gmail.com
 License: MIT
-Project-URL: Bug Tracker, https://github.com/msinamsina/automail/issues
-Project-URL: Changelog, https://github.com/msinamsina/automail/releases
-Project-URL: Documentation, https://automail.readthedocs.io/en/latest/
-Project-URL: Source Code, https://github.com/msinamsina/automail
+Project-URL: Bug Tracker, https://github.com/msinamsina/pyautomail/issues
+Project-URL: Changelog, https://github.com/msinamsina/pyautomail/releases
+Project-URL: Documentation, https://pyautomail.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/msinamsina/pyautomail
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # PyAutoMail: A Python package and command-line interface for automation sending email to your contact list
 
 
 <p align="center" width="100%">
-    <img  width="80%" src="https://github.com/msinamsina/automail/blob/main/docs/_static/automail-logo.png" >
+    <img  width="80%" src="https://github.com/msinamsina/automail/blob/main/docs/_static/automail-logo.png?raw=true" >
 </p>
 
 
 Pyautomail, an incredibly powerful Python package meticulously crafted for the purpose of automated email delivery, catering especially to large-scale Email or Gmail automation. In today's fast-paced digital era, effective communication stands as a crucial cornerstone for numerous businesses and projects that heavily rely on email as their primary medium of interaction. Nonetheless, the manual handling of individual emails or the management of bulk email campaigns can prove to be both time-consuming and prone to errors.
 
 Fear not, for pyautomail swoops in as the ultimate savior, offering a seamless and highly efficient solution for automating email communication. Be it the need to dispatch personalized emails to a vast audience, the execution of targeted email marketing campaigns, or the automation of repetitive email chores, this package serves as your ultimate go-to tool. With its user-friendly interface and an array of versatile features, pyautomail proves itself as a fitting choice for a wide range of applications, catering to startups, enterprises, professionals, and developers alike.
```

### Comparing `pyautomail-1.5.1.2/README.md` & `pyautomail-1.5.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyAutoMail: A Python package and command-line interface for automation sending email to your contact list
 
 
 <p align="center" width="100%">
-    <img  width="80%" src="https://github.com/msinamsina/automail/blob/main/docs/_static/automail-logo.png" >
+    <img  width="80%" src="https://github.com/msinamsina/automail/blob/main/docs/_static/automail-logo.png?raw=true" >
 </p>
 
 
 Pyautomail, an incredibly powerful Python package meticulously crafted for the purpose of automated email delivery, catering especially to large-scale Email or Gmail automation. In today's fast-paced digital era, effective communication stands as a crucial cornerstone for numerous businesses and projects that heavily rely on email as their primary medium of interaction. Nonetheless, the manual handling of individual emails or the management of bulk email campaigns can prove to be both time-consuming and prone to errors.
 
 Fear not, for pyautomail swoops in as the ultimate savior, offering a seamless and highly efficient solution for automating email communication. Be it the need to dispatch personalized emails to a vast audience, the execution of targeted email marketing campaigns, or the automation of repetitive email chores, this package serves as your ultimate go-to tool. With its user-friendly interface and an array of versatile features, pyautomail proves itself as a fitting choice for a wide range of applications, catering to startups, enterprises, professionals, and developers alike.
```

### Comparing `pyautomail-1.5.1.2/automail/config/config.py` & `pyautomail-1.5.1.3/automail/config/config.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/automail/emailsender.py` & `pyautomail-1.5.1.3/automail/emailsender.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/automail/manager.py` & `pyautomail-1.5.1.3/automail/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,32 @@
 # TODO: add a command to edit a process
 # TODO: add a command to edit a record
 # TODO: create a logger pkg
 
 __all__ = ['registration', 'start', 'stop', 'resume_process', 'list_processes', 'run']
 
 
-session, _ = get_session()
+def init(*args, **kwargs):
+    project_name = input('Enter the name of your project: ')
+    path = input('Enter the path to your project (default is current directory): ')
+    if path == '':
+        path = os.getcwd()
+    else:
+        path = os.path.abspath(path)
+    if not os.path.exists(path):
+        os.mkdir(path)
+    os.chdir(path)
+    session, engin = get_session()
+    create_tables(engin)
+
+    session.close()
+    engin.dispose()
 
 
-def registration(username, contacts, name, cpdf, attachment, pdf_dir, **args):
+def registration(username, contacts, name="", cpdf=False, attachment="", pdf_dir="", **args):
     """This function will register a new process and a new contact list
 
 
     Parameters
     ----------
     username : str
         the email address of the sender
@@ -67,47 +81,39 @@
     None
 
     Notes
     -----
     This function will register a new process plus records for each contact in the contacts csv file.
 
     """
-    process = Process(title=name, subject=args['subject'], sender=username,
-                      temp_file=args['template'], release_date=datetime.datetime.date(datetime.datetime.now()))
-    session.add(process)
-    session.commit()
+    from automail.storage import register_new_process
 
-    print(f"ID:{process.id} => Registering user {username} with contacts {contacts}")
-    contact_df = pd.read_csv(contacts)
-    for index, row in contact_df.iterrows():
-        filename = None
-        if attachment:
-            filename = attachment
-
-        if cpdf:
-            filename = os.path.join(pdf_dir, str(row['cpdf']) + '.pdf')
-        record = Record(receiver=row['email'], data=row.to_json(), process_id=process.id, attachment_path=filename)
-        session.add(record)
-        session.commit()
-        print(f"ID:{record.id} => Registering record for {row['email']}")
+    register_new_process(title=name, email=username, contact_list=contacts, custom_pdf=cpdf, attachment=attachment,
+                         custom_pdf_dir=pdf_dir, subject=args.get('subject', ""), template=args.get('template', ""))
+    print("Process registered successfully!")
+    print("You can start the process with 'automail start <process_id>' command")
 
 
 def run(pid, resume=True):
     """
     This function will run a process with a specific id
 
     Parameters
     ----------
     pid : int
         the process id
     resume : bool
         if True, the program will resume the process if it is paused, otherwise it prints a warning message and \
         return without doing anything
     """
+    session, engin = get_session()
+    create_tables(engin)
 
+    session.close()
+    engin.dispose()
     logger = init_logger('manager')
     logger.info("Reading arguments...")
     process = session.query(Process).filter(Process.id == pid).first()
     if not process:
         logger.error(f"ID:{pid} => Process not found. You can see all processes with 'mailmanager list' command")
         return
     sender_email = process.sender
@@ -168,14 +174,19 @@
 def start(pid, **args):
     """This function will start a process with a specific id"""
     run(pid, resume=False)
 
 
 def stop(pid, **args):
     """This function will stop a process with a specific id"""
+    session, engin = get_session()
+    create_tables(engin)
+
+    session.close()
+    engin.dispose()
     process = session.query(Process).filter(Process.id == pid).first()
     if process.status == "in progress":
         process.status = "paused"
         session.commit()
         print(f"ID: {pid} => Pausing the program")
     else:
         print(f"ID: {pid} => Program is not running")
@@ -191,28 +202,37 @@
 
     Parameters
     ----------
     pid : int
         the process id if you want to see the information of a specific process or None if you want to see the \
         information of all processes
     """
+    session, engin = get_session()
+    create_tables(engin)
+
+    session.close()
+    engin.dispose()
     if pid is None:
         processes = session.query(Process).all()
     else:
         processes = session.query(Process).filter(Process.id == pid).all()
 
     for process in processes:
         print(process.id, process.title, process.status,
               len(session.query(Record).filter(Record.process_id == process.id, Record.status == "unsent").all()),
               len(session.query(Record).filter(Record.process_id == process.id, Record.status == "sent").all()))
 
 
 def _parser():
-    parser_obj = argparse.ArgumentParser(description='Mail Manager', prog="mailmanager")
+    parser_obj = argparse.ArgumentParser(description='Automail', prog="automail")
     sud_parser = parser_obj.add_subparsers(dest='command')
+
+    init_parser = sud_parser.add_parser('init', help='Initialize the database')
+    init_parser.set_defaults(func=init)
+
     register_parser = sud_parser.add_parser('register', help='Register a new user')
     register_parser.add_argument('username', help='Username')
     register_parser.add_argument('contacts', help='Contacts')
     register_parser.add_argument('--name', help='A name')
     register_parser.add_argument('--template', help='Path to HTML or TXT Template')
     register_parser.add_argument('--subject', help='Subject of the email')
     register_parser.add_argument("--attachment", help="path to pdf file that you want to attach to your E-mail")
@@ -232,18 +252,19 @@
     resume_parser = sud_parser.add_parser('resume', help='Resume a process that is paused by id')
     resume_parser.add_argument('pid', help='process id')
     resume_parser.set_defaults(func=resume_process)
 
     list_parser = sud_parser.add_parser('list', help='List processes (all or a specific proces  by id')
     list_parser.add_argument('--pid', help='process id', default=None, required=False)
     list_parser.set_defaults(func=list_processes)
+
     return parser_obj
 
 
-def main():
-    parser_ = parser()
-    args_ = parser_.parse_args()
+def main(args=None):
+    parser_ = _parser()
+    args_ = parser_.parse_args(args)
     args_.func(**vars(args_))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pyautomail-1.5.1.2/automail/storage/model.py` & `pyautomail-1.5.1.3/automail/storage/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,7 +65,9 @@
     """str : the email address of the sender"""
     temp_file = Column(String)
     """str : the path to the template file"""
     subject = Column(String)
     """str : the subject of the email"""
     status = Column(ChoiceType(STATUSES), default='created')
     """str : the status of the process it can be choose from STATUSES"""
+    title = Column(String)
+    """str : the title of the process"""
```

### Comparing `pyautomail-1.5.1.2/docs/Makefile` & `pyautomail-1.5.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/docs/_static/automail-logo.png` & `pyautomail-1.5.1.3/docs/_static/automail-logo.png`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/docs/_templates/apidoc/package.rst_t` & `pyautomail-1.5.1.3/docs/_templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/docs/api/automail.rst` & `pyautomail-1.5.1.3/docs/api/automail.rst`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,23 @@
    :maxdepth: 2
 
    automail.config
    automail.storage
 
 
 
+automail.cli
+------------
+
+
+.. automodule:: automail.cli
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 automail.emailsender
 --------------------
 
 
 .. automodule:: automail.emailsender
    :members:
    :undoc-members:
```

### Comparing `pyautomail-1.5.1.2/docs/conf.py` & `pyautomail-1.5.1.3/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 import sys
 
 sys.path.insert(0, '../')
-project = 'Automail'
+project = 'PyAutoMail'
 copyright = '2023, Mohammad Sina Allahkaram'
 author = 'Mohammad Sina Allahkaram'
 release = '1.1.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
```

### Comparing `pyautomail-1.5.1.2/docs/getting-started.rst` & `pyautomail-1.5.1.3/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/docs/index.rst` & `pyautomail-1.5.1.3/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. Pyautomail documentation master file, created by
    sphinx-quickstart on Tue Jul 25 17:21:33 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-**PYAUTOMAIL: Automated Email Sending for Large Scale Email and Gmail Automation**
-================================================================================
+**PyAutoMail: Automated Email Sending for Large Scale Email and Gmail Automation**
+===================================================================================
 
 .. figure:: _static/automail-logo.png
    :align: center
    :alt: automail logo
    :width: 100%
 
 .. raw:: html
```

### Comparing `pyautomail-1.5.1.2/docs/introduction.rst` & `pyautomail-1.5.1.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/docs/make.bat` & `pyautomail-1.5.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/docs/tutorial/index.rst` & `pyautomail-1.5.1.3/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/document.pdf` & `pyautomail-1.5.1.3/document.pdf`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/pyautomail.egg-info/PKG-INFO` & `pyautomail-1.5.1.3/pyautomail.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pyautomail
-Version: 1.5.1.2
-Summary: A Python pkg and command-line interface for Sending email to your contact list
-Home-page: https://github.com/msinamsina/automail
+Version: 1.5.1.3
+Summary: Automated Email Sending for Large Scale Email and Gmail Automation
+Home-page: https://github.com/msinamsina/pyautomail
 Author: Mohammad sina Allahkaram
 Author-email: msinamsina@gmail.com
 License: MIT
-Project-URL: Bug Tracker, https://github.com/msinamsina/automail/issues
-Project-URL: Changelog, https://github.com/msinamsina/automail/releases
-Project-URL: Documentation, https://automail.readthedocs.io/en/latest/
-Project-URL: Source Code, https://github.com/msinamsina/automail
+Project-URL: Bug Tracker, https://github.com/msinamsina/pyautomail/issues
+Project-URL: Changelog, https://github.com/msinamsina/pyautomail/releases
+Project-URL: Documentation, https://pyautomail.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/msinamsina/pyautomail
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # PyAutoMail: A Python package and command-line interface for automation sending email to your contact list
 
 
 <p align="center" width="100%">
-    <img  width="80%" src="https://github.com/msinamsina/automail/blob/main/docs/_static/automail-logo.png" >
+    <img  width="80%" src="https://github.com/msinamsina/automail/blob/main/docs/_static/automail-logo.png?raw=true" >
 </p>
 
 
 Pyautomail, an incredibly powerful Python package meticulously crafted for the purpose of automated email delivery, catering especially to large-scale Email or Gmail automation. In today's fast-paced digital era, effective communication stands as a crucial cornerstone for numerous businesses and projects that heavily rely on email as their primary medium of interaction. Nonetheless, the manual handling of individual emails or the management of bulk email campaigns can prove to be both time-consuming and prone to errors.
 
 Fear not, for pyautomail swoops in as the ultimate savior, offering a seamless and highly efficient solution for automating email communication. Be it the need to dispatch personalized emails to a vast audience, the execution of targeted email marketing campaigns, or the automation of repetitive email chores, this package serves as your ultimate go-to tool. With its user-friendly interface and an array of versatile features, pyautomail proves itself as a fitting choice for a wide range of applications, catering to startups, enterprises, professionals, and developers alike.
```

### Comparing `pyautomail-1.5.1.2/pyautomail.egg-info/SOURCES.txt` & `pyautomail-1.5.1.3/pyautomail.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 requirements.txt
 sending_gmail.py
 setup.cfg
 setup.py
 sub.txt
 .github/workflows/publish.yml
 automail/__init__.py
+automail/__main__.py
+automail/cli.py
 automail/emailsender.py
 automail/manager.py
 automail/utils.py
 automail/config/__init__.py
 automail/config/config.py
 automail/storage/__init__.py
 automail/storage/model.py
@@ -39,8 +41,14 @@
 pyautomail.egg-info/PKG-INFO
 pyautomail.egg-info/SOURCES.txt
 pyautomail.egg-info/dependency_links.txt
 pyautomail.egg-info/entry_points.txt
 pyautomail.egg-info/requires.txt
 pyautomail.egg-info/top_level.txt
 templates/body.txt
-templates/html.html
+templates/html.html
+tests/__init__.py
+tests/test_manager.py
+tests/test_cli/__init__.py
+tests/test_cli/test_cli.py
+tests/test_cli/test_cli_init.py
+tests/test_cli/test_cli_register.py
```

### Comparing `pyautomail-1.5.1.2/sending_gmail.py` & `pyautomail-1.5.1.3/sending_gmail.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.2/setup.py` & `pyautomail-1.5.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyautomail',
-    version='1.5.0',
+    version='1.5.1.3',
     packages=find_packages(),
-    url='https://github.com/msinamsina/automail',
+    url='https://github.com/msinamsina/pyautomail',
     license='MIT',
     author='Mohammad sina Allahkaram',
     author_email="msinamsina@gmail.com",
-    description='A Python pkg and command-line interface for Sending email to your contact list',
+    description='Automated Email Sending for Large Scale Email and Gmail Automation',
     install_requires=[
         'sqlalchemy',
         'sqlalchemy_utils',
         'jinja2',
         'pandas'
     ],
     long_description=open('README.md').read(),
```

