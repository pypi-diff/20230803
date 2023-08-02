# Comparing `tmp/sharingiscaring-0.2.80.tar.gz` & `tmp/sharingiscaring-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharingiscaring-0.2.80.tar", last modified: Wed Aug  2 22:18:01 2023, max compression
+gzip compressed data, was "sharingiscaring-0.2.9.tar", last modified: Tue Apr  4 11:18:24 2023, max compression
```

## Comparing `sharingiscaring-0.2.80.tar` & `sharingiscaring-0.2.9.tar`

### file list

```diff
@@ -1,143 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.389057 sharingiscaring-0.2.80/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-02 22:18:01.389057 sharingiscaring-0.2.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:18:01.389057 sharingiscaring-0.2.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.345057 sharingiscaring-0.2.80/sharingiscaring/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.349057 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.349057 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/CCD_Types/
--rw-r--r--   0 runner    (1001) docker     (123)    33605 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/CCD_Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.353057 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/concordium/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/concordium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.353057 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/concordium/health/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/concordium/health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.353057 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/concordium/v2/
--rw-r--r--   0 runner    (1001) docker     (123)   221467 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/concordium/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/health_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.365057 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_CheckHealth.py
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetAccountInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetAccountList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetAnonymityRevokers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBakerList.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockChainParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockPendingUpdates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockSpecialEvents.py
--rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockTransactionEvents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlocksAtHeight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetElectionInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetFinalizedBlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetIdentityProviders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetInstanceInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetInstanceList.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetModuleSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPassiveDelegationInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPassiveDelegators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPoolDelegators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPoolInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetTokenomicsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_InvokeInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)    36203 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_SharedConverters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    84238 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   105670 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/GRPCClient/wadze.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.373057 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_accountByAddress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_bakerByBakerId.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_bakers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_blockByBlockHash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_passiveDelegation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_paydayStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_poolRewardMetricsForBakerPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_rewardMetricsForAccount.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_transactionByTransactionHash.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_transactionMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/exchange_account_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/ql_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    37554 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/cis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19157 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/cns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.373057 sharingiscaring-0.2.80/sharingiscaring/grpcclient/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.377057 sharingiscaring-0.2.80/sharingiscaring/grpcclient/CCD_Types/
--rw-r--r--   0 runner    (1001) docker     (123)    33605 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/CCD_Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.377057 sharingiscaring-0.2.80/sharingiscaring/grpcclient/concordium/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/concordium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.377057 sharingiscaring-0.2.80/sharingiscaring/grpcclient/concordium/health/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/concordium/health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.377057 sharingiscaring-0.2.80/sharingiscaring/grpcclient/concordium/v2/
--rw-r--r--   0 runner    (1001) docker     (123)   221467 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/concordium/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/health_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.385057 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetAccountInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetAccountList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetAnonymityRevokers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBakerList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlockInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlockPendingUpdates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlockSpecialEvents.py
--rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlockTransactionEvents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlocksAtHeight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetFinalizedBlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetIdentityProviders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetInstanceInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetInstanceList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetPassiveDelegationInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetPassiveDelegators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetPoolDelegators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetPoolDelegatorsRewardPeriod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetPoolInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetTokenomicsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    36203 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_SharedConverters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    84238 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   105670 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/grpcclient/types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.385057 sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_apy_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_baker_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_search_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_store_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/tooter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46970 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/sharingiscaring/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.345057 sharingiscaring-0.2.80/sharingiscaring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-02 22:18:01.000000 sharingiscaring-0.2.80/sharingiscaring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-02 22:18:01.000000 sharingiscaring-0.2.80/sharingiscaring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:18:01.000000 sharingiscaring-0.2.80/sharingiscaring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 22:18:01.000000 sharingiscaring-0.2.80/sharingiscaring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 22:18:01.000000 sharingiscaring-0.2.80/sharingiscaring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:18:01.389057 sharingiscaring-0.2.80/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/tests/test_namehash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/tests/test_txs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-02 22:17:49.000000 sharingiscaring-0.2.80/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.884919 sharingiscaring-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-04 11:18:24.884919 sharingiscaring-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 11:18:24.884919 sharingiscaring-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.868919 sharingiscaring-0.2.9/sharingiscaring/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.872919 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.872919 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/CCD_Types/
+-rw-r--r--   0 runner    (1001) docker     (123)    31985 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/CCD_Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.872919 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/concordium/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/concordium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.872919 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/concordium/health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/concordium/health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.872919 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/concordium/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)   221467 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/concordium/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/health_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.876919 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetAccountInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetAccountList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetAnonymityRevokers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBakerList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockChainParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockPendingUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockSpecialEvents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34853 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockTransactionEvents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlocksAtHeight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetElectionInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetFinalizedBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetIdentityProviders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetInstanceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetInstanceList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetModuleSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPassiveDelegationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPassiveDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPoolDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPoolInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetTokenomicsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_SharedConverters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84238 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105670 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/GRPCClient/wadze.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.876919 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_accountByAddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_bakerByBakerId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_bakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_blockByBlockHash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_passiveDelegation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_paydayStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_poolRewardMetricsForBakerPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_rewardMetricsForAccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_transactionByTransactionHash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_transactionMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/exchange_account_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/ql_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/cns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.880919 sharingiscaring-0.2.9/sharingiscaring/grpcclient/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.880919 sharingiscaring-0.2.9/sharingiscaring/grpcclient/CCD_Types/
+-rw-r--r--   0 runner    (1001) docker     (123)    31985 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/CCD_Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.880919 sharingiscaring-0.2.9/sharingiscaring/grpcclient/concordium/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/concordium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.880919 sharingiscaring-0.2.9/sharingiscaring/grpcclient/concordium/health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/concordium/health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.880919 sharingiscaring-0.2.9/sharingiscaring/grpcclient/concordium/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)   221467 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/concordium/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/health_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.880919 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetAccountInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetAccountList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetAnonymityRevokers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBakerList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlockInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlockPendingUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlockSpecialEvents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34853 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlockTransactionEvents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlocksAtHeight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetFinalizedBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetIdentityProviders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetInstanceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetInstanceList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPassiveDelegationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPassiveDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPoolDelegators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPoolDelegatorsRewardPeriod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPoolInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetTokenomicsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_SharedConverters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84238 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105670 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/grpcclient/types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.884919 sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_apy_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_baker_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_search_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_store_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/tooter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45046 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/sharingiscaring/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.868919 sharingiscaring-0.2.9/sharingiscaring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-04 11:18:24.000000 sharingiscaring-0.2.9/sharingiscaring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-04 11:18:24.000000 sharingiscaring-0.2.9/sharingiscaring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 11:18:24.000000 sharingiscaring-0.2.9/sharingiscaring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-04 11:18:24.000000 sharingiscaring-0.2.9/sharingiscaring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 11:18:24.000000 sharingiscaring-0.2.9/sharingiscaring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:24.884919 sharingiscaring-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/tests/test_namehash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/tests/test_txs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-04 11:18:13.000000 sharingiscaring-0.2.9/tests/test_user.py
```

### Comparing `sharingiscaring-0.2.80/setup.py` & `sharingiscaring-0.2.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="sharingiscaring",
-    version="0.2.80",
+    version="0.2.9",
     author="Sander de Ruiter",
     author_email="sdr@concordium-explorer.nl",
     description="Shared code for Concordium Explorer (Bot)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sderuiter/sharingiscaring",
     project_urls={},
@@ -19,16 +19,14 @@
     install_requires=[
         "rich",
         "python-dateutil",
         "base58",
         "eth-hash",
         "pycryptodome",
         "pytest",
-        "leb128",
-        "pydantic==1.*",
+        "pydantic",
         "pymongo",
-        "motor",
         "requests",
         "apprise",
         "py-graphql-client",
     ],
 )
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/CCD_Types/__init__.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/CCD_Types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,14 @@
     na = "0"
     Passport = "1"
     National_ID_Card = "2"
     Driving_License = "3"
     Immigration_Card = "4"
 
 
-class ProtocolVersions(Enum):
-    PROTOCOL_VERSION_1 = 0
-    PROTOCOL_VERSION_2 = 1
-    PROTOCOL_VERSION_3 = 2
-    PROTOCOL_VERSION_4 = 3
-    PROTOCOL_VERSION_5 = 4
-    PROTOCOL_VERSION_6 = 5
-
-
 class OpenStatus(Enum):
     open_for_all = 0
     closed_for_new = 1
     closed_for_all = 2
 
 
 CCD_ArIdentity = int
@@ -61,15 +52,14 @@
 CCD_TransactionHash = str
 CCD_AccountAddress = str
 CCD_AccountIndex = int
 CCD_DelegatorId = CCD_AccountIndex
 microCCD = int
 CCD_BakerId = int
 CCD_Epoch = int
-CCD_Energy = int
 CCD_DurationSeconds = int
 CCD_ModuleRef = str
 CCD_ContractEvent = str
 CCD_Memo = str
 CCD_RegisteredData = str
 CCD_BakerSignatureVerifyKey = str
 CCD_OpenStatus = int
@@ -89,16 +79,14 @@
 CCD_TransactionTime = int
 CCD_SignatureThreshold = int
 CCD_IdentityProviderIdentity = int
 CCD_ArThreshold = int
 CCD_Commitment = str
 CCD_VersionedModuleSource_ModuleSourceV0 = str
 CCD_VersionedModuleSource_ModuleSourceV1 = str
-CCD_ProtocolVersion = int
-CCD_StateHash = str
 
 CCD_SequenceNumber = int
 CCD_StakePendingChange_Remove = dt.datetime
 CCD_ContractStateV0 = str
 CCD_InitName = str
 CCD_EncryptedAmount = str
 CCD_Empty = None
@@ -109,37 +97,14 @@
 #     value: str
 
 
 class CCD_ContractAddress(BaseModel):
     index: int
     subindex: int
 
-    def to_str(self):
-        return f"<{self.index},{self.subindex}>"
-
-    @classmethod
-    def from_str(self, str_repr: str):
-        """
-        Returns a CCD_ContractAddress when the input is formed as '<2350,0>'.
-        """
-        contract_string = str_repr.split("-")[0]
-        c = CCD_ContractAddress(
-            **{
-                "index": contract_string.split(",")[0][1:],
-                "subindex": contract_string.split(",")[1][:-1],
-            }
-        )
-
-        return c
-
-    @classmethod
-    def from_index(self, index: int, subindex: int):
-        s = CCD_ContractAddress(**{"index": index, "subindex": subindex})
-        return s
-
 
 class CCD_Address(BaseModel):
     account: CCD_AccountAddress = None
     contract: CCD_ContractAddress = None
 
 
 class CCD_RejectReason_InvalidInitMethod(BaseModel):
@@ -334,16 +299,14 @@
     era_block_height: int
     finalized: bool
     genesis_index: int
     transaction_count: int
     transactions_energy_cost: int
     transactions_size: int
     transaction_hashes: list[CCD_TransactionHash] = None
-    state_hash: CCD_StateHash = None
-    protocol_version: CCD_ProtocolVersion = None
 
 
 class CCD_AccountTransactionEffects_None(BaseModel):
     transaction_type: int = None
     reject_reason: CCD_RejectReason
 
 
@@ -1157,31 +1120,7 @@
     level1_keys: CCD_HigherLevelKeys
     level2_keys: CCD_AuthorizationsV1
 
 
 class CCD_ChainParameters(BaseModel):
     v0: CCD_ChainParametersV0 = None
     v1: CCD_ChainParametersV1 = None
