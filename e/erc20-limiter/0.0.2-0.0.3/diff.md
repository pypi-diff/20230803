# Comparing `tmp/erc20-limiter-0.0.2.tar.gz` & `tmp/erc20-limiter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erc20-limiter-0.0.2.tar", last modified: Fri Jul 28 12:43:40 2023, max compression
+gzip compressed data, was "erc20-limiter-0.0.3.tar", last modified: Thu Aug  3 15:54:42 2023, max compression
```

## Comparing `erc20-limiter-0.0.2.tar` & `erc20-limiter-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/
--rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-07-28 12:43:39.000000 erc20-limiter-0.0.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      693 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/erc20_limiter/
--rw-r--r--   0 lash      (1000) lash      (1000)       29 2023-07-27 16:56:28.000000 erc20-limiter-0.0.2/erc20_limiter/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/erc20_limiter/data/
--rw-r--r--   0 lash      (1000) lash      (1000)     4898 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/Limiter.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1602 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/Limiter.json
--rw-r--r--   0 lash      (1000) lash      (1000)     2279 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/Limiter.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)     4814 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1338 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.json
--rw-r--r--   0 lash      (1000) lash      (1000)     2054 2023-07-28 11:44:53.000000 erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2023-07-27 16:57:09.000000 erc20-limiter-0.0.2/erc20_limiter/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3409 2023-07-28 11:14:14.000000 erc20-limiter-0.0.2/erc20_limiter/limiter.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2768 2023-07-28 11:30:19.000000 erc20-limiter-0.0.2/erc20_limiter/token.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/erc20_limiter/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-07-27 16:55:49.000000 erc20-limiter-0.0.2/erc20_limiter/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1938 2023-07-28 11:35:40.000000 erc20-limiter-0.0.2/erc20_limiter/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/erc20_limiter.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      693 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      719 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       14 2023-07-28 12:43:40.000000 erc20-limiter-0.0.2/erc20_limiter.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-07-27 16:54:14.000000 erc20-limiter-0.0.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      797 2023-07-28 12:43:40.256615 erc20-limiter-0.0.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      473 2023-07-28 12:36:47.000000 erc20-limiter-0.0.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       58 2023-07-27 16:55:11.000000 erc20-limiter-0.0.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-28 12:43:40.253282 erc20-limiter-0.0.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      825 2023-07-28 11:12:58.000000 erc20-limiter-0.0.2/tests/test_base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1590 2023-07-28 11:36:18.000000 erc20-limiter-0.0.2/tests/test_token_registry.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-07-28 09:50:15.000000 erc20-limiter-0.0.3/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       63 2023-07-28 12:43:39.000000 erc20-limiter-0.0.3/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/erc20_limiter/
+-rw-r--r--   0 lash      (1000) lash      (1000)       29 2023-07-27 16:56:28.000000 erc20-limiter-0.0.3/erc20_limiter/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/erc20_limiter/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5428 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/Limiter.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1602 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/Limiter.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2279 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/Limiter.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     6340 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1923 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2623 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     4978 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1338 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     2054 2023-08-03 15:51:50.000000 erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2023-07-27 16:57:09.000000 erc20-limiter-0.0.3/erc20_limiter/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2688 2023-08-03 12:50:12.000000 erc20-limiter-0.0.3/erc20_limiter/index.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3409 2023-07-28 11:14:14.000000 erc20-limiter-0.0.3/erc20_limiter/limiter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/erc20_limiter/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-07-27 16:55:49.000000 erc20-limiter-0.0.3/erc20_limiter/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1914 2023-08-03 12:51:31.000000 erc20-limiter-0.0.3/erc20_limiter/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/erc20_limiter.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      837 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       14 2023-08-03 15:54:42.000000 erc20-limiter-0.0.3/erc20_limiter.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-07-27 16:54:14.000000 erc20-limiter-0.0.3/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      797 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      473 2023-07-28 12:36:47.000000 erc20-limiter-0.0.3/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       58 2023-07-27 16:55:11.000000 erc20-limiter-0.0.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-03 15:54:42.362999 erc20-limiter-0.0.3/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      825 2023-07-28 11:12:58.000000 erc20-limiter-0.0.3/tests/test_base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1550 2023-08-03 12:51:44.000000 erc20-limiter-0.0.3/tests/test_index.py
```

### Comparing `erc20-limiter-0.0.2/PKG-INFO` & `erc20-limiter-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erc20-limiter
-Version: 0.0.2
+Version: 0.0.3
 Summary: ERC20 balance limit registry
 Home-page: https://holbrook.no/src/erc20-limiter/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,8 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
