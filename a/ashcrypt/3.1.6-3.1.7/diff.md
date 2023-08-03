# Comparing `tmp/ashcrypt-3.1.6.tar.gz` & `tmp/ashcrypt-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.1.6.tar", last modified: Thu Aug  3 11:53:29 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.1.7.tar", last modified: Thu Aug  3 14:12:23 2023, max compression
```

## Comparing `ashcrypt-3.1.6.tar` & `ashcrypt-3.1.7.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/exceptions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/sandbox/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/exceptions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/setup.py
```

### Comparing `ashcrypt-3.1.6/PKG-INFO` & `ashcrypt-3.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.6
+Version: 3.1.7
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.6/README.md` & `ashcrypt-3.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,14 @@
 
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
 python -m ashcrypt.gui
 ```
 
-**NOTE**:
-You  can use `clicrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
-
-
-To run the CLI 
-```shell
-python -m ashcrypt.clicrypt
-```
-
 ## `crypt` Module ##
 The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
```

### Comparing `ashcrypt-3.1.6/ashcrypt/clicrypt.py` & `ashcrypt-3.1.7/ashcrypt/sandbox/clicrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Experimental phase"""
+
 from ashcrypt.utils.safepack import file as af
 from ashcrypt.utils.safepack import text as at
 from typing import Optional
 import os.path
 import sys
```

### Comparing `ashcrypt-3.1.6/ashcrypt/crypt.py` & `ashcrypt-3.1.7/ashcrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt/database.py` & `ashcrypt-3.1.7/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt/filecrypt.py` & `ashcrypt-3.1.7/ashcrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt/gui.py` & `ashcrypt-3.1.7/ashcrypt/gui.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt/textcrypt.py` & `ashcrypt-3.1.7/ashcrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt/unittests/unittest_crypt.py` & `ashcrypt-3.1.7/ashcrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt/utils/exceptions/main.py` & `ashcrypt-3.1.7/ashcrypt/utils/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt/utils/safepack/file.py` & `ashcrypt-3.1.7/ashcrypt/utils/safepack/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt/utils/safepack/text.py` & `ashcrypt-3.1.7/ashcrypt/utils/safepack/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.6/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.1.7/ashcrypt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.6
+Version: 3.1.7
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.6/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.1.7/ashcrypt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 README.md
 setup.py
 ashcrypt/README.md
 ashcrypt/__init__.py
-ashcrypt/clicrypt.py
 ashcrypt/crypt.py
 ashcrypt/database.py
 ashcrypt/filecrypt.py
 ashcrypt/gui.py
 ashcrypt/textcrypt.py
 ashcrypt.egg-info/PKG-INFO
 ashcrypt.egg-info/SOURCES.txt
 ashcrypt.egg-info/dependency_links.txt
 ashcrypt.egg-info/requires.txt
 ashcrypt.egg-info/top_level.txt
+ashcrypt/sandbox/__init__.py
+ashcrypt/sandbox/clicrypt.py
 ashcrypt/unittests/__init__.py
 ashcrypt/unittests/unittest_crypt.py
 ashcrypt/utils/__init__.py
 ashcrypt/utils/exceptions/__init__.py
 ashcrypt/utils/exceptions/main.py
 ashcrypt/utils/safepack/__init__.py
 ashcrypt/utils/safepack/file.py
```

### Comparing `ashcrypt-3.1.6/setup.py` & `ashcrypt-3.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.1.6',
+    version='3.1.7',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

