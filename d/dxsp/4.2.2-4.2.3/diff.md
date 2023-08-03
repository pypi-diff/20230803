# Comparing `tmp/dxsp-4.2.2.tar.gz` & `tmp/dxsp-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.2.2.tar", max compression
+gzip compressed data, was "dxsp-4.2.3.tar", max compression
```

## Comparing `dxsp-4.2.2.tar` & `dxsp-4.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-25 19:43:39.050390 dxsp-4.2.2/LICENSE
--rw-r--r--   0        0        0     2857 2023-07-25 19:43:39.050390 dxsp-4.2.2/README.md
--rw-r--r--   0        0        0      158 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/config.py
--rw-r--r--   0        0        0    12100 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5743 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/main.py
--rw-r--r--   0        0        0      104 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1864 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1037 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4834 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6619 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1990 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/utils.py
--rw-r--r--   0        0        0     4057 2023-07-25 19:43:42.978444 dxsp-4.2.2/pyproject.toml
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 dxsp-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-03 20:04:37.012025 dxsp-4.2.3/LICENSE
+-rw-r--r--   0        0        0     2857 2023-08-03 20:04:37.012025 dxsp-4.2.3/README.md
+-rw-r--r--   0        0        0      158 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/config.py
+-rw-r--r--   0        0        0    12124 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5743 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4834 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-08-03 20:04:37.012025 dxsp-4.2.3/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     3927 2023-08-03 20:04:42.752119 dxsp-4.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 dxsp-4.2.3/PKG-INFO
```

### Comparing `dxsp-4.2.2/LICENSE` & `dxsp-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/README.md` & `dxsp-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/dxsp/default_settings.toml` & `dxsp-4.2.3/dxsp/default_settings.toml`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 dxsp_commands = "🎯 BUY WBTC\n🎯 /q WBTC\n 🏦 /bal\n 🏦 /pos\n"
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "0x"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_0x_url = "https://api.0x.org/"
+dex_0x_api_key = "123" 
 dex_router_contract_addr = "0xdef1c0ded9bec7f1a1670819833240f027b25eff"
 dex_factory_contract_addr = ""
 dex_router_abi_url = "https://raw.githubusercontent.com/0xProject/protocol/development/packages/contract-artifacts/artifacts/Exchange.json"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10
 dex_trading_slippage = 2
```

### Comparing `dxsp-4.2.2/dxsp/main.py` & `dxsp-4.2.3/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/dxsp/protocols/oneinch.py` & `dxsp-4.2.3/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/dxsp/protocols/uniswap.py` & `dxsp-4.2.3/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/dxsp/protocols/zerox.py` & `dxsp-4.2.3/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/dxsp/utils/account_utils.py` & `dxsp-4.2.3/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/dxsp/utils/contract_utils.py` & `dxsp-4.2.3/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/dxsp/utils/explorer_utils.py` & `dxsp-4.2.3/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.2/pyproject.toml` & `dxsp-4.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.2.2"
+version = "4.2.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -47,14 +47,15 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 eth_tester = "^0.9.0b2"
@@ -75,26 +76,25 @@
 ]
 
 
 
 
 
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^7.0.0"
+sphinx = ">=5,<6"
 sphinx_bootstrap_theme = "^0.8.1"
-sphinx-autoapi = "^2.1.1"
-sphinx-copybutton= "^0.5.2"
-myst-parser = "^2.0.0"
-sphinx-notfound-page = "^0.8.3"
 sphinxext-remoteliteralinclude = "^0.4.0"
-sphinx-togglebutton = "*"
+
+
+
 
 
 # [tool.semantic_release]
 # version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
 # branch = "main"
 # upload_to_pypi = true
 # upload_to_release = true
```

### Comparing `dxsp-4.2.2/PKG-INFO` & `dxsp-4.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.2.2
+Version: 4.2.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.2.2 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.2.3 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist:
 pycoingecko (>=3.1.0,<4.0.0) Requires-Dist: uniswap-python (>=0.7.0,<0.8.0)
```