+License-File: LICENSE
```

### Comparing `erc20-limiter-0.0.2/erc20_limiter/data/Limiter.bin` & `erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.bin`

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-608060405234801561001057600080fd5b50336000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550610931806100606000396000f3fe608060405234801561001057600080fd5b506004361061007f576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461008457806323778613146100b457806336db43b5146100e45780638da5cb5b14610100578063bdd554401461011e578063f2fde38b1461013a575b600080fd5b61009e60048036038101906100999190610633565b61016a565b6040516100ab919061067b565b60405180910390f35b6100ce60048036038101906100c991906106f4565b61021a565b6040516100db919061074d565b60405180910390f35b6100fe60048036038101906100f99190610794565b6102a1565b005b610108610326565b60405161011591906107e3565b60405180910390f35b610138600480360381019061013391906107fe565b61034a565b005b610154600480360381019061014f9190610851565b610494565b604051610161919061067b565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101be5760019050610215565b639493f8b27c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036102105760019050610215565b600090505b919050565b6000600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002054905092915050565b80600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff168152602001908152602001600020819055505050565b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1681565b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff1614806103cf57508173ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16145b61040e576040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610405906108db565b60405180910390fd5b80600160008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002081905550505050565b60008060008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16146104ef57600080fd5b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050826000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555060008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff167f8be0079c531659141344cd1fd0a4f28419497f9722a3daafe3b4186f6b6457e060405160405180910390a36001915050919050565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610610816105db565b811461061b57600080fd5b50565b60008135905061062d81610607565b92915050565b600060208284031215610649576106486105d6565b5b60006106578482850161061e565b91505092915050565b60008115159050919050565b61067581610660565b82525050565b6000602082019050610690600083018461066c565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006106c182610696565b9050919050565b6106d1816106b6565b81146106dc57600080fd5b50565b6000813590506106ee816106c8565b92915050565b6000806040838503121561070b5761070a6105d6565b5b6000610719858286016106df565b925050602061072a858286016106df565b9150509250929050565b6000819050919050565b61074781610734565b82525050565b6000602082019050610762600083018461073e565b92915050565b61077181610734565b811461077c57600080fd5b50565b60008135905061078e81610768565b92915050565b600080604083850312156107ab576107aa6105d6565b5b60006107b9858286016106df565b92505060206107ca8582860161077f565b9150509250929050565b6107dd816106b6565b82525050565b60006020820190506107f860008301846107d4565b92915050565b600080600060608486031215610817576108166105d6565b5b6000610825868287016106df565b9350506020610836868287016106df565b92505060406108478682870161077f565b9150509250925092565b600060208284031215610867576108666105d6565b5b6000610875848285016106df565b91505092915050565b600082825260208201905092915050565b7f4552525f41585800000000000000000000000000000000000000000000000000600082015250565b60006108c560078361087e565b91506108d08261088f565b602082019050919050565b600060208201905081810360008301526108f4816108b8565b905091905056fea2646970667358221220637537cee91db8d40743b879190b927cde6e34eee8a9524863365ce11ec024c664736f6c63430008130033
+608060405234801561001057600080fd5b506040516109b93803806109b98339818101604052810190610032919061015b565b81600160006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550806000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550505061019b565b600080fd5b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006100ea826100bf565b9050919050565b6100fa816100df565b811461010557600080fd5b50565b600081519050610117816100f1565b92915050565b6000610128826100df565b9050919050565b6101388161011d565b811461014357600080fd5b50565b6000815190506101558161012f565b92915050565b60008060408385031215610172576101716100ba565b5b600061018085828601610108565b925050602061019185828601610146565b9150509250929050565b61080f806101aa6000396000f3fe608060405234801561001057600080fd5b5060043610610074576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461007957806323778613146100a957806336db43b5146100d95780633ef25013146100f5578063bdd5544014610125575b600080fd5b610093600480360381019061008e9190610507565b610141565b6040516100a0919061054f565b60405180910390f35b6100c360048036038101906100be91906105c8565b610243565b6040516100d09190610621565b60405180910390f35b6100f360048036038101906100ee9190610668565b610306565b005b61010f600480360381019061010a91906106a8565b610315565b60405161011c919061054f565b60405180910390f35b61013f600480360381019061013a91906106d5565b6103fa565b005b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191603610195576001905061023e565b63b7bca6257c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101e7576001905061023e565b63237786137c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191603610239576001905061023e565b600090505b919050565b60008060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16632377861384846040518363ffffffff167c01000000000000000000000000000000000000000000000000000000000281526004016102bd929190610737565b602060405180830381865afa1580156102da573d6000803e3d6000fd5b505050506040513d601f19601f820116820180604052508101906102fe9190610775565b905092915050565b6103118233836103fa565b5050565b60008060008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16632377861384600160009054906101000a900473ffffffffffffffffffffffffffffffffffffffff166040518363ffffffff167c01000000000000000000000000000000000000000000000000000000000281526004016103b1929190610737565b602060405180830381865afa1580156103ce573d6000803e3d6000fd5b505050506040513d601f19601f820116820180604052508101906103f29190610775565b119050919050565b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1663bdd554408484846040518463ffffffff167c0100000000000000000000000000000000000000000000000000000000028152600401610473939291906107a2565b600060405180830381600087803b15801561048d57600080fd5b505af11580156104a1573d6000803e3d6000fd5b50505050505050565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b6104e4816104af565b81146104ef57600080fd5b50565b600081359050610501816104db565b92915050565b60006020828403121561051d5761051c6104aa565b5b600061052b848285016104f2565b91505092915050565b60008115159050919050565b61054981610534565b82525050565b60006020820190506105646000830184610540565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006105958261056a565b9050919050565b6105a58161058a565b81146105b057600080fd5b50565b6000813590506105c28161059c565b92915050565b600080604083850312156105df576105de6104aa565b5b60006105ed858286016105b3565b92505060206105fe858286016105b3565b9150509250929050565b6000819050919050565b61061b81610608565b82525050565b60006020820190506106366000830184610612565b92915050565b61064581610608565b811461065057600080fd5b50565b6000813590506106628161063c565b92915050565b6000806040838503121561067f5761067e6104aa565b5b600061068d858286016105b3565b925050602061069e85828601610653565b9150509250929050565b6000602082840312156106be576106bd6104aa565b5b60006106cc848285016105b3565b91505092915050565b6000806000606084860312156106ee576106ed6104aa565b5b60006106fc868287016105b3565b935050602061070d868287016105b3565b925050604061071e86828701610653565b9150509250925092565b6107318161058a565b82525050565b600060408201905061074c6000830185610728565b6107596020830184610728565b9392505050565b60008151905061076f8161063c565b92915050565b60006020828403121561078b5761078a6104aa565b5b600061079984828501610760565b91505092915050565b60006060820190506107b76000830186610728565b6107c46020830185610728565b6107d16040830184610612565b94935050505056fea2646970667358221220d14a5fb84c2c0c33d98c777eb16ce25087d08196d9f62f70806dcc9b49a0052464736f6c63430008130033
```

