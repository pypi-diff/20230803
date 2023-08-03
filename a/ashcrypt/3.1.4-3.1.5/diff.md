# Comparing `tmp/ashcrypt-3.1.4.tar.gz` & `tmp/ashcrypt-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.1.4.tar", last modified: Thu Aug  3 07:55:51 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.1.5.tar", last modified: Thu Aug  3 11:44:18 2023, max compression
```

## Comparing `ashcrypt-3.1.4.tar` & `ashcrypt-3.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39564 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/exceptions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/ashcrypt/utils/gui/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 07:55:50.000000 ashcrypt-3.1.4/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:55:51.000000 ashcrypt-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 07:55:38.000000 ashcrypt-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/exceptions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/ashcrypt/utils/safepack/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:44:18.000000 ashcrypt-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 11:44:01.000000 ashcrypt-3.1.5/setup.py
```

### Comparing `ashcrypt-3.1.4/PKG-INFO` & `ashcrypt-3.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.4
+Version: 3.1.5
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.4/README.md` & `ashcrypt-3.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
 
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
-python -m ashcrypt.gui
+python -m ashcrypt.safepack
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
-python -m ashcrypt.gui
+python -m ashcrypt.safepack
 ```
 
 
 ## License ##
 This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

### Comparing `ashcrypt-3.1.4/ashcrypt/clicrypt.py` & `ashcrypt-3.1.5/ashcrypt/clicrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ashcrypt import filecrypt as af
-from ashcrypt import textcrypt as at
+from ashcrypt.utils.safepack import file as af
+from ashcrypt.utils.safepack import text as at
 from typing import Optional
 import os.path
 import sys
 
 
 print('Welcome to the CLI')
```

### Comparing `ashcrypt-3.1.4/ashcrypt/crypt.py` & `ashcrypt-3.1.5/ashcrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.4/ashcrypt/database.py` & `ashcrypt-3.1.5/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.4/ashcrypt/filecrypt.py` & `ashcrypt-3.1.5/ashcrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.4/ashcrypt/gui.py` & `ashcrypt-3.1.5/ashcrypt/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import ashcrypt.utils.gui.text as At
-import ashcrypt.utils.gui.file as Af
-import ashcrypt.utils.gui.qr as qr
+import ashcrypt.utils.safepack.text as At
+import ashcrypt.utils.safepack.file as Af
+from ashcrypt.utils.safepack import qr
 import ashcrypt.database as Ad
 import ttkbootstrap as tk
 import platform
 import secrets
 import os.path
 import string
 import atexit
```

### Comparing `ashcrypt-3.1.4/ashcrypt/textcrypt.py` & `ashcrypt-3.1.5/ashcrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.4/ashcrypt/unittests/unittest_crypt.py` & `ashcrypt-3.1.5/ashcrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.4/ashcrypt/utils/exceptions/main.py` & `ashcrypt-3.1.5/ashcrypt/utils/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.4/ashcrypt/utils/gui/file.py` & `ashcrypt-3.1.5/ashcrypt/utils/safepack/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.4/ashcrypt/utils/gui/text.py` & `ashcrypt-3.1.5/ashcrypt/utils/safepack/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.4/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.1.5/ashcrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.4
+Version: 3.1.5
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.4/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.1.5/ashcrypt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 ashcrypt.egg-info/requires.txt
 ashcrypt.egg-info/top_level.txt
 ashcrypt/unittests/__init__.py
 ashcrypt/unittests/unittest_crypt.py
 ashcrypt/utils/__init__.py
 ashcrypt/utils/exceptions/__init__.py
 ashcrypt/utils/exceptions/main.py
-ashcrypt/utils/gui/__init__.py
-ashcrypt/utils/gui/file.py
-ashcrypt/utils/gui/qr.py
-ashcrypt/utils/gui/text.py
+ashcrypt/utils/safepack/__init__.py
+ashcrypt/utils/safepack/file.py
+ashcrypt/utils/safepack/qr.py
+ashcrypt/utils/safepack/text.py
```

### Comparing `ashcrypt-3.1.4/setup.py` & `ashcrypt-3.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.1.4',
+    version='3.1.5',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

