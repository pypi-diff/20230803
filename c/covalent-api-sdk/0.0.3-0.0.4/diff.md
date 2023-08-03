# Comparing `tmp/covalent-api-sdk-0.0.3.tar.gz` & `tmp/covalent-api-sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-api-sdk-0.0.3.tar", last modified: Thu Aug  3 06:24:48 2023, max compression
+gzip compressed data, was "covalent-api-sdk-0.0.4.tar", last modified: Thu Aug  3 06:37:15 2023, max compression
```

## Comparing `covalent-api-sdk-0.0.3.tar` & `covalent-api-sdk-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,38 @@
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:24:48.507400 covalent-api-sdk-0.0.3/
--rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 06:24:48.507202 covalent-api-sdk-0.0.3/PKG-INFO
--rw-r--r--   0 davidwork   (501) staff       (20)    12482 2023-08-03 01:55:34.000000 covalent-api-sdk-0.0.3/README.md
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:24:48.504291 covalent-api-sdk-0.0.3/covalent/
--rw-r--r--   0 davidwork   (501) staff       (20)       48 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/covalent/__init__.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1059 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/covalent/client.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:24:48.504939 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/
--rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 davidwork   (501) staff       (20)      530 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 davidwork   (501) staff       (20)        1 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 davidwork   (501) staff       (20)       50 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/requires.txt
--rw-r--r--   0 davidwork   (501) staff       (20)        9 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 davidwork   (501) staff       (20)       38 2023-08-03 06:24:48.507442 covalent-api-sdk-0.0.3/setup.cfg
--rw-r--r--   0 davidwork   (501) staff       (20)     1527 2023-08-03 06:23:24.000000 covalent-api-sdk-0.0.3/setup.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:24:48.506887 covalent-api-sdk-0.0.3/tests/
--rw-r--r--   0 davidwork   (501) staff       (20)     1541 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_api_helper.py
--rw-r--r--   0 davidwork   (501) staff       (20)      668 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_back_off.py
--rw-r--r--   0 davidwork   (501) staff       (20)     5313 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_balance_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     6450 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_base_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)      464 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_client.py
--rw-r--r--   0 davidwork   (501) staff       (20)    10712 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_nft_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1238 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_pricing_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)      867 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_security_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     3941 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_transaction_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     6585 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_xyk_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.499820 covalent-api-sdk-0.0.4/
+-rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 06:37:15.499596 covalent-api-sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 davidwork   (501) staff       (20)    12482 2023-08-03 01:55:34.000000 covalent-api-sdk-0.0.4/README.md
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.492146 covalent-api-sdk-0.0.4/covalent/
+-rw-r--r--   0 davidwork   (501) staff       (20)       48 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/covalent/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1059 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/covalent/client.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.494089 covalent-api-sdk-0.0.4/covalent/services/
+-rw-r--r--   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:08.000000 covalent-api-sdk-0.0.4/covalent/services/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    51117 2023-08-03 06:31:40.000000 covalent-api-sdk-0.0.4/covalent/services/balance_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    42736 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/base_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    65956 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/nft_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     8668 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/pricing_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    10643 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/security_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    28811 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/transaction_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.494840 covalent-api-sdk-0.0.4/covalent/services/util/
+-rw-r--r--   0 davidwork   (501) staff       (20)      205 2023-08-03 06:31:48.000000 covalent-api-sdk-0.0.4/covalent/services/util/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     2533 2023-08-03 06:37:07.000000 covalent-api-sdk-0.0.4/covalent/services/util/api_helper.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      990 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/covalent/services/util/back_off.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    73591 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/xyk_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.495670 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/
+-rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 davidwork   (501) staff       (20)      920 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)        1 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)       50 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)        9 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)       38 2023-08-03 06:37:15.499872 covalent-api-sdk-0.0.4/setup.cfg
+-rw-r--r--   0 davidwork   (501) staff       (20)     1527 2023-08-03 06:37:00.000000 covalent-api-sdk-0.0.4/setup.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.497730 covalent-api-sdk-0.0.4/tests/
+-rw-r--r--   0 davidwork   (501) staff       (20)     1541 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_api_helper.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      668 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_back_off.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     5313 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_balance_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     6450 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_base_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      464 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_client.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    10712 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_nft_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1238 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_pricing_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      867 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_security_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     3941 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_transaction_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     6585 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_xyk_service.py
```

### Comparing `covalent-api-sdk-0.0.3/PKG-INFO` & `covalent-api-sdk-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-api-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: covalent-api-sdk-py
 Home-page: https://github.com/covalenthq/covalent-api-sdk-py/
 Author: Covalenthq
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covalent-api-sdk-0.0.3/README.md` & `covalent-api-sdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/covalent/client.py` & `covalent-api-sdk-0.0.4/covalent/client.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/PKG-INFO` & `covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-api-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: covalent-api-sdk-py
 Home-page: https://github.com/covalenthq/covalent-api-sdk-py/
 Author: Covalenthq
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covalent-api-sdk-0.0.3/setup.py` & `covalent-api-sdk-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='covalent-api-sdk',   # Replace with the name of your package
-    version='0.0.3',             # Replace with the version of your package
+    version='0.0.4',             # Replace with the version of your package
     license="MIT",
     # Description and long_description should contain a concise and detailed description of your project.
     description='covalent-api-sdk-py',
     long_description=open('README.md').read() + "\n",
     long_description_content_type='text/markdown',
     author='Covalenthq',          # Replace with your name
     python_requires='>=3.7',
```

### Comparing `covalent-api-sdk-0.0.3/tests/test_api_helper.py` & `covalent-api-sdk-0.0.4/tests/test_api_helper.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/tests/test_back_off.py` & `covalent-api-sdk-0.0.4/tests/test_back_off.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/tests/test_balance_service.py` & `covalent-api-sdk-0.0.4/tests/test_balance_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/tests/test_base_service.py` & `covalent-api-sdk-0.0.4/tests/test_base_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/tests/test_nft_service.py` & `covalent-api-sdk-0.0.4/tests/test_nft_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/tests/test_pricing_service.py` & `covalent-api-sdk-0.0.4/tests/test_pricing_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/tests/test_security_service.py` & `covalent-api-sdk-0.0.4/tests/test_security_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/tests/test_transaction_service.py` & `covalent-api-sdk-0.0.4/tests/test_transaction_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.3/tests/test_xyk_service.py` & `covalent-api-sdk-0.0.4/tests/test_xyk_service.py`

 * *Files identical despite different names*

