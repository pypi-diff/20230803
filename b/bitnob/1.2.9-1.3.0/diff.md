# Comparing `tmp/bitnob-1.2.9.tar.gz` & `tmp/bitnob-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitnob-1.2.9.tar", last modified: Sun Jul 30 12:53:25 2023, max compression
+gzip compressed data, was "bitnob-1.3.0.tar", last modified: Thu Aug  3 15:59:25 2023, max compression
```

## Comparing `bitnob-1.2.9.tar` & `bitnob-1.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.178889 bitnob-1.2.9/
--rw-r--r--   0 gabby      (501) staff       (20)     4621 2023-07-30 12:53:25.178713 bitnob-1.2.9/PKG-INFO
--rw-r--r--   0 gabby      (501) staff       (20)     4153 2022-02-20 16:41:50.000000 bitnob-1.2.9/README.md
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.169201 bitnob-1.2.9/bitnob/
--rw-r--r--   0 gabby      (501) staff       (20)      459 2023-07-25 23:23:18.000000 bitnob-1.2.9/bitnob/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     2754 2023-07-20 09:58:05.000000 bitnob-1.2.9/bitnob/base.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.170892 bitnob-1.2.9/bitnob/customer/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:02:35.000000 bitnob-1.2.9/bitnob/customer/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)      277 2022-03-03 22:56:33.000000 bitnob-1.2.9/bitnob/customer/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     2929 2023-07-20 09:58:17.000000 bitnob-1.2.9/bitnob/customer/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.171613 bitnob-1.2.9/bitnob/exceptions/
--rw-r--r--   0 gabby      (501) staff       (20)      200 2022-02-20 16:49:05.000000 bitnob-1.2.9/bitnob/exceptions/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     1800 2022-02-20 16:49:05.000000 bitnob-1.2.9/bitnob/exceptions/exceptions.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.172357 bitnob-1.2.9/bitnob/hosted_checkout/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:04:50.000000 bitnob-1.2.9/bitnob/hosted_checkout/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     1830 2022-05-17 17:44:31.000000 bitnob-1.2.9/bitnob/hosted_checkout/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     3233 2023-07-20 09:58:17.000000 bitnob-1.2.9/bitnob/hosted_checkout/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.173185 bitnob-1.2.9/bitnob/lightning/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:22.000000 bitnob-1.2.9/bitnob/lightning/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     1722 2022-03-03 23:00:29.000000 bitnob-1.2.9/bitnob/lightning/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     4912 2023-07-20 10:07:41.000000 bitnob-1.2.9/bitnob/lightning/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.173913 bitnob-1.2.9/bitnob/ln_url/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-05-12 20:16:47.000000 bitnob-1.2.9/bitnob/ln_url/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)      505 2022-03-17 20:39:17.000000 bitnob-1.2.9/bitnob/ln_url/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     5560 2023-07-20 09:58:17.000000 bitnob-1.2.9/bitnob/ln_url/services.py
--rw-r--r--   0 gabby      (501) staff       (20)      250 2022-03-13 23:47:17.000000 bitnob-1.2.9/bitnob/model.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.174472 bitnob-1.2.9/bitnob/onchain/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:29.000000 bitnob-1.2.9/bitnob/onchain/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-03-03 22:48:54.000000 bitnob-1.2.9/bitnob/onchain/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     3090 2023-07-20 10:06:55.000000 bitnob-1.2.9/bitnob/onchain/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.175302 bitnob-1.2.9/bitnob/stablecoin/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:18:11.000000 bitnob-1.2.9/bitnob/stablecoin/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)      836 2022-08-11 16:48:09.000000 bitnob-1.2.9/bitnob/stablecoin/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     3778 2023-07-30 12:53:17.000000 bitnob-1.2.9/bitnob/stablecoin/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.176112 bitnob-1.2.9/bitnob/virtual_card/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:38.000000 bitnob-1.2.9/bitnob/virtual_card/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     2513 2022-08-09 09:26:36.000000 bitnob-1.2.9/bitnob/virtual_card/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     9437 2023-07-20 09:58:17.000000 bitnob-1.2.9/bitnob/virtual_card/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.176842 bitnob-1.2.9/bitnob/wallet/
--rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:46.000000 bitnob-1.2.9/bitnob/wallet/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)     1576 2023-07-20 10:01:51.000000 bitnob-1.2.9/bitnob/wallet/model.py
--rw-r--r--   0 gabby      (501) staff       (20)     4123 2023-07-20 10:02:33.000000 bitnob-1.2.9/bitnob/wallet/services.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.170148 bitnob-1.2.9/bitnob.egg-info/
--rw-r--r--   0 gabby      (501) staff       (20)     4621 2023-07-30 12:53:25.000000 bitnob-1.2.9/bitnob.egg-info/PKG-INFO
--rw-r--r--   0 gabby      (501) staff       (20)     1043 2023-07-30 12:53:25.000000 bitnob-1.2.9/bitnob.egg-info/SOURCES.txt
--rw-r--r--   0 gabby      (501) staff       (20)        1 2023-07-30 12:53:25.000000 bitnob-1.2.9/bitnob.egg-info/dependency_links.txt
--rw-r--r--   0 gabby      (501) staff       (20)        9 2023-07-30 12:53:25.000000 bitnob-1.2.9/bitnob.egg-info/requires.txt
--rw-r--r--   0 gabby      (501) staff       (20)       13 2023-07-30 12:53:25.000000 bitnob-1.2.9/bitnob.egg-info/top_level.txt
--rw-r--r--   0 gabby      (501) staff       (20)       38 2023-07-30 12:53:25.178942 bitnob-1.2.9/setup.cfg
--rw-r--r--   0 gabby      (501) staff       (20)      766 2023-07-30 12:53:17.000000 bitnob-1.2.9/setup.py
-drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-07-30 12:53:25.178302 bitnob-1.2.9/tests/
--rw-r--r--   0 gabby      (501) staff       (20)       28 2022-02-20 16:42:43.000000 bitnob-1.2.9/tests/__init__.py
--rw-r--r--   0 gabby      (501) staff       (20)      452 2022-02-20 17:33:40.000000 bitnob-1.2.9/tests/test_customer.py
--rw-r--r--   0 gabby      (501) staff       (20)      239 2022-02-20 21:20:16.000000 bitnob-1.2.9/tests/test_onchain.py
--rw-r--r--   0 gabby      (501) staff       (20)     1188 2022-05-25 13:00:21.000000 bitnob-1.2.9/tests/test_stablecoins.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.101733 bitnob-1.3.0/
+-rw-r--r--   0 gabby      (501) staff       (20)     4640 2023-08-03 15:59:25.101520 bitnob-1.3.0/PKG-INFO
+-rw-r--r--   0 gabby      (501) staff       (20)     4153 2022-02-20 16:41:50.000000 bitnob-1.3.0/README.md
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.092721 bitnob-1.3.0/bitnob/
+-rw-r--r--   0 gabby      (501) staff       (20)      459 2023-07-25 23:23:18.000000 bitnob-1.3.0/bitnob/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     2786 2023-08-03 15:56:02.000000 bitnob-1.3.0/bitnob/base.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.094384 bitnob-1.3.0/bitnob/customer/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:02:35.000000 bitnob-1.3.0/bitnob/customer/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)      277 2022-03-03 22:56:33.000000 bitnob-1.3.0/bitnob/customer/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     2929 2023-07-20 09:58:17.000000 bitnob-1.3.0/bitnob/customer/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.094898 bitnob-1.3.0/bitnob/exceptions/
+-rw-r--r--   0 gabby      (501) staff       (20)      200 2022-02-20 16:49:05.000000 bitnob-1.3.0/bitnob/exceptions/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1800 2022-02-20 16:49:05.000000 bitnob-1.3.0/bitnob/exceptions/exceptions.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.095693 bitnob-1.3.0/bitnob/hosted_checkout/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:04:50.000000 bitnob-1.3.0/bitnob/hosted_checkout/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1830 2022-05-17 17:44:31.000000 bitnob-1.3.0/bitnob/hosted_checkout/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     3233 2023-07-20 09:58:17.000000 bitnob-1.3.0/bitnob/hosted_checkout/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.096493 bitnob-1.3.0/bitnob/lightning/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:22.000000 bitnob-1.3.0/bitnob/lightning/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1722 2022-03-03 23:00:29.000000 bitnob-1.3.0/bitnob/lightning/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     4912 2023-07-20 10:07:41.000000 bitnob-1.3.0/bitnob/lightning/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.097180 bitnob-1.3.0/bitnob/ln_url/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-05-12 20:16:47.000000 bitnob-1.3.0/bitnob/ln_url/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)      505 2022-03-17 20:39:17.000000 bitnob-1.3.0/bitnob/ln_url/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     5560 2023-07-20 09:58:17.000000 bitnob-1.3.0/bitnob/ln_url/services.py
+-rw-r--r--   0 gabby      (501) staff       (20)      250 2022-03-13 23:47:17.000000 bitnob-1.3.0/bitnob/model.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.097748 bitnob-1.3.0/bitnob/onchain/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:29.000000 bitnob-1.3.0/bitnob/onchain/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-03-03 22:48:54.000000 bitnob-1.3.0/bitnob/onchain/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     3090 2023-07-20 10:06:55.000000 bitnob-1.3.0/bitnob/onchain/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.098379 bitnob-1.3.0/bitnob/stablecoin/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:18:11.000000 bitnob-1.3.0/bitnob/stablecoin/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)      836 2022-08-11 16:48:09.000000 bitnob-1.3.0/bitnob/stablecoin/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     3766 2023-08-03 15:57:49.000000 bitnob-1.3.0/bitnob/stablecoin/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.098991 bitnob-1.3.0/bitnob/virtual_card/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:38.000000 bitnob-1.3.0/bitnob/virtual_card/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     2513 2022-08-09 09:26:36.000000 bitnob-1.3.0/bitnob/virtual_card/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     9437 2023-07-20 09:58:17.000000 bitnob-1.3.0/bitnob/virtual_card/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.099866 bitnob-1.3.0/bitnob/wallet/
+-rw-r--r--   0 gabby      (501) staff       (20)        0 2022-02-20 21:03:46.000000 bitnob-1.3.0/bitnob/wallet/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1576 2023-07-20 10:01:51.000000 bitnob-1.3.0/bitnob/wallet/model.py
+-rw-r--r--   0 gabby      (501) staff       (20)     4123 2023-07-20 10:02:33.000000 bitnob-1.3.0/bitnob/wallet/services.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.093639 bitnob-1.3.0/bitnob.egg-info/
+-rw-r--r--   0 gabby      (501) staff       (20)     4640 2023-08-03 15:59:25.000000 bitnob-1.3.0/bitnob.egg-info/PKG-INFO
+-rw-r--r--   0 gabby      (501) staff       (20)     1043 2023-08-03 15:59:25.000000 bitnob-1.3.0/bitnob.egg-info/SOURCES.txt
+-rw-r--r--   0 gabby      (501) staff       (20)        1 2023-08-03 15:59:25.000000 bitnob-1.3.0/bitnob.egg-info/dependency_links.txt
+-rw-r--r--   0 gabby      (501) staff       (20)        9 2023-08-03 15:59:25.000000 bitnob-1.3.0/bitnob.egg-info/requires.txt
+-rw-r--r--   0 gabby      (501) staff       (20)       13 2023-08-03 15:59:25.000000 bitnob-1.3.0/bitnob.egg-info/top_level.txt
+-rw-r--r--   0 gabby      (501) staff       (20)       38 2023-08-03 15:59:25.101796 bitnob-1.3.0/setup.cfg
+-rw-r--r--   0 gabby      (501) staff       (20)      766 2023-08-03 15:59:21.000000 bitnob-1.3.0/setup.py
+drwxr-xr-x   0 gabby      (501) staff       (20)        0 2023-08-03 15:59:25.101016 bitnob-1.3.0/tests/
+-rw-r--r--   0 gabby      (501) staff       (20)       28 2022-02-20 16:42:43.000000 bitnob-1.3.0/tests/__init__.py
+-rw-r--r--   0 gabby      (501) staff       (20)      452 2022-02-20 17:33:40.000000 bitnob-1.3.0/tests/test_customer.py
+-rw-r--r--   0 gabby      (501) staff       (20)      239 2022-02-20 21:20:16.000000 bitnob-1.3.0/tests/test_onchain.py
+-rw-r--r--   0 gabby      (501) staff       (20)     1188 2022-05-25 13:00:21.000000 bitnob-1.3.0/tests/test_stablecoins.py
```

### Comparing `bitnob-1.2.9/PKG-INFO` & `bitnob-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: bitnob
-Version: 1.2.9
+Version: 1.3.0
 Summary: Python SDK for the Bitnob"s API
 Home-page: https://github.com/bitnob/bitnob_python_sdk
 Author: Bitnob
 Author-email: info@bitnob.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -151,7 +152,8 @@
 ## Contributing 
 
 Bug reports and pull requests are welcome on GitHub at [https://github.com/bitnob/bitnob_python_sdk](https://github.com/bitnob/bitnob_python_sdk). This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the code of conduct. Simply create a new branch and raise a Pull Request, we would review and merge. 
 
 ## License
 
 The package is available as open source under the terms of the [BSD License](https://opensource.org/licenses/BSD-3-Clause)
+
```

### Comparing `bitnob-1.2.9/README.md` & `bitnob-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/base.py` & `bitnob-1.3.0/bitnob/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import hmac
 import secrets
 import requests
 
 from hashlib import sha512
 from requests.exceptions import HTTPError, ConnectionError
@@ -19,17 +20,17 @@
         self.BITNOB_SANDBOX_URL = 'https://sandboxapi.bitnob.co/api/v1/'
         self.api_key = os.environ.get("BITNOB_API_KEY")
         self.production = os.environ.get("BITNOB_PRODUCTION")
         self.base_url = os.environ.get("BITNOB_BASE_URL")
         if self.api_key is None:
             raise BitnobBadKeyError()
         backupUrl = (
-           self.BITNOB_SANDBOX_URL if self.production is False else self.BITNOB_LIVE_URL
+           self.BITNOB_SANDBOX_URL if json.loads(self.production.lower()) is False else self.BITNOB_LIVE_URL
         )
-        getattr(self, "base_url", backupUrl)
+        setattr(self, "base_url", backupUrl)
 
     def send_request(self, method, path, **kwargs):
         """
         Create a request stub
         :param method:
         :param path:
         :param kwargs:
```

### Comparing `bitnob-1.2.9/bitnob/customer/services.py` & `bitnob-1.3.0/bitnob/customer/services.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/exceptions/exceptions.py` & `bitnob-1.3.0/bitnob/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/hosted_checkout/model.py` & `bitnob-1.3.0/bitnob/hosted_checkout/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/hosted_checkout/services.py` & `bitnob-1.3.0/bitnob/hosted_checkout/services.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/lightning/model.py` & `bitnob-1.3.0/bitnob/lightning/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/lightning/services.py` & `bitnob-1.3.0/bitnob/lightning/services.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/ln_url/services.py` & `bitnob-1.3.0/bitnob/ln_url/services.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/onchain/services.py` & `bitnob-1.3.0/bitnob/onchain/services.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/stablecoin/model.py` & `bitnob-1.3.0/bitnob/stablecoin/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/stablecoin/services.py` & `bitnob-1.3.0/bitnob/stablecoin/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     def send(self):
         pass
 
     @abstractmethod
     def generate_address(self):
         pass
 
-    def __generate_address_object(self, data):
+    def generate_address_object(self, data):
         return WalletAddress(
             address = data.get("address"),
             address_type=data.get("addressType"),
             label=data.get("label")
         )
     
-    def __generate_transaction_object(self, data):
+    def generate_transaction_object(self, data):
         
         return Transaction(            
             reference = data.get("reference"),
             description = data.get("description"),
             amount = data.get("amount"),
             btc_amount = data.get("btcAmount"),
             sat_amount = data.get("satAmount"),
@@ -63,15 +63,15 @@
 
         - POST Request
         """
         required_data = ["amount", "address", "chain"]
         self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "wallets/send-usdc", json=body)
-        return self.__generate_transaction_object(data=response["data"])
+        return self.generate_transaction_object(data=response["data"])
 
 
     def generate_address(self, body:dict):
         """
         Generate Address for Customer
 
         body = {
@@ -82,15 +82,15 @@
 
         - POST Request
         """
         required_data = ["customerEmail", "chain"]
         self.check_required_data(required_data, body)
 
         response =  self.send_request("POST", "addresses/generate/usdc", json=body)
-        return self.__generate_address_object(data=response["data"])
+        return self.generate_address_object(data=response["data"])
 
 class USDT(StableCoin, Bitnob): 
     
     def send(self, body:dict):
         """
         Sending USDC
 
@@ -103,15 +103,15 @@
 
         - POST Request
         """
         required_data = ["amount", "address", "chain"]
         self.check_required_data(required_data, body)
 
         response = self.send_request("POST", "wallets/send-usdt", json=body)
-        return self.__generate_transaction_object(data=response["data"])
+        return self.generate_transaction_object(data=response["data"])
 
     def generate_address(self, body:dict):
         """
         Generate Address for Customer
 
         body = {
             "label": "purchase xbox",
@@ -121,8 +121,8 @@
 
         - POST Request
         """
         required_data = ["customerEmail", "chain"]
         self.check_required_data(required_data, body)
 
         response =  self.send_request("POST", "addresses/generate/usdt", json=body)
-        return self.__generate_address_object(data=response["data"])
+        return self.generate_address_object(data=response["data"])
```

### Comparing `bitnob-1.2.9/bitnob/virtual_card/model.py` & `bitnob-1.3.0/bitnob/virtual_card/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/virtual_card/services.py` & `bitnob-1.3.0/bitnob/virtual_card/services.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/wallet/model.py` & `bitnob-1.3.0/bitnob/wallet/model.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob/wallet/services.py` & `bitnob-1.3.0/bitnob/wallet/services.py`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/bitnob.egg-info/PKG-INFO` & `bitnob-1.3.0/bitnob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: bitnob
-Version: 1.2.9
+Version: 1.3.0
 Summary: Python SDK for the Bitnob"s API
 Home-page: https://github.com/bitnob/bitnob_python_sdk
 Author: Bitnob
 Author-email: info@bitnob.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -151,7 +152,8 @@
 ## Contributing 
 
 Bug reports and pull requests are welcome on GitHub at [https://github.com/bitnob/bitnob_python_sdk](https://github.com/bitnob/bitnob_python_sdk). This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the code of conduct. Simply create a new branch and raise a Pull Request, we would review and merge. 
 
 ## License
 
 The package is available as open source under the terms of the [BSD License](https://opensource.org/licenses/BSD-3-Clause)
+
```

### Comparing `bitnob-1.2.9/bitnob.egg-info/SOURCES.txt` & `bitnob-1.3.0/bitnob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitnob-1.2.9/setup.py` & `bitnob-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="bitnob",
-    version="1.2.9",
+    version="1.3.0",
     description="Python SDK for the Bitnob\"s API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bitnob/bitnob_python_sdk",
     author="Bitnob",
     author_email="info@bitnob.com",
     license="MIT",
```

### Comparing `bitnob-1.2.9/tests/test_stablecoins.py` & `bitnob-1.3.0/tests/test_stablecoins.py`

 * *Files identical despite different names*

