# Comparing `tmp/starknet_devnet-0.5.5a0.tar.gz` & `tmp/starknet_devnet-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starknet_devnet-0.5.5a0.tar", max compression
+gzip compressed data, was "starknet_devnet-0.6.0a0.tar", max compression
```

## Comparing `starknet_devnet-0.5.5a0.tar` & `starknet_devnet-0.6.0a0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-07-03 11:45:14.809619 starknet_devnet-0.5.5a0/LICENSE
--rw-r--r--   0        0        0     1054 2023-07-03 11:45:14.809619 starknet_devnet-0.5.5a0/README.md
--rw-r--r--   0        0        0     1822 2023-07-03 11:45:14.821619 starknet_devnet-0.5.5a0/pyproject.toml
--rw-r--r--   0        0        0   208485 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
--rw-r--r--   0        0        0    32739 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/MockStarknetMessaging.json
--rw-r--r--   0        0        0    35645 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/UDC_OZ_0.5.0.json
--rw-r--r--   0        0        0     2960 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/__init__.py
--rw-r--r--   0        0        0     2779 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/account.py
--rw-r--r--   0        0        0     4161 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/account_util.py
--rw-r--r--   0        0        0     2511 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/accounts.py
--rw-r--r--   0        0        0   118818 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
--rw-r--r--   0        0        0     1784 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
--rw-r--r--   0        0        0     1866 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/block_info_generator.py
--rw-r--r--   0        0        0    12483 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blocks.py
--rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/__init__.py
--rw-r--r--   0        0        0     7585 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/base.py
--rw-r--r--   0        0        0    14072 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/feeder_gateway.py
--rw-r--r--   0        0        0     2256 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/gateway.py
--rw-r--r--   0        0        0     3959 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/postman.py
--rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/__init__.py
--rw-r--r--   0        0        0     2138 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/blocks.py
--rw-r--r--   0        0        0     2120 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/call.py
--rw-r--r--   0        0        0     2195 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/classes.py
--rw-r--r--   0        0        0     6257 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/misc.py
--rw-r--r--   0        0        0     4953 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/routes.py
--rw-r--r--   0        0        0   116673 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec.py
--rw-r--r--   0        0        0     6049 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec_write.py
--rw-r--r--   0        0        0    16310 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_trace_spec.py
--rw-r--r--   0        0        0     7135 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/schema.py
--rw-r--r--   0        0        0     1144 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/state.py
--rw-r--r--   0        0        0      929 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/storage.py
--rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/__init__.py
--rw-r--r--   0        0        0    32879 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/payloads.py
--rw-r--r--   0        0        0     6494 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/responses.py
--rw-r--r--   0        0        0     3457 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/types.py
--rw-r--r--   0        0        0     8789 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/transactions.py
--rw-r--r--   0        0        0     3542 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/utils.py
--rw-r--r--   0        0        0      899 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/shared.py
--rw-r--r--   0        0        0    24763 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/cairo_rs_py_patch.py
--rw-r--r--   0        0        0     1038 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/chargeable_account.py
--rw-r--r--   0        0        0     5310 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/compiler.py
--rw-r--r--   0        0        0     1239 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/constants.py
--rw-r--r--   0        0        0      646 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/contract_class_wrapper.py
--rw-r--r--   0        0        0    16332 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/devnet_config.py
--rw-r--r--   0        0        0      784 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/dump.py
--rw-r--r--   0        0        0     6558 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/fee_token.py
--rw-r--r--   0        0        0     8332 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/forked_state.py
--rw-r--r--   0        0        0     1640 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/general_config.py
--rw-r--r--   0        0        0     9005 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/origin.py
--rw-r--r--   0        0        0    10015 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/postman_wrapper.py
--rw-r--r--   0        0        0     2237 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/predeployed_contract_wrapper.py
--rw-r--r--   0        0        0     4353 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/server.py
--rw-r--r--   0        0        0    41451 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/starknet_wrapper.py
--rw-r--r--   0        0        0     1988 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/state.py
--rw-r--r--   0        0        0     2573 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/state_archive.py
--rw-r--r--   0        0        0    11947 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/transactions.py
--rw-r--r--   0        0        0     1822 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/udc.py
--rw-r--r--   0        0        0    11174 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/util.py
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 starknet_devnet-0.5.5a0/setup.py
--rw-r--r--   0        0        0     2193 1970-01-01 00:00:00.000000 starknet_devnet-0.5.5a0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-03 16:41:27.547742 starknet_devnet-0.6.0a0/LICENSE
+-rw-r--r--   0        0        0     1054 2023-08-03 16:41:27.547742 starknet_devnet-0.6.0a0/README.md
+-rw-r--r--   0        0        0     1840 2023-08-03 16:41:27.555743 starknet_devnet-0.6.0a0/pyproject.toml
+-rw-r--r--   0        0        0   208485 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
+-rw-r--r--   0        0        0    32739 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/MockStarknetMessaging.json
+-rw-r--r--   0        0        0    35645 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/UDC_OZ_0.5.0.json
+-rw-r--r--   0        0        0     2960 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/__init__.py
+-rw-r--r--   0        0        0     2779 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/account.py
+-rw-r--r--   0        0        0     4161 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/account_util.py
+-rw-r--r--   0        0        0     2511 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/accounts.py
+-rw-r--r--   0        0        0   118818 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
+-rw-r--r--   0        0        0     1784 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
+-rw-r--r--   0        0        0     1866 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/block_info_generator.py
+-rw-r--r--   0        0        0    12483 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/blocks.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/__init__.py
+-rw-r--r--   0        0        0     7585 2023-08-03 16:41:27.559743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/base.py
+-rw-r--r--   0        0        0    14072 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/feeder_gateway.py
+-rw-r--r--   0        0        0     2256 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/gateway.py
+-rw-r--r--   0        0        0     3959 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/postman.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/__init__.py
+-rw-r--r--   0        0        0     2138 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/blocks.py
+-rw-r--r--   0        0        0     2120 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/call.py
+-rw-r--r--   0        0        0     2195 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/classes.py
+-rw-r--r--   0        0        0     6257 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/misc.py
+-rw-r--r--   0        0        0     4953 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/routes.py
+-rw-r--r--   0        0        0   116673 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/rpc_spec.py
+-rw-r--r--   0        0        0     6049 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/rpc_spec_write.py
+-rw-r--r--   0        0        0    16310 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/rpc_trace_spec.py
+-rw-r--r--   0        0        0     7135 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/schema.py
+-rw-r--r--   0        0        0     1144 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/state.py
+-rw-r--r--   0        0        0      929 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/storage.py
+-rw-r--r--   0        0        0        0 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/structures/__init__.py
+-rw-r--r--   0        0        0    32879 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/structures/payloads.py
+-rw-r--r--   0        0        0     6494 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/structures/responses.py
+-rw-r--r--   0        0        0     3457 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/structures/types.py
+-rw-r--r--   0        0        0     8947 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/transactions.py
+-rw-r--r--   0        0        0     3542 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/utils.py
+-rw-r--r--   0        0        0      899 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/blueprints/shared.py
+-rw-r--r--   0        0        0    24763 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/cairo_rs_py_patch.py
+-rw-r--r--   0        0        0     1038 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/chargeable_account.py
+-rw-r--r--   0        0        0     5310 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/compiler.py
+-rw-r--r--   0        0        0     1250 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/constants.py
+-rw-r--r--   0        0        0      646 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/contract_class_wrapper.py
+-rw-r--r--   0        0        0    16332 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/devnet_config.py
+-rw-r--r--   0        0        0      784 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/dump.py
+-rw-r--r--   0        0        0     6558 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/fee_token.py
+-rw-r--r--   0        0        0     8332 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/forked_state.py
+-rw-r--r--   0        0        0     1680 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/general_config.py
+-rw-r--r--   0        0        0     9280 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/origin.py
+-rw-r--r--   0        0        0    10015 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/postman_wrapper.py
+-rw-r--r--   0        0        0     2237 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/predeployed_contract_wrapper.py
+-rw-r--r--   0        0        0     4353 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/server.py
+-rw-r--r--   0        0        0    41402 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/starknet_wrapper.py
+-rw-r--r--   0        0        0     1988 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/state.py
+-rw-r--r--   0        0        0     2573 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/state_archive.py
+-rw-r--r--   0        0        0    13028 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/transactions.py
+-rw-r--r--   0        0        0     1822 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/udc.py
+-rw-r--r--   0        0        0    11174 2023-08-03 16:41:27.563743 starknet_devnet-0.6.0a0/starknet_devnet/util.py
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 starknet_devnet-0.6.0a0/setup.py
+-rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 starknet_devnet-0.6.0a0/PKG-INFO
```

### Comparing `starknet_devnet-0.5.5a0/LICENSE` & `starknet_devnet-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/README.md` & `starknet_devnet-0.6.0a0/README.md`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/pyproject.toml` & `starknet_devnet-0.6.0a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "starknet_devnet"
-version = "0.5.5a0"
+version = "0.6.0a0"
 description = "A local testnet for Starknet"
 authors = ["FabijanC <fabijan.corak@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/0xSpaceShard/starknet-devnet"
 homepage = "https://github.com/0xSpaceShard/starknet-devnet"
 keywords = ["starknet", "cairo", "testnet", "local", "server"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
 Flask = {extras = ["async"], version = "~2.0.3"}
 flask-cors = "~3.0.10"
-cairo-lang = "0.12.0a0"
+cairo-lang = "0.12.1a0"
 Werkzeug = "~2.0.3"
 cloudpickle = "~2.1.0"
 crypto-cpp-py = "~1.4.0"
 marshmallow = "~3.17.0"
 typing-extensions = "~4.3.0"
 gunicorn = "~20.1.0"
 marshmallow-dataclass = "~8.4"
 jsonschema = "~4.17.0"
 web3 = "~6.0.0"
 poseidon-py = "~0.1.3"
+pyyaml = "~6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "~2.12.2"
 psutil = "~5.9.1"
 pytest-xdist = "~2.5.0"
 pylint-quotes = "~0.2.3"
 black = "~22.6"
```

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json` & `starknet_devnet-0.6.0a0/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/MockStarknetMessaging.json` & `starknet_devnet-0.6.0a0/starknet_devnet/MockStarknetMessaging.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/UDC_OZ_0.5.0.json` & `starknet_devnet-0.6.0a0/starknet_devnet/UDC_OZ_0.5.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/__init__.py` & `starknet_devnet-0.6.0a0/starknet_devnet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # pylint: disable=unused-import
 # pylint: disable=import-outside-toplevel
 
 import os
 import sys
 