### Comparing `erc20-limiter-0.0.2/erc20_limiter/data/Limiter.json` & `erc20-limiter-0.0.3/erc20_limiter/data/Limiter.json`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.2/erc20_limiter/data/Limiter.metadata.json` & `erc20-limiter-0.0.3/erc20_limiter/data/LimiterIndex.metadata.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9079218106995884%*

 * *Differences: {"'output'": "{'abi': {0: {'inputs': [OrderedDict([('internalType', 'address'), ('name', "*

 * *             "'_holder'), ('type', 'address')]), OrderedDict([('internalType', 'contract "*

 * *             "Limiter'), ('name', '_limiter'), ('type', 'address')])]}, insert: [(2, "*

 * *             "OrderedDict([('inputs', [OrderedDict([('internalType', 'address'), ('name', "*

 * *             "'_token'), ('type', 'address')])]), ('name', 'have'), ('outputs', "*

 * *             "[OrderedDict([('internalType', 'bool'), ('name', ''), ( […]*

```diff
@@ -2,15 +2,26 @@
     "compiler": {
         "version": "0.8.19+commit.7dd6d404"
     },
     "language": "Solidity",
     "output": {
         "abi": [
             {
-                "inputs": [],
+                "inputs": [
+                    {
+                        "internalType": "address",
+                        "name": "_holder",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "contract Limiter",
+                        "name": "_limiter",
+                        "type": "address"
+                    }
+                ],
                 "stateMutability": "nonpayable",
                 "type": "constructor"
             },
             {
                 "anonymous": false,
                 "inputs": [
                     {
@@ -31,14 +42,33 @@
             },
             {
                 "inputs": [
                     {
                         "internalType": "address",
                         "name": "_token",
                         "type": "address"
+                    }
+                ],
+                "name": "have",
+                "outputs": [
+                    {
+                        "internalType": "bool",
+                        "name": "",
+                        "type": "bool"
+                    }
+                ],
+                "stateMutability": "view",
+                "type": "function"
+            },
+            {
+                "inputs": [
+                    {
+                        "internalType": "address",
+                        "name": "_token",
+                        "type": "address"
                     },
                     {
                         "internalType": "address",
                         "name": "_holder",
                         "type": "address"
                     }
                 ],
@@ -155,32 +185,32 @@
             "kind": "user",
             "methods": {},
             "version": 1
         }
     },
     "settings": {
         "compilationTarget": {
-            "Limiter.sol": "Limiter"
+            "LimiterIndex.sol": "LimiterTokenRegistry"
         },
         "evmVersion": "byzantium",
         "libraries": {},
         "metadata": {
             "bytecodeHash": "ipfs"
         },
         "optimizer": {
             "enabled": false,
             "runs": 200
         },
         "remappings": []
     },
     "sources": {
-        "Limiter.sol": {
-            "keccak256": "0x5d2efe5fb5477abcc3f9ae9cb2f89caa2138ae71308f74e7860fea85999fd7c5",
+        "LimiterIndex.sol": {
+            "keccak256": "0x9fd0c38e85af9b5c270c9fd05289279487a4d23b7df0a69d58d04cce7cc96b12",
             "license": "AGPL-3.0-or-later",
             "urls": [
-                "bzz-raw://3cc9ed399ceab3c64b147cafaa577351a943a442ab3d7fece036444c88d3800e",
-                "dweb:/ipfs/Qmd41uw2HGfXd1AvKGQAHsikjvopRPLidXBDQrx5zz6igT"
+                "bzz-raw://b1e085fc05ff9b23e74cbda4cee4f8c69153d9737601ae1735c443735e2bc1d4",
+                "dweb:/ipfs/QmbqZmpnped8P1NgiMcTX8tCH9foN1rNDBKSdWL2o9r8Hd"
             ]
         }
     },
     "version": 1
 }
```

### Comparing `erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.bin` & `erc20-limiter-0.0.3/erc20_limiter/data/Limiter.bin`

 * *Files 15% similar despite different names*

```diff
@@ -1 +1 @@
-608060405234801561001057600080fd5b506040516109673803806109678339818101604052810190610032919061015b565b81600160006101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550806000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550505061019b565b600080fd5b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006100ea826100bf565b9050919050565b6100fa816100df565b811461010557600080fd5b50565b600081519050610117816100f1565b92915050565b6000610128826100df565b9050919050565b6101388161011d565b811461014357600080fd5b50565b6000815190506101558161012f565b92915050565b60008060408385031215610172576101716100ba565b5b600061018085828601610108565b925050602061019185828601610146565b9150509250929050565b6107bd806101aa6000396000f3fe608060405234801561001057600080fd5b5060043610610074576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461007957806323778613146100a957806336db43b5146100d95780633ef25013146100f5578063bdd5544014610125575b600080fd5b610093600480360381019061008e91906104b5565b610141565b6040516100a091906104fd565b60405180910390f35b6100c360048036038101906100be9190610576565b6101f1565b6040516100d091906105cf565b60405180910390f35b6100f360048036038101906100ee9190610616565b6102b4565b005b61010f600480360381019061010a9190610656565b6102c3565b60405161011c91906104fd565b60405180910390f35b61013f600480360381019061013a9190610683565b6103a8565b005b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361019557600190506101ec565b63b7bca6257c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101e757600190506101ec565b600090505b919050565b60008060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16632377861384846040518363ffffffff167c010000000000000000000000000000000000000000000000000000000002815260040161026b9291906106e5565b602060405180830381865afa158015610288573d6000803e3d6000fd5b505050506040513d601f19601f820116820180604052508101906102ac9190610723565b905092915050565b6102bf8233836103a8565b5050565b60008060008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16632377861384600160009054906101000a900473ffffffffffffffffffffffffffffffffffffffff166040518363ffffffff167c010000000000000000000000000000000000000000000000000000000002815260040161035f9291906106e5565b602060405180830381865afa15801561037c573d6000803e3d6000fd5b505050506040513d601f19601f820116820180604052508101906103a09190610723565b119050919050565b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1663bdd554408484846040518463ffffffff167c010000000000000000000000000000000000000000000000000000000002815260040161042193929190610750565b600060405180830381600087803b15801561043b57600080fd5b505af115801561044f573d6000803e3d6000fd5b50505050505050565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b6104928161045d565b811461049d57600080fd5b50565b6000813590506104af81610489565b92915050565b6000602082840312156104cb576104ca610458565b5b60006104d9848285016104a0565b91505092915050565b60008115159050919050565b6104f7816104e2565b82525050565b600060208201905061051260008301846104ee565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b600061054382610518565b9050919050565b61055381610538565b811461055e57600080fd5b50565b6000813590506105708161054a565b92915050565b6000806040838503121561058d5761058c610458565b5b600061059b85828601610561565b92505060206105ac85828601610561565b9150509250929050565b6000819050919050565b6105c9816105b6565b82525050565b60006020820190506105e460008301846105c0565b92915050565b6105f3816105b6565b81146105fe57600080fd5b50565b600081359050610610816105ea565b92915050565b6000806040838503121561062d5761062c610458565b5b600061063b85828601610561565b925050602061064c85828601610601565b9150509250929050565b60006020828403121561066c5761066b610458565b5b600061067a84828501610561565b91505092915050565b60008060006060848603121561069c5761069b610458565b5b60006106aa86828701610561565b93505060206106bb86828701610561565b92505060406106cc86828701610601565b9150509250925092565b6106df81610538565b82525050565b60006040820190506106fa60008301856106d6565b61070760208301846106d6565b9392505050565b60008151905061071d816105ea565b92915050565b60006020828403121561073957610738610458565b5b60006107478482850161070e565b91505092915050565b600060608201905061076560008301866106d6565b61077260208301856106d6565b61077f60408301846105c0565b94935050505056fea264697066735822122059ed451c7493185b9c26a93c433ec67c46b6c713de36f371528416bd733499c964736f6c63430008130033
+608060405234801561001057600080fd5b50336000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550610a3a806100606000396000f3fe608060405234801561001057600080fd5b506004361061007f576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461008457806323778613146100b457806336db43b5146100e45780638da5cb5b14610100578063bdd554401461011e578063f2fde38b1461013a575b600080fd5b61009e600480360381019061009991906106d0565b61016a565b6040516100ab9190610718565b60405180910390f35b6100ce60048036038101906100c99190610791565b61026c565b6040516100db91906107ea565b60405180910390f35b6100fe60048036038101906100f99190610831565b6102f3565b005b610108610378565b6040516101159190610880565b60405180910390f35b6101386004803603810190610133919061089b565b61039c565b005b610154600480360381019061014f91906108ee565b610531565b6040516101619190610718565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101be5760019050610267565b639493f8b27c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036102105760019050610267565b63237786137c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036102625760019050610267565b600090505b919050565b6000600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002054905092915050565b80600160008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff168152602001908152602001600020819055505050565b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1681565b60008060009054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16148061042457508273ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16145b610463576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161045a90610978565b60405180910390fd5b823b9050600081116104aa576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016104a1906109e4565b60405180910390fd5b81600160008673ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020016000208190555050505050565b60008060008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff161461058c57600080fd5b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff169050826000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555060008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff168173ffffffffffffffffffffffffffffffffffffffff167f8be0079c531659141344cd1fd0a4f28419497f9722a3daafe3b4186f6b6457e060405160405180910390a36001915050919050565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b6106ad81610678565b81146106b857600080fd5b50565b6000813590506106ca816106a4565b92915050565b6000602082840312156106e6576106e5610673565b5b60006106f4848285016106bb565b91505092915050565b60008115159050919050565b610712816106fd565b82525050565b600060208201905061072d6000830184610709565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b600061075e82610733565b9050919050565b61076e81610753565b811461077957600080fd5b50565b60008135905061078b81610765565b92915050565b600080604083850312156107a8576107a7610673565b5b60006107b68582860161077c565b92505060206107c78582860161077c565b9150509250929050565b6000819050919050565b6107e4816107d1565b82525050565b60006020820190506107ff60008301846107db565b92915050565b61080e816107d1565b811461081957600080fd5b50565b60008135905061082b81610805565b92915050565b6000806040838503121561084857610847610673565b5b60006108568582860161077c565b92505060206108678582860161081c565b9150509250929050565b61087a81610753565b82525050565b60006020820190506108956000830184610871565b92915050565b6000806000606084860312156108b4576108b3610673565b5b60006108c28682870161077c565b93505060206108d38682870161077c565b92505060406108e48682870161081c565b9150509250925092565b60006020828403121561090457610903610673565b5b60006109128482850161077c565b91505092915050565b600082825260208201905092915050565b7f4552525f41585800000000000000000000000000000000000000000000000000600082015250565b600061096260078361091b565b915061096d8261092c565b602082019050919050565b6000602082019050818103600083015261099181610955565b9050919050565b7f4552525f4143434f554e54000000000000000000000000000000000000000000600082015250565b60006109ce600b8361091b565b91506109d982610998565b602082019050919050565b600060208201905081810360008301526109fd816109c1565b905091905056fea2646970667358221220bfbd3dc4c68c3de06c71999bd996ad177fed19a8220f8c83e606cc8291101fe264736f6c63430008130033
```

### Comparing `erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.json` & `erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.json`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.2/erc20_limiter/data/LimiterTokenRegistry.metadata.json` & `erc20-limiter-0.0.3/erc20_limiter/data/LimiterTokenRegistry.metadata.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'sources'": "{'LimiterTokenRegistry.sol': {'keccak256': "*

 * *              "'0x8bc7716c5a8b9d698a4f8571a89b4da77c790d5d17f6f5e0f83f31fe6faef649', 'urls': "*

 * *              "['bzz-raw://4135e14e8203ca39fc809c7505222686b61dee82362fd3eb0f295b61bb44182a', "*

 * *              "'dweb:/ipfs/Qmf5bCwu61UAK9atMghHbZJC88tfq2X43UDwq2nxeExDZR']}}"}*

