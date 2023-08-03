# Comparing `tmp/angola-0.14.5.tar.gz` & `tmp/angola-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.14.5.tar", last modified: Tue Jul  4 07:17:32 2023, max compression
+gzip compressed data, was "angola-0.15.0.tar", last modified: Thu Aug  3 08:07:44 2023, max compression
```

## Comparing `angola-0.14.5.tar` & `angola-0.15.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.035042 angola-0.14.5/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.14.5/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.14.5/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-07-04 07:17:32.035113 angola-0.14.5/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.14.5/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-07-04 07:17:32.035376 angola-0.14.5/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      776 2023-07-04 07:17:19.000000 angola-0.14.5/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.027635 angola-0.14.5/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.031650 angola-0.14.5/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.14.5/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    51001 2023-06-28 16:10:18.000000 angola-0.14.5/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.14.5/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.14.5/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    18643 2023-07-04 07:17:12.000000 angola-0.14.5/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.14.5/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.033099 angola-0.14.5/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       47 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.034900 angola-0.14.5/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.14.5/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.14.5/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.14.5/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     4810 2023-06-30 07:41:06.000000 angola-0.14.5/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.14.5/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.283976 angola-0.15.0/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.15.0/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.15.0/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-08-03 08:07:44.284049 angola-0.15.0/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.15.0/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-08-03 08:07:44.284298 angola-0.15.0/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      793 2023-08-03 07:57:57.000000 angola-0.15.0/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.277460 angola-0.15.0/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.281396 angola-0.15.0/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.15.0/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    51001 2023-06-28 16:10:18.000000 angola-0.15.0/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.15.0/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.15.0/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18665 2023-08-03 08:03:16.000000 angola-0.15.0/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.15.0/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.282535 angola-0.15.0/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       53 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.283864 angola-0.15.0/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.15.0/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.15.0/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.15.0/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     4810 2023-06-30 07:41:06.000000 angola-0.15.0/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.15.0/tests/test_query.py
```

### Comparing `angola-0.14.5/LICENSE` & `angola-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.14.5/PKG-INFO` & `angola-0.15.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.14.5
+Version: 0.15.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.14.5/README.md` & `angola-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.14.5/setup.py` & `angola-0.15.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.14.5"
+VERSION = "0.15.0"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
@@ -18,14 +18,15 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Topic :: Database',
     ],
     python_requires='>=3.8.0',
     install_requires = [
+        "cuid2",
         "Jinja2 >= 3.0",
         "python-slugify",
         "arrow",
         "python-arango"
     ],
     packages=['angola'],
     package_dir={'':'src'}
```

### Comparing `angola-0.14.5/src/angola/database.py` & `angola-0.15.0/src/angola/database.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.5/src/angola/dict_mutator.py` & `angola-0.15.0/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.5/src/angola/dict_query.py` & `angola-0.15.0/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.5/src/angola/lib.py` & `angola-0.15.0/src/angola/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import re
 import sys
 import json
 import math
 import uuid
 import time
 import arrow
+import cuid2
 import string
 import random
 import secrets
 import hashlib
 import datetime
 from slugify import slugify
 from jinja2 import Template
@@ -81,17 +82,18 @@
     return bool(pattern.match(name)) 
 
 
 
 def gen_xid() -> str:
     """
     XID - To be used as id. 
-    Return UUID4. 32 Chars
+    Return CUID2 - 16 chars
     """
-    return str(uuid.uuid4()).replace("-", "")
+    l = 16
+    return cuid2.Cuid(length=l).generate()
 
 def gen_key() -> str:
     """
     To be used as random key
     Return UUID7. 32 Chars
     """
     return gen_xid()
```

### Comparing `angola-0.14.5/src/angola/lib_xql.py` & `angola-0.15.0/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.5/src/angola.egg-info/PKG-INFO` & `angola-0.15.0/src/angola.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.14.5
+Version: 0.15.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.14.5/tests/test_database.py` & `angola-0.15.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.5/tests/test_dict_mutator.py` & `angola-0.15.0/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.5/tests/test_lib.py` & `angola-0.15.0/tests/test_lib.py`

 * *Files identical despite different names*