-__version__ = "0.5.5a0"
+__version__ = "0.6.0a0"
 
 
 def _patch_pedersen_hash():
     """
     Improves performance by substituting the default Python implementation of Pedersen hash
     with Software Mansion's Python wrapper of C++ implementation.
     """
```

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/account.py` & `starknet_devnet-0.6.0a0/starknet_devnet/account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/account_util.py` & `starknet_devnet-0.6.0a0/starknet_devnet/account_util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/accounts.py` & `starknet_devnet-0.6.0a0/starknet_devnet/accounts.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json` & `starknet_devnet-0.6.0a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json` & `starknet_devnet-0.6.0a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/block_info_generator.py` & `starknet_devnet-0.6.0a0/starknet_devnet/block_info_generator.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blocks.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/base.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/feeder_gateway.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/feeder_gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/gateway.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/postman.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/postman.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/blocks.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/call.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/call.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/classes.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/classes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/misc.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/misc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/routes.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/routes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/rpc_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec_write.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/rpc_spec_write.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_trace_spec.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/rpc_trace_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/schema.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/schema.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/state.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/storage.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/storage.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/payloads.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/structures/payloads.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/responses.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/structures/responses.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/types.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/structures/types.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/transactions.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/transactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -129,20 +129,21 @@
     class_hash, transaction_hash = await state.starknet_wrapper.declare(
         external_tx=make_declare(declare_transaction)
     )
     status_response = await state.starknet_wrapper.transactions.get_transaction_status(
         hex(transaction_hash)
     )
 
-    if status_response["tx_status"] == "REJECTED":
-        error_message = status_response["tx_failure_reason"].error_message
-        if (
-            "Class with hash" in error_message
-            and "is already declared" in error_message
-        ):
+    assert (
+        status_response["tx_status"] != "REJECTED"
+    ), f"Invalid status response: {status_response}"
+
+    if status_response["tx_status"] == "REVERTED":
+        revert_reason = status_response["tx_revert_reason"]
+        if "is already declared" in revert_reason:
             raise RpcError.from_spec_name("CLASS_ALREADY_DECLARED")
 
     return RpcDeclareTransactionResult(
         transaction_hash=rpc_felt(transaction_hash),
         class_hash=rpc_felt(class_hash),
     )
 
@@ -158,19 +159,23 @@
     contract_address, transaction_hash = await state.starknet_wrapper.deploy_account(
         external_tx=make_deploy_account(deploy_account_transaction)
     )
 
     status_response = await state.starknet_wrapper.transactions.get_transaction_status(
         hex(transaction_hash)
     )
-    if (
-        status_response["tx_status"] == "REJECTED"
-        and "is not declared" in status_response["tx_failure_reason"].error_message
-    ):
-        raise RpcError.from_spec_name("CLASS_HASH_NOT_FOUND")
+
+    assert (
+        status_response["tx_status"] != "REJECTED"
+    ), f"Invalid status response: {status_response}"
+
+    if status_response["tx_status"] == "REVERTED":
+        revert_reason = status_response["tx_revert_reason"]
+        if "is not declared" in revert_reason:
+            raise RpcError.from_spec_name("CLASS_HASH_NOT_FOUND")
 
     return RpcDeployAccountTransactionResult(
         transaction_hash=rpc_felt(transaction_hash),
         contract_address=rpc_felt(contract_address),
     )
```

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/utils.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/shared.py` & `starknet_devnet-0.6.0a0/starknet_devnet/blueprints/shared.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/cairo_rs_py_patch.py` & `starknet_devnet-0.6.0a0/starknet_devnet/cairo_rs_py_patch.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/chargeable_account.py` & `starknet_devnet-0.6.0a0/starknet_devnet/chargeable_account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/compiler.py` & `starknet_devnet-0.6.0a0/starknet_devnet/compiler.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/constants.py` & `starknet_devnet-0.6.0a0/starknet_devnet/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 DUMMY_PENDING_BLOCK_HASH = 0
 
 DEFAULT_TIMEOUT = 60  # seconds
 
 OLD_SUPPORTED_VERSIONS = [0]
 
 # account used by Starknet CLI; calculated using