```diff
@@ -149,17 +149,17 @@
             "enabled": false,
             "runs": 200
         },
         "remappings": []
     },
     "sources": {
         "LimiterTokenRegistry.sol": {
-            "keccak256": "0xca5fd95fd62ac8530df26ea912eadfcb2c2a00bbf3df9ffe497d7a5c50b84497",
+            "keccak256": "0x8bc7716c5a8b9d698a4f8571a89b4da77c790d5d17f6f5e0f83f31fe6faef649",
             "license": "AGPL-3.0-or-later",
             "urls": [
-                "bzz-raw://7d3e45e63f2e7fa721bd1f2c6a453926e5366bad8cfe3154323ee9d0f3476f5c",
-                "dweb:/ipfs/QmQDtyCrn7rf8LyxhrfxRd3K8CMuJuP1GL4YPyGAVETgtY"
+                "bzz-raw://4135e14e8203ca39fc809c7505222686b61dee82362fd3eb0f295b61bb44182a",
+                "dweb:/ipfs/Qmf5bCwu61UAK9atMghHbZJC88tfq2X43UDwq2nxeExDZR"
             ]
         }
     },
     "version": 1
 }
```

### Comparing `erc20-limiter-0.0.2/erc20_limiter/limiter.py` & `erc20-limiter-0.0.3/erc20_limiter/limiter.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.2/erc20_limiter/token.py` & `erc20-limiter-0.0.3/erc20_limiter/index.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 
 # local imports
 from erc20_limiter.data import data_dir
 
 logg = logging.getLogger()
 
 
