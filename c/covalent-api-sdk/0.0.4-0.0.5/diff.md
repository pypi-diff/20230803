# Comparing `tmp/covalent-api-sdk-0.0.4.tar.gz` & `tmp/covalent-api-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-api-sdk-0.0.4.tar", last modified: Thu Aug  3 06:37:15 2023, max compression
+gzip compressed data, was "covalent-api-sdk-0.0.5.tar", last modified: Thu Aug  3 07:00:01 2023, max compression
```

## Comparing `covalent-api-sdk-0.0.4.tar` & `covalent-api-sdk-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.499820 covalent-api-sdk-0.0.4/
--rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 06:37:15.499596 covalent-api-sdk-0.0.4/PKG-INFO
--rw-r--r--   0 davidwork   (501) staff       (20)    12482 2023-08-03 01:55:34.000000 covalent-api-sdk-0.0.4/README.md
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.492146 covalent-api-sdk-0.0.4/covalent/
--rw-r--r--   0 davidwork   (501) staff       (20)       48 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/covalent/__init__.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1059 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/covalent/client.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.494089 covalent-api-sdk-0.0.4/covalent/services/
--rw-r--r--   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:08.000000 covalent-api-sdk-0.0.4/covalent/services/__init__.py
--rw-r--r--   0 davidwork   (501) staff       (20)    51117 2023-08-03 06:31:40.000000 covalent-api-sdk-0.0.4/covalent/services/balance_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    42736 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/base_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    65956 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/nft_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     8668 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/pricing_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    10643 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/security_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)    28811 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/transaction_service.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.494840 covalent-api-sdk-0.0.4/covalent/services/util/
--rw-r--r--   0 davidwork   (501) staff       (20)      205 2023-08-03 06:31:48.000000 covalent-api-sdk-0.0.4/covalent/services/util/__init__.py
--rw-r--r--   0 davidwork   (501) staff       (20)     2533 2023-08-03 06:37:07.000000 covalent-api-sdk-0.0.4/covalent/services/util/api_helper.py
--rw-r--r--   0 davidwork   (501) staff       (20)      990 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/covalent/services/util/back_off.py
--rw-r--r--   0 davidwork   (501) staff       (20)    73591 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.4/covalent/services/xyk_service.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.495670 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/
--rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 davidwork   (501) staff       (20)      920 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 davidwork   (501) staff       (20)        1 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 davidwork   (501) staff       (20)       50 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/requires.txt
--rw-r--r--   0 davidwork   (501) staff       (20)        9 2023-08-03 06:37:15.000000 covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 davidwork   (501) staff       (20)       38 2023-08-03 06:37:15.499872 covalent-api-sdk-0.0.4/setup.cfg
--rw-r--r--   0 davidwork   (501) staff       (20)     1527 2023-08-03 06:37:00.000000 covalent-api-sdk-0.0.4/setup.py
-drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:15.497730 covalent-api-sdk-0.0.4/tests/
--rw-r--r--   0 davidwork   (501) staff       (20)     1541 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_api_helper.py
--rw-r--r--   0 davidwork   (501) staff       (20)      668 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_back_off.py
--rw-r--r--   0 davidwork   (501) staff       (20)     5313 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_balance_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     6450 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_base_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)      464 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_client.py
--rw-r--r--   0 davidwork   (501) staff       (20)    10712 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_nft_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     1238 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_pricing_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)      867 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_security_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     3941 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_transaction_service.py
--rw-r--r--   0 davidwork   (501) staff       (20)     6585 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.4/tests/test_xyk_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 07:00:01.130354 covalent-api-sdk-0.0.5/
+-rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 07:00:01.129836 covalent-api-sdk-0.0.5/PKG-INFO
+-rw-r--r--   0 davidwork   (501) staff       (20)    12482 2023-08-03 01:55:34.000000 covalent-api-sdk-0.0.5/README.md
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 07:00:01.121847 covalent-api-sdk-0.0.5/covalent/
+-rw-r--r--   0 davidwork   (501) staff       (20)       48 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/covalent/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1059 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/covalent/client.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 07:00:01.124356 covalent-api-sdk-0.0.5/covalent/services/
+-rw-r--r--   0 davidwork   (501) staff       (20)        0 2023-08-03 06:37:08.000000 covalent-api-sdk-0.0.5/covalent/services/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    51117 2023-08-03 06:31:40.000000 covalent-api-sdk-0.0.5/covalent/services/balance_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    42736 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.5/covalent/services/base_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    65956 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.5/covalent/services/nft_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     8668 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.5/covalent/services/pricing_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    10643 2023-08-03 00:55:38.000000 covalent-api-sdk-0.0.5/covalent/services/security_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    28830 2023-08-03 06:56:09.000000 covalent-api-sdk-0.0.5/covalent/services/transaction_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 07:00:01.125930 covalent-api-sdk-0.0.5/covalent/services/util/
+-rw-r--r--   0 davidwork   (501) staff       (20)      205 2023-08-03 06:31:48.000000 covalent-api-sdk-0.0.5/covalent/services/util/__init__.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     2533 2023-08-03 06:57:46.000000 covalent-api-sdk-0.0.5/covalent/services/util/api_helper.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      990 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/covalent/services/util/back_off.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    73576 2023-08-03 06:56:56.000000 covalent-api-sdk-0.0.5/covalent/services/xyk_service.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 07:00:01.127416 covalent-api-sdk-0.0.5/covalent_api_sdk.egg-info/
+-rw-r--r--   0 davidwork   (501) staff       (20)    13121 2023-08-03 07:00:01.000000 covalent-api-sdk-0.0.5/covalent_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 davidwork   (501) staff       (20)      920 2023-08-03 07:00:01.000000 covalent-api-sdk-0.0.5/covalent_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)        1 2023-08-03 07:00:01.000000 covalent-api-sdk-0.0.5/covalent_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)       50 2023-08-03 07:00:01.000000 covalent-api-sdk-0.0.5/covalent_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)        9 2023-08-03 07:00:01.000000 covalent-api-sdk-0.0.5/covalent_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 davidwork   (501) staff       (20)       38 2023-08-03 07:00:01.130504 covalent-api-sdk-0.0.5/setup.cfg
+-rw-r--r--   0 davidwork   (501) staff       (20)     1527 2023-08-03 06:57:40.000000 covalent-api-sdk-0.0.5/setup.py
+drwxr-xr-x   0 davidwork   (501) staff       (20)        0 2023-08-03 07:00:01.129431 covalent-api-sdk-0.0.5/tests/
+-rw-r--r--   0 davidwork   (501) staff       (20)     1541 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_api_helper.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      668 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_back_off.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     5313 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_balance_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     6450 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_base_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      464 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_client.py
+-rw-r--r--   0 davidwork   (501) staff       (20)    10712 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_nft_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     1238 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_pricing_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)      867 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_security_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     3941 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_transaction_service.py
+-rw-r--r--   0 davidwork   (501) staff       (20)     6585 2023-08-02 21:32:39.000000 covalent-api-sdk-0.0.5/tests/test_xyk_service.py
```

### Comparing `covalent-api-sdk-0.0.4/PKG-INFO` & `covalent-api-sdk-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-api-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: covalent-api-sdk-py
 Home-page: https://github.com/covalenthq/covalent-api-sdk-py/
 Author: Covalenthq
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covalent-api-sdk-0.0.4/README.md` & `covalent-api-sdk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/covalent/client.py` & `covalent-api-sdk-0.0.5/covalent/client.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/covalent/services/balance_service.py` & `covalent-api-sdk-0.0.5/covalent/services/balance_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/covalent/services/base_service.py` & `covalent-api-sdk-0.0.5/covalent/services/base_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/covalent/services/nft_service.py` & `covalent-api-sdk-0.0.5/covalent/services/nft_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/covalent/services/pricing_service.py` & `covalent-api-sdk-0.0.5/covalent/services/pricing_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/covalent/services/security_service.py` & `covalent-api-sdk-0.0.5/covalent/services/security_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/covalent/services/transaction_service.py` & `covalent-api-sdk-0.0.5/covalent/services/transaction_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,24 +294,24 @@
                     data = await response.json()
         
             if data.get("error") and data.get("error_code") == 429:
                 try:
                     backoff.back_off()
                 except Exception as error:
                     has_next = False