-# poetry run python scripts/compute_compiled_class_hash.py \
+# poetry run python scripts/compute_deprecated_compiled_class_hash.py \
 #   ~/.cache/pypoetry/virtualenvs/<YOUR_VENV>/lib/python3.9/site-packages/starkware/starknet/third_party/open_zeppelin/account.json
 STARKNET_CLI_ACCOUNT_CLASS_HASH = (
-    0x2AF01407D426B1FFF03A6982813EA9F3E9467B2B19EDCC9FB612C3B5B6FFCEB
+    0x495B30BEA9715F5BD596989103C4D609917FD343B935163D58F29EDB12E2472
 )
 
 # starkware.starknet.public.abi.get_selector_from_name("replace_class")
 REPLACE_CLASS_SELECTOR = (
     0x217DF192877EED2921E241046523F8D8DA7981F0A3DDAFE0E7517F6523276D2
 )
```

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/contract_class_wrapper.py` & `starknet_devnet-0.6.0a0/starknet_devnet/contract_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/devnet_config.py` & `starknet_devnet-0.6.0a0/starknet_devnet/devnet_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/dump.py` & `starknet_devnet-0.6.0a0/starknet_devnet/dump.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/fee_token.py` & `starknet_devnet-0.6.0a0/starknet_devnet/fee_token.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/forked_state.py` & `starknet_devnet-0.6.0a0/starknet_devnet/forked_state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/general_config.py` & `starknet_devnet-0.6.0a0/starknet_devnet/general_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             "compiled_class_hash_commitment_tree_height": constants.COMPILED_CLASS_HASH_COMMITMENT_TREE_HEIGHT,
             "contract_storage_commitment_tree_height": constants.CONTRACT_STATES_COMMITMENT_TREE_HEIGHT,
             "enforce_l1_handler_fee": True,
             "event_commitment_tree_height": constants.EVENT_COMMITMENT_TREE_HEIGHT,
             "global_state_commitment_tree_height": constants.CONTRACT_ADDRESS_BITS,
             "invoke_tx_max_n_steps": DEFAULT_MAX_STEPS,
             "min_gas_price": DEFAULT_GAS_PRICE,
+            "constant_gas_price": True,
             "sequencer_address": hex(DEFAULT_SEQUENCER_ADDRESS),
             "starknet_os_config": {
                 "chain_id": chain_id.value,
                 "fee_token_address": hex(FeeToken.ADDRESS),
             },
             "tx_commitment_tree_height": constants.TRANSACTION_COMMITMENT_TREE_HEIGHT,
             "validate_max_n_steps": DEFAULT_VALIDATE_MAX_STEPS,
```

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/origin.py` & `starknet_devnet-0.6.0a0/starknet_devnet/origin.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from services.external_api.client import BadRequest
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
 from starkware.starknet.services.api.feeder_gateway.feeder_gateway_client import (
     FeederGatewayClient,
 )
 from starkware.starknet.services.api.feeder_gateway.response_objects import (
+    FinalityStatus,
     StarknetBlock,
     TransactionInfo,
     TransactionReceipt,
     TransactionStatus,
     TransactionTrace,
 )
 