-class LimiterTokenRegistry(TxFactory):
+class LimiterIndex(TxFactory):
 
     __abi = None
     __bytecode = None
 
     def constructor(self, sender_address, holder_address, limiter_address, tx_format=TxFormat.JSONRPC, version=None):
         code = self.cargs(holder_address, limiter_address, version=version)
         tx = self.template(sender_address, None, use_nonce=True)
         tx = self.set_code(tx, code)
         return self.finalize(tx, tx_format)
 
 
     @staticmethod
     def cargs(holder_address, limiter_address, version=None):
-        code = LimiterTokenRegistry.bytecode(version=version)
+        code = LimiterIndex.bytecode(version=version)
         enc = ABIContractEncoder()
         enc.address(holder_address)
         enc.address(limiter_address)
         args = enc.get()
         code += args
         logg.debug('constructor code: ' + args)
         return code
@@ -59,28 +59,28 @@
     @staticmethod
     def gas(code=None):
         return 4000000
 
 
     @staticmethod
     def abi():
-        if LimiterTokenRegistry.__abi == None:
-            f = open(os.path.join(data_dir, 'LimiterTokenRegistry.json'), 'r')
-            LimiterTokenRegistry.__abi = json.load(f)
+        if LimiterIndex.__abi == None:
+            f = open(os.path.join(data_dir, 'LimiterIndex.json'), 'r')
+            LimiterIndex.__abi = json.load(f)
             f.close()
