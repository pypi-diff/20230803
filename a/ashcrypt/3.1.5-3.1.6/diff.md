# Comparing `tmp/ashcrypt-3.1.5.tar.gz` & `tmp/ashcrypt-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.1.5.tar", last modified: Thu Aug  3 11:44:18 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.1.6.tar", last modified: Thu Aug  3 11:53:29 2023, max compression
```

## Comparing `ashcrypt-3.1.5.tar` & `ashcrypt-3.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/exceptions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/exceptions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/ashcrypt/utils/safepack/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:53:29.000000 ashcrypt-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 11:53:15.000000 ashcrypt-3.1.6/setup.py
```

### Comparing `ashcrypt-3.1.5/PKG-INFO` & `ashcrypt-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.5
+Version: 3.1.6
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.5/README.md` & `ashcrypt-3.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
 
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
-python -m ashcrypt.safepack
+python -m ashcrypt.gui
 ```
 
 **NOTE**:
 You  can use `clicrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
 
 
 To run the CLI 
@@ -335,15 +335,15 @@
 <br>`Key` for  both db's, this holds the `KeyRef` A.K.A key reference value
 #### Usage 
 The buttons are self-explanatory so do what you see fit. The result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
 <br>Just click buttons and check the result in the output console, it will guide you through the process.
 
 <br>To run the GUI anywhere
 ```shell
-python -m ashcrypt.safepack
+python -m ashcrypt.gui
 ```
 
 
 ## License ##
 This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

### Comparing `ashcrypt-3.1.5/ashcrypt/clicrypt.py` & `ashcrypt-3.1.6/ashcrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt/crypt.py` & `ashcrypt-3.1.6/ashcrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt/database.py` & `ashcrypt-3.1.6/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt/filecrypt.py` & `ashcrypt-3.1.6/ashcrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt/gui.py` & `ashcrypt-3.1.6/ashcrypt/gui.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt/textcrypt.py` & `ashcrypt-3.1.6/ashcrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt/unittests/unittest_crypt.py` & `ashcrypt-3.1.6/ashcrypt/unittests/unittest_crypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     def test_Iterations_Comp(self):
         self.assertEqual(self.ins1.iterations, self.ins2.rec_iterations)
 
     def test_Ciphertext_Comp(self):
         self.assertEqual(self.ins1.ciphertext(), self.ins2.rec_ciphertext)
 
     def test_HMAC_MismatchError(self):
-        tampered_hmac = self.ins1.encrypt(get_bytes=True)[:63] + b'1'
+        tampered_hmac = self.ins1.encrypt(get_bytes=True)[:31] + b'1'
         tampered_message = tampered_hmac + \
-            self.ins1.encrypt(get_bytes=True)[64:]
+            self.ins1.encrypt(get_bytes=True)[32:]
         with self.assertRaises(exceptions.MessageTamperingError):
             ac.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_IterationsOutOfRangeError2(self):
         enb = self.ins1.encrypt(get_bytes=True)
         tampered_message = enb[:80] + struct.pack('!I', 100001) + enb[84:]
         with self.assertRaises(exceptions.IterationsOutofRangeError):
```

### Comparing `ashcrypt-3.1.5/ashcrypt/utils/exceptions/main.py` & `ashcrypt-3.1.6/ashcrypt/utils/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt/utils/safepack/file.py` & `ashcrypt-3.1.6/ashcrypt/utils/safepack/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt/utils/safepack/text.py` & `ashcrypt-3.1.6/ashcrypt/utils/safepack/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.1.6/ashcrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.5
+Version: 3.1.6
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.5/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.1.6/ashcrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.5/setup.py` & `ashcrypt-3.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.1.5',
+    version='3.1.6',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