@@ -76,35 +77,42 @@
 
 class NullOrigin(Origin):
     """
     A default class to comply with the Origin interface.
     """
 
     async def get_transaction_status(self, transaction_hash: str):
-        return {"tx_status": TransactionStatus.NOT_RECEIVED.name}
+        return {
+            "tx_status": TransactionStatus.NOT_RECEIVED.name,
+            "finality_status": FinalityStatus.NOT_RECEIVED.name,
+            "execution_status": None,
+        }
 
     async def get_transaction(self, transaction_hash: str) -> TransactionInfo:
         return TransactionInfo.create(
-            status=TransactionStatus.NOT_RECEIVED,
+            finality_status=FinalityStatus.NOT_RECEIVED,
         )
 
     async def get_transaction_receipt(
         self, transaction_hash: str
     ) -> TransactionReceipt:
         return TransactionReceipt(
             status=TransactionStatus.NOT_RECEIVED,
+            finality_status=FinalityStatus.NOT_RECEIVED,
+            execution_status=None,
             transaction_hash=0,  # testnet returns 0 instead of received hash
             events=[],
             l2_to_l1_messages=[],
             block_hash=None,
             block_number=None,
             transaction_index=None,
             execution_resources=None,
             actual_fee=None,
             transaction_failure_reason=None,
+            revert_error=None,
             l1_to_l2_consumed_message=None,
         )
 
     async def get_transaction_trace(self, transaction_hash: str):
         tx_hash_int = int(transaction_hash, 16)
         message = f"Transaction corresponding to hash {tx_hash_int} is not found."
         raise StarknetDevnetException(
```

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/postman_wrapper.py` & `starknet_devnet-0.6.0a0/starknet_devnet/postman_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/predeployed_contract_wrapper.py` & `starknet_devnet-0.6.0a0/starknet_devnet/predeployed_contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/server.py` & `starknet_devnet-0.6.0a0/starknet_devnet/server.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/starknet_wrapper.py` & `starknet_devnet-0.6.0a0/starknet_devnet/starknet_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 )
 from starkware.starknet.services.api.feeder_gateway.response_objects import (
     LATEST_BLOCK_ID,
     PENDING_BLOCK_ID,
     BlockStateUpdate,
     ClassHashPair,
     ContractAddressHashPair,
+    ExecutionStatus,
+    FinalityStatus,
     StarknetBlock,
     StateDiff,
     StorageEntry,
     TransactionStatus,
     TransactionTrace,
 )
 from starkware.starknet.services.api.gateway.transaction import (
@@ -336,26 +338,14 @@
         return BlockStateUpdate(
             block_hash=DUMMY_PENDING_BLOCK_HASH,
             new_root=DUMMY_STATE_ROOT,
             old_root=DUMMY_STATE_ROOT,
             state_diff=state_diff,
         )
 
-    def _store_transaction(
-        self,
-        transaction: DevnetTransaction,
-        error_message: str = None,
-    ) -> StarknetBlock:
-        """Stores the provided transaction in the transaction storage."""
-        if transaction.status == TransactionStatus.REJECTED:
-            assert error_message, "error_message must be present if tx rejected"
-            transaction.set_failure_reason(error_message)
-
-        self.transactions.store(transaction.transaction_hash, transaction)
-
     async def declare(
         self, external_tx: Union[Declare, DeprecatedDeclare]
     ) -> Tuple[int, int]:
         """
         Declares the class specified with `declare_transaction`
         Returns (class_hash, transaction_hash)
         """
@@ -466,35 +456,35 @@
                 tx_hash = self.internal_tx.hash_value
 
                 if exc_type:
                     if not isinstance(exc, StarkException):
                         raise StarknetDevnetException(
                             code=StarknetErrorCode.UNEXPECTED_FAILURE, message=str(exc)
                         ) from exc
-                    status = TransactionStatus.REJECTED
 
                     # restore block info
                     self.starknet_wrapper.get_state().state.block_info = (
                         self.preserved_block_info
                     )
 
                     transaction = DevnetTransaction(
                         internal_tx=self.internal_tx,
-                        status=status,
+                        status=TransactionStatus.REVERTED,
+                        execution_status=ExecutionStatus.REVERTED,
+                        finality_status=FinalityStatus.ACCEPTED_ON_L2,
                         execution_info=TransactionExecutionInfo.empty(),
                         transaction_hash=tx_hash,
-                        block_number=None,  # Rejected txs have no block number
-                        transaction_index=None,  # Rejected txs have no tx index
+                        block_number=0,  # Rejected txs have no block number
+                        transaction_index=0,  # Rejected txs have no tx index
+                        revert_error=exc.message,
                     )
-                    self.starknet_wrapper._store_transaction(
-                        transaction, error_message=exc.message
+                    self.starknet_wrapper.transactions.store(
+                        transaction.transaction_hash, transaction
                     )
                 else:
-                    status = TransactionStatus.ACCEPTED_ON_L2
-
                     assert self.execution_info is not None
                     if self.execution_info.call_info:
                         await self.starknet_wrapper._register_new_contracts(
                             self.internal_calls,
                             tx_hash,
                             self.deployed_contracts,
                         )
@@ -508,22 +498,26 @@
 
                     next_block_number = (
                         self.starknet_wrapper.blocks.get_next_block_number()
                     )
 
                     transaction = DevnetTransaction(
                         internal_tx=self.internal_tx,
-                        status=status,
+                        status=TransactionStatus.ACCEPTED_ON_L2,
+                        execution_status=ExecutionStatus.SUCCEEDED,
+                        finality_status=FinalityStatus.ACCEPTED_ON_L2,
                         execution_info=self.execution_info,
                         transaction_hash=tx_hash,
                         block_number=next_block_number,
                         transaction_index=len(self.starknet_wrapper.pending_txs),
                     )
                     self.starknet_wrapper.pending_txs.append(transaction)
-                    self.starknet_wrapper._store_transaction(transaction)
+                    self.starknet_wrapper.transactions.store(
+                        transaction.transaction_hash, transaction
+                    )
 
                     await self.starknet_wrapper.update_pending_block(state_update)
 
                     if not self.starknet_wrapper.config.blocks_on_demand:
                         await self.starknet_wrapper.generate_latest_block()
 
                 logger.info(
@@ -907,14 +901,15 @@
                 function_invocation=FunctionInvocation.from_optional_internal(
                     execution_info.call_info
                 ),
                 fee_transfer_invocation=FunctionInvocation.from_optional_internal(
                     execution_info.fee_transfer_info
                 ),
                 signature=external_tx.signature,
+                revert_error=execution_info.revert_error,
             )
             traces.append(trace)
 
             fee_estimation_info = get_fee_estimation_info(
                 execution_info.actual_fee, state.state.block_info.gas_price
             )
             fee_estimation_infos.append(fee_estimation_info)
@@ -1033,17 +1028,17 @@
             )
 
             # Abort latest_block.
             aborted_block_hash = await self.blocks.abort_latest_block(
                 hex(last_block.block_hash)
             )
 
-            # Reject transactions.
+            # Revert transactions.
             for transaction in last_block.transactions:
-                await self.transactions.reject_transaction(
+                await self.transactions.revert_transaction_in_aborted_block(
                     tx_hash=transaction.transaction_hash
                 )
 
             aborted_blocks.append(hex(aborted_block_hash))
             parent = await self.blocks.get_by_hash(hex(last_block.parent_block_hash))
 
             if parent.block_number is not None:
```

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/state.py` & `starknet_devnet-0.6.0a0/starknet_devnet/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/state_archive.py` & `starknet_devnet-0.6.0a0/starknet_devnet/state_archive.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/transactions.py` & `starknet_devnet-0.6.0a0/starknet_devnet/transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     InternalDeploy,
     InternalTransaction,
 )
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
 from starkware.starknet.definitions.transaction_type import TransactionType
 from starkware.starknet.services.api.feeder_gateway.response_objects import (
     Event,
+    ExecutionStatus,
+    FinalityStatus,
     FunctionInvocation,
     L2ToL1Message,
     StarknetBlock,
     TransactionExecution,
     TransactionInfo,
     TransactionReceipt,
     TransactionStatus,
@@ -40,35 +42,44 @@
     """Represents the devnet transaction"""
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         internal_tx: InternalTransaction,
         status: TransactionStatus,
+        execution_status: Optional[ExecutionStatus],
+        finality_status: FinalityStatus,
         execution_info: TransactionExecutionInfo,
         block_number: Optional[int],
         transaction_index: Optional[int],
         transaction_hash: Optional[int] = None,
+        revert_error: Optional[str] = None,
     ):
         self.block: Optional[StarknetBlock] = None
         self.execution_info = execution_info
