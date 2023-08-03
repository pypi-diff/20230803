# Comparing `tmp/open-aea-web3-6.0.1.tar.gz` & `tmp/open-aea-web3-6.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-web3-6.0.1.tar", last modified: Thu Aug  3 07:20:05 2023, max compression
+gzip compressed data, was "open-aea-web3-6.0.1rc0.tar", last modified: Thu Aug  3 05:31:42 2023, max compression
```

## Comparing `open-aea-web3-6.0.1.tar` & `open-aea-web3-6.0.1rc0.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.191071 open-aea-web3-6.0.1/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-07-31 08:38:21.000000 open-aea-web3-6.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      260 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2193 2023-08-03 07:20:05.191071 open-aea-web3-6.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1294 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.115072 open-aea-web3-6.0.1/ens/
--rw-r--r--   0 root         (0) root         (0)      285 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23773 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/abis.py
--rw-r--r--   0 root         (0) root         (0)    20886 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/async_ens.py
--rw-r--r--   0 root         (0) root         (0)       41 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/auto.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/base_ens.py
--rw-r--r--   0 root         (0) root         (0)      601 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/constants.py
--rw-r--r--   0 root         (0) root         (0)   199089 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/contract_data.py
--rw-r--r--   0 root         (0) root         (0)    20044 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/ens.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8978 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ens/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.119072 open-aea-web3-6.0.1/ethpm/
--rw-r--r--   0 root         (0) root         (0)      580 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.123072 open-aea-web3-6.0.1/ethpm/_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/_utils/backend.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/_utils/cache.py
--rw-r--r--   0 root         (0) root         (0)     2848 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/_utils/chains.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/_utils/contract.py
--rw-r--r--   0 root         (0) root         (0)     5263 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/_utils/deployments.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/_utils/ipfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.123072 open-aea-web3-6.0.1/ethpm/_utils/protobuf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/_utils/protobuf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/_utils/protobuf/ipfs_file_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/_utils/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.123072 open-aea-web3-6.0.1/ethpm/assets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.123072 open-aea-web3-6.0.1/ethpm/assets/ens/
--rw-r--r--   0 root         (0) root         (0)    74682 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/ens/v3.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.123072 open-aea-web3-6.0.1/ethpm/assets/escrow/
--rw-r--r--   0 root         (0) root         (0)     8007 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/escrow/with_bytecode_v3.json
--rw-r--r--   0 root         (0) root         (0)      760 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/assets/ipfs_file.proto
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.123072 open-aea-web3-6.0.1/ethpm/assets/owned/
--rw-r--r--   0 root         (0) root         (0)     2655 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/owned/output_v3.json
--rw-r--r--   0 root         (0) root         (0)      746 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/owned/with_contract_type_v3.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.131071 open-aea-web3-6.0.1/ethpm/assets/registry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.135071 open-aea-web3-6.0.1/ethpm/assets/registry/contracts/
--rw-r--r--   0 root         (0) root         (0)     3129 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/contracts/Authority.sol
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
--rw-r--r--   0 root         (0) root         (0)     6380 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/contracts/PackageDB.sol
--rw-r--r--   0 root         (0) root         (0)    10553 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/contracts/PackageRegistry.sol
--rw-r--r--   0 root         (0) root         (0)     2966 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 root         (0) root         (0)     9041 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/contracts/ReleaseDB.sol
--rw-r--r--   0 root         (0) root         (0)     4980 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/contracts/ReleaseValidator.sol
--rw-r--r--   0 root         (0) root         (0)     1046 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/solc_input.json
--rw-r--r--   0 root         (0) root         (0)   727775 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/registry/solc_output.json
--rw-r--r--   0 root         (0) root         (0)   270218 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/registry/v3.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.139071 open-aea-web3-6.0.1/ethpm/assets/safe-math-lib/
--rw-r--r--   0 root         (0) root         (0)     2845 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.139071 open-aea-web3-6.0.1/ethpm/assets/simple-registry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.143071 open-aea-web3-6.0.1/ethpm/assets/simple-registry/contracts/
--rw-r--r--   0 root         (0) root         (0)     1841 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/simple-registry/contracts/Ownable.sol
--rw-r--r--   0 root         (0) root         (0)    12350 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
--rw-r--r--   0 root         (0) root         (0)     3278 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 root         (0) root         (0)      950 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/simple-registry/solc_input.json
--rw-r--r--   0 root         (0) root         (0)   199338 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/simple-registry/solc_output.json
--rw-r--r--   0 root         (0) root         (0)    75677 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/simple-registry/v3.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.143071 open-aea-web3-6.0.1/ethpm/assets/standard-token/
--rw-r--r--   0 root         (0) root         (0)    22292 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/standard-token/output_v3.json
--rw-r--r--   0 root         (0) root         (0)     8765 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/assets/standard-token/with_bytecode_v3.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.147071 open-aea-web3-6.0.1/ethpm/assets/vyper_registry/
--rw-r--r--   0 root         (0) root         (0)    81363 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/vyper_registry/0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     6339 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/vyper_registry/registry.vy
--rw-r--r--   0 root         (0) root         (0)     7596 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/assets/vyper_registry/registry_with_delete.vy
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.147071 open-aea-web3-6.0.1/ethpm/backends/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/backends/base.py
--rw-r--r--   0 root         (0) root         (0)     3006 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/backends/http.py
--rw-r--r--   0 root         (0) root         (0)     6551 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/backends/ipfs.py
--rw-r--r--   0 root         (0) root         (0)     4174 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/backends/registry.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/constants.py
--rw-r--r--   0 root         (0) root         (0)     6256 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/contract.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/dependencies.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/deployments.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14493 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.151071 open-aea-web3-6.0.1/ethpm/tools/
--rw-r--r--   0 root         (0) root         (0)      103 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27045 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/tools/builder.py
--rw-r--r--   0 root         (0) root         (0)    10373 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/tools/checker.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/tools/get_manifest.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.151071 open-aea-web3-6.0.1/ethpm/validation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/ethpm/validation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/validation/manifest.py
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/validation/misc.py
--rw-r--r--   0 root         (0) root         (0)     2317 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/ethpm/validation/package.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/ethpm/validation/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.155071 open-aea-web3-6.0.1/open_aea_web3.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2193 2023-08-03 07:20:05.000000 open-aea-web3-6.0.1/open_aea_web3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7546 2023-08-03 07:20:05.000000 open-aea-web3-6.0.1/open_aea_web3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 07:20:05.000000 open-aea-web3-6.0.1/open_aea_web3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-08-03 07:20:05.000000 open-aea-web3-6.0.1/open_aea_web3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 05:31:42.000000 open-aea-web3-6.0.1/open_aea_web3.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1442 2023-08-03 07:20:05.000000 open-aea-web3-6.0.1/open_aea_web3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-08-03 07:20:05.000000 open-aea-web3-6.0.1/open_aea_web3.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1055 2023-08-03 05:42:43.000000 open-aea-web3-6.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 07:20:05.191071 open-aea-web3-6.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3538 2023-08-03 06:38:29.000000 open-aea-web3-6.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.159071 open-aea-web3-6.0.1/web3/
--rw-r--r--   0 root         (0) root         (0)      761 2023-08-03 05:42:32.000000 open-aea-web3-6.0.1/web3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.167071 open-aea-web3-6.0.1/web3/_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28771 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/abi.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/async_caching.py
--rw-r--r--   0 root         (0) root         (0)     6865 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/async_transactions.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/blocks.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.167071 open-aea-web3-6.0.1/web3/_utils/compat/
--rw-r--r--   0 root         (0) root         (0)      319 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 08:38:21.000000 open-aea-web3-6.0.1/web3/_utils/compat/compat_py2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 08:38:21.000000 open-aea-web3-6.0.1/web3/_utils/compat/compat_py3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.167071 open-aea-web3-6.0.1/web3/_utils/contract_sources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6406 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/compile_contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.171071 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/address_reflector.py
--rw-r--r--   0 root         (0) root         (0)    19324 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/arrays_contract.py
--rw-r--r--   0 root         (0) root         (0)    15157 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/bytes_contracts.py
--rw-r--r--   0 root         (0) root         (0)     6219 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/constructor_contracts.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
--rw-r--r--   0 root         (0) root         (0)    38375 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/emitter_contract.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/event_contracts.py
--rw-r--r--   0 root         (0) root         (0)    16216 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/extended_resolver.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
--rw-r--r--   0 root         (0) root         (0)     7829 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/math_contract.py
--rw-r--r--   0 root         (0) root         (0)    17122 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/offchain_lookup.py
--rw-r--r--   0 root         (0) root         (0)    33495 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/offchain_resolver.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/payable_tester.py
--rw-r--r--   0 root         (0) root         (0)    17734 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
--rw-r--r--   0 root         (0) root         (0)     5410 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/reflector_contracts.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/revert_contract.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/simple_resolver.py
--rw-r--r--   0 root         (0) root         (0)    11900 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/string_contract.py
--rw-r--r--   0 root         (0) root         (0)    23756 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/tuple_contracts.py
--rw-r--r--   0 root         (0) root         (0)    14980 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/contracts.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     1738 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/empty.py
--rw-r--r--   0 root         (0) root         (0)     9065 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/encoding.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/ens.py
--rw-r--r--   0 root         (0) root         (0)    17073 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/events.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/fee_utils.py
--rw-r--r--   0 root         (0) root         (0)    11886 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/filters.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/formatters.py
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/_utils/function_identifiers.py
--rw-r--r--   0 root         (0) root         (0)      195 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/http.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/hypothesis.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/math.py
--rw-r--r--   0 root         (0) root         (0)    29717 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/method_formatters.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/miner.py
--rw-r--r--   0 root         (0) root         (0)     3147 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.175071 open-aea-web3-6.0.1/web3/_utils/module_testing/
--rw-r--r--   0 root         (0) root         (0)      539 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module_testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)   141852 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module_testing/eth_module.py
--rw-r--r--   0 root         (0) root         (0)     3406 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module_testing/go_ethereum_admin_module.py
--rw-r--r--   0 root         (0) root         (0)    10338 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module_testing/go_ethereum_personal_module.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module_testing/go_ethereum_txpool_module.py
--rw-r--r--   0 root         (0) root         (0)     4825 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module_testing/module_testing_utils.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module_testing/net_module.py
--rw-r--r--   0 root         (0) root         (0)     9335 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/module_testing/web3_module.py
--rw-r--r--   0 root         (0) root         (0)     6675 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/normalizers.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/request.py
--rw-r--r--   0 root         (0) root         (0)     9222 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/rpc_abi.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/threads.py
--rw-r--r--   0 root         (0) root         (0)     8670 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/transactions.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/type_conversion.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/utility_methods.py
--rw-r--r--   0 root         (0) root         (0)     6291 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/validation.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/_utils/windows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.175071 open-aea-web3-6.0.1/web3/auto/
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/auto/__init__.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/auto/gethdev.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.175071 open-aea-web3-6.0.1/web3/beacon/
--rw-r--r--   0 root         (0) root         (0)       91 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/beacon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/beacon/api_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     5421 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/beacon/async_beacon.py
--rw-r--r--   0 root         (0) root         (0)     4772 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/beacon/main.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.175071 open-aea-web3-6.0.1/web3/contract/
--rw-r--r--   0 root         (0) root         (0)      215 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/contract/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19756 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/contract/async_contract.py
--rw-r--r--   0 root         (0) root         (0)    35710 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/contract/base_contract.py
--rw-r--r--   0 root         (0) root         (0)    18804 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/contract/contract.py
--rw-r--r--   0 root         (0) root         (0)    12338 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/contract/utils.py
--rw-r--r--   0 root         (0) root         (0)     8271 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/datastructures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.179071 open-aea-web3-6.0.1/web3/eth/
--rw-r--r--   0 root         (0) root         (0)      166 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/eth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17870 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/eth/async_eth.py
--rw-r--r--   0 root         (0) root         (0)     5943 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/eth/base_eth.py
--rw-r--r--   0 root         (0) root         (0)    19295 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/eth/eth.py
--rw-r--r--   0 root         (0) root         (0)     5780 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.179071 open-aea-web3-6.0.1/web3/gas_strategies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/gas_strategies/__init__.py
--rw-r--r--   0 root         (0) root         (0)      430 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/gas_strategies/rpc.py
--rw-r--r--   0 root         (0) root         (0)     9010 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/gas_strategies/time_based.py
--rw-r--r--   0 root         (0) root         (0)    11826 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/geth.py
--rw-r--r--   0 root         (0) root         (0)      198 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/logs.py
--rw-r--r--   0 root         (0) root         (0)    12616 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/main.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/manager.py
--rw-r--r--   0 root         (0) root         (0)     8430 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/method.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.183071 open-aea-web3-6.0.1/web3/middleware/
--rw-r--r--   0 root         (0) root         (0)     3724 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/__init__.py
--rw-r--r--   0 root         (0) root         (0)      239 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/middleware/abi.py
--rw-r--r--   0 root         (0) root         (0)     2755 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/async_cache.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/attrdict.py
--rw-r--r--   0 root         (0) root         (0)     1785 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/buffered_gas_estimate.py
--rw-r--r--   0 root         (0) root         (0)    12617 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/cache.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/exception_handling.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/exception_retry_request.py
--rw-r--r--   0 root         (0) root         (0)    21131 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/filter.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/fixture.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/formatting.py
--rw-r--r--   0 root         (0) root         (0)     4212 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/gas_price_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/geth_poa.py
--rw-r--r--   0 root         (0) root         (0)      590 2023-07-31 08:38:21.000000 open-aea-web3-6.0.1/web3/middleware/names.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/middleware/normalize_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/middleware/pythonic.py
--rw-r--r--   0 root         (0) root         (0)     4450 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/signing.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/simulate_unmined_transaction.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/stalecheck.py
--rw-r--r--   0 root         (0) root         (0)     4573 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/middleware/validation.py
--rw-r--r--   0 root         (0) root         (0)     3615 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/module.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/net.py
--rw-r--r--   0 root         (0) root         (0)    21609 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/pm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.187071 open-aea-web3-6.0.1/web3/providers/
--rw-r--r--   0 root         (0) root         (0)      368 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3544 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/async_base.py
--rw-r--r--   0 root         (0) root         (0)     2469 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/async_rpc.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/auto.py
--rw-r--r--   0 root         (0) root         (0)     3477 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.187071 open-aea-web3-6.0.1/web3/providers/eth_tester/
--rw-r--r--   0 root         (0) root         (0)       97 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/eth_tester/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14296 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/eth_tester/defaults.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/eth_tester/main.py
--rw-r--r--   0 root         (0) root         (0)    12665 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/eth_tester/middleware.py
--rw-r--r--   0 root         (0) root         (0)     6534 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/ipc.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/rpc.py
--rw-r--r--   0 root         (0) root         (0)     3919 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/providers/websocket.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.187071 open-aea-web3-6.0.1/web3/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.187071 open-aea-web3-6.0.1/web3/scripts/release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/scripts/release/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/scripts/release/test_package.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.187071 open-aea-web3-6.0.1/web3/tools/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.191071 open-aea-web3-6.0.1/web3/tools/benchmark/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/web3/tools/benchmark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5886 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/tools/benchmark/main.py
--rw-r--r--   0 root         (0) root         (0)     3435 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/tools/benchmark/node.py
--rw-r--r--   0 root         (0) root         (0)      912 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/tools/benchmark/reporting.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1/web3/tools/benchmark/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.191071 open-aea-web3-6.0.1/web3/tools/pytest_ethereum/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/tools/pytest_ethereum/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/tools/pytest_ethereum/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/tools/pytest_ethereum/deployer.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1/web3/tools/pytest_ethereum/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3927 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/tools/pytest_ethereum/linker.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/tools/pytest_ethereum/plugins.py
--rw-r--r--   0 root         (0) root         (0)    10160 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:20:05.191071 open-aea-web3-6.0.1/web3/utils/
--rw-r--r--   0 root         (0) root         (0)      454 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/utils/abi.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/utils/address.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/utils/async_exception_handling.py
--rw-r--r--   0 root         (0) root         (0)     1521 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/utils/caching.py
--rw-r--r--   0 root         (0) root         (0)     3052 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1/web3/utils/exception_handling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.886752 open-aea-web3-6.0.1rc0/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-07-31 08:38:21.000000 open-aea-web3-6.0.1rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      260 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-08-03 05:31:42.886752 open-aea-web3-6.0.1rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1294 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.854753 open-aea-web3-6.0.1rc0/ens/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23773 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/abis.py
+-rw-r--r--   0 root         (0) root         (0)    20886 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/async_ens.py
+-rw-r--r--   0 root         (0) root         (0)       41 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/auto.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/base_ens.py
+-rw-r--r--   0 root         (0) root         (0)      601 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/constants.py
+-rw-r--r--   0 root         (0) root         (0)   199089 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/contract_data.py
+-rw-r--r--   0 root         (0) root         (0)    20044 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/ens.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8978 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ens/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.854753 open-aea-web3-6.0.1rc0/ethpm/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.854753 open-aea-web3-6.0.1rc0/ethpm/_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/backend.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/chains.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/contract.py
+-rw-r--r--   0 root         (0) root         (0)     5263 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/deployments.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/ipfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.854753 open-aea-web3-6.0.1rc0/ethpm/_utils/protobuf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/protobuf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/protobuf/ipfs_file_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/_utils/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.854753 open-aea-web3-6.0.1rc0/ethpm/assets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.854753 open-aea-web3-6.0.1rc0/ethpm/assets/ens/
+-rw-r--r--   0 root         (0) root         (0)    74682 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/ens/v3.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.854753 open-aea-web3-6.0.1rc0/ethpm/assets/escrow/
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/escrow/with_bytecode_v3.json
+-rw-r--r--   0 root         (0) root         (0)      760 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/assets/ipfs_file.proto
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.854753 open-aea-web3-6.0.1rc0/ethpm/assets/owned/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/owned/output_v3.json
+-rw-r--r--   0 root         (0) root         (0)      746 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/owned/with_contract_type_v3.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.858753 open-aea-web3-6.0.1rc0/ethpm/assets/registry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.858753 open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/Authority.sol
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
+-rw-r--r--   0 root         (0) root         (0)     6380 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/PackageDB.sol
+-rw-r--r--   0 root         (0) root         (0)    10553 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 root         (0) root         (0)     9041 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/ReleaseDB.sol
+-rw-r--r--   0 root         (0) root         (0)     4980 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/ReleaseValidator.sol
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/solc_input.json
+-rw-r--r--   0 root         (0) root         (0)   727775 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/solc_output.json
+-rw-r--r--   0 root         (0) root         (0)   270218 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/registry/v3.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.858753 open-aea-web3-6.0.1rc0/ethpm/assets/safe-math-lib/
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.858753 open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.858753 open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/contracts/
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/contracts/Ownable.sol
+-rw-r--r--   0 root         (0) root         (0)    12350 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 root         (0) root         (0)      950 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/solc_input.json
+-rw-r--r--   0 root         (0) root         (0)   199338 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/solc_output.json
+-rw-r--r--   0 root         (0) root         (0)    75677 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/v3.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.858753 open-aea-web3-6.0.1rc0/ethpm/assets/standard-token/
+-rw-r--r--   0 root         (0) root         (0)    22292 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/standard-token/output_v3.json
+-rw-r--r--   0 root         (0) root         (0)     8765 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/assets/standard-token/with_bytecode_v3.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.862753 open-aea-web3-6.0.1rc0/ethpm/assets/vyper_registry/
+-rw-r--r--   0 root         (0) root         (0)    81363 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/vyper_registry/0.1.0.json
+-rw-r--r--   0 root         (0) root         (0)     6339 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/vyper_registry/registry.vy
+-rw-r--r--   0 root         (0) root         (0)     7596 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/assets/vyper_registry/registry_with_delete.vy
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.862753 open-aea-web3-6.0.1rc0/ethpm/backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/backends/base.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/backends/http.py
+-rw-r--r--   0 root         (0) root         (0)     6551 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/backends/ipfs.py
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/backends/registry.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6256 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/contract.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/deployments.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14493 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.862753 open-aea-web3-6.0.1rc0/ethpm/tools/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27045 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/tools/builder.py
+-rw-r--r--   0 root         (0) root         (0)    10373 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/tools/checker.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/tools/get_manifest.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.862753 open-aea-web3-6.0.1rc0/ethpm/validation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/ethpm/validation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/validation/manifest.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/validation/misc.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/ethpm/validation/package.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/ethpm/validation/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.862753 open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-08-03 05:31:42.000000 open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7546 2023-08-03 05:31:42.000000 open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 05:31:42.000000 open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-08-03 05:31:42.000000 open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 05:31:42.000000 open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-08-03 05:31:42.000000 open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-03 05:31:42.000000 open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 05:31:42.886752 open-aea-web3-6.0.1rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-08-03 05:31:12.000000 open-aea-web3-6.0.1rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.866753 open-aea-web3-6.0.1rc0/web3/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.870753 open-aea-web3-6.0.1rc0/web3/_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28771 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/abi.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/async_caching.py
+-rw-r--r--   0 root         (0) root         (0)     6865 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/async_transactions.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/blocks.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.870753 open-aea-web3-6.0.1rc0/web3/_utils/compat/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 08:38:21.000000 open-aea-web3-6.0.1rc0/web3/_utils/compat/compat_py2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 08:38:21.000000 open-aea-web3-6.0.1rc0/web3/_utils/compat/compat_py3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.870753 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/compile_contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.874752 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/address_reflector.py
+-rw-r--r--   0 root         (0) root         (0)    19324 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/arrays_contract.py
+-rw-r--r--   0 root         (0) root         (0)    15157 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/bytes_contracts.py
+-rw-r--r--   0 root         (0) root         (0)     6219 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/constructor_contracts.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
+-rw-r--r--   0 root         (0) root         (0)    38375 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/emitter_contract.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/event_contracts.py
+-rw-r--r--   0 root         (0) root         (0)    16216 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/extended_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
+-rw-r--r--   0 root         (0) root         (0)     7829 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/math_contract.py
+-rw-r--r--   0 root         (0) root         (0)    17122 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/offchain_lookup.py
+-rw-r--r--   0 root         (0) root         (0)    33495 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/offchain_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/payable_tester.py
+-rw-r--r--   0 root         (0) root         (0)    17734 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
+-rw-r--r--   0 root         (0) root         (0)     5410 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/reflector_contracts.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/revert_contract.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/simple_resolver.py
+-rw-r--r--   0 root         (0) root         (0)    11900 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/string_contract.py
+-rw-r--r--   0 root         (0) root         (0)    23756 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/tuple_contracts.py
+-rw-r--r--   0 root         (0) root         (0)    14980 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/contracts.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/empty.py
+-rw-r--r--   0 root         (0) root         (0)     9065 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/encoding.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/ens.py
+-rw-r--r--   0 root         (0) root         (0)    17073 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/events.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/fee_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11886 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/filters.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/formatters.py
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/_utils/function_identifiers.py
+-rw-r--r--   0 root         (0) root         (0)      195 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/http.py
+-rw-r--r--   0 root         (0) root         (0)      209 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/hypothesis.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/math.py
+-rw-r--r--   0 root         (0) root         (0)    29717 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/method_formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/miner.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.874752 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/
+-rw-r--r--   0 root         (0) root         (0)      539 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   141852 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/eth_module.py
+-rw-r--r--   0 root         (0) root         (0)     3406 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/go_ethereum_admin_module.py
+-rw-r--r--   0 root         (0) root         (0)    10338 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/go_ethereum_personal_module.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/go_ethereum_txpool_module.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/module_testing_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/net_module.py
+-rw-r--r--   0 root         (0) root         (0)     9335 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/module_testing/web3_module.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/normalizers.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/request.py
+-rw-r--r--   0 root         (0) root         (0)     9222 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/rpc_abi.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/threads.py
+-rw-r--r--   0 root         (0) root         (0)     8670 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/transactions.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/type_conversion.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/utility_methods.py
+-rw-r--r--   0 root         (0) root         (0)     6291 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/validation.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/_utils/windows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.874752 open-aea-web3-6.0.1rc0/web3/auto/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/auto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/auto/gethdev.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.874752 open-aea-web3-6.0.1rc0/web3/beacon/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/beacon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/beacon/api_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     5421 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/beacon/async_beacon.py
+-rw-r--r--   0 root         (0) root         (0)     4772 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/beacon/main.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.878752 open-aea-web3-6.0.1rc0/web3/contract/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/contract/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19756 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/contract/async_contract.py
+-rw-r--r--   0 root         (0) root         (0)    35710 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/contract/base_contract.py
+-rw-r--r--   0 root         (0) root         (0)    18804 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/contract/contract.py
+-rw-r--r--   0 root         (0) root         (0)    12338 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/contract/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8271 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/datastructures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.878752 open-aea-web3-6.0.1rc0/web3/eth/
+-rw-r--r--   0 root         (0) root         (0)      166 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/eth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17870 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/eth/async_eth.py
+-rw-r--r--   0 root         (0) root         (0)     5943 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/eth/base_eth.py
+-rw-r--r--   0 root         (0) root         (0)    19295 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/eth/eth.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.878752 open-aea-web3-6.0.1rc0/web3/gas_strategies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/gas_strategies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      430 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/gas_strategies/rpc.py
+-rw-r--r--   0 root         (0) root         (0)     9010 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/gas_strategies/time_based.py
+-rw-r--r--   0 root         (0) root         (0)    11826 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/geth.py
+-rw-r--r--   0 root         (0) root         (0)      198 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/logs.py
+-rw-r--r--   0 root         (0) root         (0)    12616 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/main.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/manager.py
+-rw-r--r--   0 root         (0) root         (0)     8430 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/method.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.882752 open-aea-web3-6.0.1rc0/web3/middleware/
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/middleware/abi.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/async_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/attrdict.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/buffered_gas_estimate.py
+-rw-r--r--   0 root         (0) root         (0)    12617 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/exception_handling.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/exception_retry_request.py
+-rw-r--r--   0 root         (0) root         (0)    21131 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/filter.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/fixture.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/formatting.py
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/gas_price_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/geth_poa.py
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-31 08:38:21.000000 open-aea-web3-6.0.1rc0/web3/middleware/names.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/middleware/normalize_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/middleware/pythonic.py
+-rw-r--r--   0 root         (0) root         (0)     4450 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/signing.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/simulate_unmined_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/stalecheck.py
+-rw-r--r--   0 root         (0) root         (0)     4573 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/middleware/validation.py
+-rw-r--r--   0 root         (0) root         (0)     3615 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/module.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/net.py
+-rw-r--r--   0 root         (0) root         (0)    21609 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/pm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.882752 open-aea-web3-6.0.1rc0/web3/providers/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3544 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/async_base.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/async_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/auto.py
+-rw-r--r--   0 root         (0) root         (0)     3477 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.882752 open-aea-web3-6.0.1rc0/web3/providers/eth_tester/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/eth_tester/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14296 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/eth_tester/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/eth_tester/main.py
+-rw-r--r--   0 root         (0) root         (0)    12665 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/eth_tester/middleware.py
+-rw-r--r--   0 root         (0) root         (0)     6534 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/ipc.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/rpc.py
+-rw-r--r--   0 root         (0) root         (0)     3919 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/providers/websocket.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.882752 open-aea-web3-6.0.1rc0/web3/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.882752 open-aea-web3-6.0.1rc0/web3/scripts/release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/scripts/release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/scripts/release/test_package.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.882752 open-aea-web3-6.0.1rc0/web3/tools/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.882752 open-aea-web3-6.0.1rc0/web3/tools/benchmark/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/web3/tools/benchmark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/tools/benchmark/main.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/tools/benchmark/node.py
+-rw-r--r--   0 root         (0) root         (0)      912 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/tools/benchmark/reporting.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-08-01 10:55:17.000000 open-aea-web3-6.0.1rc0/web3/tools/benchmark/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.886752 open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/deployer.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-07-31 07:57:33.000000 open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/linker.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/plugins.py
+-rw-r--r--   0 root         (0) root         (0)    10160 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:31:42.886752 open-aea-web3-6.0.1rc0/web3/utils/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/utils/abi.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/utils/address.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/utils/async_exception_handling.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/utils/caching.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2023-08-03 05:27:43.000000 open-aea-web3-6.0.1rc0/web3/utils/exception_handling.py
```

### Comparing `open-aea-web3-6.0.1/LICENSE` & `open-aea-web3-6.0.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/PKG-INFO` & `open-aea-web3-6.0.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-web3
-Version: 6.0.1
+Version: 6.0.1rc0
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `open-aea-web3-6.0.1/README.md` & `open-aea-web3-6.0.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ens/abis.py` & `open-aea-web3-6.0.1rc0/ens/abis.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ens/async_ens.py` & `open-aea-web3-6.0.1rc0/ens/async_ens.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ens/base_ens.py` & `open-aea-web3-6.0.1rc0/ens/base_ens.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ens/constants.py` & `open-aea-web3-6.0.1rc0/ens/constants.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ens/contract_data.py` & `open-aea-web3-6.0.1rc0/ens/contract_data.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ens/ens.py` & `open-aea-web3-6.0.1rc0/ens/ens.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ens/exceptions.py` & `open-aea-web3-6.0.1rc0/ens/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ens/utils.py` & `open-aea-web3-6.0.1rc0/ens/utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/__init__.py` & `open-aea-web3-6.0.1rc0/ethpm/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/_utils/backend.py` & `open-aea-web3-6.0.1rc0/ethpm/_utils/backend.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/_utils/cache.py` & `open-aea-web3-6.0.1rc0/ethpm/_utils/cache.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/_utils/chains.py` & `open-aea-web3-6.0.1rc0/ethpm/_utils/chains.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/_utils/contract.py` & `open-aea-web3-6.0.1rc0/ethpm/_utils/contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/_utils/deployments.py` & `open-aea-web3-6.0.1rc0/ethpm/_utils/deployments.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/_utils/ipfs.py` & `open-aea-web3-6.0.1rc0/ethpm/_utils/ipfs.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/_utils/protobuf/ipfs_file_pb2.py` & `open-aea-web3-6.0.1rc0/ethpm/_utils/protobuf/ipfs_file_pb2.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/_utils/registry.py` & `open-aea-web3-6.0.1rc0/ethpm/_utils/registry.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/ens/v3.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/ens/v3.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/escrow/with_bytecode_v3.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/escrow/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/ipfs_file.proto` & `open-aea-web3-6.0.1rc0/ethpm/assets/ipfs_file.proto`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/owned/output_v3.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/owned/output_v3.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/owned/with_contract_type_v3.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/owned/with_contract_type_v3.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/contracts/Authority.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/Authority.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/contracts/PackageDB.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/PackageDB.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/contracts/PackageRegistry.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/contracts/PackageRegistryInterface.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/contracts/ReleaseDB.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/ReleaseDB.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/contracts/ReleaseValidator.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/contracts/ReleaseValidator.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/solc_input.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/solc_output.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/registry/v3.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/registry/v3.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/simple-registry/contracts/Ownable.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/contracts/Ownable.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/simple-registry/contracts/PackageRegistry.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol` & `open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/simple-registry/solc_input.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/simple-registry/solc_output.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/simple-registry/v3.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/simple-registry/v3.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/standard-token/output_v3.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/standard-token/output_v3.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/standard-token/with_bytecode_v3.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/standard-token/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/vyper_registry/0.1.0.json` & `open-aea-web3-6.0.1rc0/ethpm/assets/vyper_registry/0.1.0.json`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/vyper_registry/registry.vy` & `open-aea-web3-6.0.1rc0/ethpm/assets/vyper_registry/registry.vy`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/assets/vyper_registry/registry_with_delete.vy` & `open-aea-web3-6.0.1rc0/ethpm/assets/vyper_registry/registry_with_delete.vy`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/backends/base.py` & `open-aea-web3-6.0.1rc0/ethpm/backends/base.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/backends/http.py` & `open-aea-web3-6.0.1rc0/ethpm/backends/http.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/backends/ipfs.py` & `open-aea-web3-6.0.1rc0/ethpm/backends/ipfs.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/backends/registry.py` & `open-aea-web3-6.0.1rc0/ethpm/backends/registry.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/contract.py` & `open-aea-web3-6.0.1rc0/ethpm/contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/dependencies.py` & `open-aea-web3-6.0.1rc0/ethpm/dependencies.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/deployments.py` & `open-aea-web3-6.0.1rc0/ethpm/deployments.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/exceptions.py` & `open-aea-web3-6.0.1rc0/ethpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/package.py` & `open-aea-web3-6.0.1rc0/ethpm/package.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/tools/builder.py` & `open-aea-web3-6.0.1rc0/ethpm/tools/builder.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/tools/checker.py` & `open-aea-web3-6.0.1rc0/ethpm/tools/checker.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/uri.py` & `open-aea-web3-6.0.1rc0/ethpm/uri.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/validation/manifest.py` & `open-aea-web3-6.0.1rc0/ethpm/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/validation/misc.py` & `open-aea-web3-6.0.1rc0/ethpm/validation/misc.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/validation/package.py` & `open-aea-web3-6.0.1rc0/ethpm/validation/package.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/ethpm/validation/uri.py` & `open-aea-web3-6.0.1rc0/ethpm/validation/uri.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/open_aea_web3.egg-info/PKG-INFO` & `open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-web3
-Version: 6.0.1
+Version: 6.0.1rc0
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `open-aea-web3-6.0.1/open_aea_web3.egg-info/SOURCES.txt` & `open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/open_aea_web3.egg-info/requires.txt` & `open-aea-web3-6.0.1rc0/open_aea_web3.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/pyproject.toml` & `open-aea-web3-6.0.1rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.towncrier]
-    package="open-aea-web3"
+    package="web3"
     filename = "docs/releases.rst"
     directory = "newsfragments"
     underlines = ["-", "~", "^"]
     issue_format = "`#{issue} <https://github.com/ethereum/web3.py/issues/{issue}>`__"
     title_format = "v{version} ({project_date})"
 
 [[tool.towncrier.type]]