-
-
-class CCD_InvokeInstanceResponse_Success(BaseModel):
-    return_value: bytes
-    used_energy: CCD_Energy
-    effects: list[CCD_ContractTraceElement]
-
-
-class CCD_InvokeInstanceResponse_Failure(BaseModel):
-    return_value: bytes
-    used_energy: CCD_Energy
-    reason: CCD_RejectReason
-
-
-class CCD_InvokeInstanceResponse(BaseModel):
-    success: CCD_InvokeInstanceResponse_Success
-    failure: CCD_InvokeInstanceResponse_Failure
-
-
-class CCD_BlockComplete(BaseModel):
-    block_info: CCD_BlockInfo
-    transaction_summaries: list[CCD_BlockItemSummary]
-    special_events: list[CCD_BlockSpecialEvent]
-    net: str = None
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/concordium/health/__init__.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/concordium/health/__init__.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/concordium/v2/__init__.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/concordium/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/health_pb2.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/health_pb2.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/health_pb2_grpc.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/health_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-import sharingiscaring.GRPCClient.health_pb2 as health__pb2
+import health_pb2 as health__pb2
 
 
 class HealthStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Check = channel.unary_unary(
-            "/concordium.health.Health/Check",
-            request_serializer=health__pb2.NodeHealthRequest.SerializeToString,
-            response_deserializer=health__pb2.NodeHealthResponse.FromString,
-        )
+                '/concordium.health.Health/Check',
+                request_serializer=health__pb2.NodeHealthRequest.SerializeToString,
+                response_deserializer=health__pb2.NodeHealthResponse.FromString,
+                )
 
 
 class HealthServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Check(self, request, context):
         """Check the health of the node. By necessity this involves a number of
@@ -35,57 +35,44 @@
 
         If possible the client should use other queries to get a more fine-grained
         understanding of the node health. However this endpoint should provide a
         reasonable default and is usable in cases where an automatic check is
         performed that does not allow for configuration, such as in load-balancers.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_HealthServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "Check": grpc.unary_unary_rpc_method_handler(
-            servicer.Check,
-            request_deserializer=health__pb2.NodeHealthRequest.FromString,
-            response_serializer=health__pb2.NodeHealthResponse.SerializeToString,
-        ),
+            'Check': grpc.unary_unary_rpc_method_handler(
+                    servicer.Check,
+                    request_deserializer=health__pb2.NodeHealthRequest.FromString,
+                    response_serializer=health__pb2.NodeHealthResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "concordium.health.Health", rpc_method_handlers
-    )
+            'concordium.health.Health', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class Health(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Check(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def Check(request,
             target,
-            "/concordium.health.Health/Check",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/concordium.health.Health/Check',
             health__pb2.NodeHealthRequest.SerializeToString,
             health__pb2.NodeHealthResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetAccountInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetAccountInfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.json_format import MessageToJson, MessageToDict
 from google.protobuf import message
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 import os
 import sys
-from sharingiscaring.enums import NET
 
 sys.path.append(os.path.dirname("sharingiscaring"))
 from sharingiscaring.GRPCClient.CCD_Types import *
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.concordium.v2 import AccountInfo
 
 
 class Mixin(_SharedConverters):
     def convertKeysEntry(self, message) -> dict[str, CCD_AccountVerifyKey]:
         entry_dict = {}
         for index, entry in message.items():
+
             converted_value = self.convertType(entry)
             entry_dict[str(index)] = CCD_AccountVerifyKey(
                 **{"ed25519_key": converted_value}
             )
 
         return entry_dict
 
     def convertArData(self, message) -> dict[str, CCD_ChainArData]:
         entry_dict = {}
         for index, entry in message.items():
+
             converted_value = self.convertType(entry)
             entry_dict[str(index)] = CCD_ChainArData(
                 **{"enc_id_cred_pub_share": converted_value}
             )
 
         return entry_dict
 
@@ -249,39 +250,32 @@
 
                     elif type(value) == StakePendingChange:
                         result[key] = self.convertPendingChange(value)
 
             return CCD_AccountStakingInfo(**{which_one: result})
 
     def get_account_info(
-        self: GRPCClient,
-        block_hash: str,
-        hex_address: str = None,
-        account_index: int = None,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str, hex_address: str = None, baker_id: int = None
     ) -> CCD_AccountInfo:
         blockHashInput = self.generate_block_hash_input_from(block_hash)
-        if account_index is not None:
+        if baker_id is not None:
             accountIdentifierInput = (
-                self.generate_account_identifier_input_from_account_index(account_index)
+                self.generate_account_identifier_input_from_baker_id(baker_id)
             )
         elif hex_address:
             accountIdentifierInput = self.generate_account_identifier_input_from(
                 hex_address
             )
 
         account_info = AccountInfoRequest(
             block_hash=blockHashInput, account_identifier=accountIdentifierInput
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value = self.stub_mainnet.GetAccountInfo(request=account_info)
-        else:
-            grpc_return_value = self.stub_testnet.GetAccountInfo(request=account_info)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value = self.stub.GetAccountInfo(request=account_info)
 
         result = {}
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetAccountList.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBakerList.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
-import sys
 from sharingiscaring.GRPCClient.CCD_Types import *
-from sharingiscaring.enums import NET
 from typing import TYPE_CHECKING
+import sys
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 
 
 class Mixin(_SharedConverters):
-    def get_account_list(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_AccountAddress]:
+    def get_baker_list(self: GRPCClient, block_hash: str) -> list[CCD_BakerId]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                AccountAddress
-            ] = self.stub_mainnet.GetAccountList(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                AccountAddress
-            ] = self.stub_testnet.GetAccountList(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[BakerId] = self.stub.GetBakerList(
+            request=blockHashInput
+        )
+
+        for baker in list(grpc_return_value):
 
-        for account in list(grpc_return_value):
-            result.append(self.convertType(account))
+            result.append(self.convertType(baker))
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetAnonymityRevokers.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetInstanceList.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
-import sys
-from sharingiscaring.GRPCClient.CCD_Types import *
-from sharingiscaring.enums import NET
 from typing import TYPE_CHECKING
+import sys
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
+from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
-    def get_anonymity_revokers(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_ArInfo]:
+    def get_instance_list(self: GRPCClient, block_hash: str) -> list[CCD_BakerId]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                ArInfo
-            ] = self.stub_mainnet.GetAnonymityRevokers(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                ArInfo
-            ] = self.stub_testnet.GetAnonymityRevokers(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[ContractAddress] = self.stub.GetInstanceList(
+            request=blockHashInput
+        )
+
+        for instance in list(grpc_return_value):
 
-        for ar in list(grpc_return_value):
-            result.append(self.convertArInfo(ar))
+            result.append(self.convertType(instance))
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBakerList.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetInstanceList.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
-from sharingiscaring.GRPCClient.CCD_Types import *
-from sharingiscaring.enums import NET
 from typing import TYPE_CHECKING
 import sys
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
+from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
-    def get_baker_list(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_BakerId]:
+    def get_instance_list(self: GRPCClient, block_hash: str) -> list[CCD_BakerId]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[BakerId] = self.stub_mainnet.GetBakerList(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value: Iterator[BakerId] = self.stub_testnet.GetBakerList(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[ContractAddress] = self.stub.GetInstanceList(
+            request=blockHashInput
+        )
+
+        for instance in list(grpc_return_value):
 
-        for baker in list(grpc_return_value):
-            result.append(self.convertType(baker))
+            result.append(self.convertType(instance))
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockChainParameters.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockChainParameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
@@ -156,31 +155,24 @@
 
             elif type(value) == AuthorizationsV1:
                 result[key] = self.convertAuthorizationsV1(value)
 
         return CCD_ChainParametersV1(**result)
 
     def get_block_chain_parameters(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> CCD_ChainParameters:
         result = {}
 
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: ChainParameters = (
-                self.stub_mainnet.GetBlockChainParameters(request=blockHashInput)
-            )
-        else:
-            grpc_return_value: ChainParameters = (
-                self.stub_testnet.GetBlockChainParameters(request=blockHashInput)
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: ChainParameters = self.stub.GetBlockChainParameters(
+            request=blockHashInput
+        )
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
             if key == "v0" and not self.valueIsEmpty(value):
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockInfo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,42 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 
 # from sharingiscaring.GRPCClient import GRPCClient
 import os
 import sys
 import grpc
 
 sys.path.append(os.path.dirname("sharingiscaring"))
-from sharingiscaring.GRPCClient.CCD_Types import CCD_BlockInfo, ProtocolVersions
+from sharingiscaring.GRPCClient.CCD_Types import CCD_BlockInfo
 from sharingiscaring.GRPCClient.concordium.v2 import BlockInfo as BP_BlockInfo
 
 
 class Mixin(_SharedConverters):
-    def get_block_info(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> CCD_BlockInfo:
+    def get_block_info(self: GRPCClient, block_hash: str) -> CCD_BlockInfo:
         result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: BlockInfo = self.stub_mainnet.GetBlockInfo(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value: BlockInfo = self.stub_testnet.GetBlockInfo(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: BlockInfo = self.stub.GetBlockInfo(request=blockHashInput)
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
-            if key == "protocol_version":
-                result[key] = ProtocolVersions(value).name
-
-            elif type(value) in self.simple_types:
+            if type(value) in self.simple_types:
                 result[f"{key}"] = self.convertType(value)
 
         # TODO: fix for BakerId always producing 0
         # even when it's not set (as is the case for genesis blocks)
         if result["era_block_height"] == 0:
             result["baker"] = None
         return CCD_BlockInfo(**result)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockPendingUpdates.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockPendingUpdates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
@@ -51,29 +50,20 @@
 
                     elif type(value) in self.simple_types:
                         result[key] = self.convertType(value)
 
             return CCD_UpdateDetails(**result), _type
 
     def get_block_pending_updates(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> list[CCD_BlockSpecialEvent]:
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value = self.stub_mainnet.GetBlockPendingUpdates(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value = self.stub_testnet.GetBlockPendingUpdates(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value = self.stub.GetBlockPendingUpdates(request=blockHashInput)
 
         events = []
         for tx in list(grpc_return_value):
             result = {}
             for descriptor in tx.DESCRIPTOR.fields:
                 key, value = self.get_key_value_from_descriptor(descriptor, tx)
                 if self.valueIsEmpty(value):
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlockSpecialEvents.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlockSpecialEvents.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
@@ -79,29 +78,20 @@
 
             elif type(value) in self.simple_types:
                 result[key] = self.convertType(value)
 
         return CCD_BlockSpecialEvent_FinalizationRewards(**result)
 
     def get_block_special_events(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> list[CCD_BlockSpecialEvent]:
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value = self.stub_mainnet.GetBlockSpecialEvents(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value = self.stub_testnet.GetBlockSpecialEvents(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value = self.stub.GetBlockSpecialEvents(request=blockHashInput)
 
         events = []
         for tx in list(grpc_return_value):
             result = {}
             for descriptor in tx.DESCRIPTOR.fields:
                 key, value = self.get_key_value_from_descriptor(descriptor, tx)
                 if self.valueIsEmpty(value):
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetBlocksAtHeight.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetBlocksAtHeight.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
@@ -17,52 +15,41 @@
 sys.path.append(os.path.dirname("sharingiscaring"))
 from sharingiscaring.GRPCClient.CCD_Types import CCD_BlockInfo, CCD_BlockHash
 from sharingiscaring.GRPCClient.concordium.v2 import BlockInfo as BP_BlockInfo
 
 
 class Mixin(_SharedConverters):
     def get_blocks_at_height(
-        self: GRPCClient,
-        block_height: int,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_height: int
     ) -> list[CCD_BlockHash]:
         result = []
         absoluteBlockHeight = AbsoluteBlockHeight(value=block_height)
         blocksAtHeightRequestAbsolute = BlocksAtHeightRequest.Absolute(
             height=absoluteBlockHeight
         )
         blocksAtHeightRequest = BlocksAtHeightRequest(
             absolute=blocksAtHeightRequestAbsolute
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                BlocksAtHeightResponse
-            ] = self.stub_mainnet.GetBlocksAtHeight(request=blocksAtHeightRequest)
-        else:
-            grpc_return_value: Iterator[
-                BlocksAtHeightResponse
-            ] = self.stub_testnet.GetBlocksAtHeight(request=blocksAtHeightRequest)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[
+            BlocksAtHeightResponse
+        ] = self.stub.GetBlocksAtHeight(request=blocksAtHeightRequest)
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
             if key == "blocks":
                 result = self.convertList(value)
 
         return result
 
-    def get_finalized_block_at_height(
-        self,
-        block_height: int,
-        net: Enum = NET.MAINNET,
-    ) -> CCD_BlockInfo:
-        blocks_at_height = self.get_blocks_at_height(block_height, net)
+    def get_finalized_block_at_height(self, block_height: int) -> CCD_BlockInfo:
+        blocks_at_height = self.get_blocks_at_height(block_height)
         for block_hash in blocks_at_height:
-            bi: CCD_BlockInfo = self.get_block_info(block_hash, net)
+            bi: CCD_BlockInfo = self.get_block_info(block_hash)
             if bi.finalized:
                 return bi
 
         return None
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetElectionInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetElectionInfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from enum import Enum
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
@@ -25,31 +24,22 @@
         for list_entry in message:
             bakers.append(
                 CCD_ElectionInfo_Baker(**self.convertTypeWithSingleValues(list_entry))
             )
 
         return bakers
 
-    def get_election_info(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> CCD_ElectionInfo:
+    def get_election_info(self: GRPCClient, block_hash: str) -> CCD_ElectionInfo:
         result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: ElectionInfo = self.stub_mainnet.GetElectionInfo(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value: ElectionInfo = self.stub_testnet.GetElectionInfo(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: ElectionInfo = self.stub.GetElectionInfo(
+            request=blockHashInput
+        )
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
             if type(value) in self.simple_types:
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetFinalizedBlocks.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetFinalizedBlocks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
 from typing import TYPE_CHECKING
 import sys
@@ -23,18 +22,12 @@
             key, value = self.get_key_value_from_descriptor(descriptor, block)
 
             if type(value) in self.simple_types:
                 result[key] = self.convertType(value)
 
         return CCD_FinalizedBlockInfo(**result)
 
-    def get_finalized_blocks(
-        self: GRPCClient,
-        net: Enum = NET.MAINNET,
-    ) -> CCD_FinalizedBlockInfo:
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            for block in self.stub_mainnet.GetFinalizedBlocks(request=Empty()):
-                print(self.convertFinalizedBlock(block))
-        else:
-            for block in self.stub_testnet.GetFinalizedBlocks(request=Empty()):
-                print(self.convertFinalizedBlock(block))
+    def get_finalized_blocks(self: GRPCClient) -> CCD_FinalizedBlockInfo:
+
+        self.check_connection(sys._getframe().f_code.co_name)
+        for block in self.stub.GetFinalizedBlocks(request=Empty()):
+            print(self.convertFinalizedBlock(block))
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetIdentityProviders.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPassiveDelegationInfo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 from __future__ import annotations
-from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
+from sharingiscaring.GRPCClient.types_pb2 import *
+from enum import Enum
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
+import os
 import sys
-from typing import Iterator
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
+from rich import print
+
+sys.path.append(os.path.dirname("sharingiscaring"))
 from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
-    def get_identity_providers(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_IpInfo]:
-        result = []
+    def get_passive_delegation_info(
+        self: GRPCClient, block_hash: str
+    ) -> CCD_PassiveDelegationInfo:
+        prefix = ""
+        result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                IpInfo
-            ] = self.stub_mainnet.GetIdentityProviders(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                IpInfo
-            ] = self.stub_testnet.GetIdentityProviders(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: PoolInfoResponse = self.stub.GetPassiveDelegationInfo(
+            request=blockHashInput
+        )
+
+        for descriptor in grpc_return_value.DESCRIPTOR.fields:
+            key, value = self.get_key_value_from_descriptor(
+                descriptor, grpc_return_value
+            )
+            key_to_store = f"{prefix}{key}"
+            if type(value) in self.simple_types:
+                result[key_to_store] = self.convertType(value)
 
-        for ip in list(grpc_return_value):
-            result.append(self.convertIpInfo(ip))
+            elif type(value) == CommissionRates:
+                result[key] = self.convertCommissionRates(value)
 
-        return result
+        return CCD_PassiveDelegationInfo(**result)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetInstanceInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetInstanceInfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
@@ -16,14 +15,15 @@
 from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
     def convertMethods(self, message) -> list[CCD_ReceiveName]:
         methods = []
         for method in message:
+
             for descriptor in method.DESCRIPTOR.fields:
                 _, value = self.get_key_value_from_descriptor(descriptor, method)
 
                 methods.append(self.convertType(value))
 
         return methods
 
@@ -50,34 +50,26 @@
 
             elif key == "methods":
                 result[key] = self.convertMethods(value)
 
         return CCD_InstanceInfo_V1(**result)
 
     def get_instance_info(
-        self: GRPCClient,
-        contract_index: int,
-        contract_sub_index: int,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, contract_index: int, contract_sub_index: int, block_hash: str
     ) -> CCD_InstanceInfo:
+
         result = {}
         instanceInfoRequest = self.generate_instance_info_request_from(
             contract_index, contract_sub_index, block_hash
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: InstanceInfo = self.stub_mainnet.GetInstanceInfo(
-                request=instanceInfoRequest
-            )
-        else:
-            grpc_return_value: InstanceInfo = self.stub_testnet.GetInstanceInfo(
-                request=instanceInfoRequest
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: InstanceInfo = self.stub.GetInstanceInfo(
+            request=instanceInfoRequest
+        )
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
             if type(value) == InstanceInfo.V0:
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetInstanceList.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBakerList.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
+from sharingiscaring.GRPCClient.CCD_Types import *
 from typing import TYPE_CHECKING
 import sys
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
-from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
-    def get_instance_list(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_BakerId]:
+    def get_baker_list(self: GRPCClient, block_hash: str) -> list[CCD_BakerId]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                ContractAddress
-            ] = self.stub_mainnet.GetInstanceList(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                ContractAddress
-            ] = self.stub_testnet.GetInstanceList(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[BakerId] = self.stub.GetBakerList(
+            request=blockHashInput
+        )
+
+        for baker in list(grpc_return_value):
 
-        for instance in list(grpc_return_value):
-            result.append(self.convertType(instance))
+            result.append(self.convertType(baker))
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetModuleSource.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetModuleSource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
@@ -16,14 +15,15 @@
 from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
     def convertMethods(self, message) -> list[CCD_ReceiveName]:
         methods = []
         for method in message:
+
             for descriptor in method.DESCRIPTOR.fields:
                 _, value = self.get_key_value_from_descriptor(descriptor, method)
 
                 methods.append(self.convertType(value))
 
         return methods
 
@@ -50,35 +50,28 @@
 
             elif key == "methods":
                 result[key] = self.convertMethods(value)
 
         return CCD_InstanceInfo_V1(**result)
 
     def get_module_source(
-        self: GRPCClient,
-        module_ref: CCD_ModuleRef,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, module_ref: CCD_ModuleRef, block_hash: str
     ) -> CCD_VersionedModuleSource:
+
         result = {}
         moduleSourceRequest = self.generate_module_source_request_from(
             module_ref, block_hash
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: InstanceInfo = self.stub_mainnet.GetModuleSource(
-                request=moduleSourceRequest
-            )
-        else:
-            grpc_return_value: InstanceInfo = self.stub_testnet.GetModuleSource(
-                request=moduleSourceRequest
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: InstanceInfo = self.stub.GetModuleSource(
+            request=moduleSourceRequest
+        )
 
-        for field, value in grpc_return_value.ListFields():
+        for (field, value) in grpc_return_value.ListFields():
             key = field.name
             if type(value) in [
                 VersionedModuleSource.ModuleSourceV0,
                 VersionedModuleSource.ModuleSourceV1,
             ]:
                 result[key] = self.convertType(value)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPassiveDelegationInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPassiveDelegationInfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from enum import Enum
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 import os
 import sys
 from typing import TYPE_CHECKING
@@ -16,31 +15,24 @@
 
 sys.path.append(os.path.dirname("sharingiscaring"))
 from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
     def get_passive_delegation_info(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> CCD_PassiveDelegationInfo:
         prefix = ""
         result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: PoolInfoResponse = (
-                self.stub_mainnet.GetPassiveDelegationInfo(request=blockHashInput)
-            )
-        else:
-            grpc_return_value: PoolInfoResponse = (
-                self.stub_testnet.GetPassiveDelegationInfo(request=blockHashInput)
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: PoolInfoResponse = self.stub.GetPassiveDelegationInfo(
+            request=blockHashInput
+        )
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
             key_to_store = f"{prefix}{key}"
             if type(value) in self.simple_types:
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPassiveDelegators.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPassiveDelegators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
 from typing import TYPE_CHECKING
 import sys
@@ -13,32 +11,26 @@
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.CCD_Types import CCD_DelegatorInfo
 
 
 class Mixin(_SharedConverters):
     def get_delegators_for_passive_delegation(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> list[CCD_DelegatorInfo]:
         result: list[CCD_DelegatorInfo] = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                DelegatorInfo
-            ] = self.stub_mainnet.GetPassiveDelegators(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                DelegatorInfo
-            ] = self.stub_testnet.GetPassiveDelegators(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[DelegatorInfo] = self.stub.GetPassiveDelegators(
+            request=blockHashInput
+        )
 
         for delegator in list(grpc_return_value):
+
             delegator_dict = {
                 "account": self.convertAccountAddress(delegator.account),
                 "stake": self.convertAmount(delegator.stake),
             }
             if delegator.pending_change:
                 if self.valueIsEmpty(delegator.pending_change):
                     pass
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
 from sharingiscaring.GRPCClient.CCD_Types import CCD_DelegatorRewardPeriodInfo
 from typing import TYPE_CHECKING
@@ -13,36 +11,26 @@
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 
 
 class Mixin(_SharedConverters):
     def get_delegators_for_passive_delegation_in_reward_period(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> list[CCD_DelegatorRewardPeriodInfo]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                DelegatorInfo
-            ] = self.stub_mainnet.GetPassiveDelegatorsRewardPeriod(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value: Iterator[
-                DelegatorInfo
-            ] = self.stub_testnet.GetPassiveDelegatorsRewardPeriod(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[
+            DelegatorInfo
+        ] = self.stub.GetPassiveDelegatorsRewardPeriod(request=blockHashInput)
 
         for delegator in list(grpc_return_value):
+
             result.append(
                 CCD_DelegatorRewardPeriodInfo(
                     **{
                         "account": self.convertAccountAddress(delegator.account),
                         "stake": self.convertAmount(delegator.stake),
                     }
                 )
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPoolDelegators.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,43 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
 from typing import TYPE_CHECKING
 import sys
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
-from sharingiscaring.GRPCClient.CCD_Types import CCD_DelegatorInfo
+from sharingiscaring.GRPCClient.CCD_Types import CCD_DelegatorRewardPeriodInfo
 
 
 class Mixin(_SharedConverters):
-    def get_delegators_for_pool(
-        self: GRPCClient,
-        pool_id: int,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_DelegatorInfo]:
+    def get_delegators_for_pool_in_reward_period(
+        self: GRPCClient, pool_id: int, block_hash: str
+    ) -> list[CCD_DelegatorRewardPeriodInfo]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
         baker_id = BakerId(value=pool_id)
         delegatorsRequest = GetPoolDelegatorsRequest(
             baker=baker_id, block_hash=blockHashInput
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                DelegatorInfo
-            ] = self.stub_mainnet.GetPoolDelegators(request=delegatorsRequest)
-        else:
-            grpc_return_value: Iterator[
-                DelegatorInfo
-            ] = self.stub_testnet.GetPoolDelegators(request=delegatorsRequest)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[
+            DelegatorRewardPeriodInfo
+        ] = self.stub.GetPoolDelegatorsRewardPeriod(request=delegatorsRequest)
 
         for delegator in list(grpc_return_value):
-            delegator_dict = {
-                "account": self.convertAccountAddress(delegator.account),
-                "stake": self.convertAmount(delegator.stake),
-            }
-            if delegator.pending_change:
-                if self.valueIsEmpty(delegator.pending_change):
-                    pass
-                else:
-                    delegator_dict.update(
-                        {
-                            "pending_change": self.convertPendingChange(
-                                delegator.pending_change
-                            )
-                        }
-                    )
 
-            result.append(CCD_DelegatorInfo(**delegator_dict))
+            result.append(
+                CCD_DelegatorRewardPeriodInfo(
+                    **{
+                        "account": self.convertAccountAddress(delegator.account),
+                        "stake": self.convertAmount(delegator.stake),
+                    }
+                )
+            )
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPoolDelegatorsRewardPeriod.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
 from typing import TYPE_CHECKING
 import sys
@@ -13,41 +11,30 @@
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.CCD_Types import CCD_DelegatorRewardPeriodInfo
 
 
 class Mixin(_SharedConverters):
     def get_delegators_for_pool_in_reward_period(
-        self: GRPCClient,
-        pool_id: int,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, pool_id: int, block_hash: str
     ) -> list[CCD_DelegatorRewardPeriodInfo]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
         baker_id = BakerId(value=pool_id)
         delegatorsRequest = GetPoolDelegatorsRequest(
             baker=baker_id, block_hash=blockHashInput
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                DelegatorRewardPeriodInfo
-            ] = self.stub_mainnet.GetPoolDelegatorsRewardPeriod(
-                request=delegatorsRequest
-            )
-        else:
-            grpc_return_value: Iterator[
-                DelegatorRewardPeriodInfo
-            ] = self.stub_testnet.GetPoolDelegatorsRewardPeriod(
-                request=delegatorsRequest
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[
+            DelegatorRewardPeriodInfo
+        ] = self.stub.GetPoolDelegatorsRewardPeriod(request=delegatorsRequest)
 
         for delegator in list(grpc_return_value):
+
             result.append(
                 CCD_DelegatorRewardPeriodInfo(
                     **{
                         "account": self.convertAccountAddress(delegator.account),
                         "stake": self.convertAmount(delegator.stake),
                     }
                 )
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetPoolInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPoolInfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from enum import Enum
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 import os
 import sys
 from rich import print
@@ -18,34 +17,26 @@
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 
 
 class Mixin(_SharedConverters):
     def get_pool_info_for_pool(
-        self: GRPCClient,
-        pool_id: int,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, pool_id: int, block_hash: str
     ) -> CCD_PoolInfo:
         prefix = ""
         result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
         baker_id = BakerId(value=pool_id)
         poolInfoRequest = PoolInfoRequest(baker=baker_id, block_hash=blockHashInput)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: PoolInfoResponse = self.stub_mainnet.GetPoolInfo(
-                request=poolInfoRequest
-            )
-        else:
-            grpc_return_value: PoolInfoResponse = self.stub_testnet.GetPoolInfo(
-                request=poolInfoRequest
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: PoolInfoResponse = self.stub.GetPoolInfo(
+            request=poolInfoRequest
+        )
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
             key_to_store = f"{prefix}{key}"
             if type(value) in self.simple_types:
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_GetTokenomicsInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetTokenomicsInfo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from enum import Enum
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from google.protobuf.json_format import MessageToJson, MessageToDict
 import os
 import sys
@@ -46,33 +45,23 @@
                 elif type(value) == MintRate:
                     result[key] = CCD_MintRate(
                         **{"mantissa": value.mantissa, "exponent": value.exponent}
                     )
 
             return CCD_TokenomicsInfo_V1(**result)
 
-    def get_tokenomics_info(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> CCD_TokenomicsInfo:
+    def get_tokenomics_info(self: GRPCClient, block_hash: str) -> CCD_TokenomicsInfo:
         prefix = ""
         result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: BlockInfo = self.stub_mainnet.GetTokenomicsInfo(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value: BlockInfo = self.stub_testnet.GetTokenomicsInfo(
-                request=blockHashInput
-            )
-
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: BlockInfo = self.stub.GetTokenomicsInfo(
+            request=blockHashInput
+        )
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
             if type(value) == TokenomicsInfo.V0:
                 result[f"{prefix}{key}"] = self.convertTokenomicsV0(value)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_InvokeInstance.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetTokenomicsInfo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,71 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from enum import Enum
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
+from google.protobuf.json_format import MessageToJson, MessageToDict
 import os
 import sys
-from rich import print
 
 sys.path.append(os.path.dirname("sharingiscaring"))
 from sharingiscaring.GRPCClient.CCD_Types import *
+from typing import TYPE_CHECKING
 
+if TYPE_CHECKING:
+    from sharingiscaring.GRPCClient import GRPCClient
 
-class Mixin(_SharedConverters):
-    def convertSuccess(self, message) -> CCD_InvokeInstanceResponse_Success:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if key == "effects":
-                result[key] = self.convertUpdateEvents(value)
 
-            elif type(value) in self.simple_types:
-                result[key] = self.convertType(value)
+class Mixin(_SharedConverters):
+    def convertTokenomicsV0(self, message) -> CCD_TokenomicsInfo_V0:
+        if self.valueIsEmpty(message):
+            return None
+        else:
+            result = {}
+            for descriptor in message.DESCRIPTOR.fields:
+                key, value = self.get_key_value_from_descriptor(descriptor, message)
+
+                if type(value) in self.simple_types:
+                    result[key] = self.convertType(value)
+
+            return CCD_TokenomicsInfo_V0(**result)
+
+    def convertTokenomicsV1(self, message) -> CCD_TokenomicsInfo_V1:
+        if self.valueIsEmpty(message):
+            return None
+        else:
+            result = {}
+            for descriptor in message.DESCRIPTOR.fields:
+                key, value = self.get_key_value_from_descriptor(descriptor, message)
+
+                if type(value) in self.simple_types:
+                    result[key] = self.convertType(value)
+
+                elif type(value) == MintRate:
+                    result[key] = CCD_MintRate(
+                        **{"mantissa": value.mantissa, "exponent": value.exponent}
+                    )
 
-        return CCD_InvokeInstanceResponse_Success(**result)
+            return CCD_TokenomicsInfo_V1(**result)
 
-    def convertFailure(self, message) -> CCD_InvokeInstanceResponse_Failure:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) == RejectReason:
-                result[key], _ = self.convertRejectReason(value)
-
-            elif type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-        return CCD_InvokeInstanceResponse_Failure(**result)
-
-    def invoke_instance(
-        self: GRPCClient,
-        block_hash: str,
-        instance_index: int,
-        instance_subindex: int,
-        entrypoint: str,
-        parameter_bytes: bytes,
-        net: Enum = NET.MAINNET,
-    ) -> CCD_InvokeInstanceResponse:
+    def get_tokenomics_info(self: GRPCClient, block_hash: str) -> CCD_TokenomicsInfo:
+        prefix = ""
         result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
-        invokeInstanceRequest = self.generate_invoke_instance_request_from(
-            instance_index,
-            instance_subindex,
-            blockHashInput,
-            entrypoint,
-            parameter_bytes,
-        )
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: InvokeInstanceResponse = (
-                self.stub_mainnet.InvokeInstance(request=invokeInstanceRequest)
-            )
-        else:
-            grpc_return_value: InvokeInstanceResponse = (
-                self.stub_testnet.InvokeInstance(request=invokeInstanceRequest)
-            )
 
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: BlockInfo = self.stub.GetTokenomicsInfo(
+            request=blockHashInput
+        )
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
-            if type(value) == InvokeInstanceResponse.Success:
-                result[key] = self.convertSuccess(value)
-
-            elif type(value) == InvokeInstanceResponse.Failure:
-                result[key] = self.convertFailure(value)
+            if type(value) == TokenomicsInfo.V0:
+                result[f"{prefix}{key}"] = self.convertTokenomicsV0(value)
+            elif type(value) == TokenomicsInfo.V1:
+                result[f"{prefix}{key}"] = self.convertTokenomicsV1(value)
 
-        return CCD_InvokeInstanceResponse(**result)
+        return CCD_TokenomicsInfo(**result)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/queries/_SharedConverters.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_SharedConverters.py`

 * *Files 25% similar despite different names*

```diff
@@ -123,98 +123,54 @@
             bin_value = base58.b58decode_check(hex_address)[1:]
             address = AccountAddress(value=bin_value)
             account = AccountIdentifierInput(address=address)
             return account
         except:  # pragma: no cover
             return None
 
-    def generate_account_identifier_input_from_account_index(
-        self, account_index: CCD_AccountIndex
-    ):
+    def generate_account_identifier_input_from_baker_id(self, baker_id: CCD_BakerId):
         try:
-            account = AccountIdentifierInput(
-                account_index=AccountIndex(value=account_index)
-            )
+            account = AccountIdentifierInput(account_index=AccountIndex(value=baker_id))
             return account
         except:  # pragma: no cover
             return None
 
-    def valueIsEmpty(self, value, key=None, message=None):
+    def valueIsEmpty(self, value):
         if type(value) == int:
             return value is None
         else:
             if type(value) == RepeatedCompositeContainer:
                 return False
             else:
                 if hasattr(value, "DESCRIPTOR"):
-                    if message:
-                        l = list(message)
-                        key_in_message = key in l[0].__str__()
-                        if key_in_message:
-                            # special case for baker_id = 0 (doesn't get transmitted in a message)
-                            if key == "baker_removed":
-                                return False
-                            else:
-                                if MessageToDict(value) != {}:
-                                    return False
-                                else:
-                                    return True
-                        return MessageToDict(value) == {}
-                    else:
-                        return MessageToDict(value) == {}
+                    return MessageToDict(value) == {}
                 else:  # pragma: no cover
                     return False
 
-    def generate_block_hash_input_from(self, hex_block_hash: str) -> BlockHashInput:
+    def generate_block_hash_input_from(self, hex_block_hash: str):
         if hex_block_hash == "last_final":
             return BlockHashInput(last_final={})
         else:
             return BlockHashInput(given=BlockHash(value=bytes.fromhex(hex_block_hash)))
 
-    def generate_invoke_instance_request_from(
-        self,
-        contract_index: int,
-        contract_sub_index: int,
-        block_hash_input: str,
-        receive_name: str,
-        parameter_bytes: bytes,
-    ):
-        # parameter_bytes = self.get_bytes_parameter_from_hex(parameter_hex)
-        # if we include a zero subindex, grpc will complain about
-        # LengthDelimited vs VarInt.
-        if contract_sub_index == 0:
-            instance = ContractAddress(index=contract_index)
-        else:
-            instance = ContractAddress(
-                index=contract_index,
-                subindex=contract_sub_index,
-            )
-
-        return InvokeInstanceRequest(
-            block_hash=block_hash_input,
-            amount=Amount(value=0),
-            entrypoint=ReceiveName(value=receive_name),
-            parameter=Parameter(value=parameter_bytes),
-            energy=Energy(value=100_000_000_000),
-            instance=instance,
-        )
-
     def generate_instance_info_request_from(
         self, contract_index: int, contract_sub_index: int, hex_block_hash: str
     ):
+
         return InstanceInfoRequest(
             block_hash=self.generate_block_hash_input_from(hex_block_hash),
             address=ContractAddress(
                 **{"index": contract_index, "subindex": contract_sub_index}
             ),
         )
 
     def generate_module_source_request_from(
         self, module_ref: CCD_ModuleRef, hex_block_hash: str
     ):
+
         return ModuleSourceRequest(
             block_hash=self.generate_block_hash_input_from(hex_block_hash),
             module_ref=ModuleRef(value=bytes.fromhex(module_ref)),
         )
 
     def convertList(self, message):
         entries = []
@@ -439,14 +395,15 @@
                 result[key] = self.convertType(value)
 
         return result
 
     def convertPendingChange_Reduce_Remove(
         self, message
     ) -> CCD_StakePendingChange_Remove:
+
         return self.convertType(message)
 
     def convertPendingChange(self, message) -> CCD_StakePendingChange:
         result = {}
 
         for descriptor in message.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(descriptor, message)
@@ -711,266 +668,7 @@
                     if type(value) == MintRate:
                         result[key] = self.convertMintRate(value)
 
                     elif type(value) == AmountFraction:
                         result[key] = self.convertType(value)
 
         return CCD_MintDistributionCpv0(**result)
-
-    def convertEvents(self, message) -> list:
-        events = []
-        for entry in message:
-            entry_dict = {}
-            for descriptor in entry.DESCRIPTOR.fields:
-                key, value = self.get_key_value_from_descriptor(descriptor, entry)
-                if type(value) in self.simple_types:
-                    converted_value = self.convertType(value)
-                    if converted_value:
-                        # entry_dict[key] = converted_value
-                        events.append(converted_value)
-            # if entry_dict == {}:
-            #         pass
-            # else:
-            #     events.append(entry_dict)
-
-        return events
-
-    def convertInstanceInterruptedEvent(
-        self, message
-    ) -> CCD_ContractTraceElement_Interrupted:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-            if key == "events":
-                result[key] = self.convertEvents(value)
-
-        return CCD_ContractTraceElement_Interrupted(**result)
-
-    def convertInstanceUpdatedEvent(self, message) -> CCD_InstanceUpdatedEvent:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-            if key == "events":
-                result[key] = self.convertEvents(value)
-
-        return CCD_InstanceUpdatedEvent(**result)
-
-    def convertInstanceResumedEvent(self, message) -> CCD_ContractTraceElement_Resumed:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-        return CCD_ContractTraceElement_Resumed(**result)
-
-    def convertInstanceTransferredEvent(
-        self, message
-    ) -> CCD_ContractTraceElement_Transferred:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-        return CCD_ContractTraceElement_Transferred(**result)
-
-    def convertUpdateEvents(self, message) -> list:
-        events = []
-        for entry in message:
-            for descriptor in entry.DESCRIPTOR.fields:
-                entry_dict = {}
-                key, value = self.get_key_value_from_descriptor(descriptor, entry)
-                if MessageToDict(value) == {}:
-                    pass
-                else:
-                    if type(value) == InstanceUpdatedEvent:
-                        entry_dict[key] = self.convertInstanceUpdatedEvent(value)
-
-                    if type(value) == ContractTraceElement.Interrupted:
-                        entry_dict[key] = self.convertInstanceInterruptedEvent(value)
-
-                    if type(value) == ContractTraceElement.Resumed:
-                        entry_dict[key] = self.convertInstanceResumedEvent(value)
-
-                    if type(value) == ContractTraceElement.Transferred:
-                        entry_dict[key] = self.convertInstanceTransferredEvent(value)
-
-                if entry_dict == {}:
-                    pass
-                else:
-                    events.append(entry_dict)
-
-        return events
-
-    def convertCredentialRegistrationIdEntries(self, message):
-        entries = []
-
-        for list_entry in message:
-            entries.append(self.convertType(list_entry))
-
-        return entries
-
-    def convertDuplicateCredIds(self, message) -> CCD_RejectReason_DuplicateCredIds:
-        result = {}
-
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-
-            result[key] = self.convertCredentialRegistrationIdEntries(value)
-
-        return CCD_RejectReason_DuplicateCredIds(**result)
-
-    def convertRejectReason(self, message) -> CCD_RejectReason:
-        result = {}
-        _type = None
-        for field, value in message.ListFields():
-            key = field.name
-
-            # Note this next section is purely to have Coverage
-            # show us that we have not covered all possible reject
-            # reasons with adequate tests...
-            if key == "module_not_wf":
-                test_me_please = True
-            if key == "module_hash_already_exists":
-                test_me_please = True
-            if key == "invalid_account_reference":
-                test_me_please = True
-            if key == "invalid_init_method":
-                test_me_please = True
-            if key == "invalid_receive_method":
-                test_me_please = True
-            if key == "invalid_module_reference":
-                test_me_please = True
-            if key == "invalid_contract_address":
-                test_me_please = True
-            if key == "runtime_failure":
-                test_me_please = True
-            if key == "amount_too_large":
-                test_me_please = True
-            if key == "serialization_failure":
-                test_me_please = True
-            if key == "out_of_energy":
-                test_me_please = True
-            if key == "rejected_init":
-                test_me_please = True
-            if key == "rejected_receive":
-                test_me_please = True
-            if key == "invalid_proof":
-                test_me_please = True
-            if key == "already_a_baker: ":
-                test_me_please = True
-            if key == "not_a_baker":
-                test_me_please = True
-            if key == "insufficient_balance_for_baker_stake":
-                test_me_please = True
-            if key == "stake_under_minimum_threshold_for_baking":
-                test_me_please = True
-            if key == "baker_in_cooldown":
-                test_me_please = True
-            if key == "duplicate_aggregation_key":
-                test_me_please = True
-            if key == "non_existent_credential_id":
-                test_me_please = True
-            if key == "key_index_already_in_use":
-                test_me_please = True
-            if key == "invalid_account_threshold":
-                test_me_please = True
-            if key == "invalid_credential_key_sign_threshold":
-                test_me_please = True
-            if key == "invalid_encrypted_amount_transfer_proof":
-                test_me_please = True
-            if key == "invalid_transfer_to_public_proof":
-                test_me_please = True
-            if key == "encrypted_amount_self_transfer":
-                test_me_please = True
-            if key == "invalid_index_on_encrypted_transfer":
-                test_me_please = True
-            if key == "zero_scheduledAmount":
-                test_me_please = True
-            if key == "non_increasing_schedule":
-                test_me_please = True
-            if key == "first_scheduled_release_expired":
-                test_me_please = True
-            if key == "scheduled_self_transfer":
-                test_me_please = True
-            if key == "invalid_credentials":
-                test_me_please = True
-            if key == "duplicate_cred_ids":
-                test_me_please = True
-            if key == "non_existent_cred_ids":
-                test_me_please = True
-            if key == "remove_first_credential":
-                test_me_please = True
-            if key == "credential_holder_did_not_sign":
-                test_me_please = True
-            if key == "not_allowed_multiple_credentials":
-                test_me_please = True
-            if key == "not_allowed_to_receive_encrypted":
-                test_me_please = True
-            if key == "not_allowed_to_handle_encrypted":
-                test_me_please = True
-            if key == "missing_baker_add_parameters":
-                test_me_please = True
-            if key == "finalization_reward_commission_not_in_range":
-                test_me_please = True
-            if key == "baking_reward_commission_not_in_range":
-                test_me_please = True
-            if key == "transaction_fee_commission_not_in_range":
-                test_me_please = True
-            if key == "already_a_delegator":
-                test_me_please = True
-            if key == "insufficient_balance_for_delegation_stake":
-                test_me_please = True
-            if key == "missing_delegation_add_parameters":
-                test_me_please = True
-            if key == "insufficient_delegation_stak":
-                test_me_please = True
-            if key == "delegator_in_cooldown":
-                test_me_please = True
-            if key == "not_a_delegator":
-                test_me_please = True
-            if key == "delegation_target_not_a_baker: ":
-                test_me_please = True
-            if key == "stake_over_maximum_threshold_for_pool":
-                test_me_please = True
-            if key == "pool_would_become_over_delegated":
-                test_me_please = True
-            if key == "pool_closed":
-                test_me_please = True
-
-            _type = key
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-            elif type(value) in [
-                RejectReason.InvalidInitMethod,
-                RejectReason.InvalidReceiveMethod,
-                RejectReason.AmountTooLarge,
-                RejectReason.RejectedInit,
-                RejectReason.RejectedReceive,
-            ]:
-                result[key] = self.convertTypeWithSingleValues(value)
-
-            elif type(value) == RejectReason.DuplicateCredIds:
-                result[key] = self.convertDuplicateCredIds(value)
-        return result, _type
-
-    def convertRejectReasonNone(self, message) -> CCD_AccountTransactionEffects_None:
-        result = {}
-        _type = None
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-            elif type(value) == RejectReason:
-                result[key], _type = self.convertRejectReason(value)
-
-        return CCD_AccountTransactionEffects_None(**result), _type
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/service_pb2.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/service_pb2.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/service_pb2_grpc.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/types_pb2.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/GRPCClient/wadze.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/wadze.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/account.py` & `sharingiscaring-0.2.9/sharingiscaring/account.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/block.py` & `sharingiscaring-0.2.9/sharingiscaring/block.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_accountByAddress.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_accountByAddress.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_accounts.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_accounts.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_bakerByBakerId.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_bakerByBakerId.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_bakers.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_bakers.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_blockByBlockHash.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_blockByBlockHash.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_blocks.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_blocks.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_passiveDelegation.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_passiveDelegation.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_paydayStatus.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_paydayStatus.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_poolRewardMetricsForBakerPool.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_poolRewardMetricsForBakerPool.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_poolRewardMetricsForPassiveDelegation.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_rewardMetricsForAccount.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_rewardMetricsForAccount.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_search.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_search.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_transactionByTransactionHash.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_transactionByTransactionHash.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/_transactionMetrics.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/_transactionMetrics.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/exchange_account_updates.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/exchange_account_updates.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/ccdscan_queries/ql_support.py` & `sharingiscaring-0.2.9/sharingiscaring/ccdscan_queries/ql_support.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/client.py` & `sharingiscaring-0.2.9/sharingiscaring/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from functools import lru_cache
 from rich.console import Console
 import datetime as dt
 
 console = Console()
 
 CONCORDIUM_CLIENT_PREFIX = os.environ.get("CONCORDIUM_CLIENT_PREFIX", "")
-REQUESTOR_NODES = os.environ.get("REQUESTOR_NODES", "207.180.201.8,31.21.31.76")
+REQUESTOR_NODES = os.environ.get("REQUESTOR_NODES", "207.180.201.8,31.20.212.96")
 REQUESTOR_NODES = REQUESTOR_NODES.split(",")
 REQUESTOR_NODES_TESTNET = os.environ.get("REQUESTOR_NODES_TESTNET", "207.180.201.8")
 REQUESTOR_NODES_TESTNET = REQUESTOR_NODES_TESTNET.split(",")
 
 
 class RequestorType(Enum):
     accountInfo = "{"
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/cns.py` & `sharingiscaring-0.2.9/sharingiscaring/cns.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,16 @@
 import base58
 
 # import sha3
 from eth_hash.auto import keccak
 
 import json
 from enum import Enum
-from sharingiscaring.enums import NET
-
+from .client import ConcordiumClient
 from rich.console import Console
-from pymongo import ReplaceOne
-from sharingiscaring.GRPCClient import GRPCClient
-
-# from sharingiscaring.mongodb import Collections
 
 console = Console()
 
 
 class CNSActions(Enum):
     bid = "bid"
     cancel = "cancel"
@@ -89,15 +84,15 @@
     #     else:
     #         label, _, remainder = name.partition(".")
     #         return sha3.keccak_256(
     #             self.namehash(remainder)
     #             + sha3.keccak_256(bytes(label, encoding=encoding)).digest()
     #         ).digest()
 
-    def namehash_dome(self, name: str, encoding="utf-8"):
+    def namehash_dome(self, name: str, encoding="utf-16"):
         """ENS "namehash()" convention mapping of strings to bytes(32) hashes.
 
         Recursive function variant. Performs slightly better than the
         generator-based variant, but can't handle names with infinite (or
         extremely large) number of labels.
 
         :param name: name to hash, labels separated by dots