-        if status != TransactionStatus.REJECTED and execution_info.call_info:
-            self.execution_resources = execution_info.call_info.execution_resources
-        else:
-            self.execution_resources = None
+        self.execution_resources = None
         self.internal_tx = internal_tx
         self.status = status
+        self.execution_status = execution_status
+        self.finality_status = finality_status
         self.transaction_failure_reason = None
         self.transaction_index = transaction_index
         self.__block_number = block_number
         self.transaction_hash = transaction_hash
+        self.revert_error = revert_error
 
         if transaction_hash is None:
             self.transaction_hash = internal_tx.hash_value
 
+        if (
+            status not in [TransactionStatus.REJECTED, TransactionStatus.REVERTED]
+            and execution_info.call_info
+        ):
+            self.execution_resources = execution_info.call_info.execution_resources
+
     def __get_actual_fee(self) -> int:
         """Returns the actual fee"""
         return (
             self.execution_info.actual_fee
             if hasattr(self.execution_info, "actual_fee")
             else 0
         )
@@ -121,20 +132,22 @@
         return (
             self.internal_tx.signature if hasattr(self.internal_tx, "signature") else []
         )
 
     def get_tx_info(self) -> TransactionInfo:
         """Returns the transaction info"""
         return TransactionInfo.create(
-            status=self.status,
+            finality_status=self.finality_status,
+            execution_status=self.execution_status,
             transaction=self.internal_tx,
             transaction_index=self.transaction_index,
             block_hash=self.__get_block_hash(),
             block_number=self.__block_number,
             transaction_failure_reason=self.transaction_failure_reason,
+            revert_error=self.revert_error,
         )
 
     def get_receipt(self) -> TransactionReceipt:
         """Returns the transaction receipt"""
         tx_info = self.get_tx_info()
 
         return TransactionReceipt.from_tx_info(
@@ -165,26 +178,29 @@
         )
 
         return TransactionTrace(
             validate_invocation=validate_invocation,
             function_invocation=function_invocation,
             fee_transfer_invocation=fee_transfer_invocation,
             signature=self.get_signature(),
+            revert_error=self.revert_error,
         )
 
     def get_execution(self) -> TransactionExecution:
         """Returns the transaction execution"""
         return TransactionExecution(
+            execution_status=self.execution_status,
             transaction_hash=self.internal_tx.hash_value,
             transaction_index=self.transaction_index,
             actual_fee=self.__get_actual_fee(),
             events=self.__get_events(),
             execution_resources=self.execution_resources,
             l2_to_l1_messages=self.__get_l2_to_l1_messages(),
             l1_to_l2_consumed_message=None,
+            revert_error=self.revert_error,
         )
 
 
 class DevnetTransactions:
     """
     This class is used to store transactions.
     """