```

### Comparing `open-aea-web3-6.0.1/setup.py` & `open-aea-web3-6.0.1rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="open-aea-web3",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="6.0.1",
+    version="6.0.1.rc0",
     description="""web3.py""",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Piper Merriam",
     author_email="pipermerriam@gmail.com",
     url="https://github.com/ethereum/web3.py",
     include_package_data=True,
```

### Comparing `open-aea-web3-6.0.1/web3/__init__.py` & `open-aea-web3-6.0.1rc0/web3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from web3.providers.rpc import (  # noqa: E402
     HTTPProvider,
 )
 from web3.providers.websocket import (  # noqa: E402
     WebsocketProvider,
 )
 
-__version__ = pkg_resources.get_distribution("open-aea-web3").version
+__version__ = pkg_resources.get_distribution("web3").version
 
 __all__ = [
     "__version__",
     "AsyncWeb3",
     "Web3",
     "HTTPProvider",
     "IPCProvider",
```

### Comparing `open-aea-web3-6.0.1/web3/_utils/abi.py` & `open-aea-web3-6.0.1rc0/web3/_utils/abi.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/async_transactions.py` & `open-aea-web3-6.0.1rc0/web3/_utils/async_transactions.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/blocks.py` & `open-aea-web3-6.0.1rc0/web3/_utils/blocks.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/caching.py` & `open-aea-web3-6.0.1rc0/web3/_utils/caching.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/compile_contracts.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/compile_contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/_custom_contract_data.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/address_reflector.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/address_reflector.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/arrays_contract.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/arrays_contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/bytes_contracts.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/bytes_contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/constructor_contracts.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/constructor_contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/contract_caller_tester.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/emitter_contract.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/event_contracts.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/event_contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/extended_resolver.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/extended_resolver.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/fallback_function_contract.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/math_contract.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/math_contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/offchain_lookup.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/offchain_lookup.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/offchain_resolver.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/offchain_resolver.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/payable_tester.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/payable_tester.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/receive_function_contracts.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/reflector_contracts.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/reflector_contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/revert_contract.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/revert_contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/simple_resolver.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/simple_resolver.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/string_contract.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/string_contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contract_sources/contract_data/tuple_contracts.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contract_sources/contract_data/tuple_contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/contracts.py` & `open-aea-web3-6.0.1rc0/web3/_utils/contracts.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/datatypes.py` & `open-aea-web3-6.0.1rc0/web3/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/decorators.py` & `open-aea-web3-6.0.1rc0/web3/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/encoding.py` & `open-aea-web3-6.0.1rc0/web3/_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/ens.py` & `open-aea-web3-6.0.1rc0/web3/_utils/ens.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/events.py` & `open-aea-web3-6.0.1rc0/web3/_utils/events.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/fee_utils.py` & `open-aea-web3-6.0.1rc0/web3/_utils/fee_utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/filters.py` & `open-aea-web3-6.0.1rc0/web3/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/formatters.py` & `open-aea-web3-6.0.1rc0/web3/_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/math.py` & `open-aea-web3-6.0.1rc0/web3/_utils/math.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/method_formatters.py` & `open-aea-web3-6.0.1rc0/web3/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/miner.py` & `open-aea-web3-6.0.1rc0/web3/_utils/miner.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module_testing/__init__.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module_testing/eth_module.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module_testing/eth_module.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module_testing/go_ethereum_admin_module.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module_testing/go_ethereum_admin_module.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module_testing/go_ethereum_personal_module.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module_testing/go_ethereum_personal_module.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module_testing/go_ethereum_txpool_module.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module_testing/go_ethereum_txpool_module.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module_testing/module_testing_utils.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module_testing/module_testing_utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module_testing/net_module.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module_testing/net_module.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/module_testing/web3_module.py` & `open-aea-web3-6.0.1rc0/web3/_utils/module_testing/web3_module.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/normalizers.py` & `open-aea-web3-6.0.1rc0/web3/_utils/normalizers.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/request.py` & `open-aea-web3-6.0.1rc0/web3/_utils/request.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/rpc_abi.py` & `open-aea-web3-6.0.1rc0/web3/_utils/rpc_abi.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/threads.py` & `open-aea-web3-6.0.1rc0/web3/_utils/threads.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/transactions.py` & `open-aea-web3-6.0.1rc0/web3/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/type_conversion.py` & `open-aea-web3-6.0.1rc0/web3/_utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/utility_methods.py` & `open-aea-web3-6.0.1rc0/web3/_utils/utility_methods.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/validation.py` & `open-aea-web3-6.0.1rc0/web3/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/_utils/windows.py` & `open-aea-web3-6.0.1rc0/web3/_utils/windows.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/beacon/api_endpoints.py` & `open-aea-web3-6.0.1rc0/web3/beacon/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/beacon/async_beacon.py` & `open-aea-web3-6.0.1rc0/web3/beacon/async_beacon.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/beacon/main.py` & `open-aea-web3-6.0.1rc0/web3/beacon/main.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/contract/async_contract.py` & `open-aea-web3-6.0.1rc0/web3/contract/async_contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/contract/base_contract.py` & `open-aea-web3-6.0.1rc0/web3/contract/base_contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/contract/contract.py` & `open-aea-web3-6.0.1rc0/web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/contract/utils.py` & `open-aea-web3-6.0.1rc0/web3/contract/utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/datastructures.py` & `open-aea-web3-6.0.1rc0/web3/datastructures.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/eth/async_eth.py` & `open-aea-web3-6.0.1rc0/web3/eth/async_eth.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/eth/base_eth.py` & `open-aea-web3-6.0.1rc0/web3/eth/base_eth.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/eth/eth.py` & `open-aea-web3-6.0.1rc0/web3/eth/eth.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/exceptions.py` & `open-aea-web3-6.0.1rc0/web3/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/gas_strategies/time_based.py` & `open-aea-web3-6.0.1rc0/web3/gas_strategies/time_based.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/geth.py` & `open-aea-web3-6.0.1rc0/web3/geth.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/main.py` & `open-aea-web3-6.0.1rc0/web3/main.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/manager.py` & `open-aea-web3-6.0.1rc0/web3/manager.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/method.py` & `open-aea-web3-6.0.1rc0/web3/method.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/__init__.py` & `open-aea-web3-6.0.1rc0/web3/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/async_cache.py` & `open-aea-web3-6.0.1rc0/web3/middleware/async_cache.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/attrdict.py` & `open-aea-web3-6.0.1rc0/web3/middleware/attrdict.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/buffered_gas_estimate.py` & `open-aea-web3-6.0.1rc0/web3/middleware/buffered_gas_estimate.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/cache.py` & `open-aea-web3-6.0.1rc0/web3/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/exception_handling.py` & `open-aea-web3-6.0.1rc0/web3/middleware/exception_handling.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/exception_retry_request.py` & `open-aea-web3-6.0.1rc0/web3/middleware/exception_retry_request.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/filter.py` & `open-aea-web3-6.0.1rc0/web3/middleware/filter.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/fixture.py` & `open-aea-web3-6.0.1rc0/web3/middleware/fixture.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/formatting.py` & `open-aea-web3-6.0.1rc0/web3/middleware/formatting.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/gas_price_strategy.py` & `open-aea-web3-6.0.1rc0/web3/middleware/gas_price_strategy.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/geth_poa.py` & `open-aea-web3-6.0.1rc0/web3/middleware/geth_poa.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/names.py` & `open-aea-web3-6.0.1rc0/web3/middleware/names.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/signing.py` & `open-aea-web3-6.0.1rc0/web3/middleware/signing.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/simulate_unmined_transaction.py` & `open-aea-web3-6.0.1rc0/web3/middleware/simulate_unmined_transaction.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/stalecheck.py` & `open-aea-web3-6.0.1rc0/web3/middleware/stalecheck.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/middleware/validation.py` & `open-aea-web3-6.0.1rc0/web3/middleware/validation.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/module.py` & `open-aea-web3-6.0.1rc0/web3/module.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/net.py` & `open-aea-web3-6.0.1rc0/web3/net.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/pm.py` & `open-aea-web3-6.0.1rc0/web3/pm.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/async_base.py` & `open-aea-web3-6.0.1rc0/web3/providers/async_base.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/async_rpc.py` & `open-aea-web3-6.0.1rc0/web3/providers/async_rpc.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/auto.py` & `open-aea-web3-6.0.1rc0/web3/providers/auto.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/base.py` & `open-aea-web3-6.0.1rc0/web3/providers/base.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/eth_tester/defaults.py` & `open-aea-web3-6.0.1rc0/web3/providers/eth_tester/defaults.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/eth_tester/main.py` & `open-aea-web3-6.0.1rc0/web3/providers/eth_tester/main.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/eth_tester/middleware.py` & `open-aea-web3-6.0.1rc0/web3/providers/eth_tester/middleware.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/ipc.py` & `open-aea-web3-6.0.1rc0/web3/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/rpc.py` & `open-aea-web3-6.0.1rc0/web3/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/providers/websocket.py` & `open-aea-web3-6.0.1rc0/web3/providers/websocket.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/scripts/release/test_package.py` & `open-aea-web3-6.0.1rc0/web3/scripts/release/test_package.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/testing.py` & `open-aea-web3-6.0.1rc0/web3/testing.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/tools/benchmark/main.py` & `open-aea-web3-6.0.1rc0/web3/tools/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/tools/benchmark/node.py` & `open-aea-web3-6.0.1rc0/web3/tools/benchmark/node.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/tools/benchmark/reporting.py` & `open-aea-web3-6.0.1rc0/web3/tools/benchmark/reporting.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/tools/benchmark/utils.py` & `open-aea-web3-6.0.1rc0/web3/tools/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/tools/pytest_ethereum/_utils.py` & `open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/_utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/tools/pytest_ethereum/deployer.py` & `open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/deployer.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/tools/pytest_ethereum/linker.py` & `open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/linker.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/tools/pytest_ethereum/plugins.py` & `open-aea-web3-6.0.1rc0/web3/tools/pytest_ethereum/plugins.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/types.py` & `open-aea-web3-6.0.1rc0/web3/types.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/utils/address.py` & `open-aea-web3-6.0.1rc0/web3/utils/address.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/utils/async_exception_handling.py` & `open-aea-web3-6.0.1rc0/web3/utils/async_exception_handling.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/utils/caching.py` & `open-aea-web3-6.0.1rc0/web3/utils/caching.py`

 * *Files identical despite different names*

### Comparing `open-aea-web3-6.0.1/web3/utils/exception_handling.py` & `open-aea-web3-6.0.1rc0/web3/utils/exception_handling.py`

 * *Files identical despite different names*

