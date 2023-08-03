# Comparing `tmp/gitignore_parser-0.1.4.tar.gz` & `tmp/gitignore_parser-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitignore_parser-0.1.4.tar", last modified: Fri Jun 30 06:08:41 2023, max compression
+gzip compressed data, was "gitignore_parser-0.1.5.tar", last modified: Thu Aug  3 16:39:16 2023, max compression
```

## Comparing `gitignore_parser-0.1.4.tar` & `gitignore_parser-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-30 06:08:41.284660 gitignore_parser-0.1.4/
--rw-r--r--   0 michael   (1000) michael   (1000)     1103 2022-11-20 03:41:09.000000 gitignore_parser-0.1.4/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     1052 2023-06-30 06:08:41.284660 gitignore_parser-0.1.4/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2022-11-20 03:41:09.000000 gitignore_parser-0.1.4/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-30 06:08:41.284660 gitignore_parser-0.1.4/gitignore_parser.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1052 2023-06-30 06:08:41.000000 gitignore_parser-0.1.4/gitignore_parser.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-06-30 06:08:41.000000 gitignore_parser-0.1.4/gitignore_parser.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-30 06:08:41.000000 gitignore_parser-0.1.4/gitignore_parser.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-06-30 06:08:41.000000 gitignore_parser-0.1.4/gitignore_parser.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-06-30 06:08:41.000000 gitignore_parser-0.1.4/gitignore_parser.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     7457 2023-06-30 06:07:31.000000 gitignore_parser-0.1.4/gitignore_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-06-30 06:08:41.284660 gitignore_parser-0.1.4/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     1332 2023-06-30 06:08:05.000000 gitignore_parser-0.1.4/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:39:16.130197 gitignore_parser-0.1.5/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1058 2023-08-03 16:39:16.130197 gitignore_parser-0.1.5/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     1404 2022-08-29 10:41:38.000000 gitignore_parser-0.1.5/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:39:16.130197 gitignore_parser-0.1.5/gitignore_parser.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1058 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     7409 2023-08-03 16:38:19.000000 gitignore_parser-0.1.5/gitignore_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-08-03 16:39:16.130197 gitignore_parser-0.1.5/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     1332 2023-08-03 16:38:42.000000 gitignore_parser-0.1.5/setup.py
```

### Comparing `gitignore_parser-0.1.4/PKG-INFO` & `gitignore_parser-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: gitignore_parser
-Version: 0.1.4
+Version: 0.1.5
 Summary: A spec-compliant gitignore parser for Python 3.5+
 Home-page: https://github.com/mherrmann/gitignore_parser
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: MIT
+Description: A spec-compliant gitignore parser for Python 3.5+
+        
+        https://github.com/mherrmann/gitignore_parser
 Keywords: gitignore
 Platform: MacOS
 Platform: Windows
 Platform: Debian
 Platform: Fedora
 Platform: CentOS
 Classifier: Development Status :: 3 - Alpha
