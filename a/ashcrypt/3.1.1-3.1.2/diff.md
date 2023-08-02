# Comparing `tmp/ashcrypt-3.1.1.tar.gz` & `tmp/ashcrypt-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.1.1.tar", last modified: Wed Aug  2 21:00:50 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.1.2.tar", last modified: Wed Aug  2 22:05:28 2023, max compression
```

## Comparing `ashcrypt-3.1.1.tar` & `ashcrypt-3.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39554 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/exceptions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/utils/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/gui/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/gui/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39561 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/exceptions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/ashcrypt/utils/gui/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 22:05:27.000000 ashcrypt-3.1.2/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:05:28.000000 ashcrypt-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 22:05:17.000000 ashcrypt-3.1.2/setup.py
```

### Comparing `ashcrypt-3.1.1/PKG-INFO` & `ashcrypt-3.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.1
+Version: 3.1.2
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.1/README.md` & `ashcrypt-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.1/ashcrypt/clicrypt.py` & `ashcrypt-3.1.2/ashcrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.1/ashcrypt/crypt.py` & `ashcrypt-3.1.2/ashcrypt/crypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             rounds=iterations)
 
     @staticmethod
     def genkey(raw_bytes: Optional[bool] = False,
                desired_bytes: Optional[int] = 32) -> Union[str, bytes]:
         """Generates a random 256-bit ( by default )
         key as either raw bytes or a hex string. Set raw_bytes to True to get
-        the key in bytes. Set the number of desired_bytes to a strictly positive integer
+        the key in bytes. Set the number of desired_bytes to a greater or equal to 32
         to override the default value"""
         if desired_bytes < 32:
             raise ValueError("desired_bytes must be greater or equal to 32")
         key = os.urandom(desired_bytes)
         return key if raw_bytes else key.hex()
 
     def _mode(self):
@@ -83,25 +83,25 @@
 
     def iterations_bytes(self) -> bytes:
         """Packs the number of iterations into bytes using the 'big-endian' format"""
         iters_bytes = struct.pack('!I', self.iterations)
         return iters_bytes
 
     def hmac_final(self) -> bytes:
-        """Computes the HMAC-SHA256 of the ciphertext"""
+        """Computes the HMAC-SHA256 of the ciphertext bundle"""
         hmac_ = self.hmac_key
         hmac_ = hmac.HMAC(hmac_, hashes.SHA256())
         hmac_.update(self._iv + self.salt + self.pepper +
                      self.iterations_bytes() + self.ciphertext())
         return hmac_.finalize()
 
     def encrypt(self, get_bytes: Optional[bool] = False) -> Union[str, bytes]:
         """Returns the encrypted data as bytes in the form 'HMAC' -> 'IV'
         -> 'Salt value' -> 'pepper value' -> 'iterations' -> 'ciphertext.
-        Or a URL safe base 64 encoded string of the encrypted bytes data,
+        Or as a URL safe base 64 encoded string of the encrypted bytes data,
         which is the default return value"""
         raw = self.hmac_final() + self._iv + self.salt + self.pepper + \
             self.iterations_bytes() + self.ciphertext()
         return raw if get_bytes else base64.urlsafe_b64encode(
             raw).decode('UTF-8')
 
 
@@ -129,15 +129,15 @@
             self.key,
             self.rec_pepper,
             self.rec_iterations)
         if self.verify_hmac() is False:
             raise exceptions.MessageTamperingError()
 
     def calculated_hmac(self) -> bytes:
-        """Computes the HMAC-SHA256 of the received ciphertext"""
+        """Computes the HMAC-SHA256 of the received ciphertext bundle"""
         hmac_ = self.hmac_k
         hmac_ = hmac.HMAC(hmac_, hashes.SHA256())
         hmac_.update(self.rec_iv + self.rec_salt + self.rec_pepper +
                      self.rec_iters_raw + self.rec_ciphertext)
         return hmac_.finalize()
 
     def verify_hmac(self) -> bool:
@@ -153,24 +153,24 @@
         return Cipher(
             algorithms.AES(
                 key=self.dec_key),
             mode=self._mode(),
             backend=default_backend())
 
     def _cipher_decryptor(self):
-        """Returns the decryptor for the AES cipher"""
+        """Returns the decryptor object for the AES cipher"""
         return self._cipher().decryptor()
 
     def _pre_unpadding_dec(self) -> bytes:
         """Decrypts the received ciphertext and returns the pre-unpadded data"""
         return self._cipher_decryptor().update(self.rec_ciphertext) + \
             self._cipher_decryptor().finalize()
 
     def unpadded_message(self) -> bytes:
-        """Unpads the pre-unpadded data and returns the original message """
+        """Unpads the data and returns the original message """
         unpadder = padding.PKCS7(128).unpadder()
         return unpadder.update(self._pre_unpadding_dec()) + unpadder.finalize()
 
     def decrypt(self, get_bytes: Optional[bool] = False) -> Union[str, bytes]:
         """Returns the decrypted message as a UTF-8 encoded string or a bytes object"""
         raw = self.unpadded_message()
         return raw if get_bytes else raw.decode('UTF-8')
```

### Comparing `ashcrypt-3.1.1/ashcrypt/database.py` & `ashcrypt-3.1.2/ashcrypt/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,42 +127,43 @@
             except sqlite3.Error as e:
                 return 0, e
 
     def update(
             self,
             column_name: str,
             new_column_val: str,
-            id: int,
+            id_: int,
             tablename: Optional[str] = None) -> Union[int, tuple]:
         """Updates a specific column of a row based on the given ID in the specified table or the default table."""
         if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? ',
                         (new_column_val,
-                         id))
+                         id_))
                     return 11
 
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
                         f'UPDATE {tablename} SET {column_name} = ? WHERE ID = ? ',
                         (new_column_val,
-                         id))
+                         id_))
                     return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def content(self, tablename: Optional[str] = None) -> Union[Generator, tuple]:
+    def content(self, tablename: Optional[str]
+                = None) -> Union[Generator, tuple]:
         """Yields all rows from the specified table or the default table
         if no arguments are passed ( as a Generator object ) ."""
         if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(f'SELECT * FROM {self.tablename} ')
                     for row in self.c.fetchall():
@@ -178,33 +179,33 @@
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return 0, e
 
     def content_by_id(
-            self, id: int, tablename: Optional[str] = None) -> Union[Generator, tuple]:
+            self, id_: int, tablename: Optional[str] = None) -> Union[Generator, tuple]:
         """Yields a specific row from the specified table or the default table based on a given ID.
         ( Generator object )"""
         if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (id,))
+                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (id_,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'SELECT * FROM {tablename} WHERE ID = ? ', (id,))
+                        f'SELECT * FROM {tablename} WHERE ID = ? ', (id_,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return 0, e
 
     def show_contents(self, *tablenames: str) -> Union[Generator, tuple]:
@@ -272,28 +273,29 @@
                 with self.conn:
                     self.c.execute(f'DROP TABLE {self.tablename}')
                     return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def drop_content(self, id: int, tablename: Optional[str] = None) -> Union[int, tuple]:
+    def drop_content(
+            self, id_: int, tablename: Optional[str] = None) -> Union[int, tuple]:
         """Deletes a row from the specified table or the default table based on the given ID."""
         if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'DELETE FROM {self.tablename} WHERE ID = {id}')
+                        f'DELETE FROM {self.tablename} WHERE ID = {id_}')
                 return 11
 
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'DELETE FROM {tablename} WHERE ID = {id}')
+                        f'DELETE FROM {tablename} WHERE ID = {id_}')
                 return 1
 
             except sqlite3.Error as e:
                 return 0, e
```

### Comparing `ashcrypt-3.1.1/ashcrypt/filecrypt.py` & `ashcrypt-3.1.2/ashcrypt/filecrypt.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 from ashcrypt import crypt
 from ashcrypt.utils import exceptions
 import os
 
 
 class CryptFile:
-    '''Class to encrypt/decrypt a given file. Pass in the filename
-                as well as a 256-bit key '''
-    def __init__(self, filename : str, key : str):
+    """Class to encrypt/decrypt a given file. Pass in the filename
+                as well as a 256-bit key """
+
+    def __init__(self, filename: str, key: str):
         self.filename = filename
         self.not_256_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
             raise exceptions.KeyLengthError()
 
@@ -62,15 +63,15 @@
                         os.rename(self.filename, self.filename + '.crypt')
                         return 1
         except Exception:
             raise exceptions.SysError()
 
     def decrypt(self) -> int:
         if os.path.isdir(self.filename):
-           raise exceptions.GivenDirectoryError()
+            raise exceptions.GivenDirectoryError()
         if self.not_256_bit_key == 1:
             raise exceptions.KeyLengthError()
         try:
             if not os.path.exists(self.filename):
                 raise exceptions.FileDoesNotExistError()
             else:
                 if os.path.splitext(self.filename)[1] != '.crypt':
@@ -100,8 +101,8 @@
         except Exception:
             raise exceptions.SysError()
 
     def __str__(self):
         return f'Encrypting/Decrypting File {self.filename} With {self.key} Key '
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({self.filename},{self.key})'
+        return f'{self.__class__.__name__}({self.filename},{self.key})'
```

### Comparing `ashcrypt-3.1.1/ashcrypt/gui.py` & `ashcrypt-3.1.2/ashcrypt/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ashcrypt.utils.gui.text as At
 import ashcrypt.utils.gui.file as Af