@@ -236,15 +252,18 @@
         Get a transaction trace.
         """
         transaction = self.__get_transaction_by_hash(tx_hash)
 
         if transaction is None:
             return await self.origin.get_transaction_trace(tx_hash)
 
-        if transaction.status == TransactionStatus.REJECTED:
+        if transaction.status in [
+            TransactionStatus.REJECTED,
+            TransactionStatus.REVERTED,
+        ]:
             raise StarknetDevnetException(
                 code=StarknetErrorCode.NO_TRACE,
                 message=f"Transaction corresponding to hash {int(tx_hash, 16)} has no trace; status: {transaction.status.name}.",
             )
 
         return transaction.get_trace()
 
@@ -268,39 +287,42 @@
         if transaction is None:
             return await self.origin.get_transaction_status(tx_hash)
 
         tx_info = transaction.get_tx_info()
 
         status_response = {
             "tx_status": tx_info.status.name,
+            "finality_status": tx_info.finality_status.name,
+            "execution_status": tx_info.execution_status.name
+            if tx_info.execution_status
+            else None,
         }
 
         # "block_hash" will only exist after transaction enters ACCEPTED_ON_L2
-        if (
-            transaction.status == TransactionStatus.ACCEPTED_ON_L2
-            and transaction.block is not None
-        ):
+        if transaction.status == FinalityStatus.ACCEPTED_ON_L2:
+            assert transaction.block is not None
             status_response["block_hash"] = hex(transaction.block.block_hash)
 
-        # "tx_failure_reason" will only exist if the transaction was rejected.
-        if transaction.status == TransactionStatus.REJECTED:
+        if transaction.status == ExecutionStatus.REJECTED:
             status_response["tx_failure_reason"] = tx_info.transaction_failure_reason
 
+        elif tx_info.execution_status is ExecutionStatus.REVERTED:
+            status_response["tx_revert_reason"] = tx_info.revert_error
+
         return status_response
 
-    async def reject_transaction(self, tx_hash: int):
+    async def revert_transaction_in_aborted_block(self, tx_hash: int):
         """
