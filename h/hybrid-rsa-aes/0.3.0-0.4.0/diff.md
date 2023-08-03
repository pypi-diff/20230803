# Comparing `tmp/hybrid-rsa-aes-0.3.0.tar.gz` & `tmp/hybrid-rsa-aes-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybrid-rsa-aes-0.3.0.tar", last modified: Mon Jul 26 09:46:58 2021, max compression
+gzip compressed data, was "hybrid-rsa-aes-0.4.0.tar", last modified: Thu Aug  3 11:53:04 2023, max compression
```

## Comparing `hybrid-rsa-aes-0.3.0.tar` & `hybrid-rsa-aes-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:46:58.231303 hybrid-rsa-aes-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-07-26 09:46:47.000000 hybrid-rsa-aes-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-07-26 09:46:47.000000 hybrid-rsa-aes-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3109 2021-07-26 09:46:58.231303 hybrid-rsa-aes-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2021-07-26 09:46:47.000000 hybrid-rsa-aes-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:46:58.231303 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-07-26 09:46:47.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2591 2021-07-26 09:46:47.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes/cipher.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-07-26 09:46:47.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:46:58.231303 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3109 2021-07-26 09:46:58.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-07-26 09:46:58.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:46:58.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:46:58.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-07-26 09:46:58.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-07-26 09:46:58.000000 hybrid-rsa-aes-0.3.0/hybrid_rsa_aes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-07-26 09:46:47.000000 hybrid-rsa-aes-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-26 09:46:58.231303 hybrid-rsa-aes-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-07-26 09:46:47.000000 hybrid-rsa-aes-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:04.298425 hybrid-rsa-aes-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-03 11:52:55.000000 hybrid-rsa-aes-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 11:52:55.000000 hybrid-rsa-aes-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-03 11:53:04.298425 hybrid-rsa-aes-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-03 11:52:55.000000 hybrid-rsa-aes-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:04.298425 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 11:52:55.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-03 11:52:55.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 11:52:55.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:04.298425 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-03 11:53:04.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-03 11:53:04.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:53:04.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:53:04.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 11:53:04.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 11:53:04.000000 hybrid-rsa-aes-0.4.0/hybrid_rsa_aes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 11:52:55.000000 hybrid-rsa-aes-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:53:04.298425 hybrid-rsa-aes-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 11:52:55.000000 hybrid-rsa-aes-0.4.0/setup.py
```

### Comparing `hybrid-rsa-aes-0.3.0/LICENSE` & `hybrid-rsa-aes-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hybrid-rsa-aes-0.3.0/PKG-INFO` & `hybrid-rsa-aes-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 Metadata-Version: 2.1
 Name: hybrid-rsa-aes
-Version: 0.3.0
+Version: 0.4.0
 Summary: Helper for hybrid AES-RSA encryption
 Home-page: https://github.com/bigbag/hybrid-rsa-aes