@@ -19,12 +22,7 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE
-
-A spec-compliant gitignore parser for Python 3.5+
-
-https://github.com/mherrmann/gitignore_parser
```

### Comparing `gitignore_parser-0.1.4/README.md` & `gitignore_parser-0.1.5/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# gitignore_parser
-
-![CI](https://github.com/mherrmann/gitignore_parser/workflows/CI/badge.svg)
-[![PyPI version](https://badge.fury.io/py/gitignore-parser.svg)](https://badge.fury.io/py/gitignore-parser)
-
-A spec-compliant gitignore parser for Python
-
-## Installation
-
-    pip install gitignore_parser
-
-## Usage
-
-Suppose `/home/michael/project/.gitignore` contains the following:
-
-    __pycache__/
-    *.py[cod]
-
-Then:
-
-    >>> from gitignore_parser import parse_gitignore
-    >>> matches = parse_gitignore('/home/michael/project/.gitignore')
-    >>> matches('/home/michael/project/main.py')
-    False
-    >>> matches('/home/michael/project/main.pyc')
-    True
-    >>> matches('/home/michael/project/dir/main.pyc')
-    True
-    >>> matches('/home/michael/project/__pycache__')
-    True
-
-## Motivation
-
-I couldn't find a good library for doing the above on PyPI. There are
-several other libraries, but they don't seem to support all features,
-be it the square brackets in `*.py[cod]` or top-level paths `/...`.
-
-## Contributing
-
-I'm very open to merging PRs. But before you start working on one, please
-read through my
-[guidelines for PRs](https://gist.github.com/mherrmann/5ce21814789152c17abd91c0b3eaadca).
-It will save us both time and unnecessary effort.
-
-## Attribution
-
-The implementation is based on https://github.com/snark/ignorance/ by
-Steve Cook.
+# gitignore_parser
+
+![CI](https://github.com/mherrmann/gitignore_parser/workflows/CI/badge.svg)
+[![PyPI version](https://badge.fury.io/py/gitignore-parser.svg)](https://badge.fury.io/py/gitignore-parser)
+
+A spec-compliant gitignore parser for Python
+
+## Installation
+
+    pip install gitignore_parser
+
+## Usage
+
+Suppose `/home/michael/project/.gitignore` contains the following:
+
+    __pycache__/
+    *.py[cod]
+
+Then:
+
+    >>> from gitignore_parser import parse_gitignore
+    >>> matches = parse_gitignore('/home/michael/project/.gitignore')
+    >>> matches('/home/michael/project/main.py')
+    False
+    >>> matches('/home/michael/project/main.pyc')
+    True
+    >>> matches('/home/michael/project/dir/main.pyc')
+    True
+    >>> matches('/home/michael/project/__pycache__')
+    True
+
+## Motivation
+
+I couldn't find a good library for doing the above on PyPI. There are
+several other libraries, but they don't seem to support all features,
+be it the square brackets in `*.py[cod]` or top-level paths `/...`.
+
+## Contributing
+
+I'm very open to merging PRs. But before you start working on one, please
+read through my
+[guidelines for PRs](https://gist.github.com/mherrmann/5ce21814789152c17abd91c0b3eaadca).
+It will save us both time and unnecessary effort.
+
+## Attribution
+
+The implementation is based on https://github.com/snark/ignorance/ by
+Steve Cook.
```

### Comparing `gitignore_parser-0.1.4/gitignore_parser.egg-info/PKG-INFO` & `gitignore_parser-0.1.5/gitignore_parser.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: gitignore-parser
-Version: 0.1.4
+Version: 0.1.5
 Summary: A spec-compliant gitignore parser for Python 3.5+
 Home-page: https://github.com/mherrmann/gitignore_parser
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: MIT
+Description: A spec-compliant gitignore parser for Python 3.5+
+        
+        https://github.com/mherrmann/gitignore_parser
 Keywords: gitignore
 Platform: MacOS
 Platform: Windows
 Platform: Debian
 Platform: Fedora
 Platform: CentOS
 Classifier: Development Status :: 3 - Alpha
@@ -19,12 +22,7 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE
-
-A spec-compliant gitignore parser for Python 3.5+
-
-https://github.com/mherrmann/gitignore_parser
```

### Comparing `gitignore_parser-0.1.4/gitignore_parser.py` & `gitignore_parser-0.1.5/gitignore_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import collections
 import os
 import re
 
 from os.path import dirname
 from pathlib import Path
-from typing import Union
+from typing import Reversible, Union
 
-def handle_negation(file_path, rules):
-    matched = False
-    for rule in rules:
+def handle_negation(file_path, rules: Reversible["IgnoreRule"]):
+    for rule in reversed(rules):
         if rule.match(file_path):
-            if rule.negation:
-                matched = False
-            else:
-                matched = True
-    return matched
+            return not rule.negation
+    return False
 
 def parse_gitignore(full_path, base_dir=None):
     if base_dir is None:
         base_dir = dirname(full_path)
     rules = []
     with open(full_path) as ignore_file:
         counter = 0
```

### Comparing `gitignore_parser-0.1.4/setup.py` & `gitignore_parser-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from setuptools import setup
 
 description = 'A spec-compliant gitignore parser for Python 3.5+'
 setup(
     name='gitignore_parser',
-    version='0.1.4',
+    version='0.1.5',
     install_requires=["pathlib; python_version < '3.0'"],
     description=description,
     long_description=
         description + '\n\nhttps://github.com/mherrmann/gitignore_parser',
     author='Michael Herrmann',
     author_email='michael+removethisifyouarehuman@herrmann.io',
     url='https://github.com/mherrmann/gitignore_parser',
```