-                    print("An error occured", (data.error if data else response.status), ":", data.get("error_message") if data else "401 Authorization Required")
+                    print("An error occured", (data.get("error_code") if data else response.status), ":", data.get("error_message") if data else "401 Authorization Required")
             else:
                 for tx in data.get("data").get("items"):
                     data_class = Transaction(tx)
                     check_and_modify_response(data_class)
                     yield data_class
                 
                 backoff.set_num_attempts(1)
 
-                if not data.error:
+                if not data.get("error"):
                     if data.get("data") is not None and data.get("data").get("links").get("prev") is None:
                         has_next = False
                     url = data.get("data").get("links").get("prev") if data.get("data") is not None and data.get("data").get("links").get("prev") is not None else ""
                 else:
                     has_next = False
         except Exception:
             has_next = False
```

### Comparing `covalent-api-sdk-0.0.4/covalent/services/util/api_helper.py` & `covalent-api-sdk-0.0.5/covalent/services/util/api_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal
 
 chains = Literal["btc-mainnet", "eth-mainnet", "matic-mainnet", "bsc-mainnet", "avalanche-mainnet", "fantom-mainnet", "moonbeam-mainnet", "moonbeam-moonriver", "rsk-mainnet", "arbitrum-mainnet", "palm-mainnet", "klaytn-mainnet", "heco-mainnet", "nervos-godwoken-mainnet", "axie-mainnet", "evmos-mainnet", "astar-mainnet", "iotex-mainnet", "harmony-mainnet", "cronos-mainnet", "aurora-mainnet", "emerald-paratime-mainnet", "boba-mainnet", "eth-goerli", "matic-mumbai", "avalanche-testnet", "bsc-testnet", "moonbeam-moonbase-alpha", "rsk-testnet", "arbitrum-goerli", "fantom-testnet", "palm-testnet", "heco-testnet", "nervos-godwoken-testnet", "evmos-testnet", "astar-shiden", "iotex-testnet", "harmony-testnet", "aurora-testnet", "scroll-l2-testnet", "scroll-l1-testnet", "covalent-internal-network-v1", "defi-kingdoms-mainnet", "swimmer-mainnet", "boba-avalanche-mainnet", "boba-bobabeam-mainnet", "boba-bnb-mainnet", "boba-rinkeby-testnet", "boba-bobabase-testnet", "boba-bnb-testnet", "boba-avalanche-testnet", "klaytn-testnet", "gather-mainnet", "gather-testnet", "optimism-mainnet", "skale-calypso", "skale-mainnet", "skale-razor", "avalanche-dexalot-mainnet", "skale-omnus", "avalanche-dexalot-testnet", "astar-shibuya", "cronos-testnet", "defi-kingdoms-testnet", "metis-mainnet", "metis-testnet", "milkomeda-a1-mainnet", "milkomeda-a1-devnet", "milkomeda-c1-mainnet", "milkomeda-c1-devnet", "swimmer-testnet", "solana-mainnet", "skale-europa", "meter-mainnet", "meter-testnet", "skale-exorde", "boba-goerli", "neon-testnet", "skale-staging-uum", "skale-staging-lcc", "arbitrum-nova-mainnet", "canto-mainnet", "bittorrent-mainnet", "bittorrent-testnet", "flarenetworks-flare-mainnet", "flarenetworks-flare-testnet", "flarenetworks-canary-mainnet", "flarenetworks-canary-testnet", "kcc-mainnet", "kcc-testnet", "polygon-zkevm-testnet", "linea-testnet", "base-testnet", "mantle-testnet", "scroll-alpha-testnet", "oasys-mainnet", "oasys-testnet", "findora-mainnet", "findora-forge-testnet", "sx-mainnet"]
 quotes = Literal["USD", "CAD", "EUR", "SGD", "INR", "JPY", "VND", "CNY", "KRW", "RUB", "TRY", "NGN", "ARS", "AUD", "CHF", "GBP"]