-        Reject transaction in aborted block.
+        Revert transaction in aborted block.
         """
-        self.__instances[tx_hash].status = TransactionStatus.REJECTED
+        self.__instances[tx_hash].status = TransactionStatus.REVERTED
+        self.__instances[tx_hash].finality_status = FinalityStatus.ACCEPTED_ON_L2
+        self.__instances[tx_hash].execution_status = ExecutionStatus.REVERTED
         self.__instances[tx_hash].block = None
-        self.__instances[tx_hash].transaction_failure_reason = TransactionFailureReason(
-            code=StarknetErrorCode.TRANSACTION_FAILED.name,
-            error_message="Block aborted.",
-        )
+        self.__instances[tx_hash].revert_error = "Block aborted"
 
 
 def create_empty_internal_declare(tx_hash: int, class_hash: int) -> InternalDeclare:
     "Create InternalDeclare used in the genesis block"
     return InternalDeclare(
         hash_value=tx_hash,
         version=0,
@@ -342,16 +364,19 @@
         actual_resources={
             "l1_gas_usage": 0,
             "pedersen_builtin": 0,
             "range_check_builtin": 0,
             "n_steps": 0,
         },
         tx_type=tx_type,
+        revert_error=None,
     )
     return DevnetTransaction(
         internal_tx=internal_tx,
         status=TransactionStatus.ACCEPTED_ON_L2,
+        finality_status=FinalityStatus.ACCEPTED_ON_L2,
+        execution_status=ExecutionStatus.SUCCEEDED,
         execution_info=execution_info,
         block_number=block_number,
         transaction_index=transaction_index,
         transaction_hash=internal_tx.hash_value,
     )
```

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/udc.py` & `starknet_devnet-0.6.0a0/starknet_devnet/udc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/starknet_devnet/util.py` & `starknet_devnet-0.6.0a0/starknet_devnet/util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5a0/setup.py` & `starknet_devnet-0.6.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 package_data = \
 {'': ['*'],
  'starknet_devnet': ['accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/*']}
 
 install_requires = \
 ['Flask[async]>=2.0.3,<2.1.0',
  'Werkzeug>=2.0.3,<2.1.0',
- 'cairo-lang==0.12.0a0',
+ 'cairo-lang==0.12.1a0',
  'cloudpickle>=2.1.0,<2.2.0',
  'crypto-cpp-py>=1.4.0,<1.5.0',
  'flask-cors>=3.0.10,<3.1.0',
  'gunicorn>=20.1.0,<20.2.0',
  'jsonschema>=4.17.0,<4.18.0',
  'marshmallow-dataclass>=8.4,<8.5',
  'marshmallow>=3.17.0,<3.18.0',
  'poseidon-py>=0.1.3,<0.2.0',
+ 'pyyaml>=6.0.1,<6.1.0',
  'typing-extensions>=4.3.0,<4.4.0',
  'web3>=6.0.0,<6.1.0']
 
 entry_points = \
 {'console_scripts': ['starknet-devnet = starknet_devnet.server:main']}
 
 setup_kwargs = {
     'name': 'starknet-devnet',
-    'version': '0.5.5a0',
+    'version': '0.6.0a0',
     'description': 'A local testnet for Starknet',
     'long_description': '<!-- logo / title -->\n<p align="center" style="margin-bottom: 0px !important">\n  <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">\n</p>\n<h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>\n\nA Flask wrapper of Starknet state. Similar in purpose to Ganache.\n\nAims to mimic Starknet\'s Alpha testnet, but with simplified functionality.\n\n## 🌐 Docs\n\nOn the following links you can find the documentation of:\n\n- [the latest official release](https://0xspaceshard.github.io/starknet-devnet/)\n- [the latest master commit (not officially released)](https://github.com/0xSpaceShard/starknet-devnet/tree/master/page/docs)\n\n## ✏️ Contributing\n\nWe ❤️ and encourage all contributions!\n\n[Click here](https://0xspaceshard.github.io/starknet-devnet/docs/guide/development) for the development guide.\n\n## 🙌 Special Thanks\n\nSpecial thanks to all the [contributors](https://github.com/0xSpaceShard/starknet-devnet/graphs/contributors)!\n',
     'author': 'FabijanC',
     'author_email': 'fabijan.corak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xSpaceShard/starknet-devnet',
```

### Comparing `starknet_devnet-0.5.5a0/PKG-INFO` & `starknet_devnet-0.6.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: starknet-devnet
-Version: 0.5.5a0
+Version: 0.6.0a0
 Summary: A local testnet for Starknet
 Home-page: https://github.com/0xSpaceShard/starknet-devnet
 License: MIT
 Keywords: starknet,cairo,testnet,local,server
 Author: FabijanC
 Author-email: fabijan.corak@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask[async] (>=2.0.3,<2.1.0)
 Requires-Dist: Werkzeug (>=2.0.3,<2.1.0)
-Requires-Dist: cairo-lang (==0.12.0a0)
+Requires-Dist: cairo-lang (==0.12.1a0)
 Requires-Dist: cloudpickle (>=2.1.0,<2.2.0)
 Requires-Dist: crypto-cpp-py (>=1.4.0,<1.5.0)
 Requires-Dist: flask-cors (>=3.0.10,<3.1.0)
 Requires-Dist: gunicorn (>=20.1.0,<20.2.0)
 Requires-Dist: jsonschema (>=4.17.0,<4.18.0)
 Requires-Dist: marshmallow (>=3.17.0,<3.18.0)
 Requires-Dist: marshmallow-dataclass (>=8.4,<8.5)
 Requires-Dist: poseidon-py (>=0.1.3,<0.2.0)
+Requires-Dist: pyyaml (>=6.0.1,<6.1.0)
 Requires-Dist: typing-extensions (>=4.3.0,<4.4.0)
 Requires-Dist: web3 (>=6.0.0,<6.1.0)
 Project-URL: Repository, https://github.com/0xSpaceShard/starknet-devnet
 Description-Content-Type: text/markdown
 
 <!-- logo / title -->
 <p align="center" style="margin-bottom: 0px !important">
```

