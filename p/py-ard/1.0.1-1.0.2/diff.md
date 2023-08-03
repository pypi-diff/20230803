# Comparing `tmp/py-ard-1.0.1.tar.gz` & `tmp/py-ard-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ard-1.0.1.tar", last modified: Fri Jun 23 21:44:53 2023, max compression
+gzip compressed data, was "py-ard-1.0.2.tar", last modified: Thu Aug  3 14:32:21 2023, max compression
```

## Comparing `py-ard-1.0.1.tar` & `py-ard-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:44:53.928184 py-ard-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-23 21:44:42.000000 py-ard-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-23 21:44:42.000000 py-ard-1.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 21:44:42.000000 py-ard-1.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-23 21:44:42.000000 py-ard-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 21:44:42.000000 py-ard-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-06-23 21:44:53.928184 py-ard-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-06-23 21:44:42.000000 py-ard-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:44:53.924184 py-ard-1.0.1/py_ard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:44:53.928184 py-ard-1.0.1/pyard/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/CWD2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28985 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/ard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/blender.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/broad_splits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/dna_relshp.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/drbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/smart_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 21:44:42.000000 py-ard-1.0.1/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 21:44:42.000000 py-ard-1.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:44:53.928184 py-ard-1.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-06-23 21:44:42.000000 py-ard-1.0.1/scripts/pyard
--rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-06-23 21:44:42.000000 py-ard-1.0.1/scripts/pyard-import
--rwxr-xr-x   0 runner    (1001) docker     (123)    15408 2023-06-23 21:44:42.000000 py-ard-1.0.1/scripts/pyard-reduce-csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-06-23 21:44:42.000000 py-ard-1.0.1/scripts/pyard-status
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-23 21:44:53.928184 py-ard-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-23 21:44:42.000000 py-ard-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:32:21.813893 py-ard-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-03 14:32:11.000000 py-ard-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-03 14:32:11.000000 py-ard-1.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-03 14:32:11.000000 py-ard-1.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-03 14:32:11.000000 py-ard-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-03 14:32:11.000000 py-ard-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-08-03 14:32:21.813893 py-ard-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-08-03 14:32:11.000000 py-ard-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:32:21.809893 py-ard-1.0.2/py_ard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-08-03 14:32:21.000000 py-ard-1.0.2/py_ard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-03 14:32:21.000000 py-ard-1.0.2/py_ard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:32:21.000000 py-ard-1.0.2/py_ard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:32:21.000000 py-ard-1.0.2/py_ard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 14:32:21.000000 py-ard-1.0.2/py_ard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 14:32:21.000000 py-ard-1.0.2/py_ard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:32:21.813893 py-ard-1.0.2/pyard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/CWD2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29146 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/ard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/blender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/broad_splits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/dna_relshp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/drbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-03 14:32:11.000000 py-ard-1.0.2/pyard/smart_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 14:32:11.000000 py-ard-1.0.2/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 14:32:11.000000 py-ard-1.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:32:21.813893 py-ard-1.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-08-03 14:32:11.000000 py-ard-1.0.2/scripts/pyard
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-08-03 14:32:11.000000 py-ard-1.0.2/scripts/pyard-import
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15408 2023-08-03 14:32:11.000000 py-ard-1.0.2/scripts/pyard-reduce-csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-08-03 14:32:11.000000 py-ard-1.0.2/scripts/pyard-status
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 14:32:21.813893 py-ard-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-03 14:32:11.000000 py-ard-1.0.2/setup.py
```

### Comparing `py-ard-1.0.1/CONTRIBUTING.rst` & `py-ard-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/COPYING` & `py-ard-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/LICENSE` & `py-ard-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/PKG-INFO` & `py-ard-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.0.1
+Version: 1.0.2
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
```

### Comparing `py-ard-1.0.1/README.md` & `py-ard-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/py_ard.egg-info/PKG-INFO` & `py-ard-1.0.2/py_ard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.0.1
+Version: 1.0.2
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
```

### Comparing `py-ard-1.0.1/py_ard.egg-info/SOURCES.txt` & `py-ard-1.0.2/py_ard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/CWD2.csv` & `py-ard-1.0.2/pyard/CWD2.csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/__init__.py` & `py-ard-1.0.2/pyard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from .blender import blender as dr_blender
 from .broad_splits import find_splits as find_broad_splits
 from .constants import DEFAULT_CACHE_SIZE
 from .misc import get_imgt_db_versions as db_versions
 
 __author__ = """NMDP Bioinformatics"""
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 
 def init(
     imgt_version: str = "Latest",
     data_dir: str = None,
     load_mac: bool = True,
     cache_size: int = DEFAULT_CACHE_SIZE,
```

### Comparing `py-ard-1.0.1/pyard/ard.py` & `py-ard-1.0.2/pyard/ard.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #    Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA.
 #
 #    > http://www.fsf.org/licensing/licenses/lgpl.html
 #    > http://www.opensource.org/licenses/lgpl-license.php
 #
 import functools
 import re
+import sqlite3
 import sys
 from typing import Iterable, List
 
 from . import broad_splits, smart_sort
 from . import data_repository as dr
 from . import db
 from .exceptions import InvalidAlleleError, InvalidMACError, InvalidTypingError
@@ -469,15 +470,19 @@
         Not all strings are MACs e.g. ":THISISNOTAMAC"
 
         :param allele: test if it is a MAC code
         :return: True if MAC
         """
         if ":" in allele:
             code = allele.split(":")[1]
-            return db.is_valid_mac_code(self.db_connection, code)
+            try:
+                if code.isalpha():
+                    return db.is_valid_mac_code(self.db_connection, code)
+            except sqlite3.OperationalError as e:
+                print("Error: ", e)
         return False
 
     def is_v2(self, allele: str) -> bool:
         """
         Version 2 of the nomenclature is a single field.
         It does not have any ':' field separator.
             Eg: A*0104
```

### Comparing `py-ard-1.0.1/pyard/blender.py` & `py-ard-1.0.2/pyard/blender.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/broad_splits.py` & `py-ard-1.0.2/pyard/broad_splits.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/constants.py` & `py-ard-1.0.2/pyard/constants.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/data_repository.py` & `py-ard-1.0.2/pyard/data_repository.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/db.py` & `py-ard-1.0.2/pyard/db.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/drbx.py` & `py-ard-1.0.2/pyard/drbx.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/exceptions.py` & `py-ard-1.0.2/pyard/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/load.py` & `py-ard-1.0.2/pyard/load.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/mappings.py` & `py-ard-1.0.2/pyard/mappings.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/misc.py` & `py-ard-1.0.2/pyard/misc.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/pyard/smart_sort.py` & `py-ard-1.0.2/pyard/smart_sort.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/scripts/pyard` & `py-ard-1.0.2/scripts/pyard`

 * *Files 1% similar despite different names*

```diff
@@ -112,9 +112,8 @@
         print("Allele Error:", e.message, file=sys.stderr)
         sys.exit(1)
     except InvalidTypingError as e:
         print("Typing Error:", e.message, file=sys.stderr)
         sys.exit(2)
     else:
         # Remove ard and close db connection
-        print("Removing")
         del ard
```

### Comparing `py-ard-1.0.1/scripts/pyard-import` & `py-ard-1.0.2/scripts/pyard-import`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/scripts/pyard-reduce-csv` & `py-ard-1.0.2/scripts/pyard-reduce-csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/scripts/pyard-status` & `py-ard-1.0.2/scripts/pyard-status`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.1/setup.cfg` & `py-ard-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.1
+current_version = 1.0.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `py-ard-1.0.1/setup.py` & `py-ard-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="py-ard",
-    version="1.0.1",
+    version="1.0.2",
     description="ARD reduction for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="CIBMTR",
     author_email="cibmtr-pypi@nmdp.org",
     url="https://github.com/nmdp-bioinformatics/py-ard",
     packages=[
```

