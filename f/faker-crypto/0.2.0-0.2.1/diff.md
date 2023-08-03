# Comparing `tmp/faker_crypto-0.2.0.tar.gz` & `tmp/faker_crypto-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_crypto-0.2.0.tar", max compression
+gzip compressed data, was "faker_crypto-0.2.1.tar", max compression
```

## Comparing `faker_crypto-0.2.0.tar` & `faker_crypto-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      902 2023-01-26 18:40:14.528462 faker_crypto-0.2.0/README.md
--rw-r--r--   0        0        0     2208 2023-01-26 18:40:14.528462 faker_crypto-0.2.0/faker_crypto/__init__.py
--rw-r--r--   0        0        0     1139 2023-01-26 18:40:14.528462 faker_crypto-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 faker_crypto-0.2.0/setup.py
--rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 faker_crypto-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      902 2023-08-03 10:57:36.832476 faker_crypto-0.2.1/README.md
+-rw-r--r--   0        0        0     2208 2023-08-03 10:57:36.832476 faker_crypto-0.2.1/faker_crypto/__init__.py
+-rw-r--r--   0        0        0     1139 2023-08-03 10:57:36.832476 faker_crypto-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 faker_crypto-0.2.1/PKG-INFO
```

### Comparing `faker_crypto-0.2.0/README.md` & `faker_crypto-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# faker_crypto
+# faker-crypto
 
-__Version:__ 0.2.0
+__Version:__ 0.2.1
 
-faker_crypto is a Faker provider for Cryto Addreses.
+faker-crypto is a Faker provider for Cryto Addreses.
 
 Following crypto addresses are supported:
 
 - Bitcoin
 - Bitcoin Cash
 - Litecoin
 - Dogecoin
```

### Comparing `faker_crypto-0.2.0/faker_crypto/__init__.py` & `faker_crypto-0.2.1/faker_crypto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 from string import hexdigits
 
 from faker.providers import BaseProvider
```

### Comparing `faker_crypto-0.2.0/pyproject.toml` & `faker_crypto-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "faker-crypto"
-version = "0.2.0"
+version = "0.2.1"
 description = "faker-crypto is a Faker provider for cryto addreses."
 authors = ["Karambir Singh Nain <hello@karambir.in>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/karambir/faker-crypto"
 homepage = "https://github.com/karambir/faker-crypto/"
 keywords = [
```

### Comparing `faker_crypto-0.2.0/PKG-INFO` & `faker_crypto-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-crypto
-Version: 0.2.0
+Version: 0.2.1
 Summary: faker-crypto is a Faker provider for cryto addreses.
 Home-page: https://github.com/karambir/faker-crypto/
 License: MIT
 Keywords: faker,test,mock,generator,cryptocurrency
 Author: Karambir Singh Nain
 Author-email: hello@karambir.in
 Requires-Python: >=3.8.1,<4.0.0
@@ -17,19 +17,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: Faker (>=14.2)
 Project-URL: Repository, https://github.com/karambir/faker-crypto
 Description-Content-Type: text/markdown
 
-# faker_crypto
+# faker-crypto
 
-__Version:__ 0.2.0
+__Version:__ 0.2.1
 
-faker_crypto is a Faker provider for Cryto Addreses.
+faker-crypto is a Faker provider for Cryto Addreses.
 
 Following crypto addresses are supported:
 
 - Bitcoin
 - Bitcoin Cash
 - Litecoin
 - Dogecoin
```