@@ -178,148 +173,68 @@
     def address(self, bs):
         t = int.from_bytes(bs.read(1), byteorder="little")
         if t == 0:
             return self.account_address(bs)
         elif t == 1:
             return self.contract_address(bs)
         else:
-            return "x" * 50
-
-    def translate_hex_to_bytes(self, parameter_hex: str) -> bytes:
-        parameter_bytes = list(bytes.fromhex(parameter_hex))
-        parameter_bytes.insert(0, 32)
-        return bytes(parameter_bytes)
+            raise Exception("invalid type")
 
-    def get_cns_domain_name_v2(self, grpcclient: GRPCClient, hex: str, net: str):
+    def get_cns_domain_name(self, concordium_node: ConcordiumClient, hex):
         try:
-            block_hash = "last_final"
-            instance_index = 7073
-            instance_subindex = 0
-            entrypoint = "BictoryCnsNft.getTokenInfo"
-            parameter_bytes = self.translate_hex_to_bytes(hex)
-
-            ii = grpcclient.invoke_instance(
-                block_hash,
-                instance_index,
-                instance_subindex,
-                entrypoint,
-                parameter_bytes,
-                NET(net),
+            self.write_binary_to_file("0x" + hex)
+            res = concordium_node.call_client_with(
+                [
+                    "contract",
+                    "invoke",
+                    "7073",
+                    "--entrypoint",
+                    "getTokenInfo",
+                    "--parameter-binary",
+                    "token.bin",
+                ]
             )
-            if ii.success is not None:
-                res = ii.success.return_value
-                bb = list(bytes.fromhex(res.decode()))
-                domain_name = bytes(bb[5:-8]).decode()
+        except:
+            domain_name = "Unable to determine..."
+        try:
+            by = json.loads(res.split()[-2])
+            by = bytes(by[5:-8])
+            domain_name = by.decode()
         except:
             domain_name = "Unable to determine..."
         self.domain_name = domain_name
 
-    # def get_cns_domain_name(self, concordium_node: ConcordiumClient, hex):
-    #     try:
-    #         self.write_binary_to_file("0x" + hex)
-    #         res = concordium_node.call_client_with(
-    #             [
-    #                 "contract",
-    #                 "invoke",
-    #                 "7073",
-    #                 "--entrypoint",
-    #                 "getTokenInfo",
-    #                 "--parameter-binary",
-    #                 "token.bin",
-    #             ]
-    #         )
-    #     except:
-    #         domain_name = "Unable to determine..."
-    #     try:
-    #         by = json.loads(res.split()[-2])
-    #         by = bytes(by[5:-8])
-    #         domain_name = by.decode()
-    #     except:
-    #         domain_name = "Unable to determine..."
-    #     self.domain_name = domain_name
-
-    def get_domain_name_owner_v2(
-        self, grpcclient: GRPCClient, mongodb, Collections, domain_name
-    ):
+    def get_domain_name_owner(self, concordium_node: ConcordiumClient, domain_name):
         console.log(f"get_domain_name_owner for {domain_name}")
-        result = mongodb.mainnet[Collections.cns_domains].find_one(
-            {"domain_name": domain_name}
-        )
-        hex = None
-        if result:
-            hex = result["_id"]
-
+        hex = concordium_node.cns_cache_by_name.get(domain_name, None)
         if not hex:
             bb = self.namehash_dome(domain_name)
             hex = bytes.hex(bb)
-            document_to_store = ReplaceOne(
-                {
-                    "_id": hex,
-                },
-                {
-                    "_id": hex,
-                    "domain_name": domain_name,
-                },
-                upsert=True,
-            )
-            result = mongodb.mainnet[Collections.cns_domains].bulk_write(
-                [document_to_store]
-            )
-
-        block_hash = "last_final"
-        instance_index = 7073
-        instance_subindex = 0
-        entrypoint = "BictoryCnsNft.getTokenExpiry"
-        parameter_bytes = self.translate_hex_to_bytes(hex)
-
-        ii = grpcclient.invoke_instance(
-            block_hash,
-            instance_index,
-            instance_subindex,
-            entrypoint,
-            parameter_bytes,
+            concordium_node.cns_cache_by_name[domain_name] = hex
+            concordium_node.cns_cache_by_token_id[hex] = domain_name
+            concordium_node.save_cns_cache()
+            # console.log("write_to_file)")
+        self.write_binary_to_file("0x" + hex)
+        res = concordium_node.call_client_with(
+            [
+                "contract",
+                "invoke",
+                "7073",
+                "--entrypoint",
+                "getTokenExpiry",
+                "--parameter-binary",
+                "token.bin",
+            ]
         )
+        by = json.loads(res.split()[-2])
 
-        if ii.success is not None:
-            res = ii.success.return_value
-            bb = list(bytes.fromhex(res.decode()))
-            byt = io.BytesIO(bytes(bb))
-            (status, to) = CNSDomain().read_domain_owner(byt)
-            return (status, to)
-        else:
-            return (-1, None)
-
-    # def get_domain_name_owner(self, concordium_node: ConcordiumClient, domain_name):
-    #     console.log(f"get_domain_name_owner for {domain_name}")
-    #     hex = concordium_node.cns_cache_by_name.get(domain_name, None)
-    #     if not hex:
-    #         bb = self.namehash_dome(domain_name)
-    #         hex = bytes.hex(bb)
-    #         concordium_node.cns_cache_by_name[domain_name] = hex
-    #         concordium_node.cns_cache_by_token_id[hex] = domain_name
-    #         concordium_node.save_cns_cache()
-    #         # console.log("write_to_file)")
-    #     self.write_binary_to_file("0x" + hex)
-    #     res = concordium_node.call_client_with(
-    #         [
-    #             "contract",
-    #             "invoke",
-    #             "7073",
-    #             "--entrypoint",
-    #             "getTokenExpiry",
-    #             "--parameter-binary",
-    #             "token.bin",
-    #         ]
-    #     )
-    #     by = json.loads(res.split()[-2])
-
-    #     byt = io.BytesIO(bytes(by))
-    #     # console.log('read_domain_owner')
-    #     (status, to) = self.read_domain_owner(byt)
-    #     return (status, to)
+        byt = io.BytesIO(bytes(by))
+        # console.log('read_domain_owner')
+        (status, to) = self.read_domain_owner(byt)
+        return (status, to)
 
     def string(self, bs):
         # bs = io.BytesIO(bytes.fromhex(hex))
         n = int.from_bytes(bs.read(4), byteorder="little")
         name = bs.read(n)
         return bytes.decode(name, "UTF-8")
 
@@ -408,27 +323,27 @@
         return [id_, amount, from_, to, data]
 
     def token_id(self, bs):
         n = int.from_bytes(bs.read(1), byteorder="little")
         return bytes.hex(bs.read(n))
 
     def token_amount(self, bs):
-        return int.from_bytes(bs.read(1), byteorder="little")
+        return int.from_bytes(bs.read(8), byteorder="little")
 
     def percentage(self, bs):
         return int.from_bytes(bs.read(8), byteorder="little")
 
     def receiver(self, bs):
         t = int.from_bytes(bs.read(1), byteorder="little")
         if t == 0:
             return self.account_address(bs)
         elif t == 1:
             return self.contract_address(bs), self.receive_hook_name(bs)
         else:
-            return "x" * 50
+            raise Exception("invalid type")
 
     def receive_hook_name(self, bs):
         n = int.from_bytes(bs.read(2), byteorder="little")
         name = bs.read(n)
         return bytes.decode(name, "UTF-8")
 
     def additional_data(self, bs):
@@ -550,25 +465,22 @@
             None,
         )
 
         # only available for abortEvent, cancelEvent
         owner_, bidder_, amount_ = None, None, None
 
         # tag 161 is undocumented for now?
-        (
-            contract_index,
-            contract_subindex,
-            token_id_,
-        ) = (
+        contract_index, contract_subindex, token_id_, = (
             None,
             None,
             None,
         )
 
         if tag_ == 243:
+
             (
                 tag_,
                 contract_index,
                 contract_subindex,
                 token_id_,
                 seller_,
                 winner_,
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/CCD_Types/__init__.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/CCD_Types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,14 @@
     na = "0"
     Passport = "1"
     National_ID_Card = "2"
     Driving_License = "3"
     Immigration_Card = "4"
 
 
-class ProtocolVersions(Enum):
-    PROTOCOL_VERSION_1 = 0
-    PROTOCOL_VERSION_2 = 1
-    PROTOCOL_VERSION_3 = 2
-    PROTOCOL_VERSION_4 = 3
-    PROTOCOL_VERSION_5 = 4
-    PROTOCOL_VERSION_6 = 5
-
-
 class OpenStatus(Enum):
     open_for_all = 0
     closed_for_new = 1
     closed_for_all = 2
 
 
 CCD_ArIdentity = int
@@ -61,15 +52,14 @@
 CCD_TransactionHash = str
 CCD_AccountAddress = str
 CCD_AccountIndex = int
 CCD_DelegatorId = CCD_AccountIndex
 microCCD = int
 CCD_BakerId = int
 CCD_Epoch = int
-CCD_Energy = int
 CCD_DurationSeconds = int
 CCD_ModuleRef = str
 CCD_ContractEvent = str
 CCD_Memo = str
 CCD_RegisteredData = str
 CCD_BakerSignatureVerifyKey = str
 CCD_OpenStatus = int
@@ -89,16 +79,14 @@
 CCD_TransactionTime = int
 CCD_SignatureThreshold = int
 CCD_IdentityProviderIdentity = int
 CCD_ArThreshold = int
 CCD_Commitment = str
 CCD_VersionedModuleSource_ModuleSourceV0 = str
 CCD_VersionedModuleSource_ModuleSourceV1 = str
-CCD_ProtocolVersion = int
-CCD_StateHash = str
 
 CCD_SequenceNumber = int
 CCD_StakePendingChange_Remove = dt.datetime
 CCD_ContractStateV0 = str
 CCD_InitName = str
 CCD_EncryptedAmount = str
 CCD_Empty = None
@@ -109,37 +97,14 @@
 #     value: str
 
 
 class CCD_ContractAddress(BaseModel):
     index: int
     subindex: int
 
-    def to_str(self):
-        return f"<{self.index},{self.subindex}>"
-
-    @classmethod
-    def from_str(self, str_repr: str):
-        """
-        Returns a CCD_ContractAddress when the input is formed as '<2350,0>'.
-        """
-        contract_string = str_repr.split("-")[0]
-        c = CCD_ContractAddress(
-            **{
-                "index": contract_string.split(",")[0][1:],
-                "subindex": contract_string.split(",")[1][:-1],
-            }
-        )
-
-        return c
-
-    @classmethod
-    def from_index(self, index: int, subindex: int):
-        s = CCD_ContractAddress(**{"index": index, "subindex": subindex})
-        return s
-
 
 class CCD_Address(BaseModel):
     account: CCD_AccountAddress = None
     contract: CCD_ContractAddress = None
 
 
 class CCD_RejectReason_InvalidInitMethod(BaseModel):
@@ -334,16 +299,14 @@
     era_block_height: int
     finalized: bool
     genesis_index: int
     transaction_count: int
     transactions_energy_cost: int
     transactions_size: int
     transaction_hashes: list[CCD_TransactionHash] = None
-    state_hash: CCD_StateHash = None
-    protocol_version: CCD_ProtocolVersion = None
 
 
 class CCD_AccountTransactionEffects_None(BaseModel):
     transaction_type: int = None
     reject_reason: CCD_RejectReason
 
 
@@ -1157,31 +1120,7 @@
     level1_keys: CCD_HigherLevelKeys
     level2_keys: CCD_AuthorizationsV1
 
 
 class CCD_ChainParameters(BaseModel):
     v0: CCD_ChainParametersV0 = None
     v1: CCD_ChainParametersV1 = None
-
-
-class CCD_InvokeInstanceResponse_Success(BaseModel):
-    return_value: bytes
-    used_energy: CCD_Energy
-    effects: list[CCD_ContractTraceElement]
-
-
-class CCD_InvokeInstanceResponse_Failure(BaseModel):
-    return_value: bytes
-    used_energy: CCD_Energy
-    reason: CCD_RejectReason
-
-
-class CCD_InvokeInstanceResponse(BaseModel):
-    success: CCD_InvokeInstanceResponse_Success
-    failure: CCD_InvokeInstanceResponse_Failure
-
-
-class CCD_BlockComplete(BaseModel):
-    block_info: CCD_BlockInfo
-    transaction_summaries: list[CCD_BlockItemSummary]
-    special_events: list[CCD_BlockSpecialEvent]
-    net: str = None
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/concordium/health/__init__.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/concordium/health/__init__.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/concordium/v2/__init__.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/concordium/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/health_pb2.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/health_pb2.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/health_pb2_grpc.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/health_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-import sharingiscaring.GRPCClient.health_pb2 as health__pb2
+import health_pb2 as health__pb2
 
 
 class HealthStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Check = channel.unary_unary(
-            "/concordium.health.Health/Check",
-            request_serializer=health__pb2.NodeHealthRequest.SerializeToString,
-            response_deserializer=health__pb2.NodeHealthResponse.FromString,
-        )
+                '/concordium.health.Health/Check',
+                request_serializer=health__pb2.NodeHealthRequest.SerializeToString,
+                response_deserializer=health__pb2.NodeHealthResponse.FromString,
+                )
 
 
 class HealthServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Check(self, request, context):
         """Check the health of the node. By necessity this involves a number of
@@ -35,57 +35,44 @@
 
         If possible the client should use other queries to get a more fine-grained
         understanding of the node health. However this endpoint should provide a
         reasonable default and is usable in cases where an automatic check is
         performed that does not allow for configuration, such as in load-balancers.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_HealthServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "Check": grpc.unary_unary_rpc_method_handler(
-            servicer.Check,
-            request_deserializer=health__pb2.NodeHealthRequest.FromString,
-            response_serializer=health__pb2.NodeHealthResponse.SerializeToString,
-        ),
+            'Check': grpc.unary_unary_rpc_method_handler(
+                    servicer.Check,
+                    request_deserializer=health__pb2.NodeHealthRequest.FromString,
+                    response_serializer=health__pb2.NodeHealthResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "concordium.health.Health", rpc_method_handlers
-    )
+            'concordium.health.Health', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class Health(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Check(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def Check(request,
             target,
-            "/concordium.health.Health/Check",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/concordium.health.Health/Check',
             health__pb2.NodeHealthRequest.SerializeToString,
             health__pb2.NodeHealthResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetAccountInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetAccountInfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.json_format import MessageToJson, MessageToDict
 from google.protobuf import message
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 import os
 import sys
-from sharingiscaring.enums import NET
 
 sys.path.append(os.path.dirname("sharingiscaring"))
 from sharingiscaring.GRPCClient.CCD_Types import *
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.concordium.v2 import AccountInfo
 
 
 class Mixin(_SharedConverters):
     def convertKeysEntry(self, message) -> dict[str, CCD_AccountVerifyKey]:
         entry_dict = {}
         for index, entry in message.items():
+
             converted_value = self.convertType(entry)
             entry_dict[str(index)] = CCD_AccountVerifyKey(
                 **{"ed25519_key": converted_value}
             )
 
         return entry_dict
 
     def convertArData(self, message) -> dict[str, CCD_ChainArData]:
         entry_dict = {}
         for index, entry in message.items():
+
             converted_value = self.convertType(entry)
             entry_dict[str(index)] = CCD_ChainArData(
                 **{"enc_id_cred_pub_share": converted_value}
             )
 
         return entry_dict
 
@@ -249,39 +250,32 @@
 
                     elif type(value) == StakePendingChange:
                         result[key] = self.convertPendingChange(value)
 
             return CCD_AccountStakingInfo(**{which_one: result})
 
     def get_account_info(
-        self: GRPCClient,
-        block_hash: str,
-        hex_address: str = None,
-        account_index: int = None,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str, hex_address: str = None, baker_id: int = None
     ) -> CCD_AccountInfo:
         blockHashInput = self.generate_block_hash_input_from(block_hash)
-        if account_index is not None:
+        if baker_id is not None:
             accountIdentifierInput = (
-                self.generate_account_identifier_input_from_account_index(account_index)
+                self.generate_account_identifier_input_from_baker_id(baker_id)
             )
         elif hex_address:
             accountIdentifierInput = self.generate_account_identifier_input_from(
                 hex_address
             )
 
         account_info = AccountInfoRequest(
             block_hash=blockHashInput, account_identifier=accountIdentifierInput
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value = self.stub_mainnet.GetAccountInfo(request=account_info)
-        else:
-            grpc_return_value = self.stub_testnet.GetAccountInfo(request=account_info)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value = self.stub.GetAccountInfo(request=account_info)
 
         result = {}
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetAccountList.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetAccountList.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,37 +3,28 @@
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
 import sys
 from sharingiscaring.GRPCClient.CCD_Types import *
-from sharingiscaring.enums import NET
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 
 
 class Mixin(_SharedConverters):
-    def get_account_list(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_AccountAddress]:
+    def get_account_list(self: GRPCClient, block_hash: str) -> list[CCD_AccountAddress]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                AccountAddress
-            ] = self.stub_mainnet.GetAccountList(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                AccountAddress
-            ] = self.stub_testnet.GetAccountList(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[AccountAddress] = self.stub.GetAccountList(
+            request=blockHashInput
+        )
 
         for account in list(grpc_return_value):
+
             result.append(self.convertType(account))
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetAnonymityRevokers.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetFinalizedBlocks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
-import sys
-from sharingiscaring.GRPCClient.CCD_Types import *
-from sharingiscaring.enums import NET
 from typing import TYPE_CHECKING
+import sys
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
+from sharingiscaring.GRPCClient.CCD_Types import *
+from rich import print
 
 
 class Mixin(_SharedConverters):
-    def get_anonymity_revokers(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_ArInfo]:
-        result = []
-        blockHashInput = self.generate_block_hash_input_from(block_hash)
-
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                ArInfo
-            ] = self.stub_mainnet.GetAnonymityRevokers(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                ArInfo
-            ] = self.stub_testnet.GetAnonymityRevokers(request=blockHashInput)
+    def convertFinalizedBlock(self, block) -> CCD_FinalizedBlockInfo:
+        result = {}
+
+        for descriptor in block.DESCRIPTOR.fields:
+            key, value = self.get_key_value_from_descriptor(descriptor, block)
+
+            if type(value) in self.simple_types:
+                result[key] = self.convertType(value)
+
+        return CCD_FinalizedBlockInfo(**result)
 
-        for ar in list(grpc_return_value):
-            result.append(self.convertArInfo(ar))
+    def get_finalized_blocks(self: GRPCClient) -> CCD_FinalizedBlockInfo:
 
-        return result
+        self.check_connection(sys._getframe().f_code.co_name)
+        for block in self.stub.GetFinalizedBlocks(request=Empty()):
+            print(self.convertFinalizedBlock(block))
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBakerList.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlockInfo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from __future__ import annotations
-from sharingiscaring.GRPCClient.types_pb2 import *
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
+from sharingiscaring.GRPCClient.types_pb2 import *
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
-from typing import Iterator
-from sharingiscaring.GRPCClient.CCD_Types import *
-from sharingiscaring.enums import NET
-from typing import TYPE_CHECKING
+
+# from sharingiscaring.GRPCClient import GRPCClient
+import os
 import sys
+import grpc
 
-if TYPE_CHECKING:
-    from sharingiscaring.GRPCClient import GRPCClient
+sys.path.append(os.path.dirname("sharingiscaring"))
+from sharingiscaring.GRPCClient.CCD_Types import CCD_BlockInfo
+from sharingiscaring.GRPCClient.concordium.v2 import BlockInfo as BP_BlockInfo
 
 
 class Mixin(_SharedConverters):
-    def get_baker_list(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_BakerId]:
-        result = []
+    def get_block_info(self: GRPCClient, block_hash: str) -> CCD_BlockInfo:
+        result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[BakerId] = self.stub_mainnet.GetBakerList(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value: Iterator[BakerId] = self.stub_testnet.GetBakerList(
-                request=blockHashInput
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: BlockInfo = self.stub.GetBlockInfo(request=blockHashInput)
+
+        for descriptor in grpc_return_value.DESCRIPTOR.fields:
+            key, value = self.get_key_value_from_descriptor(
+                descriptor, grpc_return_value
             )
 
-        for baker in list(grpc_return_value):
-            result.append(self.convertType(baker))
+            if type(value) in self.simple_types:
+                result[f"{key}"] = self.convertType(value)
 
-        return result
+        # TODO: fix for BakerId always producing 0
+        # even when it's not set (as is the case for genesis blocks)
+        if result["era_block_height"] == 0:
+            result["baker"] = None
+        return CCD_BlockInfo(**result)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlockInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPoolInfo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from enum import Enum
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
-
-# from sharingiscaring.GRPCClient import GRPCClient
 import os
 import sys
-import grpc
+from rich import print
+from google.protobuf.json_format import MessageToJson, MessageToDict
 
 sys.path.append(os.path.dirname("sharingiscaring"))
-from sharingiscaring.GRPCClient.CCD_Types import CCD_BlockInfo, ProtocolVersions
-from sharingiscaring.GRPCClient.concordium.v2 import BlockInfo as BP_BlockInfo
+# from sharingiscaring.pool import ConcordiumPoolFromClient
+from sharingiscaring.GRPCClient.CCD_Types import CCD_PoolInfo
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from sharingiscaring.GRPCClient import GRPCClient
 
 
 class Mixin(_SharedConverters):
-    def get_block_info(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> CCD_BlockInfo:
+    def get_pool_info_for_pool(
+        self: GRPCClient, pool_id: int, block_hash: str
+    ) -> CCD_PoolInfo:
+        prefix = ""
         result = {}
         blockHashInput = self.generate_block_hash_input_from(block_hash)
+        baker_id = BakerId(value=pool_id)
+        poolInfoRequest = PoolInfoRequest(baker=baker_id, block_hash=blockHashInput)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: BlockInfo = self.stub_mainnet.GetBlockInfo(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value: BlockInfo = self.stub_testnet.GetBlockInfo(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: PoolInfoResponse = self.stub.GetPoolInfo(
+            request=poolInfoRequest
+        )
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
+            key_to_store = f"{prefix}{key}"
+            if type(value) in self.simple_types:
+                result[key_to_store] = self.convertType(value)
+
+            elif type(value) == BakerPoolInfo:
+                result[key_to_store] = self.convertBakerPoolInfo(value)
+
+            elif type(value) == PoolCurrentPaydayInfo:
+                if self.valueIsEmpty(value):
+                    result[key_to_store] = None
+                else:
+                    result[key_to_store] = self.convertPoolCurrentPaydayInfo(value)
 
-            if key == "protocol_version":
-                result[key] = ProtocolVersions(value).name
-
-            elif type(value) in self.simple_types:
-                result[f"{key}"] = self.convertType(value)
+            elif type(value) == PoolPendingChange:
+                result[key_to_store] = self.convertPendingChange(value)
 
-        # TODO: fix for BakerId always producing 0
-        # even when it's not set (as is the case for genesis blocks)
-        if result["era_block_height"] == 0:
-            result["baker"] = None
-        return CCD_BlockInfo(**result)
+        return CCD_PoolInfo(**result)
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlockPendingUpdates.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlockPendingUpdates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
@@ -51,29 +50,20 @@
 
                     elif type(value) in self.simple_types:
                         result[key] = self.convertType(value)
 
             return CCD_UpdateDetails(**result), _type
 
     def get_block_pending_updates(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> list[CCD_BlockSpecialEvent]:
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value = self.stub_mainnet.GetBlockPendingUpdates(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value = self.stub_testnet.GetBlockPendingUpdates(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value = self.stub.GetBlockPendingUpdates(request=blockHashInput)
 
         events = []
         for tx in list(grpc_return_value):
             result = {}
             for descriptor in tx.DESCRIPTOR.fields:
                 key, value = self.get_key_value_from_descriptor(descriptor, tx)
                 if self.valueIsEmpty(value):
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlockSpecialEvents.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlockSpecialEvents.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
@@ -79,29 +78,20 @@
 
             elif type(value) in self.simple_types:
                 result[key] = self.convertType(value)
 
         return CCD_BlockSpecialEvent_FinalizationRewards(**result)
 
     def get_block_special_events(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> list[CCD_BlockSpecialEvent]:
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value = self.stub_mainnet.GetBlockSpecialEvents(
-                request=blockHashInput
-            )
-        else:
-            grpc_return_value = self.stub_testnet.GetBlockSpecialEvents(
-                request=blockHashInput
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value = self.stub.GetBlockSpecialEvents(request=blockHashInput)
 
         events = []
         for tx in list(grpc_return_value):
             result = {}
             for descriptor in tx.DESCRIPTOR.fields:
                 key, value = self.get_key_value_from_descriptor(descriptor, tx)
                 if self.valueIsEmpty(value):
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetBlocksAtHeight.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetBlocksAtHeight.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
@@ -17,52 +15,41 @@
 sys.path.append(os.path.dirname("sharingiscaring"))
 from sharingiscaring.GRPCClient.CCD_Types import CCD_BlockInfo, CCD_BlockHash
 from sharingiscaring.GRPCClient.concordium.v2 import BlockInfo as BP_BlockInfo
 
 
 class Mixin(_SharedConverters):
     def get_blocks_at_height(
-        self: GRPCClient,
-        block_height: int,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_height: int
     ) -> list[CCD_BlockHash]:
         result = []
         absoluteBlockHeight = AbsoluteBlockHeight(value=block_height)
         blocksAtHeightRequestAbsolute = BlocksAtHeightRequest.Absolute(
             height=absoluteBlockHeight
         )
         blocksAtHeightRequest = BlocksAtHeightRequest(
             absolute=blocksAtHeightRequestAbsolute
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                BlocksAtHeightResponse
-            ] = self.stub_mainnet.GetBlocksAtHeight(request=blocksAtHeightRequest)
-        else:
-            grpc_return_value: Iterator[
-                BlocksAtHeightResponse
-            ] = self.stub_testnet.GetBlocksAtHeight(request=blocksAtHeightRequest)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[
+            BlocksAtHeightResponse
+        ] = self.stub.GetBlocksAtHeight(request=blocksAtHeightRequest)
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
             if key == "blocks":
                 result = self.convertList(value)
 
         return result
 
-    def get_finalized_block_at_height(
-        self,
-        block_height: int,
-        net: Enum = NET.MAINNET,
-    ) -> CCD_BlockInfo:
-        blocks_at_height = self.get_blocks_at_height(block_height, net)
+    def get_finalized_block_at_height(self, block_height: int) -> CCD_BlockInfo:
+        blocks_at_height = self.get_blocks_at_height(block_height)
         for block_hash in blocks_at_height:
-            bi: CCD_BlockInfo = self.get_block_info(block_hash, net)
+            bi: CCD_BlockInfo = self.get_block_info(block_hash)
             if bi.finalized:
                 return bi
 
         return None
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetIdentityProviders.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetIdentityProviders.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 import sys
 from typing import Iterator
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
-    def get_identity_providers(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_IpInfo]:
+    def get_identity_providers(self: GRPCClient, block_hash: str) -> list[CCD_IpInfo]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                IpInfo
-            ] = self.stub_mainnet.GetIdentityProviders(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                IpInfo
-            ] = self.stub_testnet.GetIdentityProviders(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[IpInfo] = self.stub.GetIdentityProviders(
+            request=blockHashInput
+        )
 
         for ip in list(grpc_return_value):
+
             result.append(self.convertIpInfo(ip))
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetInstanceInfo.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetInstanceInfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
@@ -16,14 +15,15 @@
 from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
     def convertMethods(self, message) -> list[CCD_ReceiveName]:
         methods = []
         for method in message:
+
             for descriptor in method.DESCRIPTOR.fields:
                 _, value = self.get_key_value_from_descriptor(descriptor, method)
 
                 methods.append(self.convertType(value))
 
         return methods
 
@@ -50,34 +50,26 @@
 
             elif key == "methods":
                 result[key] = self.convertMethods(value)
 
         return CCD_InstanceInfo_V1(**result)
 
     def get_instance_info(
-        self: GRPCClient,
-        contract_index: int,
-        contract_sub_index: int,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, contract_index: int, contract_sub_index: int, block_hash: str
     ) -> CCD_InstanceInfo:
+
         result = {}
         instanceInfoRequest = self.generate_instance_info_request_from(
             contract_index, contract_sub_index, block_hash
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: InstanceInfo = self.stub_mainnet.GetInstanceInfo(
-                request=instanceInfoRequest
-            )
-        else:
-            grpc_return_value: InstanceInfo = self.stub_testnet.GetInstanceInfo(
-                request=instanceInfoRequest
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: InstanceInfo = self.stub.GetInstanceInfo(
+            request=instanceInfoRequest
+        )
 
         for descriptor in grpc_return_value.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(
                 descriptor, grpc_return_value
             )
 
             if type(value) == InstanceInfo.V0:
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetInstanceList.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetAccountList.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
-from typing import TYPE_CHECKING
 import sys
+from sharingiscaring.GRPCClient.CCD_Types import *
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
-from sharingiscaring.GRPCClient.CCD_Types import *
 
 
 class Mixin(_SharedConverters):
-    def get_instance_list(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_BakerId]:
+    def get_account_list(self: GRPCClient, block_hash: str) -> list[CCD_AccountAddress]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                ContractAddress
-            ] = self.stub_mainnet.GetInstanceList(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                ContractAddress
-            ] = self.stub_testnet.GetInstanceList(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[AccountAddress] = self.stub.GetAccountList(
+            request=blockHashInput
+        )
+
+        for account in list(grpc_return_value):
 
-        for instance in list(grpc_return_value):
-            result.append(self.convertType(instance))
+            result.append(self.convertType(account))
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetPassiveDelegators.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_GetPassiveDelegators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
 from typing import TYPE_CHECKING
 import sys
@@ -13,32 +11,26 @@
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
 from sharingiscaring.GRPCClient.CCD_Types import CCD_DelegatorInfo
 
 
 class Mixin(_SharedConverters):
     def get_delegators_for_passive_delegation(
-        self: GRPCClient,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
+        self: GRPCClient, block_hash: str
     ) -> list[CCD_DelegatorInfo]:
         result: list[CCD_DelegatorInfo] = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                DelegatorInfo
-            ] = self.stub_mainnet.GetPassiveDelegators(request=blockHashInput)
-        else:
-            grpc_return_value: Iterator[
-                DelegatorInfo
-            ] = self.stub_testnet.GetPassiveDelegators(request=blockHashInput)
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[DelegatorInfo] = self.stub.GetPassiveDelegators(
+            request=blockHashInput
+        )
 
         for delegator in list(grpc_return_value):
+
             delegator_dict = {
                 "account": self.convertAccountAddress(delegator.account),
                 "stake": self.convertAmount(delegator.stake),
             }
             if delegator.pending_change:
                 if self.valueIsEmpty(delegator.pending_change):
                     pass
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_GetPoolDelegatorsRewardPeriod.py` & `sharingiscaring-0.2.9/sharingiscaring/GRPCClient/queries/_GetPoolDelegators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 from __future__ import annotations
 from sharingiscaring.GRPCClient.types_pb2 import *
-from sharingiscaring.enums import NET
-from enum import Enum
 from sharingiscaring.GRPCClient.service_pb2_grpc import QueriesStub
 from sharingiscaring.GRPCClient.queries._SharedConverters import (
     Mixin as _SharedConverters,
 )
 from typing import Iterator
 from typing import TYPE_CHECKING
 import sys
 
 if TYPE_CHECKING:
     from sharingiscaring.GRPCClient import GRPCClient
-from sharingiscaring.GRPCClient.CCD_Types import CCD_DelegatorRewardPeriodInfo
+from sharingiscaring.GRPCClient.CCD_Types import CCD_DelegatorInfo
 
 
 class Mixin(_SharedConverters):
-    def get_delegators_for_pool_in_reward_period(
-        self: GRPCClient,
-        pool_id: int,
-        block_hash: str,
-        net: Enum = NET.MAINNET,
-    ) -> list[CCD_DelegatorRewardPeriodInfo]:
+    def get_delegators_for_pool(
+        self: GRPCClient, pool_id: int, block_hash: str
+    ) -> list[CCD_DelegatorInfo]:
         result = []
         blockHashInput = self.generate_block_hash_input_from(block_hash)
         baker_id = BakerId(value=pool_id)
         delegatorsRequest = GetPoolDelegatorsRequest(
             baker=baker_id, block_hash=blockHashInput
         )
 
-        self.check_connection(net, sys._getframe().f_code.co_name)
-        if net == NET.MAINNET:
-            grpc_return_value: Iterator[
-                DelegatorRewardPeriodInfo
-            ] = self.stub_mainnet.GetPoolDelegatorsRewardPeriod(
-                request=delegatorsRequest
-            )
-        else:
-            grpc_return_value: Iterator[
-                DelegatorRewardPeriodInfo
-            ] = self.stub_testnet.GetPoolDelegatorsRewardPeriod(
-                request=delegatorsRequest
-            )
+        self.check_connection(sys._getframe().f_code.co_name)
+        grpc_return_value: Iterator[DelegatorInfo] = self.stub.GetPoolDelegators(
+            request=delegatorsRequest
+        )
 
         for delegator in list(grpc_return_value):
-            result.append(
-                CCD_DelegatorRewardPeriodInfo(
-                    **{
-                        "account": self.convertAccountAddress(delegator.account),
-                        "stake": self.convertAmount(delegator.stake),
-                    }
-                )
-            )
+
+            delegator_dict = {
+                "account": self.convertAccountAddress(delegator.account),
+                "stake": self.convertAmount(delegator.stake),
+            }
+            if delegator.pending_change:
+                if self.valueIsEmpty(delegator.pending_change):
+                    pass
+                else:
+                    delegator_dict.update(
+                        {
+                            "pending_change": self.convertPendingChange(
+                                delegator.pending_change
+                            )
+                        }
+                    )
+
+            result.append(CCD_DelegatorInfo(**delegator_dict))
 
         return result
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/queries/_SharedConverters.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/queries/_SharedConverters.py`

 * *Files 25% similar despite different names*

```diff
@@ -123,98 +123,54 @@
             bin_value = base58.b58decode_check(hex_address)[1:]
             address = AccountAddress(value=bin_value)
             account = AccountIdentifierInput(address=address)
             return account
         except:  # pragma: no cover
             return None
 
-    def generate_account_identifier_input_from_account_index(
-        self, account_index: CCD_AccountIndex
-    ):
+    def generate_account_identifier_input_from_baker_id(self, baker_id: CCD_BakerId):
         try:
-            account = AccountIdentifierInput(
-                account_index=AccountIndex(value=account_index)
-            )
+            account = AccountIdentifierInput(account_index=AccountIndex(value=baker_id))
             return account
         except:  # pragma: no cover
             return None
 
-    def valueIsEmpty(self, value, key=None, message=None):
+    def valueIsEmpty(self, value):
         if type(value) == int:
             return value is None
         else:
             if type(value) == RepeatedCompositeContainer:
                 return False
             else:
                 if hasattr(value, "DESCRIPTOR"):
-                    if message:
-                        l = list(message)
-                        key_in_message = key in l[0].__str__()
-                        if key_in_message:
-                            # special case for baker_id = 0 (doesn't get transmitted in a message)
-                            if key == "baker_removed":
-                                return False
-                            else:
-                                if MessageToDict(value) != {}:
-                                    return False
-                                else:
-                                    return True
-                        return MessageToDict(value) == {}
-                    else:
-                        return MessageToDict(value) == {}
+                    return MessageToDict(value) == {}
                 else:  # pragma: no cover
                     return False
 
-    def generate_block_hash_input_from(self, hex_block_hash: str) -> BlockHashInput:
+    def generate_block_hash_input_from(self, hex_block_hash: str):
         if hex_block_hash == "last_final":
             return BlockHashInput(last_final={})
         else:
             return BlockHashInput(given=BlockHash(value=bytes.fromhex(hex_block_hash)))
 
-    def generate_invoke_instance_request_from(
-        self,
-        contract_index: int,
-        contract_sub_index: int,
-        block_hash_input: str,
-        receive_name: str,
-        parameter_bytes: bytes,
-    ):
-        # parameter_bytes = self.get_bytes_parameter_from_hex(parameter_hex)
-        # if we include a zero subindex, grpc will complain about
-        # LengthDelimited vs VarInt.
-        if contract_sub_index == 0:
-            instance = ContractAddress(index=contract_index)
-        else:
-            instance = ContractAddress(
-                index=contract_index,
-                subindex=contract_sub_index,
-            )
-
-        return InvokeInstanceRequest(
-            block_hash=block_hash_input,
-            amount=Amount(value=0),
-            entrypoint=ReceiveName(value=receive_name),
-            parameter=Parameter(value=parameter_bytes),
-            energy=Energy(value=100_000_000_000),
-            instance=instance,
-        )
-
     def generate_instance_info_request_from(
         self, contract_index: int, contract_sub_index: int, hex_block_hash: str
     ):
+
         return InstanceInfoRequest(
             block_hash=self.generate_block_hash_input_from(hex_block_hash),
             address=ContractAddress(
                 **{"index": contract_index, "subindex": contract_sub_index}
             ),
         )
 
     def generate_module_source_request_from(
         self, module_ref: CCD_ModuleRef, hex_block_hash: str
     ):
+
         return ModuleSourceRequest(
             block_hash=self.generate_block_hash_input_from(hex_block_hash),
             module_ref=ModuleRef(value=bytes.fromhex(module_ref)),
         )
 
     def convertList(self, message):
         entries = []
@@ -439,14 +395,15 @@
                 result[key] = self.convertType(value)
 
         return result
 
     def convertPendingChange_Reduce_Remove(
         self, message
     ) -> CCD_StakePendingChange_Remove:
+
         return self.convertType(message)
 
     def convertPendingChange(self, message) -> CCD_StakePendingChange:
         result = {}
 
         for descriptor in message.DESCRIPTOR.fields:
             key, value = self.get_key_value_from_descriptor(descriptor, message)
@@ -711,266 +668,7 @@
                     if type(value) == MintRate:
                         result[key] = self.convertMintRate(value)
 
                     elif type(value) == AmountFraction:
                         result[key] = self.convertType(value)
 
         return CCD_MintDistributionCpv0(**result)
-
-    def convertEvents(self, message) -> list:
-        events = []
-        for entry in message:
-            entry_dict = {}
-            for descriptor in entry.DESCRIPTOR.fields:
-                key, value = self.get_key_value_from_descriptor(descriptor, entry)
-                if type(value) in self.simple_types:
-                    converted_value = self.convertType(value)
-                    if converted_value:
-                        # entry_dict[key] = converted_value
-                        events.append(converted_value)
-            # if entry_dict == {}:
-            #         pass
-            # else:
-            #     events.append(entry_dict)
-
-        return events
-
-    def convertInstanceInterruptedEvent(
-        self, message
-    ) -> CCD_ContractTraceElement_Interrupted:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-            if key == "events":
-                result[key] = self.convertEvents(value)
-
-        return CCD_ContractTraceElement_Interrupted(**result)
-
-    def convertInstanceUpdatedEvent(self, message) -> CCD_InstanceUpdatedEvent:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-            if key == "events":
-                result[key] = self.convertEvents(value)
-
-        return CCD_InstanceUpdatedEvent(**result)
-
-    def convertInstanceResumedEvent(self, message) -> CCD_ContractTraceElement_Resumed:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-        return CCD_ContractTraceElement_Resumed(**result)
-
-    def convertInstanceTransferredEvent(
-        self, message
-    ) -> CCD_ContractTraceElement_Transferred:
-        result = {}
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-        return CCD_ContractTraceElement_Transferred(**result)
-
-    def convertUpdateEvents(self, message) -> list:
-        events = []
-        for entry in message:
-            for descriptor in entry.DESCRIPTOR.fields:
-                entry_dict = {}
-                key, value = self.get_key_value_from_descriptor(descriptor, entry)
-                if MessageToDict(value) == {}:
-                    pass
-                else:
-                    if type(value) == InstanceUpdatedEvent:
-                        entry_dict[key] = self.convertInstanceUpdatedEvent(value)
-
-                    if type(value) == ContractTraceElement.Interrupted:
-                        entry_dict[key] = self.convertInstanceInterruptedEvent(value)
-
-                    if type(value) == ContractTraceElement.Resumed:
-                        entry_dict[key] = self.convertInstanceResumedEvent(value)
-
-                    if type(value) == ContractTraceElement.Transferred:
-                        entry_dict[key] = self.convertInstanceTransferredEvent(value)
-
-                if entry_dict == {}:
-                    pass
-                else:
-                    events.append(entry_dict)
-
-        return events
-
-    def convertCredentialRegistrationIdEntries(self, message):
-        entries = []
-
-        for list_entry in message:
-            entries.append(self.convertType(list_entry))
-
-        return entries
-
-    def convertDuplicateCredIds(self, message) -> CCD_RejectReason_DuplicateCredIds:
-        result = {}
-
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-
-            result[key] = self.convertCredentialRegistrationIdEntries(value)
-
-        return CCD_RejectReason_DuplicateCredIds(**result)
-
-    def convertRejectReason(self, message) -> CCD_RejectReason:
-        result = {}
-        _type = None
-        for field, value in message.ListFields():
-            key = field.name
-
-            # Note this next section is purely to have Coverage
-            # show us that we have not covered all possible reject
-            # reasons with adequate tests...
-            if key == "module_not_wf":
-                test_me_please = True
-            if key == "module_hash_already_exists":
-                test_me_please = True
-            if key == "invalid_account_reference":
-                test_me_please = True
-            if key == "invalid_init_method":
-                test_me_please = True
-            if key == "invalid_receive_method":
-                test_me_please = True
-            if key == "invalid_module_reference":
-                test_me_please = True
-            if key == "invalid_contract_address":
-                test_me_please = True
-            if key == "runtime_failure":
-                test_me_please = True
-            if key == "amount_too_large":
-                test_me_please = True
-            if key == "serialization_failure":
-                test_me_please = True
-            if key == "out_of_energy":
-                test_me_please = True
-            if key == "rejected_init":
-                test_me_please = True
-            if key == "rejected_receive":
-                test_me_please = True
-            if key == "invalid_proof":
-                test_me_please = True
-            if key == "already_a_baker: ":
-                test_me_please = True
-            if key == "not_a_baker":
-                test_me_please = True
-            if key == "insufficient_balance_for_baker_stake":
-                test_me_please = True
-            if key == "stake_under_minimum_threshold_for_baking":
-                test_me_please = True
-            if key == "baker_in_cooldown":
-                test_me_please = True
-            if key == "duplicate_aggregation_key":
-                test_me_please = True
-            if key == "non_existent_credential_id":
-                test_me_please = True
-            if key == "key_index_already_in_use":
-                test_me_please = True
-            if key == "invalid_account_threshold":
-                test_me_please = True
-            if key == "invalid_credential_key_sign_threshold":
-                test_me_please = True
-            if key == "invalid_encrypted_amount_transfer_proof":
-                test_me_please = True
-            if key == "invalid_transfer_to_public_proof":
-                test_me_please = True
-            if key == "encrypted_amount_self_transfer":
-                test_me_please = True
-            if key == "invalid_index_on_encrypted_transfer":
-                test_me_please = True
-            if key == "zero_scheduledAmount":
-                test_me_please = True
-            if key == "non_increasing_schedule":
-                test_me_please = True
-            if key == "first_scheduled_release_expired":
-                test_me_please = True
-            if key == "scheduled_self_transfer":
-                test_me_please = True
-            if key == "invalid_credentials":
-                test_me_please = True
-            if key == "duplicate_cred_ids":
-                test_me_please = True
-            if key == "non_existent_cred_ids":
-                test_me_please = True
-            if key == "remove_first_credential":
-                test_me_please = True
-            if key == "credential_holder_did_not_sign":
-                test_me_please = True
-            if key == "not_allowed_multiple_credentials":
-                test_me_please = True
-            if key == "not_allowed_to_receive_encrypted":
-                test_me_please = True
-            if key == "not_allowed_to_handle_encrypted":
-                test_me_please = True
-            if key == "missing_baker_add_parameters":
-                test_me_please = True
-            if key == "finalization_reward_commission_not_in_range":
-                test_me_please = True
-            if key == "baking_reward_commission_not_in_range":
-                test_me_please = True
-            if key == "transaction_fee_commission_not_in_range":
-                test_me_please = True
-            if key == "already_a_delegator":
-                test_me_please = True
-            if key == "insufficient_balance_for_delegation_stake":
-                test_me_please = True
-            if key == "missing_delegation_add_parameters":
-                test_me_please = True
-            if key == "insufficient_delegation_stak":
-                test_me_please = True
-            if key == "delegator_in_cooldown":
-                test_me_please = True
-            if key == "not_a_delegator":
-                test_me_please = True
-            if key == "delegation_target_not_a_baker: ":
-                test_me_please = True
-            if key == "stake_over_maximum_threshold_for_pool":
-                test_me_please = True
-            if key == "pool_would_become_over_delegated":
-                test_me_please = True
-            if key == "pool_closed":
-                test_me_please = True
-
-            _type = key
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-            elif type(value) in [
-                RejectReason.InvalidInitMethod,
-                RejectReason.InvalidReceiveMethod,
-                RejectReason.AmountTooLarge,
-                RejectReason.RejectedInit,
-                RejectReason.RejectedReceive,
-            ]:
-                result[key] = self.convertTypeWithSingleValues(value)
-
-            elif type(value) == RejectReason.DuplicateCredIds:
-                result[key] = self.convertDuplicateCredIds(value)
-        return result, _type
-
-    def convertRejectReasonNone(self, message) -> CCD_AccountTransactionEffects_None:
-        result = {}
-        _type = None
-        for descriptor in message.DESCRIPTOR.fields:
-            key, value = self.get_key_value_from_descriptor(descriptor, message)
-
-            if type(value) in self.simple_types:
-                result[key] = self.convertType(value)
-
-            elif type(value) == RejectReason:
-                result[key], _type = self.convertRejectReason(value)
-
-        return CCD_AccountTransactionEffects_None(**result), _type
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/service_pb2.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/service_pb2.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/service_pb2_grpc.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/grpcclient/types_pb2.py` & `sharingiscaring-0.2.9/sharingiscaring/grpcclient/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/mongodb.py` & `sharingiscaring-0.2.9/sharingiscaring/mongodb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from enum import Enum
-from sharingiscaring.mongodb_queries._search_transfers import Mixin as _search_transfers
-from sharingiscaring.mongodb_queries._subscriptions import Mixin as _subscriptions
-from sharingiscaring.mongodb_queries._baker_distributions import Mixin as _distributions
-from sharingiscaring.mongodb_queries._store_block import Mixin as _store_block
-from sharingiscaring.mongodb_queries._apy_calculations import Mixin as _apy_calculations
+from .mongodb_queries._search_transfers import Mixin as _search_transfers
+from .mongodb_queries._subscriptions import Mixin as _subscriptions
+from .mongodb_queries._baker_distributions import Mixin as _distributions
+from .mongodb_queries._store_block import Mixin as _store_block
+from .mongodb_queries._apy_calculations import Mixin as _apy_calculations
 from sharingiscaring.GRPCClient.CCD_Types import *
 
-import motor.motor_asyncio
-from motor.motor_asyncio import AsyncIOMotorCollection
-import os
 from pymongo import MongoClient
 from pymongo.collection import Collection
-
 from rich.console import Console
 from typing import Dict
 from sharingiscaring.tooter import Tooter, TooterType, TooterChannel
 
 console = Console()
 
 from pydantic import BaseModel, Extra, Field
@@ -70,15 +66,14 @@
     sender: str
     receiver: str = None
     sender_canonical: str
     receiver_canonical: str = None
     amount: int = None
     type: dict[str, str]
     block_height: int
-    memo: str = None
 
 
 class MongoTypeInvolvedContract(BaseModel):
     """
     Involved Contract. This type is stored in the collection `involved_contracts`.
 
     :Parameters:
@@ -275,124 +270,75 @@
     paydays = "paydays"
     paydays_performance = "paydays_performance"
     paydays_rewards = "paydays_rewards"
     paydays_apy_intermediate = "paydays_apy_intermediate"
     paydays_current_payday = "paydays_current_payday"
     paydays_helpers = "paydays_helpers"
     involved_accounts_all = "involved_accounts_all"
-    involved_accounts_all_top_list = "involved_accounts_all_top_list"
     involved_accounts_transfer = "involved_accounts_transfer"
     involved_contracts = "involved_contracts"
     nightly_accounts = "nightly_accounts"
     blocks_at_end_of_day = "blocks_at_end_of_day"
     blocks_per_day = "blocks_per_day"
     helpers = "helpers"
     memo_transaction_hashes = "memo_transaction_hashes"
     cns_domains = "cns_domains"
-    bot_messages = "bot_messages"
-    dashboard_nodes = "dashboard_nodes"
-    tokens_accounts = "tokens_accounts"
-    tokens_tags = "tokens_tags"
-    tokens_logged_events = "tokens_logged_events"
-    tokens_token_addresses = "tokens_token_addresses"
-
-
-class CollectionsUtilities(Enum):
-    labeled_accounts = "labeled_accounts"
-    labeled_accounts_metadata = "labeled_accounts_metadata"
-    users_prod = "users_prod"
-    users_dev = "users_dev"
-    exchange_rates = "exchange_rates"
-    exchange_rates_historical = "exchange_rates_historical"
-
-
-FALLBACK_URI = f"concordium-explorer.nl:27027,secondary.sprocker.nl:27027,arbiter.sprocker.nl:27027/?replicaSet=rs2"
 
 
 class MongoDB(
     _search_transfers,
     _subscriptions,
     _distributions,
     _store_block,
     _apy_calculations,
 ):
     def __init__(self, mongo_config, tooter: Tooter):
         self.tooter: Tooter = tooter
-        if "MONGODB_URI" not in mongo_config:
-            MONGO_URI = FALLBACK_URI
-        else:
-            MONGO_URI = (
-                mongo_config["MONGODB_URI"]
-                if mongo_config["MONGODB_URI"] is not None
-                else FALLBACK_URI
-            )
+
         try:
             con = MongoClient(
-                f'mongodb://admin:{mongo_config["MONGODB_PASSWORD"]}@{MONGO_URI}'
+                f'mongodb://admin:{mongo_config["MONGODB_PASSWORD"]}@{mongo_config["MONGO_IP"]}:{mongo_config["MONGO_PORT"]}'
             )
-            self.connection: MongoClient = con
+            self.db = con.concordium
+            self.testnet_db = con.concordium_testnet
+            self.mainnet_db = con.concordium_mainnet
+            self.collection_blocks = self.db["blocks"]
+            self.collection_transactions = self.db["transactions"]
+            self.collection_messages = self.db["bot_messages"]
+            self.collection_accounts_involved = self.db["accounts_involved"]
+            self.collection_paydays = self.db["paydays"]
+            self.collection_paydays_performance = self.db["paydays_performance"]
+            self.collection_paydays_rewards = self.db["paydays_rewards"]
+            self.collection_paydays_apy = self.db["paydays_apy"]
+            self.collection_paydays_apy_intermediate = self.db[
+                "paydays_apy_intermediate"
+            ]
+
+            self.collection_involved_accounts_all = self.db["involved_accounts_all"]
+            self.collection_involved_accounts_transfer = self.db[
+                "involved_accounts_transfer"
+            ]
+            self.collection_involved_contracts = self.db["involved_contracts"]
+            self.collection_nightly_accounts = self.db["nightly_accounts"]
+            self.collection_blocks_at_end_of_day = self.db["blocks_at_end_of_day"]
+            self.collection_helpers = self.db["helpers"]
+            self.collection_memo_transaction_hashes = self.db["memo_transaction_hashes"]
+            self.collection_blocks_grpc = self.db["blocks_grpc"]
+            self.collection_transactions_grpc = self.db["transactions_grpc"]
+            self.collection_instances = self.db["instances"]
 
-            self.mainnet_db = con["concordium_mainnet"]
             self.mainnet: Dict[Collections, Collection] = {}
             for collection in Collections:
                 self.mainnet[collection] = self.mainnet_db[collection.value]
 
-            self.testnet_db = con["concordium_testnet"]
             self.testnet: Dict[Collections, Collection] = {}
             for collection in Collections:
                 self.testnet[collection] = self.testnet_db[collection.value]
 
-            self.utilities_db = con["concordium_utilities"]
-            self.utilities: Dict[CollectionsUtilities, Collection] = {}
-            for collection in CollectionsUtilities:
-                self.utilities[collection] = self.utilities_db[collection.value]
-
             console.log(con.server_info()["version"])
         except Exception as e:
             print(e)
             tooter.send(
                 channel=TooterChannel.NOTIFIER,
                 message=f"BOT ERROR! Cannot connect to MongoDB, with error: {e}",
                 notifier_type=TooterType.MONGODB_ERROR,
             )
-
-
-class MongoMotor(
-    _search_transfers,
-    _subscriptions,
-    _distributions,
-    _store_block,
-    _apy_calculations,
-):
-    def __init__(self, mongo_config, tooter: Tooter):
-        self.tooter: Tooter = tooter
-        if "MONGODB_URI" not in mongo_config:
-            MONGO_URI = FALLBACK_URI
-        else:
-            MONGO_URI = (
-                mongo_config["MONGODB_URI"]
-                if mongo_config["MONGODB_URI"] is not None
-                else FALLBACK_URI
-            )
-        try:
-            con = motor.motor_asyncio.AsyncIOMotorClient(
-                f'mongodb://admin:{mongo_config["MONGODB_PASSWORD"]}@{MONGO_URI}'
-            )
-
-            self.mainnet_db = con["concordium_mainnet"]
-            self.mainnet: Dict[Collections, AsyncIOMotorCollection] = {}
-            for collection in Collections:
-                self.mainnet[collection] = self.mainnet_db[collection.value]
-
-            self.testnet_db = con["concordium_testnet"]
-            self.testnet: Dict[Collections, AsyncIOMotorCollection] = {}
-            for collection in Collections:
-                self.testnet[collection] = self.testnet_db[collection.value]
-
-            # console.log(f'Motor: {con.server_info()["version"]}')
-        except Exception as e:
-            print(e)
-            tooter.send(
-                channel=TooterChannel.NOTIFIER,
-                message=f"BOT ERROR! Cannot connect to Motor MongoDB, with error: {e}",
-                notifier_type=TooterType.MONGODB_ERROR,
-            )
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_apy_calculations.py` & `sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_apy_calculations.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_baker_distributions.py` & `sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_baker_distributions.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_search_transfers.py` & `sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_search_transfers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pymongo
-from pymongo import DESCENDING
 
 
 class Mixin:
     def search_txs_on_list_of_hashes(
         self, list_of_hashses, skip, limit, sort_on="amount", sort_direction=-1
     ):
         """
@@ -63,14 +62,15 @@
         start_block,
         end_block,
         # skip, limit,
         list_of_tx_hashes_with_memo_predicate,
         # sort_on='amount', sort_direction=-1,
         filter_on_memo_txs=False,
     ):
+
         pipeline = []
 
         if transfer_type == "scheduled":
             pipeline.extend(
                 [{"$match": {"contents": {"$in": ["transferWithSchedule"]}}}]
             )
 
@@ -101,14 +101,15 @@
         start_block,
         end_block,
         # skip, limit,
         list_of_tx_hashes_with_memo_predicate,
         # sort_on='amount', sort_direction=-1,
         filter_on_memo_txs=False,
     ):
+
         pipeline = []
 
         if transfer_type == "transferred_with_schedule":
             pipeline.extend(
                 [{"$match": {"contents": {"$in": ["transferred_with_schedule"]}}}]
             )
 
@@ -306,14 +307,15 @@
         skip,
         limit,
         list_of_tx_hashes,
         sort_on="amount",
         sort_direction=-1,
         filter_on_tx_hashes=False,
     ):
+
         sort_direction = (
             pymongo.ASCENDING if sort_direction == 1 else pymongo.DESCENDING
         )
         sort_condition = (
             {"$sort": {"amount_ccd": sort_direction}}
             if sort_on == "amount"
             else {"$sort": {"blockInfo.blockSlotTime": sort_direction}}
@@ -388,14 +390,15 @@
         skip,
         limit,
         list_of_tx_hashes,
         sort_on="amount",
         sort_direction=-1,
         filter_on_tx_hashes=False,
     ):
+
         sort_direction = (
             pymongo.ASCENDING if sort_direction == 1 else pymongo.DESCENDING
         )
         sort_condition = (
             {"$sort": {"amount_ccd": sort_direction}}
             if sort_on == "amount"
             else {"$sort": {"blockInfo.blockSlotTime": sort_direction}}
@@ -461,88 +464,65 @@
         return pipeline
 
     def search_txs_hashes_for_account_as_sender_with_params(
         self, account_id, start_block, end_block
     ):
         pipeline = [
             {"$match": {"sender_canonical": {"$eq": account_id[:29]}}},
-            {"$match": {"block_height": {"$gt": start_block, "$lte": end_block}}},
+            {"$match": {"blockHeight": {"$gt": start_block, "$lte": end_block}}},
         ]
         return pipeline
 
     def search_txs_hashes_for_account_as_receiver_with_params(
         self, account_id, start_block, end_block
     ):
         pipeline = [
             {"$match": {"receiver_canonical": {"$eq": account_id[:29]}}},
-            {"$match": {"block_height": {"$gt": start_block, "$lte": end_block}}},
-        ]
-        return pipeline
-
-    def search_txs_hashes_for_account_as_sender_with_params_id_only(
-        self, account_id, start_block, end_block
-    ):
-        pipeline = [
-            {"$match": {"sender_canonical": {"$eq": account_id[:29]}}},
-            {"$match": {"block_height": {"$gt": start_block, "$lte": end_block}}},
-            {"$project": {"_id": 1}},
-        ]
-        return pipeline
-
-    def search_txs_hashes_for_account_as_receiver_with_params_id_only(
-        self, account_id, start_block, end_block
-    ):
-        pipeline = [
-            {"$match": {"receiver_canonical": {"$eq": account_id[:29]}}},
-            {"$match": {"block_height": {"$gt": start_block, "$lte": end_block}}},
-            {"$project": {"_id": 1}},
+            {"$match": {"blockHeight": {"$gt": start_block, "$lte": end_block}}},
         ]
         return pipeline
 
     def search_txs_in_hash_list(self, tx_hashes):
-        pipeline = [
-            {"$match": {"_id": {"$in": tx_hashes}}},
-            {"$sort": {"block_info.slot_time": DESCENDING}},
-        ]
+        pipeline = [{"$match": {"_id": {"$in": tx_hashes}}}]
         return pipeline
 
     def search_txs_in_transactions(self, start_block, end_block):
         pipeline = [
             {
                 "$match": {
-                    "block_info.block_height": {"$gt": start_block, "$lte": end_block}
+                    "blockInfo.blockHeight": {"$gt": start_block, "$lte": end_block}
                 }
             },
         ]
         return pipeline
 
     def heights_with_transactions_after(self, start_block):
         pipeline = [
-            {"$match": {"block_height": {"$gt": start_block}}},
+            {"$match": {"blockHeight": {"$gt": start_block}}},
             {"$project": {"_id": 0, "blockHeight": 1}},
         ]
         return pipeline
 
     def search_txs_non_finalized(self):
         pipeline = [
-            {"$match": {"block_info.finalized": False}},
+            {"$match": {"blockInfo.finalized": False}},
         ]
         return pipeline
 
     ### exchange search
     def search_exchange_txs_as_receiver(
         self, exchanges_canonical: list, start_block: int, end_block: int
     ):
         pipeline = [
             {"$match": {"receiver_canonical": {"$in": exchanges_canonical}}},
-            {"$match": {"block_height": {"$gt": start_block, "$lte": end_block}}},
+            {"$match": {"blockHeight": {"$gt": start_block, "$lte": end_block}}},
         ]
         return pipeline
 
     def search_exchange_txs_as_sender(
         self, exchanges_canonical: list, start_block: int, end_block: int
     ):
         pipeline = [
             {"$match": {"sender_canonical": {"$in": exchanges_canonical}}},
-            {"$match": {"block_height": {"$gt": start_block, "$lte": end_block}}},
+            {"$match": {"blockHeight": {"$gt": start_block, "$lte": end_block}}},
         ]
         return pipeline
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_store_block.py` & `sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_store_block.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/mongodb_queries/_subscriptions.py` & `sharingiscaring-0.2.9/sharingiscaring/mongodb_queries/_subscriptions.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/node.py` & `sharingiscaring-0.2.9/sharingiscaring/node.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/pool.py` & `sharingiscaring-0.2.9/sharingiscaring/pool.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/sharingiscaring/tooter.py` & `sharingiscaring-0.2.9/sharingiscaring/tooter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,113 +1,91 @@
 from apprise import Apprise
 from enum import Enum
 import json
 from urllib.request import Request
 import requests
 
-
 class TooterType(Enum):
     INFO = "info"
     GRAPHQL_ERROR = "graphql error"
     MONGODB_ERROR = "mongodb error"
     REQUESTS_ERROR = "requests error"
     BOT_MAIN_LOOP_ERROR = "bot_main_loop_error"
-
+    
 
 class TooterChannel(Enum):
-    BOT = "bot"
-    NOTIFIER = "notifier"
-    SMART = "smart"
-
+    BOT = 'bot'
+    NOTIFIER = 'notifier'
 
 class Tooter:
-    def __init__(
-        self,
-        environment: str,
-        branch: str,
-        NOTIFIER_API_TOKEN: str,
-        BOT_API_TOKEN: str,
-        FASTMAIL_TOKEN: str,
-    ) -> None:
+    def __init__(self, environment: str, branch: str, 
+            NOTIFIER_API_TOKEN: str, BOT_API_TOKEN: str, FASTMAIL_TOKEN: str
+            ) -> None:
         # self.appriser           = appriser
-        self.environment = environment
-        self.branch = branch
+        self.environment        = environment
+        self.branch             = branch
         self.NOTIFIER_API_TOKEN = NOTIFIER_API_TOKEN
-        self.BOT_API_TOKEN = BOT_API_TOKEN
-        self.FASTMAIL_TOKEN = FASTMAIL_TOKEN
-        self.url = "https://tooter.concordium-explorer.nl/notify/"
-        self.email_part_1 = "mailto://fastmail.com/?to="
-        self.email_part_2 = f"&user=sdr@16april1973.nl&pass={FASTMAIL_TOKEN}&from=Concordium Explorer Bot&from=bot@concordium-explorer.nl"
+        self.BOT_API_TOKEN      = BOT_API_TOKEN
+        self.FASTMAIL_TOKEN     = FASTMAIL_TOKEN
+        self.url                = "https://tooter.concordium-explorer.nl/notify/"
+        self.email_part_1       = "mailto://fastmail.com/?to="
+        self.email_part_2       = f"&user=sdr@16april1973.nl&pass={FASTMAIL_TOKEN}&from=Concordium Explorer Bot&from=bot@concordium-explorer.nl"
 
     def email(self, title: str, body: str, email_address: str, value=None, error=None):
         payload = {
-            "urls": f"{self.email_part_1}{email_address}{self.email_part_2 }",
-            "title": title,
-            "body": body,
+            'urls': f"{self.email_part_1}{email_address}{self.email_part_2 }",
+            'title': title,
+            'body': body,
         }
         r = requests.post(self.url, json=payload)
-
-    def relay(
-        self,
-        channel: TooterChannel,
-        body: str,
-        notifier_type: TooterType,
-        title: str,
-        chat_id: int = None,
-        value=None,
-        error=None,
-        bcc=False,
-    ):
-        API_TO_USE = (
-            self.BOT_API_TOKEN
-            if channel == TooterChannel.BOT
-            else self.NOTIFIER_API_TOKEN
-        )
-        chat_id = "913126895" if channel == TooterChannel.NOTIFIER else chat_id
+        
+    
+    def relay(self, 
+        channel: TooterChannel, 
+        body: str, 
+        notifier_type: TooterType, 
+        title: str, 
+        chat_id: int=None, 
+        value=None, 
+        error=None, 
+        bcc = False
+        ):
+        API_TO_USE = self.BOT_API_TOKEN if channel == TooterChannel.BOT else self.NOTIFIER_API_TOKEN
+        chat_id = '913126895' if channel == TooterChannel.NOTIFIER else chat_id
 
         payload = {
-            "urls": f"tgram://{API_TO_USE}/{chat_id}",
-            "title": title,
-            "body": body,
-            "format": "html",
+            'urls': f'tgram://{API_TO_USE}/{chat_id}',
+            'title': title,
+            'body': body,
+            'format': 'html'
         }
         r = requests.post(self.url, json=payload)
 
         if bcc:
             payload = {
-                "urls": f"tgram://{self.NOTIFIER_API_TOKEN}/913126895",
-                "title": f"{title} | to: {chat_id}",
-                "body": body,
-                "format": "html",
+                'urls': f'tgram://{self.NOTIFIER_API_TOKEN}/913126895',
+                'title': f"{title} | to: {chat_id}",
+                'body': body,
+                'format': 'html'
             }
             r = requests.post(self.url, json=payload)
+    
+        
+    def send(self, channel: TooterChannel, message: str, notifier_type: TooterType, chat_id: int=None, value=None, error=None):
+        API_TO_USE = self.BOT_API_TOKEN if channel == TooterChannel.BOT else self.NOTIFIER_API_TOKEN
+        chat_id = '913126895' if channel == TooterChannel.NOTIFIER else chat_id
 
-    def send(
-        self,
-        channel: TooterChannel,
-        message: str,
-        notifier_type: TooterType,
-        chat_id: int = None,
-        value=None,
-        error=None,
-    ):
-        API_TO_USE = (
-            self.BOT_API_TOKEN
-            if channel == TooterChannel.BOT
-            else self.NOTIFIER_API_TOKEN
-        )
-        chat_id = "913126895" if channel == TooterChannel.NOTIFIER else chat_id
-
-        title = f"t: {notifier_type.value} | e: {self.environment} | b: {self.branch}"
-        body = message
+        title   = f"t: {notifier_type.value} | e: {self.environment} | b: {self.branch}"
+        body    = message
         if value:
-            body += "| value: {value} "
+            body += '| value: {value} '
         if error:
-            body += "| error: {error}."
+            body += '| error: {error}.' 
 
         payload = {
-            "urls": f"tgram://{API_TO_USE}/{chat_id}",
-            "title": title,
-            "body": body,
-            "format": "html",
+            'urls': f'tgram://{API_TO_USE}/{chat_id}',
+            'title': title,
+            'body': body,
+            'format': 'html'
         }
         r = requests.post(self.url, json=payload)
+
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/transaction.py` & `sharingiscaring-0.2.9/sharingiscaring/transaction.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 from enum import Enum
 import dateutil
 from .cns import CNSDomain, CNSActions
-
+from .client import ConcordiumClient
 from sharingiscaring.block import ConcordiumBlockInfo
 import io
 from rich.console import Console
-
 console = Console()
 
-
-# sender, receiver, txHash, contract, amount, tokenId, self.cns_domain.domain_name, self
+#sender, receiver, txHash, contract, amount, tokenId, self.cns_domain.domain_name, self
 class ClassificationResult:
     def __init__(self):
-        self.sender = None
-        self.receiver = None
-        self.txHash = None
-        self.contract = None
-        self.amount = None
-        self.tokenId = None
-        self.domain_name = None
-        self.type = None
-        self.contents = None
+        self.sender         = None
+        self.receiver       = None
+        self.txHash         = None
+        self.contract       = None
+        self.amount         = None
+        self.tokenId        = None
+        self.domain_name    = None
+        self.type           = None
+        self.contents       = None
         self.accounts_involved_all = False
         self.accounts_involved_transfer = False
         self.contracts_involved = False
         self.list_of_contracts_involved = set()
-
+        
 
 class DelegationAndStakingResult:
     def __init__(self):
-        self.sender = None
-        self.bakerId = None
-        self.txHash = None
-        self.message = ""
+        self.sender         = None
+        self.bakerId        = None
+        self.txHash         = None
+        self.message        = ''
         self.request_target = None
-        self.perc = None
-        self.unstaked = False
-        self.unstaked_amount = 0
-
-
-class TransactionClass(Enum):
-    AccountTransaction = "accountTransaction"
-    CredentialDeploymentTransaction = "credentialDeploymentTransaction"
-    UpdateTransaction = "updateTransaction"
-
+        self.perc           = None
+        self.unstaked       = False
+        self.unstaked_amount= 0
+
+class TransactionClass (Enum):
+    AccountTransaction='accountTransaction'
+    CredentialDeploymentTransaction='credentialDeploymentTransaction'
+    UpdateTransaction='updateTransaction'
 
 class TransactionType(Enum):
     # https://github.com/Concordium/concordium-scan/blob/e95e8b2b191fefcf381ef4b4a1c918dd1f11ae05/frontend/src/queries/useTransactionQuery.ts
     AccountCreated = """
     ... on AccountCreated {
         accountAddress {
             asString
@@ -58,119 +54,119 @@
     ... on AmountAddedByDecryption {
         amount
         accountAddress {
             asString
         }
     }
     """
-    BakerAdded = """
+    BakerAdded="""
     ... on BakerAdded {
         bakerId
         restakeEarnings
         stakedAmount
         electionKey
         signKey
         aggregationKey
         accountAddress {
             asString
         }
     }
     """
-    BakerKeysUpdated = """
+    BakerKeysUpdated="""
     ... on BakerKeysUpdated {
         bakerId
         electionKey
         signKey
         aggregationKey
         accountAddress {
             asString
         }
     }
     """
-    BakerRemoved = """
+    BakerRemoved="""
     ... on BakerRemoved {
         bakerId
         accountAddress {
             asString
         }
     }
     """
-    BakerSetBakingRewardCommission = """
+    BakerSetBakingRewardCommission="""
     ... on BakerSetBakingRewardCommission {
         bakerId
         bakingRewardCommission
         accountAddress {
             asString
         }
     }
     """
-    BakerSetFinalizationRewardCommission = """
+    BakerSetFinalizationRewardCommission="""
     ... on BakerSetFinalizationRewardCommission {
         bakerId
         finalizationRewardCommission
         accountAddress {
             asString
         }
     }
     """
-    BakerSetMetadataURL = """
+    BakerSetMetadataURL="""
     ... on BakerSetMetadataURL {
         bakerId
         metadataUrl
         accountAddress {
             asString
         }
     }
     """
-    BakerSetOpenStatus = """
+    BakerSetOpenStatus="""
     ... on BakerSetOpenStatus {
         bakerId
         openStatus
         accountAddress {
             asString
         }
     }
     """
-    BakerSetRestakeEarnings = """
+    BakerSetRestakeEarnings="""
     ... on BakerSetRestakeEarnings {
         bakerId
         restakeEarnings
         accountAddress {
             asString
         }
     }    
     """
-    BakerSetTransactionFeeCommission = """
+    BakerSetTransactionFeeCommission="""
     ... on BakerSetTransactionFeeCommission {
         bakerId
         transactionFeeCommission
         accountAddress {
             asString
         }
     }
     """
-    BakerStakeDecreased = """
+    BakerStakeDecreased="""
     ... on BakerStakeDecreased {
         bakerId
         newStakedAmount
         accountAddress {
             asString
         }
     }
     """
-    BakerStakeIncreased = """
+    BakerStakeIncreased="""
     ... on BakerStakeIncreased {
         bakerId
         newStakedAmount
         accountAddress {
             asString
         }
     }
     """
-    ChainUpdateEnqueued = """
+    ChainUpdateEnqueued="""
     ... on ChainUpdateEnqueued {
         effectiveImmediately
         __typename
 	effectiveTime
 	payload {
 		__typename
 		...on AddAnonymityRevokerChainUpdatePayload {
@@ -255,15 +251,15 @@
 				denominator
 				numerator
 			}
 		}
 	}
     }
     """
-    ContractInitialized = """
+    ContractInitialized="""
     ... on ContractInitialized {
         amount
         contractAddress {
             __typename
             asString
             index
             subIndex
@@ -271,43 +267,43 @@
         HEX:eventsAsHex {
             nodes 
         }
         initName
         moduleRef
     }
     """
-    ContractInterrupted = """
+    ContractInterrupted="""
     ... on ContractInterrupted {
         contractAddress {
             __typename
             asString
             index
             subIndex
         }
         hex_events:eventsAsHex
     }
     """
-    ContractModuleDeployed = """
+    ContractModuleDeployed="""
     ... on ContractModuleDeployed {
         moduleRef
         __typename
     }
     """
-    ContractResumed = """
+    ContractResumed="""
     ... on ContractResumed {
         contractAddress {
             __typename
             asString
             index
             subIndex
         }
         success
     }
     """
-    ContractUpdated = """
+    ContractUpdated="""
     ... on ContractUpdated {
         amount
         contractAddress {
             __typename
             asString
             index
             subIndex
@@ -328,128 +324,128 @@
                 subIndex
             }
         }
         messageAsHex
         receiveName
     }
     """
-    CredentialDeployed = """
+    CredentialDeployed="""
     ... on CredentialDeployed {
         accountAddress {
             asString
         }
         regId
     }
     """
-    CredentialKeysUpdated = """
+    CredentialKeysUpdated="""
     ... on CredentialKeysUpdated {
         credId
     }
     """
-    CredentialsUpdated = """
+    CredentialsUpdated="""
     ... on CredentialsUpdated {
         accountAddress {
             asString
         }
         newCredIds
         newThreshold
         removedCredIds
     }
     """
-    DataRegistered = """
+    DataRegistered="""
     ... on DataRegistered {
         dataAsHex
     }
     """
-    DelegationAdded = """
+    DelegationAdded="""
     ... on DelegationAdded {
         accountAddress {
             asString
         }
         delegatorId
     }
     """
-    DelegationRemoved = """
+    DelegationRemoved="""
     ... on DelegationRemoved {
         accountAddress {
             asString
         }
         delegatorId
     }
     """
-    DelegationSetDelegationTarget = """
+    DelegationSetDelegationTarget="""
     ... on DelegationSetDelegationTarget {
         accountAddress {
             asString
         }
         delegationTarget {
             __typename
             ... on BakerDelegationTarget {
                 bakerId
             }
         }
         delegatorId
     }
     """
-    DelegationSetRestakeEarnings = """
+    DelegationSetRestakeEarnings="""
     ... on DelegationSetRestakeEarnings {
         accountAddress {
             asString
         }
         delegatorId
         restakeEarnings
     }
     """
-    DelegationStakeDecreased = """
+    DelegationStakeDecreased="""
     ... on DelegationStakeDecreased {
         accountAddress {
             asString
         }
         delegatorId
         newStakedAmount
     }
     """
-    DelegationStakeIncreased = """
+    DelegationStakeIncreased="""
     ... on DelegationStakeIncreased {
         accountAddress {
             asString
         }
         delegatorId
         newStakedAmount
     }
     """
-    EncryptedAmountsRemoved = """
+    EncryptedAmountsRemoved="""
     ... on EncryptedAmountsRemoved {
         accountAddress {
                 asString
             }
         inputAmount
         newEncryptedAmount
         upToIndex
     }
     """
-    EncryptedSelfAmountAdded = """
+    EncryptedSelfAmountAdded="""
     ... on EncryptedSelfAmountAdded {
         accountAddress {
                 asString
             }
         amount
         newEncryptedAmount
     }
     """
-    NewEncryptedAmount = """
+    NewEncryptedAmount="""
     ... on NewEncryptedAmount {
         accountAddress {
                 asString
             }
         encryptedAmount
         newIndex
     }
     """
-    TransferMemo = """
+    TransferMemo="""
     ... on TransferMemo {
         decoded {
             text
         }
         rawHex
     }
     """
@@ -500,875 +496,735 @@
             asString
         }
         totalAmount
         }
         
     """
 
-
 class EventOpenStatusFromQLToNode(Enum):
-    OPEN_FOR_ALL = "openForAll"
-    CLOSED_FOR_NEW = "closedForNew"
-    CLOSED_FOR_ALL = "closedForAll"
-
+    OPEN_FOR_ALL = 'openForAll'
+    CLOSED_FOR_NEW = 'closedForNew'
+    CLOSED_FOR_ALL = 'closedForAll'
 
 class TransactionTypeFromQLToNode(Enum):
-    AccountTransaction = "accountTransaction"
-    CredentialDeploymentTransaction = "credentialDeploymentTransaction"
-    UpdateTransaction = "updateTransaction"
-
+    AccountTransaction              = 'accountTransaction'
+    CredentialDeploymentTransaction = 'credentialDeploymentTransaction'
+    UpdateTransaction               = 'updateTransaction'
 
 class TransactionContentsFromQLToNode(Enum):
     # AccountTransaction
-    ADD_BAKER = "addBaker"
-    CONFIGURE_BAKER = "configureBaker"
-    CONFIGURE_DELEGATION = "configureDelegation"
-    DEPLOY_MODULE = "deployModule"
-    ENCRYPTED_TRANSFER = "encryptedAmountTransfer"
-    ENCRYPTED_TRANSFER_WITH_MEMO = "encryptedAmountTransferWithMemo"
-    INITIALIZE_SMART_CONTRACT_INSTANCE = "initContract"
-    REGISTER_DATA = "registerData"
-    REMOVE_BAKER = "removeBaker"
-    SIMPLE_TRANSFER = "transfer"
-    SIMPLE_TRANSFER_WITH_MEMO = "transferWithMemo"
-    TRANSFER_TO_ENCRYPTED = "transferToEncrypted"
-    TRANSFER_TO_PUBLIC = "transferToPublic"
-    TRANSFER_WITH_SCHEDULE = "transferWithSchedule"
-    TRANSFER_WITH_SCHEDULE_WITH_MEMO = "transferWithScheduleAndMemo"
-    UPDATE_BAKER_KEYS = "updateBakerKeys"
-    UPDATE_BAKER_RESTAKE_EARNINGS = "updateBakerRestakeEarnings"
-    UPDATE_BAKER_STAKE = "updateBakerStake"
-    UPDATE_CREDENTIAL_KEYS = "updateCredentialKeys"
-    UPDATE_CREDENTIALS = "updateCredentials"
-    UPDATE_SMART_CONTRACT_INSTANCE = "update"
-    UNKNOWN = "_unknown"
+    ADD_BAKER = 'addBaker'
+    CONFIGURE_BAKER = 'configureBaker'
+    CONFIGURE_DELEGATION = 'configureDelegation'
+    DEPLOY_MODULE = 'deployModule'
+    ENCRYPTED_TRANSFER = 'encryptedAmountTransfer'
+    ENCRYPTED_TRANSFER_WITH_MEMO = 'encryptedAmountTransferWithMemo'
+    INITIALIZE_SMART_CONTRACT_INSTANCE = 'initContract'
+    REGISTER_DATA = 'registerData'
+    REMOVE_BAKER = 'removeBaker'
+    SIMPLE_TRANSFER = 'transfer'
+    SIMPLE_TRANSFER_WITH_MEMO = 'transferWithMemo'
+    TRANSFER_TO_ENCRYPTED = 'transferToEncrypted'
+    TRANSFER_TO_PUBLIC = 'transferToPublic'
+    TRANSFER_WITH_SCHEDULE = 'transferWithSchedule'
+    TRANSFER_WITH_SCHEDULE_WITH_MEMO = 'transferWithScheduleAndMemo'
+    UPDATE_BAKER_KEYS = 'updateBakerKeys'
+    UPDATE_BAKER_RESTAKE_EARNINGS = 'updateBakerRestakeEarnings'
+    UPDATE_BAKER_STAKE = 'updateBakerStake'
+    UPDATE_CREDENTIAL_KEYS = 'updateCredentialKeys'
+    UPDATE_CREDENTIALS = 'updateCredentials'
+    UPDATE_SMART_CONTRACT_INSTANCE = 'update'
+    UNKNOWN = '_unknown'
 
     # CredentialDeploymentTransaction
-    NORMAL = "normal"
-    INITIAL = "initial"
+    NORMAL = 'normal'
+    INITIAL = 'initial'
 
     # UpdateTransaction
-    UPDATE_ADD_ANONYMITY_REVOKER = "updateAddAnonymityRevoker"
-    UPDATE_ADD_IDENTITY_PROVIDER = "updateAddIdentityProvider"
-    UPDATE_BAKER_STAKE_THRESHOLD = "updateBakerStake"
-    UPDATE_COOLDOWN_PARAMETERS = "updateCooldownParameters"
-    UPDATE_ELECTION_DIFFICULTY = "updateElectionDifficulty"
-    UPDATE_EURO_PER_ENERGY = "updateEuroPerEnergy"
-    UPDATE_FOUNDATION_ACCOUNT = "updateFoundationAccount"
-    UPDATE_GAS_REWARDS = "updateGASRewards"
-    UPDATE_LEVEL1_KEYS = "updateLevel1Keys"
-    UPDATE_LEVEL2_KEYS = "updateLevel2Keys"
-    UPDATE_MICRO_GTU_PER_EURO = "updateMicroGTUPerEuro"
-    UPDATE_MINT_DISTRIBUTION = "updateMintDistribution"
-    UPDATE_POOL_PARAMETERS = "updatePoolParameters"
-    UPDATE_PROTOCOL = "updateProtocol"
-    UPDATE_ROOT_KEYS = "updateRootKeys"
-    UPDATE_TIME_PARAMETERS = "updateTimeParameters"
-    UPDATE_TRANSACTION_FEE_DISTRIBUTION = "updateTransactionFeeDistribution"
-
+    UPDATE_ADD_ANONYMITY_REVOKER = 'updateAddAnonymityRevoker'
+    UPDATE_ADD_IDENTITY_PROVIDER = 'updateAddIdentityProvider'
+    UPDATE_BAKER_STAKE_THRESHOLD = 'updateBakerStake'
+    UPDATE_COOLDOWN_PARAMETERS = 'updateCooldownParameters'
+    UPDATE_ELECTION_DIFFICULTY = 'updateElectionDifficulty'
+    UPDATE_EURO_PER_ENERGY = 'updateEuroPerEnergy'
+    UPDATE_FOUNDATION_ACCOUNT = 'updateFoundationAccount'
+    UPDATE_GAS_REWARDS = 'updateGASRewards'
+    UPDATE_LEVEL1_KEYS = 'updateLevel1Keys'
+    UPDATE_LEVEL2_KEYS = 'updateLevel2Keys'
+    UPDATE_MICRO_GTU_PER_EURO = 'updateMicroGTUPerEuro'
+    UPDATE_MINT_DISTRIBUTION = 'updateMintDistribution'
+    UPDATE_POOL_PARAMETERS = 'updatePoolParameters'
+    UPDATE_PROTOCOL = 'updateProtocol'
+    UPDATE_ROOT_KEYS = 'updateRootKeys'
+    UPDATE_TIME_PARAMETERS = 'updateTimeParameters'
+    UPDATE_TRANSACTION_FEE_DISTRIBUTION = 'updateTransactionFeeDistribution'
 
 class Reward:
-    """ """
+    '''
+    '''
 
     def __init__(self, r):
         self.r = r
-
+    
+    
     def account_reward(self):
         r = self.r
-        self.tag = r["tag"]
-
-        if self.tag == "PaydayAccountReward":
-            return r["account"]
+        self.tag = r['tag']
+        
+        if  self.tag == 'PaydayAccountReward':
+            return r['account']
         else:
             return None
 
     def pool_reward(self):
         r = self.r
-        self.tag = r["tag"]
-
-        if self.tag == "PaydayPoolReward":
-            return r["poolOwner"]
+        self.tag = r['tag']
+        
+        if  self.tag == 'PaydayPoolReward':
+            return r['poolOwner']
         else:
             return None
-
-
+            
 class Event:
     def __init__(self, _event):
         self._event = _event
         self.d = {}
-
+        
     def determineAddress(self, address):
         a = {}
 
-        if address["__typename"] == "AccountAddress":
-            a = {"type": "AddressAccount", "address": address["asString"]}
-        elif address["__typename"] == "ContractAddress":
-            a = {
-                "type": "AddressContract",
-                "address": {"index": address["index"], "subindex": address["subIndex"]},
-            }
-        return a
+        if address['__typename'] == 'AccountAddress':
+            a = {'type': 'AddressAccount', 'address': address['asString']}
+        elif address['__typename'] == 'ContractAddress':
+            a = {'type': 'AddressContract', 'address': {'index': address['index'], 'subindex': address['subIndex']} }
+        return a 
 
     def decode_memo(self, hex):
         # bs = bytes.fromhex(hex)
         # return bytes.decode(bs[1:], 'UTF-8')
         try:
-            bs = io.BytesIO(bytes.fromhex(hex))
-            n = int.from_bytes(bs.read(1), byteorder="little")
+            bs=io.BytesIO(bytes.fromhex(hex))
+            n = int.from_bytes(bs.read(1), byteorder='little')
             value = bs.read(n)
             try:
-                memo = bytes.decode(value, "UTF-8")
+                memo = bytes.decode(value, 'UTF-8')
                 return memo
             except UnicodeDecodeError:
-                memo = bytes.decode(value[1:], "UTF-8")
+                memo = bytes.decode(value[1:], 'UTF-8')
                 return memo
         except:
-            return "Decoding failure..."
+            return 'Decoding failure...'
 
     def translate_memo_if_present(self):
-        if self._event["tag"] == "TransferMemo":
-            self._event["memo"] = self.decode_memo(self._event["memo"])
-
+        if self._event['tag'] == 'TransferMemo':
+            self._event['memo'] = self.decode_memo(self._event['memo'])
+       
     def translate_event_from_graphQL(self):
         e = self._event
-        etype = e["__typename"]
-        self.d["tag"] = etype
-
+        etype = e['__typename']
+        self.d['tag'] = etype
+        
         if etype == TransactionType.AccountCreated.name:
-            self.d["contents"] = e["accountAddress"]["asString"]
+            self.d['contents'] = e['accountAddress']['asString']
 
         if etype == TransactionType.AmountAddedByDecryption.name:
-            self.d["amount"] = int(e["amount"])
-            self.d["account"] = e["accountAddress"]["asString"]
-
+            self.d['amount'] = int(e['amount'])
+            self.d['account'] = e['accountAddress']['asString']
+        
         elif etype == TransactionType.BakerSetOpenStatus.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["openStatus"] = EventOpenStatusFromQLToNode[e["openStatus"]].value
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['openStatus'] = EventOpenStatusFromQLToNode[e['openStatus']].value
 
         elif etype == TransactionType.BakerSetBakingRewardCommission.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["bakingRewardCommission"] = e["bakingRewardCommission"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['bakingRewardCommission'] = e['bakingRewardCommission']
+        
         elif etype == TransactionType.BakerSetFinalizationRewardCommission.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["finalizationRewardCommission"] = e["finalizationRewardCommission"]
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['finalizationRewardCommission'] = e['finalizationRewardCommission']
 
         elif etype == TransactionType.BakerSetTransactionFeeCommission.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["transactionFeeCommission"] = e["transactionFeeCommission"]
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['transactionFeeCommission'] = e['transactionFeeCommission']
 
         elif etype == TransactionType.BakerSetMetadataURL.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["metadataUrl"] = e["metadataUrl"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['metadataUrl'] = e['metadataUrl']
+        
         elif etype == TransactionType.DelegationAdded.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["delegatorId"] = e["delegatorId"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['delegatorId'] = e['delegatorId']
+        
         elif etype == TransactionType.DelegationSetDelegationTarget.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["delegatorId"] = e["delegatorId"]
-            if e["delegationTarget"]["__typename"] == "PassiveDelegationTarget":
-                self.d["delegationTarget"] = {"delegateType": "Passive"}
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['delegatorId'] = e['delegatorId']
+            if e['delegationTarget']['__typename'] == 'PassiveDelegationTarget':
+                self.d['delegationTarget'] = {'delegateType': 'Passive'}
             else:
-                self.d["delegationTarget"] = {
-                    "delegateType": "Baker",
-                    "bakerId": e["delegationTarget"]["bakerId"],
-                }
-
+                self.d['delegationTarget'] = {'delegateType': 'Baker', 'bakerId': e['delegationTarget']['bakerId']}
+            
         elif etype == TransactionType.DelegationSetRestakeEarnings.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["delegatorId"] = e["delegatorId"]
-            self.d["restakeEarnings"] = e["restakeEarnings"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['delegatorId'] = e['delegatorId']
+            self.d['restakeEarnings'] = e['restakeEarnings']
+        
         elif etype == TransactionType.DelegationRemoved.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["delegatorId"] = e["delegatorId"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['delegatorId'] = e['delegatorId']
+        
         elif etype == TransactionType.DelegationStakeDecreased.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["delegatorId"] = e["delegatorId"]
-            self.d["newStake"] = e["newStakedAmount"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['delegatorId'] = e['delegatorId']
+            self.d['newStake'] = e['newStakedAmount']
+        
         elif etype == TransactionType.DelegationStakeIncreased.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["delegatorId"] = e["delegatorId"]
-            self.d["newStake"] = e["newStakedAmount"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['delegatorId'] = e['delegatorId']
+            self.d['newStake'] = e['newStakedAmount']
+            
         elif etype == TransactionType.BakerAdded.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["aggregationKey"] = e["aggregationKey"]
-            self.d["electionKey"] = e["electionKey"]
-            self.d["restakeEarnings"] = e["restakeEarnings"]
-            self.d["signKey"] = e["signKey"]
-            self.d["stake"] = e["stakedAmount"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['aggregationKey'] = e['aggregationKey']
+            self.d['electionKey'] = e['electionKey']
+            self.d['restakeEarnings'] = e['restakeEarnings']
+            self.d['signKey'] = e['signKey']
+            self.d['stake'] = e['stakedAmount']
+            
         elif etype == TransactionType.BakerKeysUpdated.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["aggregationKey"] = e["aggregationKey"]
-            self.d["electionKey"] = e["electionKey"]
-            self.d["signKey"] = e["signKey"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['aggregationKey'] = e['aggregationKey']
+            self.d['electionKey'] = e['electionKey']
+            self.d['signKey'] = e['signKey']
+            
         elif etype == TransactionType.BakerRemoved.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            
         elif etype == TransactionType.BakerSetRestakeEarnings.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["restakeEarnings"] = e["restakeEarnings"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['restakeEarnings'] = e['restakeEarnings']
+        
         elif etype == TransactionType.BakerStakeDecreased.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["newStake"] = e["newStakedAmount"]
-
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['newStake'] = e['newStakedAmount']
+        
         elif etype == TransactionType.BakerStakeIncreased.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["bakerId"] = e["bakerId"]
-            self.d["newStake"] = e["newStakedAmount"]
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['bakerId'] = e['bakerId']
+            self.d['newStake'] = e['newStakedAmount']
 
         elif etype == TransactionType.ChainUpdateEnqueued.name:
-            self.d["effectiveTime"] = dateutil.parser.parse(
-                e["effectiveTime"]
-            ).timestamp()
-            if e["payload"]["__typename"] == "BakerStakeThresholdChainUpdatePayload":
-                self.d["payload"] = {}
-                self.d["payload"]["update"] = {
-                    "minimumThresholdForBaking": e["payload"]["amount"]
-                }
-                self.d["payload"]["updateType"] = "bakerStakeThreshold"
-
-            elif e["payload"]["__typename"] == "ProtocolChainUpdatePayload":
-                self.d["payload"] = {}
-                self.d["payload"]["update"] = {
-                    "specificationUrl": e["payload"]["specificationUrl"],
-                    "message": e["payload"]["message"],
-                    "specificationHash": e["payload"]["specificationHash"],
-                    "specificationAuxiliaryData": e["payload"][
-                        "specificationAuxiliaryDataAsHex"
-                    ],
-                }
-                self.d["payload"]["updateType"] = "protocol"
+            self.d['effectiveTime'] = dateutil.parser.parse(e['effectiveTime']).timestamp()
+            if e['payload']['__typename'] == 'BakerStakeThresholdChainUpdatePayload':
+                self.d['payload'] = {}
+                self.d['payload']['update'] = {'minimumThresholdForBaking': e['payload']['amount']}
+                self.d['payload']['updateType'] = 'bakerStakeThreshold'
+
+            elif e['payload']['__typename'] == 'ProtocolChainUpdatePayload':
+                self.d['payload'] = {}
+                self.d['payload']['update'] = {
+                    'specificationUrl': e['payload']['specificationUrl'],
+                    'message': e['payload']['message'],
+                    'specificationHash': e['payload']['specificationHash'],
+                    'specificationAuxiliaryData': e['payload']['specificationAuxiliaryDataAsHex']
+                    }
+                self.d['payload']['updateType'] = 'protocol'
             else:
-                self.d["payload"] = e["payload"]
+                self.d['payload'] = e['payload']
 
         elif etype == TransactionType.ContractInitialized.name:
-            self.d["address"] = {
-                "index": e["contractAddress"]["index"],
-                "subindex": e["contractAddress"]["subIndex"],
-            }
-            self.d["amount"] = e["amount"]
-            self.d["contractVersion"] = 0  # note: not available in QL
-            self.d["initName"] = e["initName"]
-            self.d["ref"] = e["moduleRef"]
-            self.d["events"] = e["HEX"]["nodes"]
+            self.d['address'] = {'index': e['contractAddress']['index'], 'subindex': e['contractAddress']['subIndex'] }
+            self.d['amount'] = e['amount']
+            self.d['contractVersion'] = 0 # note: not available in QL
+            self.d['initName'] = e['initName']
+            self.d['ref'] = e['moduleRef']
+            self.d['events'] = e['HEX']['nodes']
 
         elif etype == TransactionType.ContractResumed.name:
-            self.d["address"] = {
-                "index": e["contractAddress"]["index"],
-                "subindex": e["contractAddress"]["subIndex"],
-            }
-            self.d["success"] = e["success"]
+            self.d['address'] = {'index': e['contractAddress']['index'], 'subindex': e['contractAddress']['subIndex']}
+            self.d['success'] = e['success']
 
         elif etype == TransactionType.ContractInterrupted.name:
-            self.d["address"] = {
-                "index": e["contractAddress"]["index"],
-                "subindex": e["contractAddress"]["subIndex"],
-            }
-            self.d["events"] = e["hex_events"]
-
+            self.d['address'] = {'index': e['contractAddress']['index'], 'subindex': e['contractAddress']['subIndex']}
+            self.d['events'] = e['hex_events']
+            
         elif etype == TransactionType.ContractUpdated.name:
-            self.d["address"] = {
-                "index": e["contractAddress"]["index"],
-                "subindex": e["contractAddress"]["subIndex"],
-            }
-            self.d["amount"] = e["amount"]
-            self.d["contractVersion"] = 0  # note: not available in QL
-            self.d["instigator"] = self.determineAddress(e["instigator"])
-            self.d["message"] = e["messageAsHex"]
-            self.d["receiveName"] = e["receiveName"]
-            self.d["events"] = e["eventsAsHex"]["nodes"]
+            self.d['address'] = {'index': e['contractAddress']['index'], 'subindex': e['contractAddress']['subIndex']}
+            self.d['amount'] = e['amount']
+            self.d['contractVersion'] = 0  # note: not available in QL
+            self.d['instigator'] = self.determineAddress(e['instigator'])
+            self.d['message'] = e['messageAsHex']
+            self.d['receiveName'] = e['receiveName']
+            self.d['events'] = e['eventsAsHex']['nodes']
 
         elif etype == TransactionType.ContractModuleDeployed.name:
-            self.d["contents"] = e["moduleRef"]
-
+            self.d['contents'] = e['moduleRef']
+            
         elif etype == TransactionType.CredentialDeployed.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["regId"] = e["regId"]
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['regId'] = e['regId']
+            
 
         elif etype == TransactionType.CredentialsUpdated.name:
-            self.d["account"] = e["accountAddress"]["asString"]
-            self.d["newCredIds"] = e["newCredIds"]
-            self.d["newThreshold"] = e["newThreshold"]
-            self.d["removedCredIds"] = e["removedCredIds"]
+            self.d['account'] = e['accountAddress']['asString']
+            self.d['newCredIds'] = e['newCredIds']
+            self.d['newThreshold'] = e['newThreshold']
+            self.d['removedCredIds'] = e['removedCredIds']
 
         elif etype == TransactionType.DataRegistered.name:
-            self.d["data"] = e["dataAsHex"]
-
+            self.d['data'] = e['dataAsHex']
+            
         elif etype == TransactionType.EncryptedAmountsRemoved.name:
             pass
 
         elif etype == TransactionType.NewEncryptedAmount.name:
             pass
-
+        
         elif etype == TransactionType.TransferMemo.name:
             # note this is actually NOT the same as the node, as the node does NOT decode.
-            self.d["memo"] = e["decoded"]["text"]
-
+            self.d['memo'] = e['decoded']['text']
+            
         elif etype == TransactionType.Transferred.name:
-            self.d["amount"] = int(e["amount"])
-            self.d["from"] = self.determineAddress(e["from"])
-            self.d["to"] = self.determineAddress(e["to"])
-
+            self.d['amount'] = int(e['amount'])
+            self.d['from'] = self.determineAddress(e['from'])
+            self.d['to']   = self.determineAddress(e['to'])
+            
         elif etype == TransactionType.TransferredWithSchedule.name:
-            self.d["from"] = e["fromAccountAddress"]["asString"]
-            self.d["to"] = e["toAccountAddress"]["asString"]
-            self.d["amount"] = [
-                (dateutil.parser.parse(x["timestamp"]).timestamp() * 1000, x["amount"])
-                for x in e["amountsSchedule"]["nodes"]
-            ]
-
+            self.d['from'] = e['fromAccountAddress']['asString']
+            self.d['to']   = e['toAccountAddress']['asString']
+            self.d['amount'] = [(dateutil.parser.parse(x['timestamp']).timestamp()*1000, x['amount']) for x in e['amountsSchedule']['nodes']]
+    
         return self.d
 
-
 class Transaction:
-    """
+    '''
     Canonical Transaction. Transactions from either the node or GraphQL will be morphed to fit this class
-    Node language will be the go-to point, so graphQL terms are translated to fit the node.
-    """
+    Node language will be the go-to point, so graphQL terms are translated to fit the node. 
+    '''
 
     def __init__(self, node):
         self.node = node
         self.block: ConcordiumBlockInfo
-
+        
+        
     def find_memo_and_amount(self):
         self.memo = None
         self.amount = None
-        if (self.contents == "transferWithMemo") or (self.contents == "Transferred"):
-            if "events" in self.result:
-                for event in self.result.get("events", []):
-                    if event["tag"] == TransactionType.TransferMemo.name:
-                        self.memo = event["memo"]
-                    if event["tag"] == TransactionType.Transferred.name:
-                        self.amount = event["amount"]
+        if ((self.contents == 'transferWithMemo') or (self.contents == 'Transferred')):
+            if 'events' in self.result:
+                for event in self.result.get('events', []):
+                    if event['tag'] == TransactionType.TransferMemo.name:
+                        self.memo = event['memo']
+                    if event['tag'] == TransactionType.Transferred.name:
+                        self.amount = event['amount']
 
         return self
 
     def get_domain_from_cache_or_node(self):
         if self.cns_domain.tokenId in self.node.cns_cache_by_token_id:
-            self.cns_domain.domain_name = self.node.cns_cache_by_token_id[
-                self.cns_domain.tokenId
-            ]
+            self.cns_domain.domain_name = self.node.cns_cache_by_token_id[self.cns_domain.tokenId]
             console.log(f"Using cache for {self.cns_domain.domain_name}")
         else:
             self.cns_domain.get_cns_domain_name(self.node, self.cns_domain.tokenId)
 
-            self.node.cns_cache_by_token_id[
-                self.cns_domain.tokenId
-            ] = self.cns_domain.domain_name
-            self.node.cns_cache_by_name[
-                self.cns_domain.domain_name
-            ] = self.cns_domain.tokenId
+            self.node.cns_cache_by_token_id[self.cns_domain.tokenId] = self.cns_domain.domain_name
+            self.node.cns_cache_by_name[self.cns_domain.domain_name] = self.cns_domain.tokenId
             self.node.save_cns_cache()
             console.log(f"Saving cache for {self.cns_domain.domain_name}")
 
+
     def set_possible_cns_domain(self):
         self.cns_domain = CNSDomain()
-        if "events" in self.result:
-            for event in self.result.get("events", []):
-                if event["tag"] in [
-                    TransactionType.ContractInterrupted.name,
-                    "Interrupted",
-                ]:
+        if 'events' in self.result:
+            for event in self.result.get('events', []):
+                if event['tag'] in [TransactionType.ContractInterrupted.name, 'Interrupted']:
                     # console.log(f'{event["tag"]=}')
-                    if "events" in event:
-                        if len(event["events"]) > 0:
-                            the_event = event["events"][0]
-
-                            (
-                                tag_,
-                                contract_index,
-                                contract_subindex,
-                                token_id_,
-                                seller_,
-                                winner_,
-                                price_,
-                                seller_share,
-                                royalty_length_,
-                                royalties,
-                                owner_,
-                                bidder_,
-                                amount_,
-                            ) = self.cns_domain.finalize(the_event)
-
-                            # tag_, contract_index, contract_subindex, \
-                            # token_id_, bidder_, amount_ = self.cns_domain.bidEvent(the_event)
-
-                            self.cns_domain.tokenId = token_id_
-                            # self.cns_domain.amount = amount_
-
-                            self.get_domain_from_cache_or_node()
+                    if 'events' in event:
+                        if (len (event['events']) > 0):
+                                the_event = event["events"][0]
+                                    
+                                tag_, contract_index, contract_subindex, token_id_, \
+                                seller_, winner_, price_, seller_share, royalty_length_, \
+                                royalties, owner_, bidder_, amount_ = self.cns_domain.finalize(the_event)
+                                
+                                # tag_, contract_index, contract_subindex, \
+                                # token_id_, bidder_, amount_ = self.cns_domain.bidEvent(the_event)
+
+                                self.cns_domain.tokenId = token_id_
+                                # self.cns_domain.amount = amount_  
+                                
+                                self.get_domain_from_cache_or_node()
                 # console.log(f"{event['tag']=}")
-                if event["tag"] in [TransactionType.ContractUpdated.name, "Updated"]:
+                if event['tag'] in [TransactionType.ContractUpdated.name, 'Updated']:
                     # console.log(f'{event["receiveName"]=}')
-                    self.cns_domain.function_calls[event["receiveName"]] = event[
-                        "message"
-                    ]
-
-                    if event["receiveName"] == "BictoryCnsNft.transfer":
+                    self.cns_domain.function_calls[event["receiveName"]] = event["message"]
+                    
+                    if event["receiveName"] == 'BictoryCnsNft.transfer':
                         self.cns_domain.action = CNSActions.transfer
-                        (
-                            self.cns_domain.tokenId,
-                            self.cns_domain.transfer_to,
-                        ) = self.cns_domain.decode_transfer_to_from(event["message"])
-
+                        self.cns_domain.tokenId, self.cns_domain.transfer_to = \
+                            self.cns_domain.decode_transfer_to_from(event["message"])
+                        
                         self.get_domain_from_cache_or_node()
 
-                    if event["receiveName"] == "BictoryCns.register":
-                        self.cns_domain.amount = event["amount"]
+                    if event["receiveName"] == 'BictoryCns.register':
+                        self.cns_domain.amount = event['amount']
                         self.cns_domain.action = CNSActions.register
-                        (
-                            self.cns_domain.domain_name,
-                            self.cns_domain.register_address,
-                            self.cns_domain.duration_years,
-                        ) = self.cns_domain.decode_from_register(event["message"])
+                        self.cns_domain.domain_name, self.cns_domain.register_address, self.cns_domain.duration_years = \
+                            self.cns_domain.decode_from_register(event["message"])
 
-                    if event["receiveName"] == "BictoryCns.extend":
-                        self.cns_domain.amount = event["amount"]
+                    if event["receiveName"] == 'BictoryCns.extend':
+                        self.cns_domain.amount = event['amount']
                         self.cns_domain.action = CNSActions.extend
-                        (
-                            self.cns_domain.domain_name,
-                            self.cns_domain.duration_years,
-                        ) = self.cns_domain.decode_from_extend(event["message"])
-
-                    if event["receiveName"] == "BictoryCns.createSubdomain":
+                        self.cns_domain.domain_name, self.cns_domain.duration_years = \
+                            self.cns_domain.decode_from_extend(event["message"])
+                        
+                    if event["receiveName"] == 'BictoryCns.createSubdomain':
                         self.cns_domain.action = CNSActions.createSubdomain
-                        self.cns_domain.amount = event["amount"]
-                        self.cns_domain.subdomain = (
-                            self.cns_domain.decode_subdomain_from(event["message"])
-                        )
-
-                    if event["receiveName"] == "BictoryCns.setAddress":
+                        self.cns_domain.amount = event['amount']
+                        self.cns_domain.subdomain = self.cns_domain.decode_subdomain_from(event["message"])
+                        
+                    if event["receiveName"] == 'BictoryCns.setAddress':
                         self.cns_domain.action = CNSActions.setAddress
-                        (
-                            self.cns_domain.domain_name,
-                            self.cns_domain.set_address,
-                        ) = self.cns_domain.decode_set_address_from(event["message"])
-
-                    if event["receiveName"] == "BictoryCns.setData":
+                        self.cns_domain.domain_name, self.cns_domain.set_address = \
+                            self.cns_domain.decode_set_address_from(event["message"])
+                        
+                    if event["receiveName"] == 'BictoryCns.setData':
                         self.cns_domain.action = CNSActions.setData
-                        (
-                            self.cns_domain.domain_name,
-                            self.cns_domain.set_data_key,
-                            self.cns_domain.set_data_value,
-                        ) = self.cns_domain.decode_set_data_from(event["message"])
-
-                    if event["receiveName"] == "BictoryNftAuction.bid":
+                        self.cns_domain.domain_name, self.cns_domain.set_data_key, self.cns_domain.set_data_value = \
+                            self.cns_domain.decode_set_data_from(event["message"])
+                        
+                    if event["receiveName"] == 'BictoryNftAuction.bid':
                         self.cns_domain.action = CNSActions.bid
 
-                        if len(event["events"]) > 0:
+                        if (len (event['events']) > 0):
                             the_event = event["events"][0]
-
-                            (
-                                tag_,
-                                contract_index,
-                                contract_subindex,
-                                token_id_,
-                                bidder_,
-                                amount_,
-                            ) = self.cns_domain.bidEvent(the_event)
-
+                            
+                            tag_, contract_index, contract_subindex, \
+                            token_id_, bidder_, amount_ = self.cns_domain.bidEvent(the_event)
+                            
                             self.cns_domain.tokenId = token_id_
-                            self.cns_domain.amount = amount_
+                            self.cns_domain.amount = amount_  
 
                             self.get_domain_from_cache_or_node()
-
-                    if event["receiveName"] == "BictoryNftAuction.finalize":
+                        
+                    if event["receiveName"] == 'BictoryNftAuction.finalize':
                         self.cns_domain.action = CNSActions.finalize
 
-                        if len(event["events"]) > 0:
+                        if (len (event['events']) > 0):
                             the_event = event["events"][0]
-
-                            (
-                                tag_,
-                                contract_index,
-                                contract_subindex,
-                                token_id_,
-                                seller_,
-                                winner_,
-                                price_,
-                                seller_share,
-                                royalty_length_,
-                                royalties,
-                                owner_,
-                                bidder_,
-                                amount_,
-                            ) = self.cns_domain.finalize(the_event)
-
+                                
+                            tag_, contract_index, contract_subindex, token_id_, \
+                            seller_, winner_, price_, seller_share, royalty_length_, \
+                            royalties, owner_, bidder_, amount_ = self.cns_domain.finalize(the_event)
+                            
                             self.cns_domain.tokenId = token_id_
-
+                            
                             self.get_domain_from_cache_or_node()
 
-                    if event["receiveName"] == "BictoryNftAuction.cancel":
+                    if event["receiveName"] == 'BictoryNftAuction.cancel':
                         self.cns_domain.action = CNSActions.cancel
-
-                        if len(event["events"]) > 0:
+                        
+                        
+                        if (len (event['events']) > 0):
                             the_event = event["events"][0]
-
-                            (
-                                tag_,
-                                contract_index,
-                                contract_subindex,
-                                token_id_,
-                                owner_,
-                            ) = self.cns_domain.cancelEvent(the_event)
-
+                                
+                            tag_, contract_index, contract_subindex, \
+                            token_id_, owner_ = self.cns_domain.cancelEvent(the_event)
+                            
                             self.cns_domain.tokenId = token_id_
-
+                            
                             self.get_domain_from_cache_or_node()
-
-                    if event["receiveName"] == "BictoryCnsNft.getTokenExpiry":
+                        
+                    
+                    if event["receiveName"] == 'BictoryCnsNft.getTokenExpiry':
                         self.cns_domain.action = CNSActions.getTokenExpiry
-                        self.cns_domain.tokenId = self.cns_domain.decode_token_id_from(
-                            event["message"]
-                        )
+                        self.cns_domain.tokenId = self.cns_domain.decode_token_id_from(event["message"])
 
                         self.get_domain_from_cache_or_node()
-
+        
     def decode_possible_memo(self):
         _events = []
-        if "events" in self.result:
-            for event in self.result.get("events", []):
+        if 'events' in self.result:
+            for event in self.result.get('events', []):
                 Event(event).translate_memo_if_present()
-
+                
     def init_from_node(self, t):
+        
         # note that only blockHash, blockHeight, blockSlotTime, finalized is used
-        self.block: ConcordiumBlockInfo = t.get("blockInfo", None)
+        self.block: ConcordiumBlockInfo = t.get('blockInfo', None)
         if not self.block:
             self.block = {}
-            self.block["blockHash"] = t["hash"]
-            self.block["blockHeight"] = t["blockHeight"]
-            self.block["blockSlotTime"] = t["blockSlotTime"]
-        self.cost = t["cost"]
-        self.energyCost = t["energyCost"]
-        self.hash = t["hash"]
-        self.index = t["index"]
-        if t["result"]["outcome"] == "success":
-            self.result = {
-                "events": t["result"]["events"],
-                "outcome": t["result"]["outcome"],
-            }
+            self.block['blockHash'] = t['hash']
+            self.block['blockHeight'] = t['blockHeight']
+            self.block['blockSlotTime'] = t['blockSlotTime']
+        self.cost       = t['cost']
+        self.energyCost = t['energyCost']
+        self.hash       = t['hash']
+        self.index      = t['index']
+        if t['result']['outcome'] == 'success':
+            self.result     = {'events': t['result']['events'], 'outcome': t['result']['outcome']}
         else:
-            self.result = {"outcome": t["result"]["outcome"]}
-        self.sender = t["sender"]
-        self.type = t["type"]["type"]  # accountTransaction
-        self.contents = t["type"]["contents"]  # transfer
+            self.result     = {'outcome': t['result']['outcome']}
+        self.sender     = t['sender']
+        self.type       = t['type']['type'] # accountTransaction
+        self.contents   = t['type']['contents'] # transfer
         self.decode_possible_memo()
         self.set_possible_cns_domain()
         # self.node = None
         # console.log(f"{self.hash=} | {self.cns_domain.domain_name=}")
         return self
 
     def init_from_mongo_tx(self, t):
+        
         # note that only blockHash, blockHeight, blockSlotTime, finalized is used
-        self.block = {}
-        self.block["blockHash"] = t["blockHash"]
-        self.block["blockHeight"] = t["blockHeight"]
-        self.block["blockSlotTime"] = t["blockSlotTime"]
-        self.cost = t["cost"]
-        self.energyCost = t["energyCost"]
-        self.hash = t["hash"]
-        self.index = t["index"]
-        if t["result"]["outcome"] == "success":
-            self.result = {
-                "events": t["result"]["events"],
-                "outcome": t["result"]["outcome"],
-            }
+        self.block      = {}
+        self.block['blockHash'] = t['blockHash']
+        self.block['blockHeight'] = t['blockHeight']
+        self.block['blockSlotTime'] = t['blockSlotTime']
+        self.cost       = t['cost']
+        self.energyCost = t['energyCost']
+        self.hash       = t['hash']
+        self.index      = t['index']
+        if t['result']['outcome'] == 'success':
+            self.result     = {'events': t['result']['events'], 'outcome': t['result']['outcome']}
         else:
-            self.result = {"outcome": t["result"]["outcome"]}
-        self.sender = t["sender"]
-        self.type = t["type"]["type"]  # accountTransaction
-        self.contents = t["type"]["contents"]  # transfer
+            self.result     = {'outcome': t['result']['outcome']}
+        self.sender     = t['sender']
+        self.type       = t['type']['type'] # accountTransaction
+        self.contents   = t['type']['contents'] # transfer
         self.decode_possible_memo()
         self.set_possible_cns_domain()
         # self.node = None
         # console.log(f"{self.hash=} | {self.cns_domain.domain_name=}")
         return self
+       
 
     # Bot classification requirements
     def get_sum_amount_from_scheduled_transfer(self, events):
         sum = 0
-        for event in events[0]["amount"]:
+        for event in events[0]['amount']:
             sum += int(event[1])
         return sum
-
+    
     def classify_transaction_for_bot(self):
         # console.log(f"BOT: {self.hash=} | {self.cns_domain.domain_name=}")
         t = self
         result = ClassificationResult()
         result.domain_name = self.cns_domain.domain_name
         result.accounts_involved_all = True
         result.type = t.type
         result.contents = t.contents
         result.sender = t.sender
         result.txHash = t.hash
         result.receiver = None
-
-        if self.type == "credentialDeploymentTransaction":
-            if t.result["outcome"] == "success":
-                events = t.result["events"]
+        
+        if self.type == 'credentialDeploymentTransaction':
+            if t.result['outcome'] == 'success':
+                events =  t.result["events"]
 
                 for event in events:
-                    if event["tag"] == "AccountCreated":
-                        result.sender = event["contents"]
+                    if event['tag'] == 'AccountCreated':
+                        result.sender = event['contents']
 
-        if self.type == "accountTransaction":
-            if t.result["outcome"] == "success":
-                events = t.result["events"]
+        if self.type == 'accountTransaction':
+            if t.result['outcome'] == 'success':
+                events =  t.result["events"]
 
                 for event in events:
-                    if event["tag"] == "Transferred":
-                        result.receiver = event["to"]["address"]
-                        result.amount = event["amount"]
+                    if event['tag'] == 'Transferred':
+                        result.receiver = event['to']['address']
+                        result.amount = event['amount']
                         result.accounts_involved_transfer = True
-
-                    elif event["tag"] == "TransferredWithSchedule":
-                        result.receiver = event["to"]
-                        result.amount = self.get_sum_amount_from_scheduled_transfer(
-                            events
-                        )
+                    
+                    elif event['tag'] == 'TransferredWithSchedule':
+                        result.receiver = event['to']
+                        result.amount = self.get_sum_amount_from_scheduled_transfer(events)
                         result.accounts_involved_transfer = True
 
-                    elif event["tag"] == "ContractInitialized":
-                        result.contract = {
-                            "tag": event["tag"],
-                            "index": event["address"]["index"],
-                            "subindex": event["address"]["subindex"],
-                        }
-
-                        result.list_of_contracts_involved.add(
-                            (event["address"]["index"], event["address"]["subindex"])
-                        )
+                    elif event['tag'] == 'ContractInitialized':
+                        result.contract = {'tag': event['tag'],
+                                    'index': event['address']['index'],
+                                    'subindex': event['address']['subindex']}
+                        
+                        result.list_of_contracts_involved.add((event['address']['index'],event['address']['subindex']))
                         result.contracts_involved = True
 
-                    elif event["tag"] == "Updated":
-                        result.contract = {
-                            "tag": event["tag"],
-                            "index": event["address"]["index"],
-                            "subindex": event["address"]["subindex"],
-                        }
-
-                        result.list_of_contracts_involved.add(
-                            (event["address"]["index"], event["address"]["subindex"])
-                        )
+                    elif event['tag'] == 'Updated':
+                        result.contract = {'tag': event['tag'],
+                                    'index': event['address']['index'],
+                                    'subindex': event['address']['subindex']}
+                        
+                        result.list_of_contracts_involved.add((event['address']['index'],event['address']['subindex']))
                         result.contracts_involved = True
 
-                    elif event["tag"] == "Resumed":
-                        result.contract = {
-                            "tag": event["tag"],
-                            "index": event["address"]["index"],
-                            "subindex": event["address"]["subindex"],
-                        }
-
-                        result.list_of_contracts_involved.add(
-                            (event["address"]["index"], event["address"]["subindex"])
-                        )
+                    elif event['tag'] == 'Resumed':
+                        result.contract = {'tag': event['tag'],
+                                    'index': event['address']['index'],
+                                    'subindex': event['address']['subindex']}
+                        
+                        result.list_of_contracts_involved.add((event['address']['index'],event['address']['subindex']))
                         result.contracts_involved = True
 
-                    elif event["tag"] == "Interrupted":
-                        result.contract = {
-                            "tag": event["tag"],
-                            "index": event["address"]["index"],
-                            "subindex": event["address"]["subindex"],
-                        }
-
-                        result.list_of_contracts_involved.add(
-                            (event["address"]["index"], event["address"]["subindex"])
-                        )
+                    elif event['tag'] == 'Interrupted':
+                        result.contract = {'tag': event['tag'],
+                                    'index': event['address']['index'],
+                                    'subindex': event['address']['subindex']}
+                        
+                        result.list_of_contracts_involved.add((event['address']['index'],event['address']['subindex']))
                         result.contracts_involved = True
 
         if result.amount:
             result.amount = int(result.amount) / 1_000_000
         return result, self
-
-    def request_delegated_amount_for_account_on_previous_block(
-        self, account_id, block_height
-    ):
+    
+    def request_delegated_amount_for_account_on_previous_block(self, account_id, block_height):
         previous_block_hash = self.node.request_block_hash_at_height(block_height - 1)
-        account_info_at_previous_block = self.node.request_accountInfo_at(
-            previous_block_hash, account_id
-        )
-        if "accountDelegation" in account_info_at_previous_block:
-            previous_amount = account_info_at_previous_block["accountDelegation"][
-                "stakedAmount"
-            ]
+        account_info_at_previous_block = self.node.request_accountInfo_at(previous_block_hash, account_id)
+        if 'accountDelegation' in account_info_at_previous_block:
+            previous_amount = account_info_at_previous_block['accountDelegation']['stakedAmount']
         else:
             previous_amount = None
         return previous_amount
 
-    def request_staked_amount_for_account_on_previous_block(
-        self, account_id, block_height
-    ):
+    def request_staked_amount_for_account_on_previous_block(self, account_id, block_height):
         previous_block_hash = self.node.request_block_hash_at_height(block_height - 1)
-        account_info_at_previous_block = self.node.request_accountInfo_at(
-            previous_block_hash, account_id
-        )
-        if "accountBaker" in account_info_at_previous_block:
-            previous_amount = account_info_at_previous_block["accountBaker"][
-                "stakedAmount"
-            ]
+        account_info_at_previous_block = self.node.request_accountInfo_at(previous_block_hash, account_id)
+        if 'accountBaker' in account_info_at_previous_block:
+            previous_amount = account_info_at_previous_block['accountBaker']['stakedAmount']
         else:
             previous_amount = None
         return previous_amount
 
     def classify_transaction_for_bot_for_delegation_and_staking(self):
         t = self
         result = DelegationAndStakingResult()
-
-        if self.type == "accountTransaction":
+        
+        
+        if  self.type == 'accountTransaction':
             result.sender = t.sender
             result.txHash = t.hash
-
-            if t.result["outcome"] == "success":
-                events = t.result["events"]
-
+            
+            if t.result['outcome'] == 'success':
+                events =  t.result["events"]
+                
                 for event in events:
-                    perc = ""
+                    perc = ''
                     # print (f"event = {event}")
-                    if event["tag"] in ["BakerStakeDecreased"]:
-                        result.bakerId = event["bakerId"]
-                        previous_amount = (
-                            self.request_staked_amount_for_account_on_previous_block(
-                                result.sender, self.block.blockHeight
-                            )
-                        )
+                    if event['tag'] in ['BakerStakeDecreased']:
+                        result.bakerId = event['bakerId']
+                        previous_amount = self.request_staked_amount_for_account_on_previous_block(result.sender, self.block.blockHeight)
                         if previous_amount:
                             if int(previous_amount) > 0:
                                 result.perc = f" ({(100*(int(previous_amount) - int(event['newStake']))/int(previous_amount)):,.2f}%)"
-                                result.unstaked_amount = (
-                                    int(previous_amount) - int(event["newStake"])
-                                ) / 1_000_000
-
-                    if event["tag"] in [
-                        "DelegationStakeIncreased",
-                        "DelegationStakeDecreased",
-                    ]:
-                        previous_amount = (
-                            self.request_delegated_amount_for_account_on_previous_block(
-                                result.sender, self.block.blockHeight
-                            )
-                        )
+                                result.unstaked_amount = (int(previous_amount) - int(event['newStake'])) / 1_000_000
+
+                    if event['tag'] in ['DelegationStakeIncreased', 'DelegationStakeDecreased']:
+                        previous_amount = self.request_delegated_amount_for_account_on_previous_block(result.sender, self.block.blockHeight)
                         if previous_amount:
                             if int(previous_amount) > 0:
-                                if int(event["newStake"]) > int(previous_amount):
+                                if int(event['newStake']) > int(previous_amount):
                                     result.perc = f" ({(100*((int(event['newStake'])/int(previous_amount)) - 1)):,.2f}%)"
                                 else:
                                     result.perc = f" ({(100*(int(previous_amount) - int(event['newStake']))/int(previous_amount)):,.2f}%)"
 
-                    if event["tag"] == "DelegationSetDelegationTarget":
-                        if event["delegationTarget"]["delegateType"] == "Baker":
-                            result.bakerId = event["delegationTarget"]["bakerId"]
-                            result.message += (
-                                f"Delegation target set to {result.bakerId:,.0f}. "
-                            )
-
-                    elif event["tag"] == "DelegationStakeIncreased":
+                    if event['tag'] == 'DelegationSetDelegationTarget':
+                        if event['delegationTarget']['delegateType'] == 'Baker':
+                            result.bakerId = event['delegationTarget']['bakerId']
+                            result.message += f"Delegation target set to {result.bakerId:,.0f}. "
+                    
+                    elif event['tag'] == 'DelegationStakeIncreased':
                         if previous_amount:
                             result.message += f"Stake increased{result.perc} to {(int(event['newStake'])/1_000_000):,.0f} CCD."
                         else:
                             result.message += f"Stake set to {(int(event['newStake'])/1_000_000):,.0f} CCD."
                         result.request_target = True
-
-                    elif event["tag"] == "DelegationStakeDecreased":
+                    
+                    elif event['tag'] == 'DelegationStakeDecreased':
                         result.message += f"Stake decreased{result.perc} to {(int(event['newStake'])/1_000_000):,.0f} CCD."
                         result.request_target = True
 
-                    elif event["tag"] == "BakerStakeDecreased":
+                    elif event['tag'] == 'BakerStakeDecreased':
                         result.message += f"Baker stake decreased {result.unstaked_amount:,.0f} CCD{result.perc} to {(int(event['newStake'])/1_000_000):,.0f} CCD."
                         result.request_target = False
                         result.unstaked = True
 
-                    elif event["tag"] == "DelegationRemoved":
+                    elif event['tag'] == 'DelegationRemoved':
                         result.message += f"Delegation removed."
                         result.request_target = True
-
+                    
+                    
         return result
 
     def define_type_and_contents_from_graphQL(self, t):
-        _type = t["transactionType"]["__typename"]  # AccountTransaction
-
-        if _type == "AccountTransaction":
+        _type       = t['transactionType']['__typename'] # AccountTransaction
+        
+        if _type == 'AccountTransaction':
             try:
-                _contents = t["transactionType"]["accountTransactionType"]
+                _contents = t['transactionType']['accountTransactionType']
             except:
-                _contents = "UNKNOWN"
-        elif _type == "CredentialDeploymentTransaction":
+                _contents = 'UNKNOWN'
+        elif _type == 'CredentialDeploymentTransaction':
             try:
-                _contents = t["transactionType"]["credentialDeploymentTransactionType"]
+                _contents = t['transactionType']['credentialDeploymentTransactionType']
             except:
-                _contents = "UNKNOWN"
-        elif _type == "UpdateTransaction":
+                _contents = 'UNKNOWN'
+        elif _type == 'UpdateTransaction':
             try:
-                _contents = t["transactionType"]["updateTransactionType"]
+                _contents = t['transactionType']['updateTransactionType']
             except:
-                _contents = "UNKNOWN"
+                _contents = 'UNKNOWN'
         else:
-            _contents = "UNKNOWN"
+            _contents = 'UNKNOWN'
 
         # now translate to node language
         # console.log(f"{_type=}, {_contents=}")
-        self.type = TransactionTypeFromQLToNode[_type].value
-        if t["result"]["__typename"] == "Success":
-            self.contents = TransactionContentsFromQLToNode[_contents].value
+        self.type       = TransactionTypeFromQLToNode[_type].value
+        if t['result']['__typename'] == 'Success':
+            self.contents   = TransactionContentsFromQLToNode[_contents].value
         else:
             self.contents = None
 
     def translate_result_from_graphQL(self, t):
-        if t["result"]["__typename"] == "Success":
-            _outcome = "success"
-        elif t["result"]["__typename"] == "Rejected":
-            _outcome = "reject"
+        if t['result']['__typename'] == 'Success':
+            _outcome = 'success'
+        elif t['result']['__typename'] == 'Rejected':
+            _outcome = 'reject'
             _rejectReason = t["result"]["reason"]["__typename"]
-
+        
         _events = []
-        if "events" in t["result"]:
-            for event in t["result"]["events"]["nodes"]:
+        if 'events' in t['result']:
+            for event in t['result']['events']['nodes']:
                 e = Event(event).translate_event_from_graphQL()
                 _events.append(e)
 
-        if _outcome == "success":
-            return {"events": _events, "outcome": _outcome}
+        if _outcome == 'success':
+            return  {'events': _events, 'outcome': _outcome}
         else:
-            return {
-                "events": _events,
-                "outcome": _outcome,
-                "rejectReason": _rejectReason,
-            }
+            return  {'events': _events, 'outcome': _outcome, 'rejectReason': _rejectReason}
+        
 
     def init_from_graphQL(self, t):
         # try:
         #     t['block']['blockSlotTime'] = dateutil.parser.parse(t['block']['blockSlotTime'])
         # except:
         #     pass
-        self.block = t["block"]
-        self.cost = t["ccdCost"]
-        self.energyCost = t["energyCost"]
-        self.hash = t["transactionHash"]
-        self.index = t["transactionIndex"]
-        self.sender = (
-            t["senderAccountAddress"]["asString"]
-            if t["senderAccountAddress"] is not None
-            else None
-        )
+        self.block      = t['block']
+        self.cost       = t['ccdCost']
+        self.energyCost = t['energyCost']
+        self.hash       = t['transactionHash']
+        self.index      = t['transactionIndex'] 
+        self.sender     = t['senderAccountAddress']['asString'] if t['senderAccountAddress'] is not None else None
         self.define_type_and_contents_from_graphQL(t)
-        self.result = self.translate_result_from_graphQL(t)
+        self.result     = self.translate_result_from_graphQL(t)
         self.set_possible_cns_domain()
         self.node = None
         return self
+
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring/user.py` & `sharingiscaring-0.2.9/sharingiscaring/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,18 @@
 import json
 import os
 from dateutil.relativedelta import relativedelta
-from pydantic import BaseModel, Extra, Field
-
-# from fastapi import Request
-
-from .GRPCClient import GRPCClient
-from .mongodb import (
-    MongoDB,
-    Collections,
-    MongoTypeInvolvedAccount,
-    CollectionsUtilities,
-)
+from .transaction import Transaction
+from .client import ConcordiumClient
+from .ccdscan import CCDScan
+from .mongodb import MongoDB
 from enum import Enum
 import datetime as dt
 import dateutil.parser
 from datetime import timezone
-from rich.console import Console
-
-console = Console()
-
-
-class SmartContractRequest(BaseModel):
-    chat_id: str
-    init: bool
-    update: bool
-    cns_domain: bool
-
-
-class UnstakeLimitRequest(BaseModel):
-    chat_id: str
-    limit: int
-
-
-class TransactionLimitRequest(BaseModel):
-    chat_id: str
-    limit: int
-    exch_only: bool
-
-
-class CheckItemRequest(BaseModel):
-    chat_id: str
-    itemId: str
-
-
-class AddEditItemRequest(BaseModel):
-    chat_id: str
-    itemId: str
-    account_id: str = None
-    baker_id: int = None
-    label: str = None
-    node_ip: str = None
-    node_port: str = None
-    account_notify: bool
-    baker_notify: bool
-    edit_save: bool = False
-
-
-class DeleteItemRequest(BaseModel):
-    chat_id: str
-    account_id: str
-    baker_id: int = None
 
 
 class UserReminderStatus(Enum):
     NO_NEED = -1  # there is no need to remind. The bot has plenty of credits
     RUNNING_OUT_IN_2_DAYS = 0  #
     OUT_OF_CREDITS_1 = 1
     OUT_OF_CREDITS_2 = 2
@@ -99,173 +47,45 @@
 class SubscriptionPlans(Enum):
     PLUS = "Plus"
     DELEGATION = "Delegation"
     UNLIMITED = "Unlimited"
     NO_PLAN = "No Plan"
 
 
-class Subscription(BaseModel):
-    start_date: dt.datetime = None
-    payment_transactions: list = []
-    subscription_active: bool = False
-    subscription_active: bool = (
-        False  # If True, the user has paid enough to pay for one-time fee
-    )
-    delegator_active: bool = False  # If True, the user has paid any amount from an account that is an active delegator
-    site_active: bool = False  # This is the indicator that a user can use the site
-    bot_active: bool = False  # If True, the user has paid enough to cover the one-time fee and sent messages
-
-    unlimited: bool = (
-        False  # If True, the user has paid enough for subscription_unlimited
-    )
-    # unlimited credits
-    unlimited_end_date: dt.datetime = None
-    remaining_message_credits: int = 0
-    count_messages: int = 0
-    paid_amount = 0
-    messages_per_hour: int = 0
-    plan = SubscriptionPlans.NO_PLAN
-
-
-class User(BaseModel):
-    id: str = Field(..., alias="_id")
-    nodes: dict = None
-    bakers_to_follow: list[int] = []
-    chat_id: int = None
-    first_name: str = None
-    language_code: str = None
-    token: str = "x" * 10
-    username: str = None
-    accounts_to_follow: list[str] = []
-    labels: dict = {}
-    tags: dict = {}
-    transactions_downloaded: dict = None
-    smart_init: bool = None
-    smart_update: bool = None
-    cns_domain: bool = None
-    unstake_limit_notifier: int = None
-    transaction_limit_notifier_to_exchange_only: bool = None
-    subscription: Subscription = Subscription()
-    explorer_ccd_transactions: list[dict] = []
-    explorer_ccd_delegators: dict = {}
-    last_refreshed_for_user: dt.datetime = None
-    transaction_limit_notifier: int = None
-    environment: str = "dev"
-    testing: bool = False
-
-    @classmethod
-    def read_user_from_collection(self, chat_id, mongodb: MongoDB):
-        coll = mongodb.utilities[CollectionsUtilities.users_prod]
-
-        user = coll.find_one({"chat_id": chat_id})
-        existing_user = None
-        if user:
-            existing_user = User(**user)
-        return existing_user
-
-    def save_user_to_collection(self, request=None, mongodb: MongoDB = None):
-        query = {"_id": self.token}
-        if mongodb:
-            m = mongodb
-        else:
-            m = request.app.mongodb
-
-        if self.environment == "prod":
-            coll = m.utilities[CollectionsUtilities.users_prod]
-        else:
-            coll = m.utilities[CollectionsUtilities.users_dev]
-
-        coll.replace_one(
-            query,
-            json.loads(self.json(exclude_none=True)),
-            upsert=True,
-        )
-
-    def save_smart_contracts(
-        self, request, smart_contract_request: SmartContractRequest
-    ):
-        self.smart_init = smart_contract_request.init
-        self.smart_update = smart_contract_request.update
-        self.cns_domain = smart_contract_request.cns_domain
-        self.save_user_to_collection(request)
-
-    def save_unstake_limit(self, request, unstake_limit_request: UnstakeLimitRequest):
-        self.unstake_limit_notifier = unstake_limit_request.limit
-        self.save_user_to_collection(request)
-
-    def save_limit(self, request, transaction_limit_request: TransactionLimitRequest):
-        self.transaction_limit_notifier = transaction_limit_request.limit
-        self.transaction_limit_notifier_to_exchange_only = (
-            transaction_limit_request.exch_only
+class Subscription:
+    def __init__(self):
+        self.start_date = None
+        self.payment_transactions = []
+        self.subscription_active = (
+            False  # If True, the user has paid enough to pay for one-time fee
         )
-        self.save_user_to_collection(request)
+        self.delegator_active = False  # If True, the user has paid any amount from an account that is an active delegator
+        self.site_active = False  # This is the indicator that a user can use the site
+        self.bot_active = False  # If True, the user has paid enough to cover the one-time fee and sent messages
 
-    def save_transactions_download(self, request, account_id):
-        self.transactions_downloaded[account_id] = (
-            self.transactions_downloaded.get(account_id, 0) + 1
+        self.unlimited = (
+            False  # If True, the user has paid enough for subscription_unlimited
         )
-        self.save_user_to_collection(request)
-
-    def add_edit_item(
-        self,
-        request,
-        add_edit_item_request: AddEditItemRequest,
-    ):
-        if add_edit_item_request.baker_id:
-            if add_edit_item_request.baker_notify:
-                self.bakers_to_follow.append(add_edit_item_request.baker_id)
-                self.bakers_to_follow = sorted(list(set(self.bakers_to_follow)))
-            else:
-                try:
-                    self.bakers_to_follow.remove(add_edit_item_request.baker_id)
-                except:
-                    pass
-
-            # node
-            if add_edit_item_request.node_ip and add_edit_item_request.node_port:
-                nodes = self.nodes
-                nodes[str(add_edit_item_request.baker_id)] = {
-                    "ip": add_edit_item_request.node_ip,
-                    "port": add_edit_item_request.node_port,
-                }
-                self.nodes = nodes
-
-        if add_edit_item_request.account_notify:
-            self.accounts_to_follow.append(add_edit_item_request.account_id)
-            self.accounts_to_follow = sorted(list(set(self.accounts_to_follow)))
-        else:
-            try:
-                self.accounts_to_follow.remove(add_edit_item_request.account_id)
-            except:
-                pass
-
-        self.labels[add_edit_item_request.account_id] = add_edit_item_request.label
-        self.save_user_to_collection(request)
-
-    def remove_item(self, request, delete_item_request: DeleteItemRequest):
-        try:
-            self.accounts_to_follow.remove(delete_item_request.account_id)
-        except:
-            pass
-
-        try:
-            self.bakers_to_follow.remove(delete_item_request.baker_id)
-        except:
-            pass
-
-        try:
-            del self.nodes[str(delete_item_request.baker_id)]
-        except:
-            pass
-
-        # remove label
-        if delete_item_request.account_id in self.labels:
-            _ = self.labels.pop(delete_item_request.account_id, None)
-
-        self.save_user_to_collection(request)
+        # unlimited credits
+        self.unlimited_end_date = None
+        self.remaining_message_credits = 0
+        self.count_messages = 0
+        self.paid_amount = 0
+        self.messages_per_hour = 0
+        self.plan = SubscriptionPlans.NO_PLAN
+
+
+class User:
+    def __init__(self):
+        self.bakers_to_follow = []
+        self.tags = {}
+        self.explorer_ccd_transactions = []
+        self.explorer_ccd_delegators = []
+        self.token = "x" * 10
+        self.subscription = Subscription()
 
     def add_user_from_telegram(self, user):
         self.first_name = user.first_name
         self.username = user.username
         self.chat_id = user.id
         self.language_code = user.language_code
         return self
@@ -291,164 +111,164 @@
         self.cns_domain = user.get("cns_domain", False)
         self.nodes = user.get("nodes", {})
         # self.subscription                   = Subscription()
         return self
 
     def prepare_for_subscription_logic(
         self,
-        mongodb: MongoDB,
-        grpcclient: GRPCClient,
-        txs_as_receiver: list[MongoTypeInvolvedAccount] = None,
-        explorer_ccd_delegators: dict = None,
+        client: ConcordiumClient,
+        ccdscan: CCDScan,
     ):
-        grpcclient.switch_to_net("mainnet")
-        if not txs_as_receiver:
-            console.log("Need to get explorer transactions...")
-            self.get_explorer_transactions(mongodb, grpcclient)
-        else:
-            self.explorer_ccd_transactions = txs_as_receiver
-
-        if not explorer_ccd_delegators:
-            console.log("Need to get explorer delegators...")
-            self.get_explorer_delegators(grpcclient)
-        else:
-            self.explorer_ccd_delegators = explorer_ccd_delegators
-        self.last_refreshed_for_user = dt.datetime.utcnow()
+        self.get_explorer_transactions(client, ccdscan)
+        self.get_explorer_delegators(ccdscan)
 
-    def get_explorer_transactions(self, mongodb: MongoDB, grpcclient: GRPCClient):
+    def get_explorer_transactions(self, client: ConcordiumClient, ccdscan: CCDScan):
         try:
-            pipeline = mongodb.search_txs_hashes_for_account_as_receiver_with_params(
-                SubscriptionDetails.EXPLORER_CCD.value, 0, 1_000_000_000
+            (
+                explorer_ccd_transactions,
+                _,
+            ) = ccdscan.ql_get_all_transactions_for_explorer_ccd(
+                None, SubscriptionDetails.EXPLORER_CCD.value
             )
-            txs_as_receiver = [
-                MongoTypeInvolvedAccount(**x)
-                for x in mongodb.mainnet[
-                    Collections.involved_accounts_transfer
-                ].aggregate(pipeline)
+            self.explorer_ccd_transactions = [
+                Transaction(client)
+                .init_from_graphQL(x["node"]["transaction"])
+                .find_memo_and_amount()
+                for x in explorer_ccd_transactions
             ]
-
-            self.explorer_ccd_transactions = txs_as_receiver
         except:
             self.explorer_ccd_transactions = []
 
-    def get_explorer_delegators(self, grpcclient: GRPCClient):
+    def get_explorer_delegators(self, ccdscan: CCDScan):
         try:
-            explorer_ccd_delegators = grpcclient.get_delegators_for_pool(
-                SubscriptionDetails.BAKER_ID.value, "last_final"
+            explorer_ccd_delegators, _ = ccdscan.ql_get_all_delegators_for_explorer_ccd(
+                None, SubscriptionDetails.BAKER_ID.value
             )
-
             # keyed on accountAddress
             self.explorer_ccd_delegators = {
-                x.account: x for x in explorer_ccd_delegators
+                x["node"]["accountAddress"]["asString"]: x["node"]
+                for x in explorer_ccd_delegators
             }
         except:
             self.explorer_ccd_delegators = []
 
     def set_count_messages(self, mongodb: MongoDB, ENVIRONMENT: str):
         # get count of messages sent to this user
         # only count from subscription.start_date
         if self.subscription.start_date:
             try:
                 pipeline = mongodb.get_bot_messages_for_user(
                     self, ENVIRONMENT, self.subscription.start_date
                 )
-                result = list(
-                    mongodb.mainnet[Collections.bot_messages].aggregate(pipeline)
-                )
+                result = list(mongodb.collection_messages.aggregate(pipeline))
 
                 self.subscription.count_messages = 0
                 if len(result) > 0:
                     if "count_messages" in result[0]:
                         self.subscription.count_messages = result[0]["count_messages"]
 
             except:
                 pass
 
-    def perform_subscription_logic(self, grpcclient: GRPCClient):
-        grpcclient.switch_to_net("mainnet")
+    def perform_subscription_logic(self):
+
+        # payment_memo = 'coffee'
         payment_memo = self.token[:6]
 
         # check if the right memo is set, if so, count towards user.
         payment_txs = []
         paid_amount = 0
         SUBSCRIPTION_ONE_TIME_FEE_set = False
         ACTIVE_DELEGATOR_set = False
 
         for concordium_tx in self.explorer_ccd_transactions:
+            # concordium_tx = Transaction(client).init_from_graphQL(tx).find_memo_and_amount()
             if concordium_tx.memo:
                 if payment_memo in concordium_tx.memo:
-                    slot_time = grpcclient.get_finalized_block_at_height(
-                        concordium_tx.block_height
-                    ).slot_time
-
                     paid_amount += concordium_tx.amount / 1_000_000
 
                     # Is this sender a current active delegator?
                     if not ACTIVE_DELEGATOR_set:
                         if concordium_tx.sender in self.explorer_ccd_delegators:
                             sender_delegated_stake = (
-                                self.explorer_ccd_delegators[concordium_tx.sender].stake
+                                self.explorer_ccd_delegators[concordium_tx.sender][
+                                    "stakedAmount"
+                                ]
                                 / 1_000_000
                             )
                             self.subscription.delegator_active = (
                                 sender_delegated_stake
                                 >= SubscriptionDetails.SUBSCRIPTION_DELEGATOR_STAKE_LIMIT.value
                             )
 
                             # Make sure that multiple transactions to not UNset this if later transactions make this invalid.
                             if self.subscription.delegator_active:
                                 ACTIVE_DELEGATOR_set = True
                                 self.subscription.plan = SubscriptionPlans.DELEGATION
+                                if isinstance(
+                                    concordium_tx.block["blockSlotTime"], dt.datetime
+                                ):
+                                    blockSlotTime = concordium_tx.block["blockSlotTime"]
+                                else:
+                                    blockSlotTime = dateutil.parser.parse(
+                                        concordium_tx.block["blockSlotTime"]
+                                    )
 
                                 # some users have purchased before the official start date.
                                 self.subscription.start_date = max(
                                     SubscriptionDetails.SUBSCRIPTION_PLAN_START_DATE.value,
-                                    slot_time,
+                                    blockSlotTime,
                                 )
 
                     # Has the user paid the one time fee? If so, record the subscription start date
                     if not SUBSCRIPTION_ONE_TIME_FEE_set:
                         self.subscription.subscription_active = (
                             paid_amount
                             >= SubscriptionDetails.SUBSCRIPTION_ONE_TIME_FEE.value
                         )
 
                         # Make sure that multiple transactions to not UNset this if later transactions make this invalid.
                         if self.subscription.subscription_active:
                             SUBSCRIPTION_ONE_TIME_FEE_set = True
                             self.subscription.plan = SubscriptionPlans.PLUS
 
+                            if isinstance(
+                                concordium_tx.block["blockSlotTime"], dt.datetime
+                            ):
+                                blockSlotTime = concordium_tx.block["blockSlotTime"]
+                            else:
+                                blockSlotTime = dateutil.parser.parse(
+                                    concordium_tx.block["blockSlotTime"]
+                                )
+
                             # some users have purchased before the official start date.
                             self.subscription.start_date = max(
                                 SubscriptionDetails.SUBSCRIPTION_PLAN_START_DATE.value,
-                                slot_time,
+                                blockSlotTime,
                             )
 
                     # Has the user paid enough for unlimited? If so, record the unlimited end date
                     self.subscription.unlimited = (
                         paid_amount >= SubscriptionDetails.SUBSCRIPTION_UNLIMITED.value
                     )
                     if self.subscription.unlimited:
                         self.subscription.plan = SubscriptionPlans.UNLIMITED
-                        self.subscription.unlimited_end_date = (
-                            slot_time + relativedelta(years=1)
-                        )
-                        # if isinstance(
-                        #     concordium_tx.block["blockSlotTime"], dt.datetime
-                        # ):
-                        #     self.subscription.unlimited_end_date = concordium_tx.block[
-                        #         "blockSlotTime"
-                        #     ] + relativedelta(years=1)
-                        # else:
-                        #     self.subscription.unlimited_end_date = (
-                        #         dateutil.parser.parse(
-                        #             concordium_tx.block["blockSlotTime"]
-                        #         )
-                        #         + relativedelta(years=1)
-                        #     )
+                        if isinstance(
+                            concordium_tx.block["blockSlotTime"], dt.datetime
+                        ):
+                            self.subscription.unlimited_end_date = concordium_tx.block[
+                                "blockSlotTime"
+                            ] + relativedelta(years=1)
+                        else:
+                            self.subscription.unlimited_end_date = (
+                                dateutil.parser.parse(
+                                    concordium_tx.block["blockSlotTime"]
+                                )
+                                + relativedelta(years=1)
+                            )
                     payment_txs.append(concordium_tx)
 
         self.subscription.payment_transactions = payment_txs
         self.subscription.paid_amount = paid_amount
 
         # This is the indicator that a user can use the site.
         self.subscription.site_active = (
@@ -457,20 +277,19 @@
 
         # exclude me
         if self.token == "e2410784-fde1-11ec-a3b9-de5c44736176":
             self.subscription.bot_active = True
             self.subscription.site_active = True
             self.subscription.subscription_active = True
             self.subscription.unlimited = True
-            self.subscription.unlimited_end_date = dt.datetime(
-                2040, 4, 16, 23, 59, 59
-            ).astimezone(timezone.utc)
+            self.subscription.unlimited_end_date = dt.datetime(2040, 4, 16, 0, 0, 0)
             self.subscription.plan = SubscriptionPlans.UNLIMITED
 
     def determine_bot_status(self):
+
         # update remaining message credits
         FEE_TO_USE = (
             SubscriptionDetails.SUBSCRIPTION_DELEGATION_FEE
             if self.subscription.plan == SubscriptionPlans.DELEGATION
             else SubscriptionDetails.SUBSCRIPTION_ONE_TIME_FEE
         )
         self.subscription.remaining_message_credits = max(
```

### Comparing `sharingiscaring-0.2.80/sharingiscaring.egg-info/SOURCES.txt` & `sharingiscaring-0.2.9/sharingiscaring.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 README.md
 setup.py
 sharingiscaring/__init__.py
 sharingiscaring/account.py
 sharingiscaring/block.py
 sharingiscaring/ccdscan.py
-sharingiscaring/cis.py
 sharingiscaring/client.py
 sharingiscaring/cns.py
 sharingiscaring/credential.py
 sharingiscaring/enums.py
 sharingiscaring/mongodb.py
 sharingiscaring/node.py
 sharingiscaring/pool.py
@@ -29,15 +28,14 @@
 sharingiscaring/GRPCClient/types_pb2.py
 sharingiscaring/GRPCClient/types_pb2_grpc.py
 sharingiscaring/GRPCClient/wadze.py
 sharingiscaring/GRPCClient/CCD_Types/__init__.py
 sharingiscaring/GRPCClient/concordium/__init__.py
 sharingiscaring/GRPCClient/concordium/health/__init__.py
 sharingiscaring/GRPCClient/concordium/v2/__init__.py
-sharingiscaring/GRPCClient/queries/_CheckHealth.py
 sharingiscaring/GRPCClient/queries/_GetAccountInfo.py
 sharingiscaring/GRPCClient/queries/_GetAccountList.py
 sharingiscaring/GRPCClient/queries/_GetAnonymityRevokers.py
 sharingiscaring/GRPCClient/queries/_GetBakerList.py
 sharingiscaring/GRPCClient/queries/_GetBlockChainParameters.py
 sharingiscaring/GRPCClient/queries/_GetBlockInfo.py
 sharingiscaring/GRPCClient/queries/_GetBlockPendingUpdates.py
@@ -53,15 +51,14 @@
 sharingiscaring/GRPCClient/queries/_GetPassiveDelegationInfo.py
 sharingiscaring/GRPCClient/queries/_GetPassiveDelegators.py
 sharingiscaring/GRPCClient/queries/_GetPassiveDelegatorsRewardPeriod.py
 sharingiscaring/GRPCClient/queries/_GetPoolDelegators.py
 sharingiscaring/GRPCClient/queries/_GetPoolDelegatorsRewardPeriod.py
 sharingiscaring/GRPCClient/queries/_GetPoolInfo.py
 sharingiscaring/GRPCClient/queries/_GetTokenomicsInfo.py
-sharingiscaring/GRPCClient/queries/_InvokeInstance.py
 sharingiscaring/GRPCClient/queries/_SharedConverters.py
 sharingiscaring/GRPCClient/queries/__init__.py
 sharingiscaring/ccdscan_queries/__init__.py
 sharingiscaring/ccdscan_queries/_accountByAddress.py
 sharingiscaring/ccdscan_queries/_accounts.py
 sharingiscaring/ccdscan_queries/_bakerByBakerId.py
 sharingiscaring/ccdscan_queries/_bakers.py
```

### Comparing `sharingiscaring-0.2.80/tests/test_pool.py` & `sharingiscaring-0.2.9/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/tests/test_txs.py` & `sharingiscaring-0.2.9/tests/test_txs.py`

 * *Files identical despite different names*

### Comparing `sharingiscaring-0.2.80/tests/test_user.py` & `sharingiscaring-0.2.9/tests/test_user.py`

 * *Files identical despite different names*

