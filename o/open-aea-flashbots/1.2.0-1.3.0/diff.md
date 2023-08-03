# Comparing `tmp/open-aea-flashbots-1.2.0.tar.gz` & `tmp/open-aea-flashbots-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-flashbots-1.2.0.tar", last modified: Fri Jul 28 08:55:47 2023, max compression
+gzip compressed data, was "open-aea-flashbots-1.3.0.tar", last modified: Thu Aug  3 07:34:31 2023, max compression
```

## Comparing `open-aea-flashbots-1.2.0.tar` & `open-aea-flashbots-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:55:47.369845 open-aea-flashbots-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1066 2023-07-24 08:53:20.000000 open-aea-flashbots-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2178 2023-07-28 08:55:47.369845 open-aea-flashbots-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1834 2023-07-24 08:53:20.000000 open-aea-flashbots-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:55:47.365845 open-aea-flashbots-1.2.0/flashbots/
--rw-r--r--   0 root         (0) root         (0)     1095 2023-07-24 08:53:20.000000 open-aea-flashbots-1.2.0/flashbots/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16817 2023-07-24 09:20:54.000000 open-aea-flashbots-1.2.0/flashbots/flashbots.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-07-24 08:53:20.000000 open-aea-flashbots-1.2.0/flashbots/middleware.py
--rw-r--r--   0 root         (0) root         (0)     2265 2023-07-24 09:12:35.000000 open-aea-flashbots-1.2.0/flashbots/provider.py
--rw-r--r--   0 root         (0) root         (0)     1923 2023-07-24 08:53:20.000000 open-aea-flashbots-1.2.0/flashbots/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:55:47.369845 open-aea-flashbots-1.2.0/open_aea_flashbots.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2178 2023-07-28 08:55:47.000000 open-aea-flashbots-1.2.0/open_aea_flashbots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      360 2023-07-28 08:55:47.000000 open-aea-flashbots-1.2.0/open_aea_flashbots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 08:55:47.000000 open-aea-flashbots-1.2.0/open_aea_flashbots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-28 08:55:47.000000 open-aea-flashbots-1.2.0/open_aea_flashbots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-28 08:55:47.000000 open-aea-flashbots-1.2.0/open_aea_flashbots.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      591 2023-07-27 08:05:12.000000 open-aea-flashbots-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 08:55:47.369845 open-aea-flashbots-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2721 2023-07-28 08:52:41.000000 open-aea-flashbots-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:34:31.185497 open-aea-flashbots-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-07-24 08:53:20.000000 open-aea-flashbots-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-08-03 07:34:31.185497 open-aea-flashbots-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-07-24 08:53:20.000000 open-aea-flashbots-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:34:31.185497 open-aea-flashbots-1.3.0/flashbots/
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-07-24 08:53:20.000000 open-aea-flashbots-1.3.0/flashbots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16817 2023-07-24 09:20:54.000000 open-aea-flashbots-1.3.0/flashbots/flashbots.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-07-24 08:53:20.000000 open-aea-flashbots-1.3.0/flashbots/middleware.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-07-24 09:12:35.000000 open-aea-flashbots-1.3.0/flashbots/provider.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-24 08:53:20.000000 open-aea-flashbots-1.3.0/flashbots/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:34:31.185497 open-aea-flashbots-1.3.0/open_aea_flashbots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-08-03 07:34:31.000000 open-aea-flashbots-1.3.0/open_aea_flashbots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      360 2023-08-03 07:34:31.000000 open-aea-flashbots-1.3.0/open_aea_flashbots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 07:34:31.000000 open-aea-flashbots-1.3.0/open_aea_flashbots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-08-03 07:34:31.000000 open-aea-flashbots-1.3.0/open_aea_flashbots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-03 07:34:31.000000 open-aea-flashbots-1.3.0/open_aea_flashbots.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      592 2023-08-03 07:26:43.000000 open-aea-flashbots-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 07:34:31.185497 open-aea-flashbots-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-08-03 07:26:36.000000 open-aea-flashbots-1.3.0/setup.py
```

### Comparing `open-aea-flashbots-1.2.0/LICENSE` & `open-aea-flashbots-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-flashbots-1.2.0/PKG-INFO` & `open-aea-flashbots-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-flashbots
-Version: 1.2.0
+Version: 1.3.0
 Summary: web3-flashbots.py
 Home-page: https://github.com/valory-xyz/web3-flashbots
 Author: Georgios Konstantopoulos
 Author-email: me@gakonst.com
 Maintainer: zeroXbrock
 Maintainer-email: brock@flashbots.net
 Requires-Python: >=3.9,<4.0