-user_agent = "com.covalenthq.sdk.python/0.0.4"
+user_agent = "com.covalenthq.sdk.python/0.0.5"
 
 def check_and_modify_response(json_obj):
     """ modify reponse and remove next_update_at """
     for key in list(vars(json_obj).keys()):
         if key == 'next_update_at':
             del vars(json_obj)[key]
         elif isinstance(vars(json_obj)[key], dict):
```

### Comparing `covalent-api-sdk-0.0.4/covalent/services/util/back_off.py` & `covalent-api-sdk-0.0.5/covalent/services/util/back_off.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/covalent/services/xyk_service.py` & `covalent-api-sdk-0.0.5/covalent/services/xyk_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from datetime import datetime
 from typing import Generic, TypeVar, List, Optional
-import aiohttp
 import requests
 from .util.api_helper import check_and_modify_response, chains, quotes, user_agent
 from .util.back_off import ExponentialBackoff
 
 class PoolResponse:
     updated_at: datetime
     """ The timestamp when the response was generated. Useful to show data staleness to users. """
```

### Comparing `covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/PKG-INFO` & `covalent-api-sdk-0.0.5/covalent_api_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-api-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: covalent-api-sdk-py
 Home-page: https://github.com/covalenthq/covalent-api-sdk-py/
 Author: Covalenthq
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covalent-api-sdk-0.0.4/covalent_api_sdk.egg-info/SOURCES.txt` & `covalent-api-sdk-0.0.5/covalent_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/setup.py` & `covalent-api-sdk-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='covalent-api-sdk',   # Replace with the name of your package
-    version='0.0.4',             # Replace with the version of your package
+    version='0.0.5',             # Replace with the version of your package
     license="MIT",
     # Description and long_description should contain a concise and detailed description of your project.
     description='covalent-api-sdk-py',
     long_description=open('README.md').read() + "\n",
     long_description_content_type='text/markdown',
     author='Covalenthq',          # Replace with your name
     python_requires='>=3.7',
```

### Comparing `covalent-api-sdk-0.0.4/tests/test_api_helper.py` & `covalent-api-sdk-0.0.5/tests/test_api_helper.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/tests/test_back_off.py` & `covalent-api-sdk-0.0.5/tests/test_back_off.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/tests/test_balance_service.py` & `covalent-api-sdk-0.0.5/tests/test_balance_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/tests/test_base_service.py` & `covalent-api-sdk-0.0.5/tests/test_base_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/tests/test_nft_service.py` & `covalent-api-sdk-0.0.5/tests/test_nft_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/tests/test_pricing_service.py` & `covalent-api-sdk-0.0.5/tests/test_pricing_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/tests/test_security_service.py` & `covalent-api-sdk-0.0.5/tests/test_security_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/tests/test_transaction_service.py` & `covalent-api-sdk-0.0.5/tests/test_transaction_service.py`

 * *Files identical despite different names*

### Comparing `covalent-api-sdk-0.0.4/tests/test_xyk_service.py` & `covalent-api-sdk-0.0.5/tests/test_xyk_service.py`

 * *Files identical despite different names*

