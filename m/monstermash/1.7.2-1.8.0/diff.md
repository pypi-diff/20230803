# Comparing `tmp/monstermash-1.7.2.tar.gz` & `tmp/monstermash-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstermash-1.7.2.tar", max compression
+gzip compressed data, was "monstermash-1.8.0.tar", max compression
```

## Comparing `monstermash-1.7.2.tar` & `monstermash-1.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2170 2023-07-01 03:51:37.894007 monstermash-1.7.2/README.md
--rw-r--r--   0        0        0     1152 2023-07-01 03:51:37.894007 monstermash-1.7.2/pyproject.toml
--rw-r--r--   0        0        0       86 2023-07-01 03:51:37.894007 monstermash-1.7.2/src/monstermash/__init__.py
--rw-r--r--   0        0        0     4205 2023-07-01 03:51:37.894007 monstermash-1.7.2/src/monstermash/__main__.py
--rw-r--r--   0        0        0     1024 2023-07-01 03:51:37.894007 monstermash-1.7.2/src/monstermash/config.py
--rw-r--r--   0        0        0     3680 2023-07-01 03:51:37.894007 monstermash-1.7.2/src/monstermash/crypt.py
--rw-r--r--   0        0        0      399 2023-07-01 03:51:37.898007 monstermash-1.7.2/src/monstermash/datamodels.py
--rw-r--r--   0        0        0     1272 2023-07-01 03:51:37.898007 monstermash-1.7.2/src/monstermash/parser.py
--rw-r--r--   0        0        0        0 2023-07-01 03:51:37.898007 monstermash-1.7.2/src/monstermash/utils/__init__.py
--rw-r--r--   0        0        0      709 2023-07-01 03:51:37.898007 monstermash-1.7.2/src/monstermash/utils/file.py
--rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 monstermash-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     2170 2023-07-01 12:04:30.967983 monstermash-1.8.0/README.md
+-rw-r--r--   0        0        0     1154 2023-07-01 12:04:30.967983 monstermash-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-07-01 12:04:30.967983 monstermash-1.8.0/src/monstermash/__init__.py
+-rw-r--r--   0        0        0     4205 2023-07-01 12:04:30.967983 monstermash-1.8.0/src/monstermash/__main__.py
+-rw-r--r--   0        0        0     1052 2023-07-01 12:04:30.967983 monstermash-1.8.0/src/monstermash/config.py
+-rw-r--r--   0        0        0     3753 2023-07-01 12:04:30.967983 monstermash-1.8.0/src/monstermash/crypt.py
+-rw-r--r--   0        0        0      399 2023-07-01 12:04:30.967983 monstermash-1.8.0/src/monstermash/datamodels.py
+-rw-r--r--   0        0        0     1272 2023-07-01 12:04:30.967983 monstermash-1.8.0/src/monstermash/parser.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:04:30.967983 monstermash-1.8.0/src/monstermash/utils/__init__.py
+-rw-r--r--   0        0        0      751 2023-07-01 12:04:30.967983 monstermash-1.8.0/src/monstermash/utils/file.py
+-rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 monstermash-1.8.0/PKG-INFO
```

### Comparing `monstermash-1.7.2/README.md` & `monstermash-1.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.7.2
+> 1️⃣ version: 1.8.0
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

### Comparing `monstermash-1.7.2/pyproject.toml` & `monstermash-1.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "monstermash"
-version = "1.7.2"
+version = "1.8.0"
 description = ""
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "monstermash", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 pynacl = "^1.5.0"
 click = "^8.1.3"
-pydantic = "^1.10.7"
-questionary = "^1.10.0"
+pydantic = "^2.0"
+pydantic-settings = "^2.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 bumpversion = "^0.6.0"
 twine = "^4.0.2"
 flake8 = "^6.0.0"
 dlint = "^0.14.0"
```

### Comparing `monstermash-1.7.2/src/monstermash/__main__.py` & `monstermash-1.8.0/src/monstermash/__main__.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.7.2/src/monstermash/config.py` & `monstermash-1.8.0/src/monstermash/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 
-from pydantic import BaseSettings, validator
+from pydantic import field_validator
+from pydantic_settings import BaseSettings
 
 
 class Config(BaseSettings):
     """
     Config class provides a model for application configuration settings,
     which includes the path to the configuration file.
 
     Attributes:
         config_file (str): The path to the configuration file. Default is '~/.monstermashcfg'.
     """
 
     config_file: str = '~/.monstermashcfg'
 
-    @validator('config_file', always=True)
+    @field_validator('config_file')
     def validate_file(cls, v: str) -> str:
         """
         Validate and normalize the path of the configuration file.
 
         This validator check that if the config_file path starts with '~', it is expanded to the full path in the
         user's home directory. If not we store it where you have asked.
```

### Comparing `monstermash-1.7.2/src/monstermash/crypt.py` & `monstermash-1.8.0/src/monstermash/crypt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from nacl.encoding import HexEncoder
 from nacl.public import Box, PrivateKey, PublicKey
+from pydantic import SecretStr
 
 from monstermash.datamodels import KeyPair
 
 
 class Crypt:
     """
     Crypt class provides methods for encryption and decryption of messages using NaCl (Salt) cryptographic library.
@@ -64,15 +65,17 @@
 
         Returns:
             KeyPair: A tuple containing the encoded private key and public key.
         """
         private_key = PrivateKey.generate()
         private_key_encoded = private_key.encode(encoder)
         public_key_encoded = private_key.public_key.encode(encoder)
-        return KeyPair(private_key=private_key_encoded, public_key=public_key_encoded)
+        return KeyPair(
+            private_key=SecretStr(private_key_encoded.decode()), public_key=public_key_encoded
+        )
 
     def encrypt(self, message: bytes, public_key: bytes) -> bytes:
         """
         Encrypt a message using a given public key. We append the public key to the ciphertext so that decryption
         becomes easy. The size of the key has to be consistent between encryption and decryption so that we can split
         the ciphertext based off the key size.
```

### Comparing `monstermash-1.7.2/src/monstermash/parser.py` & `monstermash-1.8.0/src/monstermash/parser.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.7.2/src/monstermash/utils/file.py` & `monstermash-1.8.0/src/monstermash/utils/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import re
-from typing import Any
+from typing import Union
+
+from pydantic import Json
 
 NEW_LINE_EXPR = re.compile(r'[\n\r]')
 
 
-def open_file(file) -> Any:
+def open_file(file) -> Union[Json, str]:
     """
     Open a file and return its contents. For JSON files, the contents are returned as a dictionary.
     For non-JSON files, the contents are returned as a string.
 
     Args:
         file (str): The path to the file to open.
```

### Comparing `monstermash-1.7.2/PKG-INFO` & `monstermash-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: monstermash
-Version: 1.7.2
+Version: 1.8.0
 Summary: 
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic-settings (>=2.0.0,<3.0.0)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
-Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.7.2
+> 1️⃣ version: 1.8.0
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

