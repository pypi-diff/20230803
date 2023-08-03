# Comparing `tmp/aliyun-python-sdk-adb-1.1.4.tar.gz` & `tmp/aliyun-python-sdk-adb-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-adb-1.1.4.tar", last modified: Wed Aug  2 07:56:10 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-adb-1.1.5.tar", last modified: Thu Aug  3 06:19:11 2023, max compression
```

## Comparing `aliyun-python-sdk-adb-1.1.4.tar` & `aliyun-python-sdk-adb-1.1.5.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/
--rw-r--r--   0 root         (0) root         (0)      575 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyun_python_sdk_adb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyun_python_sdk_adb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6898 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyun_python_sdk_adb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyun_python_sdk_adb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyun_python_sdk_adb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyun_python_sdk_adb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/
--rw-r--r--   0 root         (0) root         (0)     2604 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/AllocateClusterPublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ApplyAdviceByIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/AttachUserENIRequest.py
--rw-r--r--   0 root         (0) root         (0)     1877 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/BatchApplyAdviceByIdListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/BindDBResourceGroupWithUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     2689 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/BindDBResourcePoolWithUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     7672 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateDBClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateDBResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateDBResourcePoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     4952 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateElasticPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteDBClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteDBResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteDBResourcePoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2534 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteElasticPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAdviceServiceEnabledRequest.py
--rw-r--r--   0 root         (0) root         (0)     2317 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAllAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2697 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAllDataSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAppliedAdvicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAuditLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     4471 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAuditLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAutoRenewAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAvailableAdvicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAvailableResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3220 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2685 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeColumnsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeComputeResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeConnectionCountRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2343 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterAccessWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterHealthStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterNetInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterResourcePoolPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     3992 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2510 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBResourcePoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2221 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisDimensionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisMonitorPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4650 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2461 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisSQLInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2691 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDownloadRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3332 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeEIURangeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3307 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeElasticDailyPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     3000 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeElasticPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeInclinedTablesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3548 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeLoadTasksRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeMaintenanceActionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeOperatorPermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribePatternPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3560 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeProcessListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2187 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSQLPatternAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2698 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSQLPatternsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSQLPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSQLPlanTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSchemasRequest.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2844 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSlowLogTrendRequest.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSqlPatternRequest.py
--rw-r--r--   0 root         (0) root         (0)     2392 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTableAccessCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTableDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2713 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTablePartitionDiagnoseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTableStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTablesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTaskInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DetachUserENIRequest.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DisableAdviceServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DownloadDiagnosisRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DryRunClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/EnableAdviceServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2713 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/GrantOperatorPermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/KillProcessRequest.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyAccountDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2534 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyAuditLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2906 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyAutoRenewAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3572 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3026 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyClusterConnectionStringRequest.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterAccessWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2582 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterMaintainTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterPayTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2574 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBResourcePoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     4952 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyElasticPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyLogBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2689 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyMaintenanceActionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ReleaseClusterPublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ResetAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/RevokeOperatorPermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/UnbindDBResourceGroupWithUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/UnbindDBResourcePoolWithUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     2976 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-08-02 07:56:10.000000 aliyun-python-sdk-adb-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyun_python_sdk_adb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyun_python_sdk_adb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6898 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyun_python_sdk_adb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyun_python_sdk_adb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyun_python_sdk_adb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyun_python_sdk_adb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/
+-rw-r--r--   0 root         (0) root         (0)     2604 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/AllocateClusterPublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ApplyAdviceByIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/AttachUserENIRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/BatchApplyAdviceByIdListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/BindDBResourceGroupWithUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/BindDBResourcePoolWithUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7672 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateDBClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateDBResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateDBResourcePoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4952 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateElasticPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteDBClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteDBResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteDBResourcePoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2534 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteElasticPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAdviceServiceEnabledRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAllAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAllDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAppliedAdvicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAuditLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAuditLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAutoRenewAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAvailableAdvicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAvailableResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeColumnsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeComputeResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeConnectionCountRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2343 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterAccessWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterHealthStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterNetInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterResourcePoolPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2510 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBResourcePoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisDimensionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisMonitorPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4650 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisSQLInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDownloadRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeEIURangeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeElasticDailyPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeElasticPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeInclinedTablesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3548 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeLoadTasksRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeMaintenanceActionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeOperatorPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribePatternPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeProcessListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSQLPatternAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSQLPatternsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSQLPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSQLPlanTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSchemasRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSlowLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSlowLogTrendRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSqlPatternRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2392 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTableAccessCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTableDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTablePartitionDiagnoseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTableStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTablesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTaskInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DetachUserENIRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DisableAdviceServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DownloadDiagnosisRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DryRunClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/EnableAdviceServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/GrantOperatorPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/KillProcessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyAccountDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2534 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyAuditLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyAutoRenewAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyClusterConnectionStringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterAccessWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterMaintainTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterPayTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBResourcePoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4952 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyElasticPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyLogBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyMaintenanceActionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ReleaseClusterPublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ResetAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/RevokeOperatorPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/UnbindDBResourceGroupWithUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/UnbindDBResourcePoolWithUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2976 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-03 06:19:11.000000 aliyun-python-sdk-adb-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-08-03 06:19:10.000000 aliyun-python-sdk-adb-1.1.5/setup.py
```

### Comparing `aliyun-python-sdk-adb-1.1.4/LICENSE` & `aliyun-python-sdk-adb-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/PKG-INFO` & `aliyun-python-sdk-adb-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-adb
-Version: 1.1.4
+Version: 1.1.5
 Summary: The adb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-adb