```

### Comparing `open-aea-flashbots-1.2.0/README.md` & `open-aea-flashbots-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `open-aea-flashbots-1.2.0/flashbots/__init__.py` & `open-aea-flashbots-1.3.0/flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-flashbots-1.2.0/flashbots/flashbots.py` & `open-aea-flashbots-1.3.0/flashbots/flashbots.py`

 * *Files identical despite different names*

### Comparing `open-aea-flashbots-1.2.0/flashbots/middleware.py` & `open-aea-flashbots-1.3.0/flashbots/middleware.py`

 * *Files identical despite different names*

### Comparing `open-aea-flashbots-1.2.0/flashbots/provider.py` & `open-aea-flashbots-1.3.0/flashbots/provider.py`

 * *Files identical despite different names*

### Comparing `open-aea-flashbots-1.2.0/flashbots/types.py` & `open-aea-flashbots-1.3.0/flashbots/types.py`

 * *Files identical despite different names*

### Comparing `open-aea-flashbots-1.2.0/open_aea_flashbots.egg-info/PKG-INFO` & `open-aea-flashbots-1.3.0/open_aea_flashbots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-flashbots
-Version: 1.2.0
+Version: 1.3.0
 Summary: web3-flashbots.py
 Home-page: https://github.com/valory-xyz/web3-flashbots
 Author: Georgios Konstantopoulos
 Author-email: me@gakonst.com
 Maintainer: zeroXbrock
 Maintainer-email: brock@flashbots.net
 Requires-Python: >=3.9,<4.0
```

### Comparing `open-aea-flashbots-1.2.0/setup.py` & `open-aea-flashbots-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from setuptools import find_packages, setup
 
 packages = ["flashbots"]
 
 package_data = {"": ["*"]}
 
 install_requires = [
-    "web3>=6.0.0,<7.0.0",
+    "open-aea-web3==6.0.1",
     "coincurve>=18.0.0,<19.0.0",
 ]
 
 setup_kwargs = {
     "name": "open-aea-flashbots",
-    "version": "1.2.0",
+    "version": "1.3.0",
     "description": "web3-flashbots.py",
     "long_description": 'This library works by injecting flashbots as a new module in the Web3.py instance, which allows submitting "bundles" of transactions directly to miners. This is done by also creating a middleware which captures calls to `eth_sendBundle` and `eth_callBundle`, and sends them to an RPC endpoint which you have specified, which corresponds to `mev-geth`.\n\nTo apply correct headers we use the `flashbot` method which injects the correct header on POST.\n\n## Quickstart\n\n```python\nfrom eth_account.signers.local import LocalAccount\nfrom web3 import Web3, HTTPProvider\nfrom flashbots import flashbot\nfrom eth_account.account import Account\nimport os\n\nETH_ACCOUNT_SIGNATURE: LocalAccount = Account.from_key(os.environ.get("ETH_SIGNATURE_KEY"))\n\n\nw3 = Web3(HTTPProvider("http://localhost:8545"))\nflashbot(w3, ETH_ACCOUNT_SIGNATURE)\n```\n\nNow the `w3.flashbots.sendBundle` method should be available to you. Look in [examples/simple.py](./examples/simple.py) for usage examples.\n\n### Goerli\n\nTo use goerli, add the goerli relay RPC to the `flashbot` function arguments.\n\n```python\nflashbot(w3, ETH_ACCOUNT_SIGNATURE, "https://relay-goerli.flashbots.net")\n```\n\n## Development and testing\n\nInstall [poetry](https://python-poetry.org/)\n\nPoetry will automatically fix your venv and all packages needed.\n\n```sh\npoetry install\n```\n\nTips: PyCharm has a poetry plugin\n\n## Simple Goerli Example\n\nSee [examples/simple.py](./examples/simple.py) for environment variable definitions.\n\n```sh\npoetry shell\nETH_SENDER_KEY=<sender_private_key> \\nPROVIDER_URL=https://eth-goerli.alchemyapi.io/v2/<alchemy_key> \\nETH_SIGNER_KEY=<signer_private_key> \\npython examples/simple.py\n```\n\n## Linting\n\nIt\'s advisable to run black with default rules for linting\n\n```sh\nsudo pip install black # Black should be installed with a global entrypoint\nblack .\n```',
     "long_description_content_type": "text/markdown",
     "author": "Georgios Konstantopoulos",
     "author_email": "me@gakonst.com",
     "maintainer": "zeroXbrock",
     "maintainer_email": "brock@flashbots.net",
```

