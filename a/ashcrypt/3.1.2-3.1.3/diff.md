# Comparing `tmp/ashcrypt-3.1.2.tar.gz` & `tmp/ashcrypt-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.1.2.tar", last modified: Wed Aug  2 22:05:28 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.1.3.tar", last modified: Wed Aug  2 22:46:57 2023, max compression
```

## Comparing `ashcrypt-3.1.2.tar` & `ashcrypt-3.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39561 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/exceptions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39564 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/exceptions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/ashcrypt/utils/gui/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:46:57.000000 ashcrypt-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 22:46:44.000000 ashcrypt-3.1.3/setup.py
```

### Comparing `ashcrypt-3.1.2/PKG-INFO` & `ashcrypt-3.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.2
+Version: 3.1.3
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.2/README.md` & `ashcrypt-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt/clicrypt.py` & `ashcrypt-3.1.3/ashcrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt/crypt.py` & `ashcrypt-3.1.3/ashcrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt/database.py` & `ashcrypt-3.1.3/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt/filecrypt.py` & `ashcrypt-3.1.3/ashcrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt/gui.py` & `ashcrypt-3.1.3/ashcrypt/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ashcrypt.utils.gui.text as At
 import ashcrypt.utils.gui.file as Af
-import ashcrypt.utils.gui as qr
+import ashcrypt.utils.gui.qr as qr
 import ashcrypt.database as Ad
 import ttkbootstrap as tk
 import platform
 import secrets
 import os.path
 import string
 import atexit
```

### Comparing `ashcrypt-3.1.2/ashcrypt/textcrypt.py` & `ashcrypt-3.1.3/ashcrypt/textcrypt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 """This module is used to encrypt and decrypt text data"""
 
-
-from ashcrypt import crypt as cp
 from ashcrypt.utils import exceptions
+from ashcrypt import crypt as ac
 from typing import Union
 
 
 class Crypt:
     def __init__(self, text: Union[str, bytes], key: str):
         self.text = text
         if self.keyverify(key) == 1:
             self.key = key
         else:
             raise exceptions.KeyLengthError()
 
     @staticmethod
     def genkey() -> str:
-        return cp.Enc.genkey()
+        return ac.Enc.genkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
         try:
             a = bytes.fromhex(key.strip())
             if len(a) == 32:
                 return 1
         except BaseException:
             return 0
 
     def encrypt(self) -> tuple:
         if self.text:
             try:
-                ins = cp.Enc(self.text, self.key)
+                ins = ac.Enc(self.text, self.key)
                 new_content = ins.encrypt()
                 return 1, new_content
             except BaseException:
                 raise exceptions.CryptError()
         else:
             raise exceptions.EmptyContentError()
 
     def decrypt(self) -> tuple:
         if self.text:
             try:
-                dec_instance = cp.Dec(message=self.text, mainkey=self.key)
+                dec_instance = ac.Dec(message=self.text, mainkey=self.key)
                 a = dec_instance.decrypt()
                 output = a
                 return 1, output
             except BaseException:
                 raise exceptions.CryptError()
         else:
             raise exceptions.EmptyContentError()
```

### Comparing `ashcrypt-3.1.2/ashcrypt/unittests/unittest_crypt.py` & `ashcrypt-3.1.3/ashcrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt/utils/exceptions/main.py` & `ashcrypt-3.1.3/ashcrypt/utils/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt/utils/gui/file.py` & `ashcrypt-3.1.3/ashcrypt/utils/gui/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt/utils/gui/text.py` & `ashcrypt-3.1.3/ashcrypt/utils/gui/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.1.3/ashcrypt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.2
+Version: 3.1.3
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.2/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.1.3/ashcrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.2/setup.py` & `ashcrypt-3.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.1.2',
+    version='3.1.3',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