+import ashcrypt.utils.gui as qr
 import ashcrypt.database as Ad
 import ttkbootstrap as tk
-import ashcrypt.qr as qr
 import platform
 import secrets
 import os.path
 import string
 import atexit
 import json
 import re
```

### Comparing `ashcrypt-3.1.1/ashcrypt/textcrypt.py` & `ashcrypt-3.1.2/ashcrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.1/ashcrypt/unittests/unittest_crypt.py` & `ashcrypt-3.1.2/ashcrypt/unittests/unittest_crypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import struct
 
 
 class CryptModuleTesting(unittest.TestCase):
     def setUp(self) -> None:
         self.message1 = 'Hello there testing if it works'
         self.message2 = b'this is bytes now'
-        self.mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
+        self.mainkey = ac.Enc.genkey()
         self.ins1 = ac.Enc(message=self.message1, mainkey=self.mainkey)
         self.string_message = self.ins1.encrypt()
         self.bytes_message = self.ins1.encrypt(get_bytes=True)
         self.ins2 = ac.Dec(message=self.bytes_message, mainkey=self.mainkey)
 
     def tearDown(self) -> None:
         pass
```

### Comparing `ashcrypt-3.1.1/ashcrypt/utils/exceptions/main.py` & `ashcrypt-3.1.2/ashcrypt/utils/exceptions/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,64 +1,70 @@
-
-
 class IterationsOutofRangeError(Exception):
     """Exception raised when iterations come to be out of range usually due to message tampering
     where the bytes representing the KDF iterations get touched"""
 
     def __init__(self, num: any) -> None:
         self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num}'
         super().__init__(self.display)
 
+
 class MessageTamperingError(Exception):
     """Raised when any part of the message gets tampered with. DISCARD THE MESSAGE"""
 
     def __init__(self) -> None:
         self.display = 'HMAC mismatch ! Message has been TAMPERED with ,\n' \
                        ' or Possible key difference'
         super().__init__(self.display)
 
+
 class KeyLengthError(Exception):
     def __init__(self):
         self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
 
 
 class EmptyContentError(Exception):
     def __init__(self):
         self.display = 'Empty content !'
         super().__init__(self.display)
 
+
 class GivenDirectoryError(Exception):
     def __init__(self):
         self.display = 'Given directory instead of file'
         super().__init__(self.display)
 
+
 class FileDoesNotExistError(Exception):
     def __init__(self):
         self.display = 'Given path does not contain the specified file !'
         super().__init__(self.display)
 
 
 class SysError(Exception):
     def __init__(self):
         self.display = 'System related Error. Check if the file is busy !'
         super().__init__(self.display)
 
+
 class FileCryptError(Exception):
     def __init__(self):
         self.display = 'Error in enc/dec probable file distortion, message tampering or wrong key !'
         super().__init__(self.display)
 
+
 class CryptError(Exception):
     def __init__(self):
         self.display = 'Message tampering or wrong key !'
         super().__init__(self.display)
 
+
 class AlreadyEncryptedError(Exception):
     def __init__(self):
         self.display = 'File is already encrypted !'
         super().__init__(self.display)
 
+
 class AlreadyDecryptedError(Exception):
     def __init__(self):
         self.display = 'File is already decrypted !'
         super().__init__(self.display)
```

### Comparing `ashcrypt-3.1.1/ashcrypt/utils/gui/file.py` & `ashcrypt-3.1.2/ashcrypt/utils/gui/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.1/ashcrypt/utils/gui/text.py` & `ashcrypt-3.1.2/ashcrypt/utils/gui/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.1/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.1.2/ashcrypt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.1
+Version: 3.1.2
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.1/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.1.2/ashcrypt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 ashcrypt/README.md
 ashcrypt/__init__.py
 ashcrypt/clicrypt.py
 ashcrypt/crypt.py
 ashcrypt/database.py
 ashcrypt/filecrypt.py
 ashcrypt/gui.py
-ashcrypt/qr.py
 ashcrypt/textcrypt.py
 ashcrypt.egg-info/PKG-INFO
 ashcrypt.egg-info/SOURCES.txt
 ashcrypt.egg-info/dependency_links.txt
 ashcrypt.egg-info/requires.txt
 ashcrypt.egg-info/top_level.txt
 ashcrypt/unittests/__init__.py
 ashcrypt/unittests/unittest_crypt.py
 ashcrypt/utils/__init__.py
 ashcrypt/utils/exceptions/__init__.py
 ashcrypt/utils/exceptions/main.py
 ashcrypt/utils/gui/__init__.py
 ashcrypt/utils/gui/file.py
+ashcrypt/utils/gui/qr.py
 ashcrypt/utils/gui/text.py
```

### Comparing `ashcrypt-3.1.1/setup.py` & `ashcrypt-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.1.1',
+    version='3.1.2',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