-        return LimiterTokenRegistry.__abi
+        return LimiterIndex.__abi
 
 
     @staticmethod
     def bytecode(version=None):
-        if LimiterTokenRegistry.__bytecode == None:
-            f = open(os.path.join(data_dir, 'LimiterTokenRegistry.bin'))
-            LimiterTokenRegistry.__bytecode = f.read()
+        if LimiterIndex.__bytecode == None:
+            f = open(os.path.join(data_dir, 'LimiterIndex.bin'))
+            LimiterIndex.__bytecode = f.read()
             f.close()
-        return LimiterTokenRegistry.__bytecode
+        return LimiterIndex.__bytecode
 
 
     def have(self, contract_address, token_address, sender_address=ZERO_ADDRESS, id_generator=None):
         j = JSONRPCRequest(id_generator)
         o = j.template()
         o['method'] = 'eth_call'
         enc = ABIContractEncoder()
```

### Comparing `erc20-limiter-0.0.2/erc20_limiter/unittest/base.py` & `erc20-limiter-0.0.3/erc20_limiter/unittest/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from chainlib.eth.nonce import RPCNonceOracle
 from chainlib.eth.tx import receipt
 from chainlib.eth.address import to_checksum_address
 from chainlib.eth.block import block_latest
 
 # local imports
 from erc20_limiter import Limiter