```

### Comparing `aliyun-python-sdk-adb-1.1.4/README.rst` & `aliyun-python-sdk-adb-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyun_python_sdk_adb.egg-info/PKG-INFO` & `aliyun-python-sdk-adb-1.1.5/aliyun_python_sdk_adb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-adb
-Version: 1.1.4
+Version: 1.1.5
 Summary: The adb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-adb
```

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyun_python_sdk_adb.egg-info/SOURCES.txt` & `aliyun-python-sdk-adb-1.1.5/aliyun_python_sdk_adb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/endpoint.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/AllocateClusterPublicConnectionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/AllocateClusterPublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ApplyAdviceByIdRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ApplyAdviceByIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/AttachUserENIRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/AttachUserENIRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/BatchApplyAdviceByIdListRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/BatchApplyAdviceByIdListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/BindDBResourceGroupWithUserRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/BindDBResourceGroupWithUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/BindDBResourcePoolWithUserRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/BindDBResourcePoolWithUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateAccountRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateDBClusterRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateDBClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateDBResourceGroupRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateDBResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateDBResourcePoolRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateDBResourcePoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/CreateElasticPlanRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/CreateElasticPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteAccountRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteDBClusterRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteDBClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteDBResourceGroupRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteDBResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteDBResourcePoolRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteDBResourcePoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DeleteElasticPlanRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DeleteElasticPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAccountsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAccountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAdviceServiceEnabledRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAdviceServiceEnabledRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAllAccountsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAllAccountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAllDataSourceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAllDataSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAppliedAdvicesRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAppliedAdvicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAuditLogConfigRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAuditLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAuditLogRecordsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAuditLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAutoRenewAttributeRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAvailableAdvicesRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAvailableAdvicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeAvailableResourceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeAvailableResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeBackupPolicyRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeBackupsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeColumnsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeColumnsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeComputeResourceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeComputeResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeConnectionCountRecordsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeConnectionCountRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterAccessWhiteListRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterAccessWhiteListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterAttributeRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterHealthStatusRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterHealthStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterNetInfoRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterNetInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterPerformanceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterResourcePoolPerformanceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterResourcePoolPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClusterStatusRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClusterStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBClustersRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBResourceGroupRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDBResourcePoolRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDBResourcePoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisDimensionsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisDimensionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisMonitorPerformanceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisMonitorPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisRecordsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisSQLInfoRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisSQLInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDiagnosisTasksRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDiagnosisTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeDownloadRecordsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeDownloadRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeEIURangeRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeEIURangeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeElasticDailyPlanRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeElasticDailyPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeElasticPlanRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeElasticPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeInclinedTablesRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeInclinedTablesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeLoadTasksRecordsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeLoadTasksRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeMaintenanceActionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeMaintenanceActionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeOperatorPermissionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeOperatorPermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribePatternPerformanceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribePatternPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeProcessListRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeProcessListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeRegionsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSQLPatternAttributeRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSQLPatternAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSQLPatternsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSQLPatternsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSQLPlanRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSQLPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSQLPlanTaskRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSQLPlanTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSchemasRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSchemasRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSlowLogRecordsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSlowLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSlowLogTrendRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSlowLogTrendRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeSqlPatternRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeSqlPatternRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTableAccessCountRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTableAccessCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTableDetailRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTableDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTablePartitionDiagnoseRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTablePartitionDiagnoseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTableStatisticsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTableStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTablesRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTablesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DescribeTaskInfoRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DescribeTaskInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DetachUserENIRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DetachUserENIRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DisableAdviceServiceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DisableAdviceServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DownloadDiagnosisRecordsRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DownloadDiagnosisRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/DryRunClusterRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/DryRunClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/EnableAdviceServiceRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/EnableAdviceServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/GrantOperatorPermissionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/GrantOperatorPermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/KillProcessRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/KillProcessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ListTagResourcesRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyAccountDescriptionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyAccountDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyAuditLogConfigRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyAuditLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyAutoRenewAttributeRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyBackupPolicyRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyClusterConnectionStringRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyClusterConnectionStringRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterAccessWhiteListRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterAccessWhiteListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterDescriptionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterMaintainTimeRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterMaintainTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterPayTypeRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterPayTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBClusterResourceGroupRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBClusterResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBResourceGroupRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyDBResourcePoolRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyDBResourcePoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyElasticPlanRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyElasticPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyLogBackupPolicyRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyLogBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ModifyMaintenanceActionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ModifyMaintenanceActionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ReleaseClusterPublicConnectionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ReleaseClusterPublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/ResetAccountPasswordRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/ResetAccountPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/RevokeOperatorPermissionRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/RevokeOperatorPermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/TagResourcesRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/UnbindDBResourceGroupWithUserRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/UnbindDBResourceGroupWithUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/UnbindDBResourcePoolWithUserRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/UnbindDBResourcePoolWithUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/aliyunsdkadb/request/v20190315/UntagResourcesRequest.py` & `aliyun-python-sdk-adb-1.1.5/aliyunsdkadb/request/v20190315/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-adb-1.1.4/setup.py` & `aliyun-python-sdk-adb-1.1.5/setup.py`

 * *Files identical despite different names*

