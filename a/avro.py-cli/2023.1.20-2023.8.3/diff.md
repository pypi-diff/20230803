# Comparing `tmp/avro.py-cli-2023.1.20.tar.gz` & `tmp/avro.py-cli-2023.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro.py-cli-2023.1.20.tar", last modified: Fri Jan 20 16:59:22 2023, max compression
+gzip compressed data, was "avro.py-cli-2023.8.3.tar", last modified: Thu Aug  3 08:21:37 2023, max compression
```

## Comparing `avro.py-cli-2023.1.20.tar` & `avro.py-cli-2023.8.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:59:22.729627 avro.py-cli-2023.1.20/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-20 16:59:11.000000 avro.py-cli-2023.1.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-01-20 16:59:22.729627 avro.py-cli-2023.1.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-01-20 16:59:11.000000 avro.py-cli-2023.1.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:59:22.729627 avro.py-cli-2023.1.20/avro.py_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-01-20 16:59:22.000000 avro.py-cli-2023.1.20/avro.py_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-20 16:59:22.000000 avro.py-cli-2023.1.20/avro.py_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 16:59:22.000000 avro.py-cli-2023.1.20/avro.py_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-20 16:59:22.000000 avro.py-cli-2023.1.20/avro.py_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-20 16:59:22.000000 avro.py-cli-2023.1.20/avro.py_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-20 16:59:22.000000 avro.py-cli-2023.1.20/avro.py_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:59:22.729627 avro.py-cli-2023.1.20/avrocli/
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-20 16:59:11.000000 avro.py-cli-2023.1.20/avrocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-01-20 16:59:11.000000 avro.py-cli-2023.1.20/avrocli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-20 16:59:11.000000 avro.py-cli-2023.1.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 16:59:22.729627 avro.py-cli-2023.1.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-01-20 16:59:11.000000 avro.py-cli-2023.1.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:21:37.093445 avro.py-cli-2023.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 08:21:25.000000 avro.py-cli-2023.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-03 08:21:37.093445 avro.py-cli-2023.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-03 08:21:25.000000 avro.py-cli-2023.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:21:37.093445 avro.py-cli-2023.8.3/avro.py_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-03 08:21:37.000000 avro.py-cli-2023.8.3/avro.py_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 08:21:37.000000 avro.py-cli-2023.8.3/avro.py_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:21:37.000000 avro.py-cli-2023.8.3/avro.py_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 08:21:37.000000 avro.py-cli-2023.8.3/avro.py_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 08:21:37.000000 avro.py-cli-2023.8.3/avro.py_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 08:21:37.000000 avro.py-cli-2023.8.3/avro.py_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:21:37.093445 avro.py-cli-2023.8.3/avrocli/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 08:21:25.000000 avro.py-cli-2023.8.3/avrocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-03 08:21:25.000000 avro.py-cli-2023.8.3/avrocli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 08:21:25.000000 avro.py-cli-2023.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:21:37.093445 avro.py-cli-2023.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-03 08:21:25.000000 avro.py-cli-2023.8.3/setup.py
```

### Comparing `avro.py-cli-2023.1.20/LICENSE` & `avro.py-cli-2023.8.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 HitBlast
+Copyright (c) 2023 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `avro.py-cli-2023.1.20/setup.py` & `avro.py-cli-2023.8.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+# SPDX-License-Identifier: MIT
+
+
 # Import both local and third-party setup modules.
-import os
 import codecs
-from setuptools import setup, find_packages
+import os
+
+from setuptools import find_packages, setup
 
 # Import version information from local module.
 from avrocli import __version__
 
 # Constants.
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # Call the setup() function.
 setup(
     name='avro.py-cli',
     version=__version__,
-    description='A command-line wrapper for avro.py to ease '
-    + 'Bangla phonetic workflow inside your terminal.',
+    description='A simple CLI for avro.py to ease Bangla phonetic workflow inside your terminal.',
     long_description_content_type='text/markdown',
     long_description=long_description,
     author='HitBlast',
     author_email='hitblastlive@gmail.com',
     url='https://github.com/hitblast/avro.py-cli',
     packages=find_packages(),
     license='MIT',
```