-from erc20_limiter.token import LimiterTokenRegistry
+from erc20_limiter.index import LimiterIndex
 
 logg = logging.getLogger(__name__)
 
 class TestLimiter(EthTesterCase):
 
     def setUp(self):
         super(TestLimiter, self).setUp()
@@ -33,19 +33,19 @@
         r = self.rpc.do(o)
         self.assertEqual(r['status'], 1)
         address = to_checksum_address(r['contract_address'])
         logg.debug('published limiter on address {} with hash {}'.format(address, tx_hash))
         return address
 
 
-class TestLimiterTokenRegistry(TestLimiter):
+class TestLimiterIndex(TestLimiter):
 
     def publish_token_registry(self, holder_address, limiter_address):
         nonce_oracle = RPCNonceOracle(self.accounts[0], conn=self.conn)
-        c = LimiterTokenRegistry(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
+        c = LimiterIndex(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         (tx_hash, o) = c.constructor(self.accounts[0], holder_address, limiter_address)
         self.rpc.do(o)
         o = receipt(tx_hash)
         r = self.rpc.do(o)
         self.assertEqual(r['status'], 1)
         address = to_checksum_address(r['contract_address'])
         logg.debug('published limiter token registry proxy on address {} with hash {}'.format(address, tx_hash))
```

### Comparing `erc20-limiter-0.0.2/erc20_limiter.egg-info/PKG-INFO` & `erc20-limiter-0.0.3/erc20_limiter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erc20-limiter
-Version: 0.0.2
+Version: 0.0.3
 Summary: ERC20 balance limit registry
 Home-page: https://holbrook.no/src/erc20-limiter/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,8 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
+License-File: LICENSE
```

### Comparing `erc20-limiter-0.0.2/setup.cfg` & `erc20-limiter-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erc20-limiter
-version = 0.0.2
+version = 0.0.3
 description = ERC20 balance limit registry
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/erc20-limiter/log.html
 keywords = 
 	dlt
 	blockchain
```

### Comparing `erc20-limiter-0.0.2/tests/test_base.py` & `erc20-limiter-0.0.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `erc20-limiter-0.0.2/tests/test_token_registry.py` & `erc20-limiter-0.0.3/tests/test_index.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,47 +4,47 @@
 
 # external imports
 from chainlib.eth.nonce import RPCNonceOracle
 from chainlib.eth.tx import receipt
 
 # local imports
 from erc20_limiter import Limiter
-from erc20_limiter.token import LimiterTokenRegistry
-from erc20_limiter.unittest import TestLimiterTokenRegistry
+from erc20_limiter.index import LimiterIndex
+from erc20_limiter.unittest import TestLimiterIndex
 
 logging.basicConfig(level=logging.DEBUG)
 logg = logging.getLogger()
 
 
-class TestLimiterBase(TestLimiterTokenRegistry):
+class TestLimiterBase(TestLimiterIndex):
 
     def setUp(self):
         super(TestLimiterBase, self).setUp()
         self.publish_limiter()
         self.token_registry = self.publish_token_registry(self.accounts[0], self.address)
         logg.debug('tokenreg {}'.format(self.token_registry))
 
 
     def test_limit(self):
         nonce_oracle = RPCNonceOracle(self.accounts[0], conn=self.conn)
 
         foo_token = '2c26b46b68ffc68ff99b453c1d30413413422d70'
-        c = LimiterTokenRegistry(self.chain_spec)
+        c = LimiterIndex(self.chain_spec)
         o = c.have(self.token_registry, foo_token, sender_address=self.accounts[0])
         r = self.rpc.do(o)
         self.assertEqual(int(r, 16), 0)
 
         c = Limiter(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         (tx_hash, o) = c.set_limit(self.address, self.accounts[0], foo_token, 42)
         self.rpc.do(o)
         o = receipt(tx_hash)
         r = self.rpc.do(o)
         self.assertEqual(r['status'], 1)
 
-        c = LimiterTokenRegistry(self.chain_spec)
+        c = LimiterIndex(self.chain_spec)
         o = c.have(self.token_registry, foo_token, sender_address=self.accounts[0])
         r = self.rpc.do(o)
         self.assertEqual(int(r, 16), 1)
 
 
 if __name__ == '__main__':
     unittest.main()
```

