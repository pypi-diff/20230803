# Comparing `tmp/covalent-api-sdk-0.0.2.tar.gz` & `tmp/covalent-api-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-api-sdk-0.0.2.tar", last modified: Thu Aug  3 01:56:23 2023, max compression
+gzip compressed data, was "covalent-api-sdk-0.0.3.tar", last modified: Thu Aug  3 06:24:48 2023, max compression
```

## Comparing `covalent-api-sdk-0.0.2.tar` & `covalent-api-sdk-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 01:56:23.468673 covalent-api-sdk-0.0.2/
--rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 01:56:23.468353 covalent-api-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 davidwork   (501) staff       (20)    12482 2023-08-03 01:55:34.000000 covalent-api-sdk-0.0.2/README.md
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 01:56:23.464876 covalent-api-sdk-0.0.2/covalent/
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 01:56:23.465862 covalent-api-sdk-0.0.2/covalent/covalent_api_sdk.egg-info/
--rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 01:56:23.000000 covalent-api-sdk-0.0.2/covalent/covalent_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 davidwork   (501) staff       (20)      535 2023-08-03 01:56:23.000000 covalent-api-sdk-0.0.2/covalent/covalent_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 davidwork   (501) staff       (20)        1 2023-08-03 01:56:23.000000 covalent-api-sdk-0.0.2/covalent/covalent_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 davidwork   (501) staff       (20)       50 2023-08-03 01:56:23.000000 covalent-api-sdk-0.0.2/covalent/covalent_api_sdk.egg-info/requires.txt
--rw-r--r--   0 davidwork   (501) staff       (20)        1 2023-08-03 01:56:23.000000 covalent-api-sdk-0.0.2/covalent/covalent_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 davidwork   (501) staff       (20)       38 2023-08-03 01:56:23.468721 covalent-api-sdk-0.0.2/setup.cfg
--rw-r--r--   0 davidwork   (501) staff       (20)     1577 2023-08-03 01:55:41.000000 covalent-api-sdk-0.0.2/setup.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 01:56:23.468074 covalent-api-sdk-0.0.2/tests/
--rw-r--r--   0 davidwork   (501) staff       (20)     1541 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_api_helper.py
--rw-r--r--   0 davidwork   (501) staff       (20)      668 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_back_off.py
--rw-r--r--   0 davidwork   (501) staff       (20)     5313 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_balance_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     6450 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_base_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)      464 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_client.py
--rw-r--r--   0 davidwork   (501) staff       (20)    10712 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_nft_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1238 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_pricing_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)      867 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_security_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     3941 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_transaction_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     6585 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.2/tests/test_xyk_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:24:48.507400 covalent-api-sdk-0.0.3/
+-rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 06:24:48.507202 covalent-api-sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 davidwork   (501) staff       (20)    12482 2023-08-03 01:55:34.000000 covalent-api-sdk-0.0.3/README.md
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:24:48.504291 covalent-api-sdk-0.0.3/covalent/
+-rw-r--r--   0 davidwork   (501) staff       (20)       48 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/covalent/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1059 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/covalent/client.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:24:48.504939 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/
+-rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 davidwork   (501) staff       (20)      530 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)        1 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)       50 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)        9 2023-08-03 06:24:48.000000 covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)       38 2023-08-03 06:24:48.507442 covalent-api-sdk-0.0.3/setup.cfg
+-rw-r--r--   0 davidwork   (501) staff       (20)     1527 2023-08-03 06:23:24.000000 covalent-api-sdk-0.0.3/setup.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:24:48.506887 covalent-api-sdk-0.0.3/tests/
+-rw-r--r--   0 davidwork   (501) staff       (20)     1541 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_api_helper.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      668 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_back_off.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     5313 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_balance_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     6450 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_base_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      464 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_client.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    10712 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_nft_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1238 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_pricing_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      867 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_security_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     3941 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_transaction_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     6585 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.3/tests/test_xyk_service.py
```

### Comparing `covalent-api-sdk-0.0.2/PKG-INFO` & `covalent-api-sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-api-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: covalent-api-sdk-py
 Home-page: https://github.com/covalenthq/covalent-api-sdk-py/
 Author: Covalenthq
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covalent-api-sdk-0.0.2/README.md` & `covalent-api-sdk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/covalent/covalent_api_sdk.egg-info/PKG-INFO` & `covalent-api-sdk-0.0.3/covalent_api_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-api-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: covalent-api-sdk-py
 Home-page: https://github.com/covalenthq/covalent-api-sdk-py/
 Author: Covalenthq
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covalent-api-sdk-0.0.2/setup.py` & `covalent-api-sdk-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='covalent-api-sdk',   # Replace with the name of your package
-    version='0.0.2',             # Replace with the version of your package
+    version='0.0.3',             # Replace with the version of your package
     license="MIT",
     # Description and long_description should contain a concise and detailed description of your project.
     description='covalent-api-sdk-py',
     long_description=open('README.md').read() + "\n",
     long_description_content_type='text/markdown',
     author='Covalenthq',          # Replace with your name
     python_requires='>=3.7',
     url='https://github.com/covalenthq/covalent-api-sdk-py/',  # Replace with the URL of your project repository
-    package_dir={"":"covalent"},
-    packages=find_packages(where="covalent",exclude=['tests', 'tests.*']),    # Automatically find all packages in your project directory
+    packages=find_packages(exclude=['tests', 'tests.*']),    # Automatically find all packages in your project directory
 
     # Add any dependencies required by your package
     install_requires=[
         # Add your dependencies here, e.g., 'numpy>=1.18.0'
         'aiohttp',
         'pytest',
         'requests',
```

### Comparing `covalent-api-sdk-0.0.2/tests/test_api_helper.py` & `covalent-api-sdk-0.0.3/tests/test_api_helper.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/tests/test_back_off.py` & `covalent-api-sdk-0.0.3/tests/test_back_off.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/tests/test_balance_service.py` & `covalent-api-sdk-0.0.3/tests/test_balance_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/tests/test_base_service.py` & `covalent-api-sdk-0.0.3/tests/test_base_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/tests/test_nft_service.py` & `covalent-api-sdk-0.0.3/tests/test_nft_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/tests/test_pricing_service.py` & `covalent-api-sdk-0.0.3/tests/test_pricing_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/tests/test_security_service.py` & `covalent-api-sdk-0.0.3/tests/test_security_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/tests/test_transaction_service.py` & `covalent-api-sdk-0.0.3/tests/test_transaction_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.2/tests/test_xyk_service.py` & `covalent-api-sdk-0.0.3/tests/test_xyk_service.py`

 * *Files identical despite different names*

