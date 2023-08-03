# Comparing `tmp/pyiosbackup-0.2.2.tar.gz` & `tmp/pyiosbackup-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiosbackup-0.2.2.tar", last modified: Fri May 12 10:49:23 2023, max compression
+gzip compressed data, was "pyiosbackup-0.2.3.tar", last modified: Thu Aug  3 07:56:58 2023, max compression
```

## Comparing `pyiosbackup-0.2.2.tar` & `pyiosbackup-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43919 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/pyiosbackup/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/keybag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/manifest_db_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/mbdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_plist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/pyiosbackup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43919 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/tests/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/tests/test_keybag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:56:58.794718 pyiosbackup-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43919 2023-08-03 07:56:58.794718 pyiosbackup-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:56:58.794718 pyiosbackup-0.2.3/pyiosbackup/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/keybag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:56:58.794718 pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/manifest_db_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/mbdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyiosbackup/manifest_plist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:56:58.794718 pyiosbackup-0.2.3/pyiosbackup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43919 2023-08-03 07:56:58.000000 pyiosbackup-0.2.3/pyiosbackup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-03 07:56:58.000000 pyiosbackup-0.2.3/pyiosbackup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:56:58.000000 pyiosbackup-0.2.3/pyiosbackup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 07:56:58.000000 pyiosbackup-0.2.3/pyiosbackup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 07:56:58.000000 pyiosbackup-0.2.3/pyiosbackup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 07:56:58.000000 pyiosbackup-0.2.3/pyiosbackup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:56:58.794718 pyiosbackup-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:56:58.794718 pyiosbackup-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/tests/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 07:56:44.000000 pyiosbackup-0.2.3/tests/test_keybag.py
```

### Comparing `pyiosbackup-0.2.2/LICENSE` & `pyiosbackup-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/PKG-INFO` & `pyiosbackup-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiosbackup
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python parser for iOS backups
 Author-email: Matan Perelman <matan1008@gmail.com>
 Maintainer-email: Matan Perelman <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pyiosbackup-0.2.2/README.md` & `pyiosbackup-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup/__main__.py` & `pyiosbackup-0.2.3/pyiosbackup/__main__.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup/backup.py` & `pyiosbackup-0.2.3/pyiosbackup/backup.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup/entry.py` & `pyiosbackup-0.2.3/pyiosbackup/entry.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup/keybag.py` & `pyiosbackup-0.2.3/pyiosbackup/keybag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import hashlib
 import logging
+import math
 
 from construct import Bytes, this, Int32ub, GreedyRange, IfThenElse
-from packaging.version import Version
 from construct import Struct, GreedyBytes, Int32ul
-from cryptography.hazmat.primitives.keywrap import aes_key_unwrap
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from cryptography.hazmat.primitives.keywrap import aes_key_unwrap
+from packaging.version import Version
 
 from pyiosbackup.manifest_plist import ManifestPlist
 
 logger = logging.getLogger('pyiosbackup')
 
 encryption_key_struct = Struct(
     'class_' / Int32ul,
@@ -54,15 +55,16 @@
         :param manifest: Loaded Manifest.plist file.
         :param password: Password to encrypted backup.
         :return: Keybag object.
         :rtype: Keybag
         """
         keybag = keybag_struct.parse(manifest.keybag)
         # The class count excludes the root class (first class in the keybag) and is one based.
-        class_count = [e.data for e in keybag if e.tag == b'CLAS'][0] - 1
+        first_class_index = [i for i in range(len(keybag)) if keybag[i].tag == b'CLAS'][0]
+        class_count = math.ceil((len(keybag) - first_class_index) / Keybag.CLASS_ELEMENTS_COUNT)
         logger.debug(f'Found {class_count} key classes')
         classes_index = len(keybag) - (Keybag.CLASS_ELEMENTS_COUNT * class_count)
         decryption_key = Keybag._decryption_key_from_password(password, keybag[:classes_index], manifest)
         logger.debug(f'Using decryption key {decryption_key.hex()}')
 
         classes_keys = {}
         for cls_offset in range(classes_index, len(keybag), Keybag.CLASS_ELEMENTS_COUNT):
```

### Comparing `pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/factory.py` & `pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/factory.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/manifest_db_interface.py` & `pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/manifest_db_interface.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/mbdb.py` & `pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/mbdb.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/sqlite3.py` & `pyiosbackup-0.2.3/pyiosbackup/manifest_dbs/sqlite3.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup/manifest_plist.py` & `pyiosbackup-0.2.3/pyiosbackup/manifest_plist.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyiosbackup.egg-info/PKG-INFO` & `pyiosbackup-0.2.3/pyiosbackup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiosbackup
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python parser for iOS backups
 Author-email: Matan Perelman <matan1008@gmail.com>
 Maintainer-email: Matan Perelman <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pyiosbackup-0.2.2/pyiosbackup.egg-info/SOURCES.txt` & `pyiosbackup-0.2.3/pyiosbackup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/pyproject.toml` & `pyiosbackup-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyiosbackup"
-version = "0.2.2"
+version = "0.2.3"
 description = "A python parser for iOS backups"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["ios", "backup", "automation"]
 authors = [
     { name = "Matan Perelman", email = "matan1008@gmail.com" }
```

### Comparing `pyiosbackup-0.2.2/tests/test_backup.py` & `pyiosbackup-0.2.3/tests/test_backup.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.2/tests/test_keybag.py` & `pyiosbackup-0.2.3/tests/test_keybag.py`

 * *Files identical despite different names*