+Download-URL: https://pypi.python.org/pypi/hybrid-rsa-aes
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/hybrid-rsa-aes
-Description: # hybrid-rsa-aes
-        
-        [![CI](https://github.com/bigbag/hybrid-rsa-aes/workflows/CI/badge.svg)](https://github.com/bigbag/hybrid-rsa-aes/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/hybrid-rsa-aes/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/hybrid-rsa-aes)
-        [![pypi](https://img.shields.io/pypi/v/hybrid-rsa-aes.svg)](https://pypi.python.org/pypi/hybrid-rsa-aes)
-        [![downloads](https://img.shields.io/pypi/dm/hybrid-rsa-aes.svg)](https://pypistats.org/packages/hybrid-rsa-aes)
-        [![versions](https://img.shields.io/pypi/pyversions/hybrid-rsa-aes.svg)](https://github.com/bigbag/hybrid-rsa-aes)
-        [![license](https://img.shields.io/github/license/bigbag/hybrid-rsa-aes.svg)](https://github.com/bigbag/hybrid-rsa-aes/blob/master/LICENSE)
-        
-        
-        **hybrid-rsa-aes** is a helper for hybrid AES-RSA encryption.
-        
-        
-        ## Installation
-        
-        hybrid-rsa-aes is available on PyPI.
-        Use pip to install:
-        
-            $ pip install hybrid-rsa-aes
-        
-        ## Basic Usage
-        
-        ```py
-        from cryptography.hazmat.backends import default_backend
-        from cryptography.hazmat.primitives.asymmetric import rsa
-        
-        from hybrid_rsa_aes import HybridCipher
-        
-        rsa_private_key = rsa.generate_private_key(
-            public_exponent=65537, key_size=2048, backend=default_backend()
-        )
-        rsa_public_key = rsa_private_key.public_key()
-        
-        encrypt_message = HybridCipher().encrypt(rsa_public_key=rsa_public_key, data={"test": "demo"})
-        
-        decrypt_message = HybridCipher().decrypt(
-            rsa_private_key=rsa_private_key, cipher_text=encrypt_message
-        )
-        assert "test" in decrypt_message and decrypt_message["test"] == "demo"
-        ```
-        
-        ## License
-        
-        hybrid-rsa-aes is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/hybrid-rsa-aes/security/policy).
 Platform: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# hybrid-rsa-aes
+
+[![CI](https://github.com/bigbag/hybrid-rsa-aes/workflows/CI/badge.svg)](https://github.com/bigbag/hybrid-rsa-aes/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/hybrid-rsa-aes/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/hybrid-rsa-aes)
+[![pypi](https://img.shields.io/pypi/v/hybrid-rsa-aes.svg)](https://pypi.python.org/pypi/hybrid-rsa-aes)
+[![downloads](https://img.shields.io/pypi/dm/hybrid-rsa-aes.svg)](https://pypistats.org/packages/hybrid-rsa-aes)
+[![versions](https://img.shields.io/pypi/pyversions/hybrid-rsa-aes.svg)](https://github.com/bigbag/hybrid-rsa-aes)
+[![license](https://img.shields.io/github/license/bigbag/hybrid-rsa-aes.svg)](https://github.com/bigbag/hybrid-rsa-aes/blob/master/LICENSE)
+
+
+**hybrid-rsa-aes** is a helper for hybrid AES-RSA encryption.
+
+
+## Installation
+
+hybrid-rsa-aes is available on PyPI.
+Use pip to install:
+
+    $ pip install hybrid-rsa-aes
+
+## Basic Usage
+
+```py
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives.asymmetric import rsa
+
+from hybrid_rsa_aes import HybridCipher
+
+rsa_private_key = rsa.generate_private_key(
+    public_exponent=65537, key_size=2048, backend=default_backend()
+)
+rsa_public_key = rsa_private_key.public_key()
+
+encrypt_message = HybridCipher().encrypt(rsa_public_key=rsa_public_key, data={"test": "demo"})
+
+decrypt_message = HybridCipher().decrypt(
+    rsa_private_key=rsa_private_key, cipher_text=encrypt_message
+)
+assert "test" in decrypt_message and decrypt_message["test"] == "demo"
+```
+
+## License
+
+hybrid-rsa-aes is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/hybrid-rsa-aes/security/policy).
```

### Comparing `hybrid-rsa-aes-0.3.0/README.md` & `hybrid-rsa-aes-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hybrid-rsa-aes-0.3.0/hybrid_rsa_aes/cipher.py` & `hybrid-rsa-aes-0.4.0/hybrid_rsa_aes/cipher.py`

 * *Files identical despite different names*

### Comparing `hybrid-rsa-aes-0.3.0/hybrid_rsa_aes.egg-info/PKG-INFO` & `hybrid-rsa-aes-0.4.0/hybrid_rsa_aes.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 Metadata-Version: 2.1
 Name: hybrid-rsa-aes
-Version: 0.3.0
+Version: 0.4.0
 Summary: Helper for hybrid AES-RSA encryption
 Home-page: https://github.com/bigbag/hybrid-rsa-aes
+Download-URL: https://pypi.python.org/pypi/hybrid-rsa-aes
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/hybrid-rsa-aes
-Description: # hybrid-rsa-aes
-        
-        [![CI](https://github.com/bigbag/hybrid-rsa-aes/workflows/CI/badge.svg)](https://github.com/bigbag/hybrid-rsa-aes/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/hybrid-rsa-aes/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/hybrid-rsa-aes)
-        [![pypi](https://img.shields.io/pypi/v/hybrid-rsa-aes.svg)](https://pypi.python.org/pypi/hybrid-rsa-aes)
-        [![downloads](https://img.shields.io/pypi/dm/hybrid-rsa-aes.svg)](https://pypistats.org/packages/hybrid-rsa-aes)
-        [![versions](https://img.shields.io/pypi/pyversions/hybrid-rsa-aes.svg)](https://github.com/bigbag/hybrid-rsa-aes)
-        [![license](https://img.shields.io/github/license/bigbag/hybrid-rsa-aes.svg)](https://github.com/bigbag/hybrid-rsa-aes/blob/master/LICENSE)
-        
-        
-        **hybrid-rsa-aes** is a helper for hybrid AES-RSA encryption.
-        
-        
-        ## Installation
-        
-        hybrid-rsa-aes is available on PyPI.
-        Use pip to install:
-        
-            $ pip install hybrid-rsa-aes
-        
-        ## Basic Usage
-        
-        ```py
-        from cryptography.hazmat.backends import default_backend
-        from cryptography.hazmat.primitives.asymmetric import rsa
-        
-        from hybrid_rsa_aes import HybridCipher
-        
-        rsa_private_key = rsa.generate_private_key(
-            public_exponent=65537, key_size=2048, backend=default_backend()
-        )
-        rsa_public_key = rsa_private_key.public_key()
-        
-        encrypt_message = HybridCipher().encrypt(rsa_public_key=rsa_public_key, data={"test": "demo"})
-        
-        decrypt_message = HybridCipher().decrypt(
-            rsa_private_key=rsa_private_key, cipher_text=encrypt_message
-        )
-        assert "test" in decrypt_message and decrypt_message["test"] == "demo"
-        ```
-        
-        ## License
-        
-        hybrid-rsa-aes is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/hybrid-rsa-aes/security/policy).
 Platform: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# hybrid-rsa-aes
+
+[![CI](https://github.com/bigbag/hybrid-rsa-aes/workflows/CI/badge.svg)](https://github.com/bigbag/hybrid-rsa-aes/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/hybrid-rsa-aes/branch/main/graph/badge.svg)](https://codecov.io/gh/bigbag/hybrid-rsa-aes)
+[![pypi](https://img.shields.io/pypi/v/hybrid-rsa-aes.svg)](https://pypi.python.org/pypi/hybrid-rsa-aes)
+[![downloads](https://img.shields.io/pypi/dm/hybrid-rsa-aes.svg)](https://pypistats.org/packages/hybrid-rsa-aes)
+[![versions](https://img.shields.io/pypi/pyversions/hybrid-rsa-aes.svg)](https://github.com/bigbag/hybrid-rsa-aes)
+[![license](https://img.shields.io/github/license/bigbag/hybrid-rsa-aes.svg)](https://github.com/bigbag/hybrid-rsa-aes/blob/master/LICENSE)
+
+
+**hybrid-rsa-aes** is a helper for hybrid AES-RSA encryption.
+
+
+## Installation
+
+hybrid-rsa-aes is available on PyPI.
+Use pip to install:
+
+    $ pip install hybrid-rsa-aes
+
+## Basic Usage
+
+```py
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives.asymmetric import rsa
+
+from hybrid_rsa_aes import HybridCipher
+
+rsa_private_key = rsa.generate_private_key(
+    public_exponent=65537, key_size=2048, backend=default_backend()
+)
+rsa_public_key = rsa_private_key.public_key()
+
+encrypt_message = HybridCipher().encrypt(rsa_public_key=rsa_public_key, data={"test": "demo"})
+
+decrypt_message = HybridCipher().decrypt(
+    rsa_private_key=rsa_private_key, cipher_text=encrypt_message
+)
+assert "test" in decrypt_message and decrypt_message["test"] == "demo"
+```
+
+## License
+
+hybrid-rsa-aes is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/hybrid-rsa-aes/security/policy).
```

### Comparing `hybrid-rsa-aes-0.3.0/setup.py` & `hybrid-rsa-aes-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: POSIX",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Environment :: Console",
     "Intended Audience :: Developers",
 ]
```

