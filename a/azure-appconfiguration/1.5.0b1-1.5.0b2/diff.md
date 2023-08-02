# Comparing `tmp/azure-appconfiguration-1.5.0b1.zip` & `tmp/azure-appconfiguration-1.5.0b2.zip`

## zipinfo {}

```diff
@@ -1,98 +1,98 @@
-Zip file size: 147926 bytes, number of entries: 96
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/samples/
--rw-rw-r--  2.0 unx     2482 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/setup.py
--rw-rw-r--  2.0 unx      188 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/LICENSE
--rw-rw-r--  2.0 unx    18279 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/README.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/setup.cfg
--rw-rw-r--  2.0 unx     4294 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx       59 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/pyproject.toml
--rw-rw-r--  2.0 unx    22915 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/PKG-INFO
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/CHANGELOG.md
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/tests/perfstress_tests/
--rw-rw-r--  2.0 unx    33084 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad.py
--rw-rw-r--  2.0 unx     4383 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/testcase.py
--rw-rw-r--  2.0 unx     2029 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/conftest.py
--rw-rw-r--  2.0 unx     4662 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_sync_token_policy.py
--rw-rw-r--  2.0 unx     2207 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/asynctestcase.py
--rw-rw-r--  2.0 unx    42558 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client.py
--rw-rw-r--  2.0 unx     2283 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/preparers.py
--rw-rw-r--  2.0 unx    37229 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad_async.py
--rw-rw-r--  2.0 unx     4923 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_consistency.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/consts.py
--rw-rw-r--  2.0 unx    47189 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_async.py
--rw-rw-r--  2.0 unx     1364 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/async_preparers.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/perfstress_tests/get.py
--rw-rw-r--  2.0 unx     1681 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/perfstress_tests/set.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/
--rw-rw-r--  2.0 unx       81 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/
--rw-rw-r--  2.0 unx    35741 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_client.py
--rw-rw-r--  2.0 unx     1232 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/__init__.py
--rw-rw-r--  2.0 unx     2472 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_utils.py
--rw-rw-r--  2.0 unx    19911 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_models.py
--rw-rw-r--  2.0 unx      859 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py
--rw-rw-r--  2.0 unx      530 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_error.py
--rw-rw-r--  2.0 unx      313 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_user_agent.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/py.typed
--rw-rw-r--  2.0 unx      172 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_version.py
--rw-rw-r--  2.0 unx      441 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_constants.py
--rw-rw-r--  2.0 unx     3145 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py
--rw-rw-r--  2.0 unx     5026 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_sync_token.py
--rw-rw-r--  2.0 unx      595 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/__init__.py
--rw-rw-r--  2.0 unx    35061 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
--rw-rw-r--  2.0 unx     4231 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_sync_token_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/
--rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_serialization.py
--rw-rw-r--  2.0 unx      850 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_patch.py
--rw-rw-r--  2.0 unx     1828 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_vendor.py
--rw-rw-r--  2.0 unx     3786 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py
--rw-rw-r--  2.0 unx     2816 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_configuration.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/
--rw-rw-r--  2.0 unx      850 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx     1063 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_vendor.py
--rw-rw-r--  2.0 unx     3891 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
--rw-rw-r--  2.0 unx     2826 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx      837 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    99054 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
--rw-rw-r--  2.0 unx      837 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_patch.py
--rw-rw-r--  2.0 unx   128662 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
--rw-rw-r--  2.0 unx     1983 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/__init__.py
--rw-rw-r--  2.0 unx     2180 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_patch.py
--rw-rw-r--  2.0 unx    21674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_models_py3.py
--rw-rw-r--  2.0 unx        6 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx    22915 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx       41 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/requires.txt
--rw-rw-r--  2.0 unx     3253 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx     2409 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample.py
--rw-rw-r--  2.0 unx     2912 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/snapshot_samples.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/sync_token_samples.py
--rw-rw-r--  2.0 unx     1949 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/hello_world_sample.py
--rw-rw-r--  2.0 unx     2512 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample_async.py
--rw-rw-r--  2.0 unx     2017 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/hello_world_sample_async.py
--rw-rw-r--  2.0 unx     4498 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/README.md
--rw-rw-r--  2.0 unx     2062 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/read_only_sample_async.py
--rw-rw-r--  2.0 unx     1954 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/read_only_sample.py
--rw-rw-r--  2.0 unx     2313 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample_async.py
--rw-rw-r--  2.0 unx     1769 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/list_revision_sample_async.py
--rw-rw-r--  2.0 unx     1309 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/util.py
--rw-rw-r--  2.0 unx     2356 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample.py
--rw-rw-r--  2.0 unx     3086 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/snapshot_samples_async.py
--rw-rw-r--  2.0 unx     1661 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/list_revision_sample.py
--rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/sync_token_samples_async.py
-96 files, 766414 bytes uncompressed, 127612 bytes compressed:  83.3%
+Zip file size: 148686 bytes, number of entries: 96
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/samples/
+-rw-rw-r--  2.0 unx     4294 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/LICENSE
+-rw-rw-r--  2.0 unx    23169 b- defN 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/PKG-INFO
+-rw-rw-r--  2.0 unx      188 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/MANIFEST.in
+-rw-rw-r--  2.0 unx     2482 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/setup.py
+-rw-rw-r--  2.0 unx     4028 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/CHANGELOG.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/setup.cfg
+-rw-rw-r--  2.0 unx    18229 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/README.md
+-rw-rw-r--  2.0 unx       59 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/pyproject.toml
+-rw-rw-r--  2.0 unx     3253 b- defN 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx    23169 b- defN 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        6 b- defN 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx       41 b- defN 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/requires.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx     2283 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/preparers.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/consts.py
+-rw-rw-r--  2.0 unx     4365 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/testcase.py
+-rw-rw-r--  2.0 unx    47152 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_async.py
+-rw-rw-r--  2.0 unx     2207 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/asynctestcase.py
+-rw-rw-r--  2.0 unx    36267 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_aad_async.py
+-rw-rw-r--  2.0 unx    42517 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client.py
+-rw-rw-r--  2.0 unx     4923 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/test_consistency.py
+-rw-rw-r--  2.0 unx     4662 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/test_sync_token_policy.py
+-rw-rw-r--  2.0 unx     1364 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/async_preparers.py
+-rw-rw-r--  2.0 unx     2029 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/conftest.py
+-rw-rw-r--  2.0 unx    31340 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_aad.py
+-rw-rw-r--  2.0 unx     1681 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/perfstress_tests/set.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/perfstress_tests/get.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/tests/perfstress_tests/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure/appconfiguration/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/
+-rw-rw-r--  2.0 unx      172 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_version.py
+-rw-rw-r--  2.0 unx      530 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_error.py
+-rw-rw-r--  2.0 unx     3145 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_requests.py
+-rw-rw-r--  2.0 unx     5026 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_sync_token.py
+-rw-rw-r--  2.0 unx      313 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_user_agent.py
+-rw-rw-r--  2.0 unx     1232 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/__init__.py
+-rw-rw-r--  2.0 unx      441 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_constants.py
+-rw-rw-r--  2.0 unx      859 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_credential.py
+-rw-rw-r--  2.0 unx    35975 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_client.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/py.typed
+-rw-rw-r--  2.0 unx     2472 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_utils.py
+-rw-rw-r--  2.0 unx    21236 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_models.py
+-rw-rw-r--  2.0 unx    35324 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
+-rw-rw-r--  2.0 unx      595 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/__init__.py
+-rw-rw-r--  2.0 unx     4231 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/_sync_token_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/
+-rw-rw-r--  2.0 unx     2816 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      850 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_patch.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_serialization.py
+-rw-rw-r--  2.0 unx     1828 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_vendor.py
+-rw-rw-r--  2.0 unx     3786 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_azure_app_configuration.py
+-rw-rw-r--  2.0 unx     1983 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_patch.py
+-rw-rw-r--  2.0 unx     2180 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
+-rw-rw-r--  2.0 unx    21674 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-02 16:36 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/
+-rw-rw-r--  2.0 unx     2826 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx      850 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3891 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
+-rw-rw-r--  2.0 unx    99054 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
+-rw-rw-r--  2.0 unx      837 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx   128662 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
+-rw-rw-r--  2.0 unx      837 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx     1949 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/hello_world_sample.py
+-rw-rw-r--  2.0 unx     1591 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/sync_token_samples_async.py
+-rw-rw-r--  2.0 unx     1954 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/read_only_sample.py
+-rw-rw-r--  2.0 unx     1661 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/list_revision_sample.py
+-rw-rw-r--  2.0 unx     1769 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/list_revision_sample_async.py
+-rw-rw-r--  2.0 unx     2017 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/hello_world_sample_async.py
+-rw-rw-r--  2.0 unx     2409 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/hello_world_advanced_sample.py
+-rw-rw-r--  2.0 unx     1309 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/util.py
+-rw-rw-r--  2.0 unx     2512 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/conditional_operation_sample_async.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/sync_token_samples.py
+-rw-rw-r--  2.0 unx     2938 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/snapshot_samples.py
+-rw-rw-r--  2.0 unx     3112 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/snapshot_samples_async.py
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/read_only_sample_async.py
+-rw-rw-r--  2.0 unx     4498 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/README.md
+-rw-rw-r--  2.0 unx     2313 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/hello_world_advanced_sample_async.py
+-rw-rw-r--  2.0 unx     2356 b- defN 23-Aug-02 16:35 azure-appconfiguration-1.5.0b2/samples/conditional_operation_sample.py
+96 files, 766248 bytes uncompressed, 128372 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -1,289 +1,289 @@
-Filename: azure-appconfiguration-1.5.0b1/
+Filename: azure-appconfiguration-1.5.0b2/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/
+Filename: azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/
+Filename: azure-appconfiguration-1.5.0b2/tests/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/
+Filename: azure-appconfiguration-1.5.0b2/azure/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/
+Filename: azure-appconfiguration-1.5.0b2/samples/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/setup.py
+Filename: azure-appconfiguration-1.5.0b2/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/MANIFEST.in
+Filename: azure-appconfiguration-1.5.0b2/LICENSE
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/LICENSE
+Filename: azure-appconfiguration-1.5.0b2/PKG-INFO
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/README.md
+Filename: azure-appconfiguration-1.5.0b2/MANIFEST.in
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/setup.cfg
+Filename: azure-appconfiguration-1.5.0b2/setup.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/TROUBLESHOOTING.md
+Filename: azure-appconfiguration-1.5.0b2/CHANGELOG.md
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/pyproject.toml
+Filename: azure-appconfiguration-1.5.0b2/setup.cfg
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/PKG-INFO
+Filename: azure-appconfiguration-1.5.0b2/README.md
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/CHANGELOG.md
+Filename: azure-appconfiguration-1.5.0b2/pyproject.toml
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/perfstress_tests/
+Filename: azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad.py
+Filename: azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/testcase.py
+Filename: azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/conftest.py
+Filename: azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/test_sync_token_policy.py
+Filename: azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/asynctestcase.py
+Filename: azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/requires.txt
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client.py
+Filename: azure-appconfiguration-1.5.0b2/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/preparers.py
+Filename: azure-appconfiguration-1.5.0b2/tests/preparers.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad_async.py
+Filename: azure-appconfiguration-1.5.0b2/tests/consts.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/test_consistency.py
+Filename: azure-appconfiguration-1.5.0b2/tests/testcase.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/consts.py
+Filename: azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_async.py
+Filename: azure-appconfiguration-1.5.0b2/tests/asynctestcase.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/async_preparers.py
+Filename: azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_aad_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/perfstress_tests/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/perfstress_tests/get.py
+Filename: azure-appconfiguration-1.5.0b2/tests/test_consistency.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/tests/perfstress_tests/set.py
+Filename: azure-appconfiguration-1.5.0b2/tests/test_sync_token_policy.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/
+Filename: azure-appconfiguration-1.5.0b2/tests/async_preparers.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/tests/conftest.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/
+Filename: azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_aad.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/
+Filename: azure-appconfiguration-1.5.0b2/tests/perfstress_tests/set.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_client.py
+Filename: azure-appconfiguration-1.5.0b2/tests/perfstress_tests/get.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_utils.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_models.py
+Filename: azure-appconfiguration-1.5.0b2/azure/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_error.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_user_agent.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_version.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/py.typed
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_error.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_version.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_requests.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_constants.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_sync_token.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_user_agent.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_sync_token.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_constants.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_credential.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_sync_token_async.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_client.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/py.typed
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_utils.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_models.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_serialization.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_patch.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/_sync_token_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_vendor.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_configuration.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_configuration.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_patch.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_vendor.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_serialization.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_vendor.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_configuration.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_azure_app_configuration.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_models_py3.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_patch.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/__init__.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_patch.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_vendor.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_models_py3.py
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/top_level.txt
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/not-zip-safe
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/PKG-INFO
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/dependency_links.txt
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/requires.txt
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/SOURCES.txt
+Filename: azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample.py
+Filename: azure-appconfiguration-1.5.0b2/samples/hello_world_sample.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/snapshot_samples.py
+Filename: azure-appconfiguration-1.5.0b2/samples/sync_token_samples_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/sync_token_samples.py
+Filename: azure-appconfiguration-1.5.0b2/samples/read_only_sample.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/hello_world_sample.py
+Filename: azure-appconfiguration-1.5.0b2/samples/list_revision_sample.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample_async.py
+Filename: azure-appconfiguration-1.5.0b2/samples/list_revision_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/hello_world_sample_async.py
+Filename: azure-appconfiguration-1.5.0b2/samples/hello_world_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/README.md
+Filename: azure-appconfiguration-1.5.0b2/samples/hello_world_advanced_sample.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/read_only_sample_async.py
+Filename: azure-appconfiguration-1.5.0b2/samples/util.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/read_only_sample.py
+Filename: azure-appconfiguration-1.5.0b2/samples/conditional_operation_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample_async.py
+Filename: azure-appconfiguration-1.5.0b2/samples/sync_token_samples.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/list_revision_sample_async.py
+Filename: azure-appconfiguration-1.5.0b2/samples/snapshot_samples.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/util.py
+Filename: azure-appconfiguration-1.5.0b2/samples/snapshot_samples_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample.py
+Filename: azure-appconfiguration-1.5.0b2/samples/read_only_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/snapshot_samples_async.py
+Filename: azure-appconfiguration-1.5.0b2/samples/README.md
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/list_revision_sample.py
+Filename: azure-appconfiguration-1.5.0b2/samples/hello_world_advanced_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.5.0b1/samples/sync_token_samples_async.py
+Filename: azure-appconfiguration-1.5.0b2/samples/conditional_operation_sample.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-appconfiguration-1.5.0b1/setup.py` & `azure-appconfiguration-1.5.0b2/setup.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/LICENSE` & `azure-appconfiguration-1.5.0b2/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/README.md` & `azure-appconfiguration-1.5.0b2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -252,48 +252,48 @@
 
 <!-- SNIPPET:snapshot_samples.create_snapshot -->
 
 ```python
 from azure.appconfiguration import ConfigurationSettingFilter
 
 filters = [ConfigurationSettingFilter(key="my_key1", label="my_label1")]
-response = client.begin_create_snapshot(name="my_snapshot_name", filters=filters)
+response = client.begin_create_snapshot(name=snapshot_name, filters=filters)
 created_snapshot = response.result()
 print_snapshot(created_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### Get a Snapshot
 
 <!-- SNIPPET:snapshot_samples.get_snapshot -->
 
 ```python
-received_snapshot = client.get_snapshot(name="my_snapshot_name")
+received_snapshot = client.get_snapshot(name=snapshot_name)
 ```
 
 <!-- END SNIPPET -->
 
 ### Archive a Snapshot
 
 <!-- SNIPPET:snapshot_samples.archive_snapshot -->
 
 ```python
-archived_snapshot = client.archive_snapshot(name="my_snapshot_name")
+archived_snapshot = client.archive_snapshot(name=snapshot_name)
 print_snapshot(archived_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### Recover a Snapshot
 
 <!-- SNIPPET:snapshot_samples.recover_snapshot -->
 
 ```python
-recovered_snapshot = client.recover_snapshot(name="my_snapshot_name")
+recovered_snapshot = client.recover_snapshot(name=snapshot_name)
 print_snapshot(recovered_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### List Snapshots
 
@@ -307,15 +307,15 @@
 <!-- END SNIPPET -->
 
 ### List Configuration Settings of a Snapshot
 
 <!-- SNIPPET:snapshot_samples.list_snapshot_configuration_settings -->
 
 ```python
-for config_setting in client.list_snapshot_configuration_settings(name="my_snapshot_name"):
+for config_setting in client.list_snapshot_configuration_settings(name=snapshot_name):
     print_configuration_setting(config_setting)
 ```
 
 <!-- END SNIPPET -->
 
 ### Async APIs
 
@@ -361,42 +361,42 @@
 
 <!-- SNIPPET:snapshot_samples_async.create_snapshot -->
 
 ```python
 from azure.appconfiguration import ConfigurationSettingFilter
 
 filters = [ConfigurationSettingFilter(key="my_key1", label="my_label1")]
-response = await client.begin_create_snapshot(name="my_snapshot_name", filters=filters)
+response = await client.begin_create_snapshot(name=snapshot_name, filters=filters)
 created_snapshot = await response.result()
 print_snapshot(created_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.get_snapshot -->
 
 ```python
-received_snapshot = await client.get_snapshot(name="my_snapshot_name")
+received_snapshot = await client.get_snapshot(name=snapshot_name)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.archive_snapshot -->
 
 ```python
-archived_snapshot = await client.archive_snapshot(name="my_snapshot_name")
+archived_snapshot = await client.archive_snapshot(name=snapshot_name)
 print_snapshot(archived_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.recover_snapshot -->
 
 ```python
-recovered_snapshot = await client.recover_snapshot(name="my_snapshot_name")
+recovered_snapshot = await client.recover_snapshot(name=snapshot_name)
 print_snapshot(recovered_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.list_snapshots -->
 
@@ -406,15 +406,15 @@
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.list_snapshot_configuration_settings -->
 
 ```python
-async for config_setting in client.list_snapshot_configuration_settings(name="my_snapshot_name"):
+async for config_setting in client.list_snapshot_configuration_settings(name=snapshot_name):
     print_configuration_setting(config_setting)
 ```
 
 <!-- END SNIPPET -->
 
 ## Troubleshooting
```

## Comparing `azure-appconfiguration-1.5.0b1/TROUBLESHOOTING.md` & `azure-appconfiguration-1.5.0b2/TROUBLESHOOTING.md`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/PKG-INFO` & `azure-appconfiguration-1.5.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-appconfiguration
-Version: 1.5.0b1
+Version: 1.5.0b2
 Summary: Microsoft App Configuration Data Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/appconfiguration/azure-appconfiguration
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -274,48 +274,48 @@
 
 <!-- SNIPPET:snapshot_samples.create_snapshot -->
 
 ```python
 from azure.appconfiguration import ConfigurationSettingFilter
 
 filters = [ConfigurationSettingFilter(key="my_key1", label="my_label1")]
-response = client.begin_create_snapshot(name="my_snapshot_name", filters=filters)
+response = client.begin_create_snapshot(name=snapshot_name, filters=filters)
 created_snapshot = response.result()
 print_snapshot(created_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### Get a Snapshot
 
 <!-- SNIPPET:snapshot_samples.get_snapshot -->
 
 ```python
-received_snapshot = client.get_snapshot(name="my_snapshot_name")
+received_snapshot = client.get_snapshot(name=snapshot_name)
 ```
 
 <!-- END SNIPPET -->
 
 ### Archive a Snapshot
 
 <!-- SNIPPET:snapshot_samples.archive_snapshot -->
 
 ```python
-archived_snapshot = client.archive_snapshot(name="my_snapshot_name")
+archived_snapshot = client.archive_snapshot(name=snapshot_name)
 print_snapshot(archived_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### Recover a Snapshot
 
 <!-- SNIPPET:snapshot_samples.recover_snapshot -->
 
 ```python
-recovered_snapshot = client.recover_snapshot(name="my_snapshot_name")
+recovered_snapshot = client.recover_snapshot(name=snapshot_name)
 print_snapshot(recovered_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### List Snapshots
 
@@ -329,15 +329,15 @@
 <!-- END SNIPPET -->
 
 ### List Configuration Settings of a Snapshot
 
 <!-- SNIPPET:snapshot_samples.list_snapshot_configuration_settings -->
 
 ```python
-for config_setting in client.list_snapshot_configuration_settings(name="my_snapshot_name"):
+for config_setting in client.list_snapshot_configuration_settings(name=snapshot_name):
     print_configuration_setting(config_setting)
 ```
 
 <!-- END SNIPPET -->
 
 ### Async APIs
 
@@ -383,42 +383,42 @@
 
 <!-- SNIPPET:snapshot_samples_async.create_snapshot -->
 
 ```python
 from azure.appconfiguration import ConfigurationSettingFilter
 
 filters = [ConfigurationSettingFilter(key="my_key1", label="my_label1")]
-response = await client.begin_create_snapshot(name="my_snapshot_name", filters=filters)
+response = await client.begin_create_snapshot(name=snapshot_name, filters=filters)
 created_snapshot = await response.result()
 print_snapshot(created_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.get_snapshot -->
 
 ```python
-received_snapshot = await client.get_snapshot(name="my_snapshot_name")
+received_snapshot = await client.get_snapshot(name=snapshot_name)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.archive_snapshot -->
 
 ```python
-archived_snapshot = await client.archive_snapshot(name="my_snapshot_name")
+archived_snapshot = await client.archive_snapshot(name=snapshot_name)
 print_snapshot(archived_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.recover_snapshot -->
 
 ```python
-recovered_snapshot = await client.recover_snapshot(name="my_snapshot_name")
+recovered_snapshot = await client.recover_snapshot(name=snapshot_name)
 print_snapshot(recovered_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.list_snapshots -->
 
@@ -428,15 +428,15 @@
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.list_snapshot_configuration_settings -->
 
 ```python
-async for config_setting in client.list_snapshot_configuration_settings(name="my_snapshot_name"):
+async for config_setting in client.list_snapshot_configuration_settings(name=snapshot_name):
     print_configuration_setting(config_setting)
 ```
 
 <!-- END SNIPPET -->
 
 ## Troubleshooting
 
@@ -489,14 +489,20 @@
 [coc_contact]: mailto:opencode@microsoft.com
 [troubleshooting_guide]: https://aka.ms/azsdk/python/appconfiguration/troubleshoot
 [label_concept]: https://docs.microsoft.com/azure/azure-app-configuration/concept-key-value#label-keys
 
 
 # Release History
 
+## 1.5.0b2 (2023-08-02)
+
+### Bugs Fixed
+- Fixed a bug in deserializing and serializing Snapshot when `filters` property is `None`.
+- Fixed a bug when creating `FeatureFlagConfigurationSetting` from SDK but having an error in portal.([#31326](https://github.com/Azure/azure-sdk-for-python/issues/31326))
+
 ## 1.5.0b1 (2023-07-11)
 
 ### Features Added
 - Added support for `Snapshot` CRUD operations.
 
 ### Bugs Fixed
 - Fixed async `update_sync_token` to use async/await keywords
```

## Comparing `azure-appconfiguration-1.5.0b1/CHANGELOG.md` & `azure-appconfiguration-1.5.0b2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 1.5.0b2 (2023-08-02)
+
+### Bugs Fixed
+- Fixed a bug in deserializing and serializing Snapshot when `filters` property is `None`.
+- Fixed a bug when creating `FeatureFlagConfigurationSetting` from SDK but having an error in portal.([#31326](https://github.com/Azure/azure-sdk-for-python/issues/31326))
+
 ## 1.5.0b1 (2023-07-11)
 
 ### Features Added
 - Added support for `Snapshot` CRUD operations.
 
 ### Bugs Fixed
 - Fixed async `update_sync_token` to use async/await keywords
```

## Comparing `azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad.py` & `azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_aad.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,45 +40,42 @@
 
 class TestAppConfigurationClientAAD(AppConfigTestCase):
     # method: add_configuration_setting
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_add_configuration_setting(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
-        kv = ConfigurationSetting(
+        test_config_setting = ConfigurationSetting(
             key=KEY + "_ADD",
             label=LABEL,
             value=TEST_VALUE,
             content_type=TEST_CONTENT_TYPE,
             tags={"tag1": "tag1", "tag2": "tag2"},
         )
-        created_kv = client.add_configuration_setting(kv)
+        created_kv = client.add_configuration_setting(test_config_setting)
         assert (
-            created_kv.label == kv.label
-            and kv.value == kv.value
-            and created_kv.content_type == kv.content_type
-            and created_kv.tags == kv.tags
+            created_kv.label == test_config_setting.label
+            and created_kv.value == test_config_setting.value
+            and created_kv.content_type == test_config_setting.content_type
+            and created_kv.tags == test_config_setting.tags
+            and created_kv.etag != None
+            and created_kv.etag != test_config_setting.etag
+            and created_kv.last_modified != None
+            and created_kv.read_only == False
         )
-        assert created_kv.etag is not None and created_kv.last_modified is not None and created_kv.read_only is False
-        client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
-    @app_config_aad_decorator
-    @recorded_by_proxy
-    def test_add_existing_configuration_setting(self, appconfiguration_endpoint_string):
-        client = self.create_aad_client(appconfiguration_endpoint_string)
-        test_config_setting = self.create_config_setting()
-        self.add_for_test(client, test_config_setting)
+        # test add existing configuration setting
         with pytest.raises(ResourceExistsError):
             client.add_configuration_setting(
                 ConfigurationSetting(
                     key=test_config_setting.key,
                     label=test_config_setting.label,
                 )
             )
-        client.delete_configuration_setting(key=test_config_setting.key, label=test_config_setting.label)
+        client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
     # method: set_configuration_setting
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_set_existing_configuration_setting_label_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_set_kv = self.create_config_setting()
@@ -93,155 +90,117 @@
             and to_set_kv.tags == set_kv.tags
             and to_set_kv.etag != set_kv.etag
         )
         client.delete_configuration_setting(key=to_set_kv.key, label=to_set_kv.label)
 
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_set_existing_configuration_setting_label_wrong_etag(self, appconfiguration_endpoint_string):
+    def test_set_configuration_setting_wrong_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_set_kv = self.create_config_setting()
         to_set_kv.value = to_set_kv.value + "a"
         to_set_kv.tags = {"a": "b", "c": "d"}
         to_set_kv.etag = "wrong etag"
         with pytest.raises(ResourceModifiedError):
             client.set_configuration_setting(to_set_kv, match_condition=MatchConditions.IfNotModified)
 
-    @app_config_aad_decorator
-    @recorded_by_proxy
-    def test_set_configuration_setting_etag(self, appconfiguration_endpoint_string):
-        client = self.create_aad_client(appconfiguration_endpoint_string)
-        kv = ConfigurationSetting(
-            key=KEY + "_SET",
-            label=LABEL,
-            value=TEST_VALUE,
-            content_type=TEST_CONTENT_TYPE,
-            tags={"tag1": "tag1", "tag2": "tag2"},
-        )
-        kv.etag = "random etag"
-        with pytest.raises(ResourceModifiedError):
-            client.set_configuration_setting(kv, match_condition=MatchConditions.IfNotModified)
-
-    @app_config_aad_decorator
-    @recorded_by_proxy
-    def test_set_configuration_setting_no_etag(self, appconfiguration_endpoint_string):
-        client = self.create_aad_client(appconfiguration_endpoint_string)
-        to_set_kv = ConfigurationSetting(
-            key=KEY + "_SET",
-            label=LABEL,
-            value=TEST_VALUE,
-            content_type=TEST_CONTENT_TYPE,
-            tags={"tag1": "tag1", "tag2": "tag2"},
-        )
-        set_kv = client.set_configuration_setting(to_set_kv)
-        assert (
-            to_set_kv.key == set_kv.key
-            and to_set_kv.label == set_kv.label
-            and to_set_kv.value == set_kv.value
-            and to_set_kv.content_type == set_kv.content_type
-            and to_set_kv.tags == set_kv.tags
-            and to_set_kv.etag != set_kv.etag
-        )
-        client.delete_configuration_setting(key=to_set_kv.key, label=to_set_kv.label)
-
     # method: get_configuration_setting
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_get_configuration_setting_no_label(self, appconfiguration_endpoint_string):
+    def test_get_configuration_setting(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
-        compare_kv = self.create_config_setting_no_label()
+        compare_kv = self.create_config_setting()
         self.add_for_test(client, compare_kv)
-        fetched_kv = client.get_configuration_setting(compare_kv.key)
+        fetched_kv = client.get_configuration_setting(compare_kv.key, compare_kv.label)
         assert (
             fetched_kv.key == compare_kv.key
             and fetched_kv.value == compare_kv.value
             and fetched_kv.content_type == compare_kv.content_type
             and fetched_kv.tags == compare_kv.tags
+            and fetched_kv.label == compare_kv.label
         )
-        assert fetched_kv.label is None
+        assert fetched_kv.label is not None
         client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_get_configuration_setting_label(self, appconfiguration_endpoint_string):
+    def test_get_non_existing_configuration_setting(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         compare_kv = self.create_config_setting()
-        self.add_for_test(client, compare_kv)
-        fetched_kv = client.get_configuration_setting(compare_kv.key, compare_kv.label)
-        assert (
-            fetched_kv.key == compare_kv.key
-            and fetched_kv.value == compare_kv.value
-            and fetched_kv.content_type == compare_kv.content_type
-            and fetched_kv.tags == compare_kv.tags
-        )
-        assert fetched_kv.label is not None
-        client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
+        with pytest.raises(ResourceNotFoundError):
+            client.get_configuration_setting(compare_kv.key, compare_kv.label + "a")
 
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_get_non_existing_configuration_setting(self, appconfiguration_endpoint_string):
+    def test_get_configuration_setting_with_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         compare_kv = self.create_config_setting()
         self.add_for_test(client, compare_kv)
+        compare_kv = client.get_configuration_setting(compare_kv.key, compare_kv.label)
+
+        # test get with wrong etag
+        with pytest.raises(ResourceModifiedError):
+            client.get_configuration_setting(
+                compare_kv.key, compare_kv.label, etag="wrong etag", match_condition=MatchConditions.IfNotModified
+            )
+        # test get with correct etag
         with pytest.raises(ResourceNotFoundError):
-            client.get_configuration_setting(compare_kv.key, compare_kv.label + "a")
+            client.get_configuration_setting(compare_kv.key, etag=compare_kv.etag)
+        client.get_configuration_setting(compare_kv.key, compare_kv.label, etag=compare_kv.etag)
+
         client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     # method: delete_configuration_setting
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_delete_with_key_no_label(self, appconfiguration_endpoint_string):
+    def test_delete_configuration_setting_with_key_no_label(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_delete_kv = self.create_config_setting_no_label()
         self.add_for_test(client, to_delete_kv)
         deleted_kv = client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
         assert deleted_kv is not None
         with pytest.raises(ResourceNotFoundError):
             client.get_configuration_setting(to_delete_kv.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_delete_with_key_label(self, appconfiguration_endpoint_string):
+    def test_delete_configuration_setting_with_key_label(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_delete_kv = self.create_config_setting()
         self.add_for_test(client, to_delete_kv)
         deleted_kv = client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
         assert deleted_kv is not None
         with pytest.raises(ResourceNotFoundError):
             client.get_configuration_setting(to_delete_kv.key, label=to_delete_kv.label)
 
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_delete_not_existing(self, appconfiguration_endpoint_string):
+    def test_delete_not_existing_configuration_setting(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         deleted_kv = client.delete_configuration_setting("not_exist_" + KEY)
         assert deleted_kv is None
 
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_delete_correct_etag(self, appconfiguration_endpoint_string):
+    def test_delete_configuration_setting_with_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_delete_kv = self.create_config_setting_no_label()
         self.add_for_test(client, to_delete_kv)
-        deleted_kv = client.delete_configuration_setting(to_delete_kv.key, etag=to_delete_kv.etag)
-        assert deleted_kv is not None
-        with pytest.raises(ResourceNotFoundError):
-            client.get_configuration_setting(to_delete_kv.key)
+        to_delete_kv = client.get_configuration_setting(to_delete_kv.key, to_delete_kv.label)
 
-    @app_config_aad_decorator
-    @recorded_by_proxy
-    def test_delete_wrong_etag(self, appconfiguration_endpoint_string):
-        client = self.create_aad_client(appconfiguration_endpoint_string)
-        to_delete_kv = self.create_config_setting_no_label()
-        self.add_for_test(client, to_delete_kv)
+        # test delete with wrong etag
         with pytest.raises(ResourceModifiedError):
             client.delete_configuration_setting(
                 to_delete_kv.key, etag="wrong etag", match_condition=MatchConditions.IfNotModified
             )
-        client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
+        # test delete with correct etag
+        deleted_kv = client.delete_configuration_setting(to_delete_kv.key, etag=to_delete_kv.etag)
+        assert deleted_kv is not None
+        with pytest.raises(ResourceNotFoundError):
+            client.get_configuration_setting(to_delete_kv.key)
 
     # method: list_configuration_settings
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_key_label(self, appconfiguration_endpoint_string):
         self.set_up(appconfiguration_endpoint_string, is_aad=True)
         items = list(self.client.list_configuration_settings(label_filter=LABEL, key_filter=KEY))
@@ -301,14 +260,15 @@
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_correct_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_list_kv = self.create_config_setting()
         self.add_for_test(client, to_list_kv)
+        to_list_kv = client.get_configuration_setting(to_list_kv.key, to_list_kv.label)
         custom_headers = {"If-Match": to_list_kv.etag}
         items = list(
             client.list_configuration_settings(
                 key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
             )
         )
         assert len(items) == 1
@@ -407,75 +367,57 @@
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_revisions_correct_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_list_kv = self.create_config_setting()
         self.add_for_test(client, to_list_kv)
+        to_list_kv = client.get_configuration_setting(to_list_kv.key, to_list_kv.label)
         custom_headers = {"If-Match": to_list_kv.etag}
         items = list(
             client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
         )
         assert len(items) >= 1
         assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
         client.delete_configuration_setting(to_list_kv.key)
 
+    # method: set_read_only
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_read_only(self, appconfiguration_endpoint_string):
+    def test_set_read_only(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
-        kv = self.create_config_setting_no_label()
-        self.add_for_test(client, kv)
-        read_only_kv = client.set_read_only(kv)
-        assert read_only_kv.read_only
-        readable_kv = client.set_read_only(read_only_kv, False)
-        assert not readable_kv.read_only
-        client.delete_configuration_setting(kv.key)
+        to_set_kv = self.create_config_setting()
+        self.add_for_test(client, to_set_kv)
+        to_set_kv = client.get_configuration_setting(to_set_kv.key, to_set_kv.label)
 
-    @app_config_aad_decorator
-    @recorded_by_proxy
-    def test_delete_read_only(self, appconfiguration_endpoint_string):
-        client = self.create_aad_client(appconfiguration_endpoint_string)
-        to_delete_kv = self.create_config_setting_no_label()
-        self.add_for_test(client, to_delete_kv)
-        read_only_kv = client.set_read_only(to_delete_kv)
+        read_only_kv = client.set_read_only(to_set_kv)
+        assert read_only_kv.read_only
         with pytest.raises(ResourceReadOnlyError):
-            client.delete_configuration_setting(to_delete_kv.key)
-        client.set_read_only(read_only_kv, False)
-        client.delete_configuration_setting(to_delete_kv.key)
-        with pytest.raises(ResourceNotFoundError):
-            client.get_configuration_setting(to_delete_kv.key)
+            client.set_configuration_setting(read_only_kv)
+        with pytest.raises(ResourceReadOnlyError):
+            client.delete_configuration_setting(read_only_kv.key, read_only_kv.label)
+
+        writable_kv = client.set_read_only(read_only_kv, False)
+        assert not writable_kv.read_only
+        client.set_configuration_setting(writable_kv)
+        client.delete_configuration_setting(writable_kv.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
-    def test_set_read_only(self, appconfiguration_endpoint_string):
+    def test_set_read_only_with_wrong_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_set_kv = self.create_config_setting()
         self.add_for_test(client, to_set_kv)
-        to_set_kv.value = to_set_kv.value + "a"
-        to_set_kv.tags = {"a": "b", "c": "d"}
-        read_only_kv = client.set_read_only(to_set_kv)
-        with pytest.raises(ResourceReadOnlyError):
-            client.set_configuration_setting(read_only_kv)
-        readable_kv = client.set_read_only(read_only_kv, False)
-        readable_kv.value = to_set_kv.value
-        readable_kv.tags = to_set_kv.tags
-        set_kv = client.set_configuration_setting(readable_kv)
-        assert (
-            to_set_kv.key == set_kv.key
-            and to_set_kv.label == to_set_kv.label
-            and to_set_kv.value == set_kv.value
-            and to_set_kv.content_type == set_kv.content_type
-            and to_set_kv.tags == set_kv.tags
-            and to_set_kv.etag != set_kv.etag
-        )
-        set_kv.etag = "bad"
+        to_set_kv = client.get_configuration_setting(to_set_kv.key, to_set_kv.label)
+
+        to_set_kv.etag = "wrong etag"
         with pytest.raises(ResourceModifiedError):
-            client.set_read_only(set_kv, True, match_condition=MatchConditions.IfNotModified)
-        client.delete_configuration_setting(to_set_kv.key)
+            client.set_read_only(to_set_kv, False, match_condition=MatchConditions.IfNotModified)
+
+        client.delete_configuration_setting(to_set_kv)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_sync_tokens_with_configuration_setting(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         sync_tokens = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header = self._order_dict(sync_tokens)
@@ -505,15 +447,16 @@
 
         client.set_configuration_setting(new)
         sync_tokens3 = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header3 = self._order_dict(sync_tokens3)
         sync_token_header3 = ",".join(str(x) for x in sync_token_header3.values())
         assert sync_token_header2 != sync_token_header3
 
-        client.delete_configuration_setting(new.key)
+        client.delete_configuration_setting("KEY1")
+        client.delete_configuration_setting("KEY2")
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_sync_tokens_with_feature_flag_configuration_setting(self, appconfiguration_endpoint_string):
         self.set_up(appconfiguration_endpoint_string, is_aad=True)
         new = FeatureFlagConfigurationSetting(
             "custom",
@@ -574,37 +517,51 @@
         self.client.delete_configuration_setting(new.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_config_setting_feature_flag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         feature_flag = FeatureFlagConfigurationSetting("test_feature", enabled=True)
-        set_flag = client.set_configuration_setting(feature_flag)
 
+        set_flag = client.set_configuration_setting(feature_flag)
         self._assert_same_keys(feature_flag, set_flag)
+        set_flag_value = json.loads(set_flag.value)
+        assert set_flag_value["id"] == "test_feature"
+        assert set_flag_value["enabled"] == True
+        assert set_flag_value["conditions"] != None
 
         set_flag.enabled = not set_flag.enabled
         changed_flag = client.set_configuration_setting(set_flag)
-
-        changed_flag.enabled = False
+        assert changed_flag.enabled == False
         temp = json.loads(changed_flag.value)
+        assert temp["id"] == set_flag_value["id"]
         assert temp["enabled"] == False
+        assert temp["conditions"] == set_flag_value["conditions"]
 
-        c = json.loads(copy.deepcopy(changed_flag.value))
+        c = json.loads(changed_flag.value)
         c["enabled"] = True
         changed_flag.value = json.dumps(c)
         assert changed_flag.enabled == True
+        temp = json.loads(changed_flag.value)
+        assert temp["id"] == set_flag_value["id"]
+        assert temp["enabled"] == True
+        assert temp["conditions"] == set_flag_value["conditions"]
 
         changed_flag.value = json.dumps({})
         assert changed_flag.enabled == None
-        assert changed_flag.value == json.dumps({"enabled": None, "conditions": {"client_filters": None}})
+        temp = json.loads(changed_flag.value)
+        assert temp["id"] == set_flag_value["id"]
+        assert temp["enabled"] == None
+        assert temp["conditions"] != None
+        assert temp["conditions"]["client_filters"] == None
 
         set_flag.value = "bad_value"
         assert set_flag.enabled == None
         assert set_flag.filters == None
+        assert set_flag.value == "bad_value"
 
         client.delete_configuration_setting(changed_flag.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_config_setting_secret_reference(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
```

## Comparing `azure-appconfiguration-1.5.0b1/tests/testcase.py` & `azure-appconfiguration-1.5.0b2/tests/testcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,21 +80,20 @@
     def _assert_same_keys(self, key1, key2):
         assert type(key1) == type(key2)
         assert key1.key == key2.key
         assert key1.label == key2.label
         assert key1.content_type == key2.content_type
         assert key1.tags == key2.tags
         assert key1.etag != key2.etag
+        assert key1.value == key2.value
         if isinstance(key1, FeatureFlagConfigurationSetting):
             assert key1.enabled == key2.enabled
             assert len(key1.filters) == len(key2.filters)
         elif isinstance(key1, SecretReferenceConfigurationSetting):
             assert key1.secret_id == key2.secret_id
-        else:
-            assert key1.value == key2.value
 
     def _assert_snapshots(self, snapshot: Snapshot, expected_snapshot: Snapshot):
         assert snapshot.composition_type == expected_snapshot.composition_type
         assert snapshot.created == expected_snapshot.created
         assert snapshot.etag == expected_snapshot.etag
         assert snapshot.expires == expected_snapshot.expires
         assert len(snapshot.filters) == len(expected_snapshot.filters)
```

## Comparing `azure-appconfiguration-1.5.0b1/tests/conftest.py` & `azure-appconfiguration-1.5.0b2/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/tests/test_sync_token_policy.py` & `azure-appconfiguration-1.5.0b2/tests/test_sync_token_policy.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/tests/asynctestcase.py` & `azure-appconfiguration-1.5.0b2/tests/asynctestcase.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client.py` & `azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,113 +43,73 @@
 
 class TestAppConfigurationClient(AppConfigTestCase):
     # method: add_configuration_setting
     @app_config_decorator
     @recorded_by_proxy
     def test_add_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
-        kv = ConfigurationSetting(
+        test_config_setting = ConfigurationSetting(
             key=KEY + "_ADD",
             label=LABEL,
             value=TEST_VALUE,
             content_type=TEST_CONTENT_TYPE,
             tags={"tag1": "tag1", "tag2": "tag2"},
         )
-        created_kv = client.add_configuration_setting(kv)
+        created_kv = client.add_configuration_setting(test_config_setting)
         assert (
-            created_kv.label == kv.label
-            and kv.value == kv.value
-            and created_kv.content_type == kv.content_type
-            and created_kv.tags == kv.tags
+            created_kv.label == test_config_setting.label
+            and created_kv.value == test_config_setting.value
+            and created_kv.content_type == test_config_setting.content_type
+            and created_kv.tags == test_config_setting.tags
+            and created_kv.etag != None
+            and created_kv.etag != test_config_setting.etag
+            and created_kv.last_modified != None
+            and created_kv.read_only == False
         )
-        assert created_kv.etag is not None and created_kv.last_modified is not None and created_kv.read_only is False
-        client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
-    @app_config_decorator
-    @recorded_by_proxy
-    def test_add_existing_configuration_setting(self, appconfiguration_connection_string):
-        client = self.create_client(appconfiguration_connection_string)
-        test_config_setting = self.create_config_setting()
-        self.add_for_test(client, test_config_setting)
+        # test add existing configuration setting
         with pytest.raises(ResourceExistsError):
             client.add_configuration_setting(
                 ConfigurationSetting(
                     key=test_config_setting.key,
                     label=test_config_setting.label,
                 )
             )
-        client.delete_configuration_setting(key=test_config_setting.key, label=test_config_setting.label)
+        client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
     # method: set_configuration_setting
     @app_config_decorator
     @recorded_by_proxy
-    def test_set_existing_configuration_setting_label_etag(self, appconfiguration_connection_string):
+    def test_set_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_set_kv = self.create_config_setting()
         to_set_kv.value = to_set_kv.value + "a"
         to_set_kv.tags = {"a": "b", "c": "d"}
         set_kv = client.set_configuration_setting(to_set_kv)
         assert (
             to_set_kv.key == set_kv.key
-            and to_set_kv.label == to_set_kv.label
+            and to_set_kv.label == set_kv.label
             and to_set_kv.value == set_kv.value
             and to_set_kv.content_type == set_kv.content_type
             and to_set_kv.tags == set_kv.tags
             and to_set_kv.etag != set_kv.etag
         )
         client.delete_configuration_setting(key=to_set_kv.key, label=to_set_kv.label)
 
     @app_config_decorator
     @recorded_by_proxy
-    def test_set_existing_configuration_setting_label_wrong_etag(self, appconfiguration_connection_string):
+    def test_set_configuration_setting_wrong_etag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_set_kv = self.create_config_setting()
         to_set_kv.value = to_set_kv.value + "a"
         to_set_kv.tags = {"a": "b", "c": "d"}
         to_set_kv.etag = "wrong etag"
         with pytest.raises(ResourceModifiedError):
             client.set_configuration_setting(to_set_kv, match_condition=MatchConditions.IfNotModified)
 
-    @app_config_decorator
-    @recorded_by_proxy
-    def test_set_configuration_setting_etag(self, appconfiguration_connection_string):
-        client = self.create_client(appconfiguration_connection_string)
-        kv = ConfigurationSetting(
-            key=KEY + "_SET",
-            label=LABEL,
-            value=TEST_VALUE,
-            content_type=TEST_CONTENT_TYPE,
-            tags={"tag1": "tag1", "tag2": "tag2"},
-        )
-        kv.etag = "random etag"
-        with pytest.raises(ResourceModifiedError):
-            client.set_configuration_setting(kv, match_condition=MatchConditions.IfNotModified)
-
-    @app_config_decorator
-    @recorded_by_proxy
-    def test_set_configuration_setting_no_etag(self, appconfiguration_connection_string):
-        client = self.create_client(appconfiguration_connection_string)
-        to_set_kv = ConfigurationSetting(
-            key=KEY + "_SET",
-            label=LABEL,
-            value=TEST_VALUE,
-            content_type=TEST_CONTENT_TYPE,
-            tags={"tag1": "tag1", "tag2": "tag2"},
-        )
-        set_kv = client.set_configuration_setting(to_set_kv)
-        assert (
-            to_set_kv.key == set_kv.key
-            and to_set_kv.label == set_kv.label
-            and to_set_kv.value == set_kv.value
-            and to_set_kv.content_type == set_kv.content_type
-            and to_set_kv.tags == set_kv.tags
-            and to_set_kv.etag != set_kv.etag
-        )
-        client.delete_configuration_setting(key=to_set_kv.key, label=to_set_kv.label)
-
     # method: get_configuration_setting
     @app_config_decorator
     @recorded_by_proxy
     def test_get_configuration_setting_no_label(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         compare_kv = self.create_config_setting_no_label()
         self.add_for_test(client, compare_kv)
@@ -161,15 +121,15 @@
             and fetched_kv.tags == compare_kv.tags
         )
         assert fetched_kv.label is None
         client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     @app_config_decorator
     @recorded_by_proxy
-    def test_get_configuration_setting_label(self, appconfiguration_connection_string):
+    def test_get_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         compare_kv = self.create_config_setting()
         self.add_for_test(client, compare_kv)
         fetched_kv = client.get_configuration_setting(compare_kv.key, compare_kv.label)
         assert (
             fetched_kv.key == compare_kv.key
             and fetched_kv.value == compare_kv.value
@@ -181,71 +141,85 @@
         client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_get_non_existing_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         compare_kv = self.create_config_setting()
-        self.add_for_test(client, compare_kv)
         with pytest.raises(ResourceNotFoundError):
             client.get_configuration_setting(compare_kv.key, compare_kv.label + "a")
+
+    @app_config_decorator
+    @recorded_by_proxy
+    def test_get_configuration_setting_with_etag(self, appconfiguration_connection_string):
+        client = self.create_client(appconfiguration_connection_string)
+        compare_kv = self.create_config_setting()
+        self.add_for_test(client, compare_kv)
+        compare_kv = client.get_configuration_setting(compare_kv.key, compare_kv.label)
+
+        # test get with wrong etag
+        with pytest.raises(ResourceModifiedError):
+            client.get_configuration_setting(
+                compare_kv.key, compare_kv.label, etag="wrong etag", match_condition=MatchConditions.IfNotModified
+            )
+        # test get with correct etag
+        with pytest.raises(ResourceNotFoundError):
+            client.get_configuration_setting(compare_kv.key, etag=compare_kv.etag)
+        client.get_configuration_setting(compare_kv.key, compare_kv.label, etag=compare_kv.etag)
+
         client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     # method: delete_configuration_setting
     @app_config_decorator
     @recorded_by_proxy
-    def test_delete_with_key_no_label(self, appconfiguration_connection_string):
+    def test_delete_configuration_setting_with_key_no_label(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_delete_kv = self.create_config_setting_no_label()
         self.add_for_test(client, to_delete_kv)
         deleted_kv = client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
         assert deleted_kv is not None
         with pytest.raises(ResourceNotFoundError):
             client.get_configuration_setting(to_delete_kv.key)
 
     @app_config_decorator
     @recorded_by_proxy
-    def test_delete_with_key_label(self, appconfiguration_connection_string):
+    def test_delete_configuration_setting_with_key_label(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_delete_kv = self.create_config_setting()
         self.add_for_test(client, to_delete_kv)
         deleted_kv = client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
         assert deleted_kv is not None
         with pytest.raises(ResourceNotFoundError):
             client.get_configuration_setting(to_delete_kv.key, label=to_delete_kv.label)
 
     @app_config_decorator
     @recorded_by_proxy
-    def test_delete_not_existing(self, appconfiguration_connection_string):
+    def test_delete_not_existing_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         deleted_kv = client.delete_configuration_setting("not_exist_" + KEY)
         assert deleted_kv is None
 
     @app_config_decorator
     @recorded_by_proxy
-    def test_delete_correct_etag(self, appconfiguration_connection_string):
+    def test_delete_configuration_setting_with_etag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_delete_kv = self.create_config_setting_no_label()
         self.add_for_test(client, to_delete_kv)
-        deleted_kv = client.delete_configuration_setting(to_delete_kv.key, etag=to_delete_kv.etag)
-        assert deleted_kv is not None
-        with pytest.raises(ResourceNotFoundError):
-            client.get_configuration_setting(to_delete_kv.key)
+        to_delete_kv = client.get_configuration_setting(to_delete_kv.key, to_delete_kv.label)
 
-    @app_config_decorator
-    @recorded_by_proxy
-    def test_delete_wrong_etag(self, appconfiguration_connection_string):
-        client = self.create_client(appconfiguration_connection_string)
-        to_delete_kv = self.create_config_setting_no_label()
-        self.add_for_test(client, to_delete_kv)
+        # test delete with wrong etag
         with pytest.raises(ResourceModifiedError):
             client.delete_configuration_setting(
                 to_delete_kv.key, etag="wrong etag", match_condition=MatchConditions.IfNotModified
             )
-        client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
+        # test delete with correct etag
+        deleted_kv = client.delete_configuration_setting(to_delete_kv.key, etag=to_delete_kv.etag)
+        assert deleted_kv is not None
+        with pytest.raises(ResourceNotFoundError):
+            client.get_configuration_setting(to_delete_kv.key)
 
     # method: list_configuration_settings
     @app_config_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_key_label(self, appconfiguration_connection_string):
         self.set_up(appconfiguration_connection_string)
         items = list(self.client.list_configuration_settings(label_filter=LABEL, key_filter=KEY))
@@ -305,14 +279,15 @@
 
     @app_config_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_correct_etag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_list_kv = self.create_config_setting()
         self.add_for_test(client, to_list_kv)
+        to_list_kv = client.get_configuration_setting(to_list_kv.key, to_list_kv.label)
         custom_headers = {"If-Match": to_list_kv.etag}
         items = list(
             client.list_configuration_settings(
                 key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
             )
         )
         assert len(items) == 1
@@ -414,75 +389,58 @@
 
     @app_config_decorator
     @recorded_by_proxy
     def test_list_revisions_correct_etag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_list_kv = self.create_config_setting()
         self.add_for_test(client, to_list_kv)
+        to_list_kv = client.get_configuration_setting(to_list_kv.key, to_list_kv.label)
         custom_headers = {"If-Match": to_list_kv.etag}
         items = list(
             client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
         )
         assert len(items) >= 1
         assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
+
         client.delete_configuration_setting(to_list_kv.key)
 
+    # method: set_read_only
     @app_config_decorator
     @recorded_by_proxy
-    def test_read_only(self, appconfiguration_connection_string):
+    def test_set_read_only(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
-        kv = self.create_config_setting_no_label()
-        self.add_for_test(client, kv)
-        read_only_kv = client.set_read_only(kv)
-        assert read_only_kv.read_only
-        readable_kv = client.set_read_only(read_only_kv, False)
-        assert not readable_kv.read_only
-        client.delete_configuration_setting(kv.key)
+        to_set_kv = self.create_config_setting()
+        self.add_for_test(client, to_set_kv)
+        to_set_kv = client.get_configuration_setting(to_set_kv.key, to_set_kv.label)
 
-    @app_config_decorator
-    @recorded_by_proxy
-    def test_delete_read_only(self, appconfiguration_connection_string):
-        client = self.create_client(appconfiguration_connection_string)
-        to_delete_kv = self.create_config_setting_no_label()
-        self.add_for_test(client, to_delete_kv)
-        read_only_kv = client.set_read_only(to_delete_kv)
+        read_only_kv = client.set_read_only(to_set_kv)
+        assert read_only_kv.read_only
         with pytest.raises(ResourceReadOnlyError):
-            client.delete_configuration_setting(to_delete_kv.key)
-        client.set_read_only(read_only_kv, False)
-        client.delete_configuration_setting(to_delete_kv.key)
-        with pytest.raises(ResourceNotFoundError):
-            client.get_configuration_setting(to_delete_kv.key)
+            client.set_configuration_setting(read_only_kv)
+        with pytest.raises(ResourceReadOnlyError):
+            client.delete_configuration_setting(read_only_kv.key, read_only_kv.label)
+
+        writable_kv = client.set_read_only(read_only_kv, False)
+        assert not writable_kv.read_only
+        client.set_configuration_setting(writable_kv)
+        client.delete_configuration_setting(writable_kv.key)
 
     @app_config_decorator
     @recorded_by_proxy
-    def test_set_read_only(self, appconfiguration_connection_string):
+    def test_set_read_only_with_wrong_etag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_set_kv = self.create_config_setting()
         self.add_for_test(client, to_set_kv)
-        to_set_kv.value = to_set_kv.value + "a"
-        to_set_kv.tags = {"a": "b", "c": "d"}
-        read_only_kv = client.set_read_only(to_set_kv)
-        with pytest.raises(ResourceReadOnlyError):
-            client.set_configuration_setting(read_only_kv)
-        readable_kv = client.set_read_only(read_only_kv, False)
-        readable_kv.value = to_set_kv.value
-        readable_kv.tags = to_set_kv.tags
-        set_kv = client.set_configuration_setting(readable_kv)
-        assert (
-            to_set_kv.key == set_kv.key
-            and to_set_kv.label == to_set_kv.label
-            and to_set_kv.value == set_kv.value
-            and to_set_kv.content_type == set_kv.content_type
-            and to_set_kv.tags == set_kv.tags
-            and to_set_kv.etag != set_kv.etag
-        )
-        set_kv.etag = "bad"
+        to_set_kv = client.get_configuration_setting(to_set_kv.key, to_set_kv.label)
+
+        to_set_kv.etag = "wrong etag"
         with pytest.raises(ResourceModifiedError):
-            client.set_read_only(set_kv, True, match_condition=MatchConditions.IfNotModified)
-        client.delete_configuration_setting(to_set_kv.key)
+            client.set_read_only(to_set_kv, False, match_condition=MatchConditions.IfNotModified)
+
+        client.delete_configuration_setting(to_set_kv)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_sync_tokens_with_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         sync_tokens = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header = self._order_dict(sync_tokens)
@@ -512,15 +470,16 @@
 
         client.set_configuration_setting(new)
         sync_tokens3 = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header3 = self._order_dict(sync_tokens3)
         sync_token_header3 = ",".join(str(x) for x in sync_token_header3.values())
         assert sync_token_header2 != sync_token_header3
 
-        client.delete_configuration_setting(new.key)
+        client.delete_configuration_setting("KEY1")
+        client.delete_configuration_setting("KEY2")
 
     @app_config_decorator
     @recorded_by_proxy
     def test_sync_tokens_with_feature_flag_configuration_setting(self, appconfiguration_connection_string):
         self.set_up(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
             "custom",
@@ -581,37 +540,51 @@
         self.client.delete_configuration_setting(new.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_config_setting_feature_flag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         feature_flag = FeatureFlagConfigurationSetting("test_feature", enabled=True)
-        set_flag = client.set_configuration_setting(feature_flag)
 
+        set_flag = client.set_configuration_setting(feature_flag)
         self._assert_same_keys(feature_flag, set_flag)
+        set_flag_value = json.loads(set_flag.value)
+        assert set_flag_value["id"] == "test_feature"
+        assert set_flag_value["enabled"] == True
+        assert set_flag_value["conditions"] != None
 
         set_flag.enabled = not set_flag.enabled
         changed_flag = client.set_configuration_setting(set_flag)
-
-        changed_flag.enabled = False
+        assert changed_flag.enabled == False
         temp = json.loads(changed_flag.value)
+        assert temp["id"] == set_flag_value["id"]
         assert temp["enabled"] == False
+        assert temp["conditions"] == set_flag_value["conditions"]
 
         c = json.loads(changed_flag.value)
         c["enabled"] = True
         changed_flag.value = json.dumps(c)
         assert changed_flag.enabled == True
+        temp = json.loads(changed_flag.value)
+        assert temp["id"] == set_flag_value["id"]
+        assert temp["enabled"] == True
+        assert temp["conditions"] == set_flag_value["conditions"]
 
         changed_flag.value = json.dumps({})
         assert changed_flag.enabled == None
-        assert changed_flag.value == json.dumps({"enabled": None, "conditions": {"client_filters": None}})
+        temp = json.loads(changed_flag.value)
+        assert temp["id"] == set_flag_value["id"]
+        assert temp["enabled"] == None
+        assert temp["conditions"] != None
+        assert temp["conditions"]["client_filters"] == None
 
         set_flag.value = "bad_value"
         assert set_flag.enabled == None
         assert set_flag.filters == None
+        assert set_flag.value == "bad_value"
 
         client.delete_configuration_setting(changed_flag.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_config_setting_secret_reference(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
@@ -871,14 +844,16 @@
     @recorded_by_proxy
     def test_breaking_with_secret_reference_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         new = SecretReferenceConfigurationSetting("aref", "notaurl")  # cspell:disable-line
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
+        client.delete_configuration_setting(new.key)
+
         new = SecretReferenceConfigurationSetting("aref1", "notaurl")  # cspell:disable-line
         new.content_type = "fkaeyjfdkal;"  # cspell:disable-line
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
         client.delete_configuration_setting(new.key)
 
@@ -917,14 +892,34 @@
         recovered_snapshot = self.client.recover_snapshot(name=snapshot_name)
         assert recovered_snapshot.status == "ready"
 
         self.tear_down()
 
     @app_config_decorator
     @recorded_by_proxy
+    def test_update_snapshot_status_with_etag(self, appconfiguration_connection_string):
+        self.set_up(appconfiguration_connection_string)
+        snapshot_name = self.get_resource_name("snapshot")
+        filters = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response = self.client.begin_create_snapshot(name=snapshot_name, filters=filters)
+        created_snapshot = response.result()
+
+        # test update with wrong etag
+        with pytest.raises(ResourceModifiedError):
+            self.client.archive_snapshot(
+                name=snapshot_name, etag="wrong etag", match_condition=MatchConditions.IfNotModified
+            )
+        # test update with correct etag
+        archived_snapshot = self.client.archive_snapshot(name=snapshot_name, etag=created_snapshot.etag)
+        assert archived_snapshot.status == "archived"
+
+        self.tear_down()
+
+    @app_config_decorator
+    @recorded_by_proxy
     def test_list_snapshots(self, appconfiguration_connection_string):
         self.set_up(appconfiguration_connection_string)
 
         result = self.client.list_snapshots()
         initial_snapshots = len(list(result))
 
         snapshot_name1 = self.get_resource_name("snapshot1")
```

## Comparing `azure-appconfiguration-1.5.0b1/tests/preparers.py` & `azure-appconfiguration-1.5.0b2/tests/preparers.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad_async.py` & `azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_aad_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,52 +41,47 @@
 
 class TestAppConfigurationClientAADAsync(AsyncAppConfigTestCase):
     # method: add_configuration_setting
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_add_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
-            kv = ConfigurationSetting(
+            test_config_setting = ConfigurationSetting(
                 key=KEY + "_ADD",
                 label=LABEL,
                 value=TEST_VALUE,
                 content_type=TEST_CONTENT_TYPE,
                 tags={"tag1": "tag1", "tag2": "tag2"},
             )
-            created_kv = await client.add_configuration_setting(kv)
+            created_kv = await client.add_configuration_setting(test_config_setting)
             assert (
-                created_kv.label == kv.label
-                and kv.value == kv.value
-                and created_kv.content_type == kv.content_type
-                and created_kv.tags == kv.tags
+                created_kv.label == test_config_setting.label
+                and created_kv.value == test_config_setting.value
+                and created_kv.content_type == test_config_setting.content_type
+                and created_kv.tags == test_config_setting.tags
+                and created_kv.etag != None
+                and created_kv.etag != test_config_setting.etag
+                and created_kv.last_modified != None
+                and created_kv.read_only == False
             )
-            assert (
-                created_kv.etag is not None and created_kv.last_modified is not None and created_kv.read_only is False
-            )
-            await client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
-    @app_config_aad_decorator_async
-    @recorded_by_proxy_async
-    async def test_add_existing_configuration_setting(self, appconfiguration_endpoint_string):
-        async with self.create_aad_client(appconfiguration_endpoint_string) as client:
-            test_config_setting = self.create_config_setting()
-            await self.add_for_test(client, test_config_setting)
+            # test add existing configuration setting
             with pytest.raises(ResourceExistsError):
                 await client.add_configuration_setting(
                     ConfigurationSetting(
                         key=test_config_setting.key,
                         label=test_config_setting.label,
                     )
                 )
-            await client.delete_configuration_setting(key=test_config_setting.key, label=test_config_setting.label)
+            await client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
     # method: set_configuration_setting
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
-    async def test_set_existing_configuration_setting_label_etag(self, appconfiguration_endpoint_string):
+    async def test_set_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             to_set_kv = self.create_config_setting()
             to_set_kv.value = to_set_kv.value + "a"
             to_set_kv.tags = {"a": "b", "c": "d"}
             set_kv = await client.set_configuration_setting(to_set_kv)
             assert (
                 to_set_kv.key == set_kv.key
@@ -96,60 +91,23 @@
                 and to_set_kv.tags == set_kv.tags
                 and to_set_kv.etag != set_kv.etag
             )
             await client.delete_configuration_setting(key=to_set_kv.key, label=to_set_kv.label)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
-    async def test_set_existing_configuration_setting_label_wrong_etag(self, appconfiguration_endpoint_string):
+    async def test_set_configuration1_setting_with_wrong_etag(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             to_set_kv = self.create_config_setting()
             to_set_kv.value = to_set_kv.value + "a"
             to_set_kv.tags = {"a": "b", "c": "d"}
             to_set_kv.etag = "wrong etag"
             with pytest.raises(ResourceModifiedError):
                 await client.set_configuration_setting(to_set_kv, match_condition=MatchConditions.IfNotModified)
 
-    @app_config_aad_decorator_async
-    @recorded_by_proxy_async
-    async def test_set_configuration_setting_etag(self, appconfiguration_endpoint_string):
-        async with self.create_aad_client(appconfiguration_endpoint_string) as client:
-            kv = ConfigurationSetting(
-                key=KEY + "_SET",
-                label=LABEL,
-                value=TEST_VALUE,
-                content_type=TEST_CONTENT_TYPE,
-                tags={"tag1": "tag1", "tag2": "tag2"},
-            )
-            kv.etag = "random etag"
-            with pytest.raises(ResourceModifiedError):
-                await client.set_configuration_setting(kv, match_condition=MatchConditions.IfNotModified)
-
-    @app_config_aad_decorator_async
-    @recorded_by_proxy_async
-    async def test_set_configuration_setting_no_etag(self, appconfiguration_endpoint_string):
-        async with self.create_aad_client(appconfiguration_endpoint_string) as client:
-            to_set_kv = ConfigurationSetting(
-                key=KEY + "_SET",
-                label=LABEL,
-                value=TEST_VALUE,
-                content_type=TEST_CONTENT_TYPE,
-                tags={"tag1": "tag1", "tag2": "tag2"},
-            )
-            set_kv = await client.set_configuration_setting(to_set_kv)
-            assert (
-                to_set_kv.key == set_kv.key
-                and to_set_kv.label == set_kv.label
-                and to_set_kv.value == set_kv.value
-                and to_set_kv.content_type == set_kv.content_type
-                and to_set_kv.tags == set_kv.tags
-                and to_set_kv.etag != set_kv.etag
-            )
-            await client.delete_configuration_setting(key=to_set_kv.key, label=to_set_kv.label)
-
     # method: get_configuration_setting
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_get_configuration_setting_no_label(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             compare_kv = self.create_config_setting_no_label()
             await self.add_for_test(client, compare_kv)
@@ -161,87 +119,105 @@
                 and fetched_kv.tags == compare_kv.tags
             )
             assert fetched_kv.label is None
             await client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
-    async def test_get_configuration_setting_label(self, appconfiguration_endpoint_string):
+    async def test_get_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             compare_kv = self.create_config_setting()
             await self.add_for_test(client, compare_kv)
             fetched_kv = await client.get_configuration_setting(compare_kv.key, compare_kv.label)
             assert (
                 fetched_kv.key == compare_kv.key
                 and fetched_kv.value == compare_kv.value
                 and fetched_kv.content_type == compare_kv.content_type
                 and fetched_kv.tags == compare_kv.tags
+                and fetched_kv.label == compare_kv.label
             )
             assert fetched_kv.label is not None
             await client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_get_non_existing_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             compare_kv = self.create_config_setting()
             with pytest.raises(ResourceNotFoundError):
                 await client.get_configuration_setting(compare_kv.key, compare_kv.label + "a")
 
+    @app_config_aad_decorator_async
+    @recorded_by_proxy_async
+    async def test_get_configuration_setting_with_etag(self, appconfiguration_endpoint_string):
+        async with self.create_aad_client(appconfiguration_endpoint_string) as client:
+            compare_kv = self.create_config_setting()
+            await self.add_for_test(client, compare_kv)
+            compare_kv = await client.get_configuration_setting(compare_kv.key, compare_kv.label)
+
+            # test get with wrong etag
+            with pytest.raises(ResourceModifiedError):
+                await client.get_configuration_setting(
+                    compare_kv.key, compare_kv.label, etag="wrong etag", match_condition=MatchConditions.IfNotModified
+                )
+            # test get with correct etag
+            with pytest.raises(ResourceNotFoundError):
+                await client.get_configuration_setting(compare_kv.key, etag=compare_kv.etag)
+            await client.get_configuration_setting(compare_kv.key, compare_kv.label, etag=compare_kv.etag)
+
+            await client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
+
     # method: delete_configuration_setting
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
-    async def test_delete_with_key_no_label(self, appconfiguration_endpoint_string):
+    async def test_delete_configuration_setting_with_key_no_label(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             to_delete_kv = self.create_config_setting_no_label()
             await self.add_for_test(client, to_delete_kv)
             deleted_kv = await client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
             assert deleted_kv is not None
             with pytest.raises(ResourceNotFoundError):
                 await client.get_configuration_setting(to_delete_kv.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
-    async def test_delete_with_key_label(self, appconfiguration_endpoint_string):
+    async def test_delete_configuration_setting_with_key_label(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             to_delete_kv = self.create_config_setting()
             await self.add_for_test(client, to_delete_kv)
             deleted_kv = await client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
             assert deleted_kv is not None
             with pytest.raises(ResourceNotFoundError):
                 await client.get_configuration_setting(to_delete_kv.key, label=to_delete_kv.label)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
-    async def test_delete_not_existing(self, appconfiguration_endpoint_string):
+    async def test_delete_not_existing_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             deleted_kv = await client.delete_configuration_setting("not_exist_" + KEY)
             assert deleted_kv is None
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
-    async def test_delete_correct_etag(self, appconfiguration_endpoint_string):
+    async def test_delete_configuration_setting_with_etag(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             to_delete_kv = self.create_config_setting_no_label()
             await self.add_for_test(client, to_delete_kv)
-            deleted_kv = await client.delete_configuration_setting(to_delete_kv.key, etag=to_delete_kv.etag)
-            assert deleted_kv is not None
-            with pytest.raises(ResourceNotFoundError):
-                await client.get_configuration_setting(to_delete_kv.key)
+            to_delete_kv = await client.get_configuration_setting(to_delete_kv.key, to_delete_kv.label)
 
-    @app_config_aad_decorator_async
-    @recorded_by_proxy_async
-    async def test_delete_wrong_etag(self, appconfiguration_endpoint_string):
-        async with self.create_aad_client(appconfiguration_endpoint_string) as client:
-            to_delete_kv = self.create_config_setting_no_label()
+            # test delete with wrong etag
             with pytest.raises(ResourceModifiedError):
                 await client.delete_configuration_setting(
                     to_delete_kv.key, etag="wrong etag", match_condition=MatchConditions.IfNotModified
                 )
-            await client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
+            # test delete with correct etag
+            deleted_kv = await client.delete_configuration_setting(to_delete_kv.key, etag=to_delete_kv.etag)
+            assert deleted_kv is not None
+            with pytest.raises(ResourceNotFoundError):
+                await client.get_configuration_setting(to_delete_kv.key)
 
     # method: list_configuration_settings
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_key_label(self, appconfiguration_endpoint_string):
         await self.set_up(appconfiguration_endpoint_string, is_aad=True)
         items = await self.convert_to_list(self.client.list_configuration_settings(label_filter=LABEL, key_filter=KEY))
@@ -302,14 +278,15 @@
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_correct_etag(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             to_list_kv = self.create_config_setting()
             await self.add_for_test(client, to_list_kv)
+            to_list_kv = await client.get_configuration_setting(to_list_kv.key, to_list_kv.label)
             custom_headers = {"If-Match": to_list_kv.etag or ""}
             items = await self.convert_to_list(
                 client.list_configuration_settings(
                     key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
                 )
             )
             assert len(items) == 1
@@ -413,80 +390,64 @@
         )
         assert all(x.key and not x.label and x.content_type and not x.tags and not x.etag for x in items)
         await self.tear_down()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_correct_etag(self, appconfiguration_endpoint_string):
-        await self.set_up(appconfiguration_endpoint_string, is_aad=True)
-        to_list_kv = self.create_config_setting()
-        custom_headers = {"If-Match": to_list_kv.etag or ""}
-        items = await self.convert_to_list(
-            self.client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
-        )
-        assert len(items) >= 1
-        assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
-        await self.tear_down()
-
-    @app_config_aad_decorator_async
-    @recorded_by_proxy_async
-    async def test_read_only(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
-            kv = self.create_config_setting_no_label()
-            await self.add_for_test(client, kv)
-            read_only_kv = await client.set_read_only(kv)
-            assert read_only_kv.read_only
-            readable_kv = await client.set_read_only(read_only_kv, False)
-            assert not readable_kv.read_only
-            await client.delete_configuration_setting(kv.key)
+            to_list_kv = self.create_config_setting()
+            await self.add_for_test(client, to_list_kv)
+            to_list_kv = await client.get_configuration_setting(to_list_kv.key, to_list_kv.label)
+            custom_headers = {"If-Match": to_list_kv.etag or ""}
+            items = await self.convert_to_list(
+                client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
+            )
+            assert len(items) >= 1
+            assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
 
-    @app_config_aad_decorator_async
-    @recorded_by_proxy_async
-    async def test_delete_read_only(self, appconfiguration_endpoint_string):
-        async with self.create_aad_client(appconfiguration_endpoint_string) as client:
-            to_delete_kv = self.create_config_setting_no_label()
-            await self.add_for_test(client, to_delete_kv)
-            read_only_kv = await client.set_read_only(to_delete_kv)
-            with pytest.raises(ResourceReadOnlyError):
-                await client.delete_configuration_setting(to_delete_kv.key)
-            await client.set_read_only(read_only_kv, False)
-            await client.delete_configuration_setting(to_delete_kv.key)
-            with pytest.raises(ResourceNotFoundError):
-                await client.get_configuration_setting(to_delete_kv.key)
+            await client.delete_configuration_setting(to_list_kv.key)
 
+    # method: set_read_only
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_set_read_only(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
-            to_set_kv = self.create_config_setting_no_label()
+            to_set_kv = self.create_config_setting()
             await self.add_for_test(client, to_set_kv)
-            to_set_kv.value = to_set_kv.value + "a"
-            to_set_kv.tags = {"a": "b", "c": "d"}
+            to_set_kv = await client.get_configuration_setting(to_set_kv.key, to_set_kv.label)
+
             read_only_kv = await client.set_read_only(to_set_kv)
+            assert read_only_kv.read_only
             with pytest.raises(ResourceReadOnlyError):
                 await client.set_configuration_setting(read_only_kv)
-            readable_kv = await client.set_read_only(read_only_kv, False)
-            readable_kv.value = to_set_kv.value
-            readable_kv.tags = to_set_kv.tags
-            set_kv = await client.set_configuration_setting(readable_kv)
-            assert (
-                to_set_kv.key == set_kv.key
-                and to_set_kv.label == to_set_kv.label
-                and to_set_kv.value == set_kv.value
-                and to_set_kv.content_type == set_kv.content_type
-                and to_set_kv.tags == set_kv.tags
-                and to_set_kv.etag != set_kv.etag
-            )
-            set_kv.etag = "bad"
-            with pytest.raises(ResourceModifiedError):
-                await client.set_read_only(set_kv, True, match_condition=MatchConditions.IfNotModified)
+            with pytest.raises(ResourceReadOnlyError):
+                await client.delete_configuration_setting(read_only_kv.key, read_only_kv.label)
+
+            writable_kv = await client.set_read_only(read_only_kv, False)
+            assert not writable_kv.read_only
+            await client.set_configuration_setting(writable_kv)
             await client.delete_configuration_setting(to_set_kv.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
+    async def test_set_read_only_with_wrong_etag(self, appconfiguration_endpoint_string):
+        async with self.create_aad_client(appconfiguration_endpoint_string) as client:
+            to_set_kv = self.create_config_setting()
+            await self.add_for_test(client, to_set_kv)
+            to_set_kv = await client.get_configuration_setting(to_set_kv.key, to_set_kv.label)
+
+            to_set_kv.etag = "wrong etag"
+            with pytest.raises(ResourceModifiedError):
+                await client.set_read_only(to_set_kv, False, match_condition=MatchConditions.IfNotModified)
+
+            await client.delete_configuration_setting(to_set_kv)
+
+    @app_config_aad_decorator_async
+    @recorded_by_proxy_async
     async def test_sync_tokens_with_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             sync_tokens = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header = self._order_dict(sync_tokens)
             sync_token_header = ",".join(str(x) for x in sync_token_header.values())
 
             new = ConfigurationSetting(
@@ -583,37 +544,51 @@
         await self.client.close()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_config_setting_feature_flag(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             feature_flag = FeatureFlagConfigurationSetting("test_feature", enabled=True)
-            set_flag = await client.set_configuration_setting(feature_flag)
 
+            set_flag = await client.set_configuration_setting(feature_flag)
             self._assert_same_keys(feature_flag, set_flag)
+            set_flag_value = json.loads(set_flag.value)
+            assert set_flag_value["id"] == "test_feature"
+            assert set_flag_value["enabled"] == True
+            assert set_flag_value["conditions"] != None
 
             set_flag.enabled = not set_flag.enabled
             changed_flag = await client.set_configuration_setting(set_flag)
-
-            changed_flag.enabled = False
+            assert changed_flag.enabled == False
             temp = json.loads(changed_flag.value)
+            assert temp["id"] == set_flag_value["id"]
             assert temp["enabled"] == False
+            assert temp["conditions"] == set_flag_value["conditions"]
 
-            c = json.loads(copy.deepcopy(changed_flag.value))
+            c = json.loads(changed_flag.value)
             c["enabled"] = True
             changed_flag.value = json.dumps(c)
             assert changed_flag.enabled == True
+            temp = json.loads(changed_flag.value)
+            assert temp["id"] == set_flag_value["id"]
+            assert temp["enabled"] == True
+            assert temp["conditions"] == set_flag_value["conditions"]
 
             changed_flag.value = json.dumps({})
             assert changed_flag.enabled == None
-            assert changed_flag.value == json.dumps({"enabled": None, "conditions": {"client_filters": None}})
+            temp = json.loads(changed_flag.value)
+            assert temp["id"] == set_flag_value["id"]
+            assert temp["enabled"] == None
+            assert temp["conditions"] != None
+            assert temp["conditions"]["client_filters"] == None
 
             set_flag.value = "bad_value"
             assert set_flag.enabled == None
             assert set_flag.filters == None
+            assert set_flag.value == "bad_value"
 
             await client.delete_configuration_setting(changed_flag.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_config_setting_secret_reference(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
```

## Comparing `azure-appconfiguration-1.5.0b1/tests/test_consistency.py` & `azure-appconfiguration-1.5.0b2/tests/test_consistency.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/tests/consts.py` & `azure-appconfiguration-1.5.0b2/tests/consts.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_async.py` & `azure-appconfiguration-1.5.0b2/tests/test_azure_appconfiguration_client_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,52 +43,47 @@
 
 class TestAppConfigurationClientAsync(AsyncAppConfigTestCase):
     # method: add_configuration_setting
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_add_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
-            kv = ConfigurationSetting(
+            test_config_setting = ConfigurationSetting(
                 key=KEY + "_ADD",
                 label=LABEL,
                 value=TEST_VALUE,
                 content_type=TEST_CONTENT_TYPE,
                 tags={"tag1": "tag1", "tag2": "tag2"},
             )
-            created_kv = await client.add_configuration_setting(kv)
+            created_kv = await client.add_configuration_setting(test_config_setting)
             assert (
-                created_kv.label == kv.label
-                and kv.value == kv.value
-                and created_kv.content_type == kv.content_type
-                and created_kv.tags == kv.tags
+                created_kv.label == test_config_setting.label
+                and created_kv.value == test_config_setting.value
+                and created_kv.content_type == test_config_setting.content_type
+                and created_kv.tags == test_config_setting.tags
+                and created_kv.etag != None
+                and created_kv.etag != test_config_setting.etag
+                and created_kv.last_modified != None
+                and created_kv.read_only == False
             )
-            assert (
-                created_kv.etag is not None and created_kv.last_modified is not None and created_kv.read_only is False
-            )
-            await client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
-    @app_config_decorator_async
-    @recorded_by_proxy_async
-    async def test_add_existing_configuration_setting(self, appconfiguration_connection_string):
-        async with self.create_client(appconfiguration_connection_string) as client:
-            test_config_setting = self.create_config_setting()
-            await self.add_for_test(client, test_config_setting)
+            # test add existing configuration setting
             with pytest.raises(ResourceExistsError):
                 await client.add_configuration_setting(
                     ConfigurationSetting(
                         key=test_config_setting.key,
                         label=test_config_setting.label,
                     )
                 )
-            await client.delete_configuration_setting(key=test_config_setting.key, label=test_config_setting.label)
+            await client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
     # method: set_configuration_setting
     @app_config_decorator_async
     @recorded_by_proxy_async
-    async def test_set_existing_configuration_setting_label_etag(self, appconfiguration_connection_string):
+    async def test_set_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             to_set_kv = self.create_config_setting()
             to_set_kv.value = to_set_kv.value + "a"
             to_set_kv.tags = {"a": "b", "c": "d"}
             set_kv = await client.set_configuration_setting(to_set_kv)
             assert (
                 to_set_kv.key == set_kv.key
@@ -98,60 +93,23 @@
                 and to_set_kv.tags == set_kv.tags
                 and to_set_kv.etag != set_kv.etag
             )
             await client.delete_configuration_setting(key=to_set_kv.key, label=to_set_kv.label)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
-    async def test_set_existing_configuration_setting_label_wrong_etag(self, appconfiguration_connection_string):
+    async def test_set_configuration1_setting_with_wrong_etag(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             to_set_kv = self.create_config_setting()
             to_set_kv.value = to_set_kv.value + "a"
             to_set_kv.tags = {"a": "b", "c": "d"}
             to_set_kv.etag = "wrong etag"
             with pytest.raises(ResourceModifiedError):
                 await client.set_configuration_setting(to_set_kv, match_condition=MatchConditions.IfNotModified)
 
-    @app_config_decorator_async
-    @recorded_by_proxy_async
-    async def test_set_configuration_setting_etag(self, appconfiguration_connection_string):
-        async with self.create_client(appconfiguration_connection_string) as client:
-            kv = ConfigurationSetting(
-                key=KEY + "_SET",
-                label=LABEL,
-                value=TEST_VALUE,
-                content_type=TEST_CONTENT_TYPE,
-                tags={"tag1": "tag1", "tag2": "tag2"},
-            )
-            kv.etag = "random etag"
-            with pytest.raises(ResourceModifiedError):
-                await client.set_configuration_setting(kv, match_condition=MatchConditions.IfNotModified)
-
-    @app_config_decorator_async
-    @recorded_by_proxy_async
-    async def test_set_configuration_setting_no_etag(self, appconfiguration_connection_string):
-        async with self.create_client(appconfiguration_connection_string) as client:
-            to_set_kv = ConfigurationSetting(
-                key=KEY + "_SET",
-                label=LABEL,
-                value=TEST_VALUE,
-                content_type=TEST_CONTENT_TYPE,
-                tags={"tag1": "tag1", "tag2": "tag2"},
-            )
-            set_kv = await client.set_configuration_setting(to_set_kv)
-            assert (
-                to_set_kv.key == set_kv.key
-                and to_set_kv.label == set_kv.label
-                and to_set_kv.value == set_kv.value
-                and to_set_kv.content_type == set_kv.content_type
-                and to_set_kv.tags == set_kv.tags
-                and to_set_kv.etag != set_kv.etag
-            )
-            await client.delete_configuration_setting(key=to_set_kv.key, label=to_set_kv.label)
-
     # method: get_configuration_setting
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_get_configuration_setting_no_label(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             compare_kv = self.create_config_setting_no_label()
             await self.add_for_test(client, compare_kv)
@@ -163,90 +121,105 @@
                 and fetched_kv.tags == compare_kv.tags
             )
             assert fetched_kv.label is None
             await client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
-    async def test_get_configuration_setting_label(self, appconfiguration_connection_string):
+    async def test_get_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             compare_kv = self.create_config_setting()
             await self.add_for_test(client, compare_kv)
             fetched_kv = await client.get_configuration_setting(compare_kv.key, compare_kv.label)
             assert (
                 fetched_kv.key == compare_kv.key
                 and fetched_kv.value == compare_kv.value
                 and fetched_kv.content_type == compare_kv.content_type
                 and fetched_kv.tags == compare_kv.tags
+                and fetched_kv.label == compare_kv.label
             )
             assert fetched_kv.label is not None
             await client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_get_non_existing_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             compare_kv = self.create_config_setting()
-            await self.add_for_test(client, compare_kv)
             with pytest.raises(ResourceNotFoundError):
                 await client.get_configuration_setting(compare_kv.key, compare_kv.label + "a")
+
+    @app_config_decorator_async
+    @recorded_by_proxy_async
+    async def test_get_configuration_setting_with_etag(self, appconfiguration_connection_string):
+        async with self.create_client(appconfiguration_connection_string) as client:
+            compare_kv = self.create_config_setting()
+            await self.add_for_test(client, compare_kv)
+            compare_kv = await client.get_configuration_setting(compare_kv.key, compare_kv.label)
+
+            # test get with wrong etag
+            with pytest.raises(ResourceModifiedError):
+                await client.get_configuration_setting(
+                    compare_kv.key, compare_kv.label, etag="wrong etag", match_condition=MatchConditions.IfNotModified
+                )
+            # test get with correct etag
+            with pytest.raises(ResourceNotFoundError):
+                await client.get_configuration_setting(compare_kv.key, etag=compare_kv.etag)
+            await client.get_configuration_setting(compare_kv.key, compare_kv.label, etag=compare_kv.etag)
+
             await client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     # method: delete_configuration_setting
     @app_config_decorator_async
     @recorded_by_proxy_async
-    async def test_delete_with_key_no_label(self, appconfiguration_connection_string):
+    async def test_delete_configuration_setting_with_key_no_label(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             to_delete_kv = self.create_config_setting_no_label()
             await self.add_for_test(client, to_delete_kv)
             deleted_kv = await client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
             assert deleted_kv is not None
             with pytest.raises(ResourceNotFoundError):
                 await client.get_configuration_setting(to_delete_kv.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
-    async def test_delete_with_key_label(self, appconfiguration_connection_string):
+    async def test_delete_configuration_setting_with_key_label(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             to_delete_kv = self.create_config_setting()
             await self.add_for_test(client, to_delete_kv)
             deleted_kv = await client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
             assert deleted_kv is not None
             with pytest.raises(ResourceNotFoundError):
                 await client.get_configuration_setting(to_delete_kv.key, label=to_delete_kv.label)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
-    async def test_delete_not_existing(self, appconfiguration_connection_string):
+    async def test_delete_not_existing_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             deleted_kv = await client.delete_configuration_setting("not_exist_" + KEY)
             assert deleted_kv is None
 
     @app_config_decorator_async
     @recorded_by_proxy_async
-    async def test_delete_correct_etag(self, appconfiguration_connection_string):
+    async def test_delete_configuration_setting_with_etag(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             to_delete_kv = self.create_config_setting_no_label()
             await self.add_for_test(client, to_delete_kv)
-            deleted_kv = await client.delete_configuration_setting(to_delete_kv.key, etag=to_delete_kv.etag)
-            assert deleted_kv is not None
-            with pytest.raises(ResourceNotFoundError):
-                await client.get_configuration_setting(to_delete_kv.key)
+            to_delete_kv = await client.get_configuration_setting(to_delete_kv.key, to_delete_kv.label)
 
-    @app_config_decorator_async
-    @recorded_by_proxy_async
-    async def test_delete_wrong_etag(self, appconfiguration_connection_string):
-        async with self.create_client(appconfiguration_connection_string) as client:
-            to_delete_kv = self.create_config_setting_no_label()
-            await self.add_for_test(client, to_delete_kv)
+            # test delete with wrong etag
             with pytest.raises(ResourceModifiedError):
                 await client.delete_configuration_setting(
                     to_delete_kv.key, etag="wrong etag", match_condition=MatchConditions.IfNotModified
                 )
-            await client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
+            # test delete with correct etag
+            deleted_kv = await client.delete_configuration_setting(to_delete_kv.key, etag=to_delete_kv.etag)
+            assert deleted_kv is not None
+            with pytest.raises(ResourceNotFoundError):
+                await client.get_configuration_setting(to_delete_kv.key)
 
     # method: list_configuration_settings
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_key_label(self, appconfiguration_connection_string):
         await self.set_up(appconfiguration_connection_string)
         items = await self.convert_to_list(self.client.list_configuration_settings(label_filter=LABEL, key_filter=KEY))
@@ -306,15 +279,16 @@
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_correct_etag(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             to_list_kv = self.create_config_setting()
             await self.add_for_test(client, to_list_kv)
-            custom_headers = {"If-Match": to_list_kv.etag or ""}
+            to_list_kv = await client.get_configuration_setting(to_list_kv.key, to_list_kv.label)
+            custom_headers = {"If-Match": to_list_kv.etag}
             items = await self.convert_to_list(
                 client.list_configuration_settings(
                     key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
                 )
             )
             assert len(items) == 1
             assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
@@ -420,80 +394,64 @@
         )
         assert all(x.key and not x.label and x.content_type and not x.tags and not x.etag for x in items)
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_correct_etag(self, appconfiguration_connection_string):
-        await self.set_up(appconfiguration_connection_string)
-        to_list_kv = self.create_config_setting()
-        custom_headers = {"If-Match": to_list_kv.etag or ""}
-        items = await self.convert_to_list(
-            self.client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
-        )
-        assert len(items) >= 1
-        assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
-        await self.tear_down()
-
-    @app_config_decorator_async
-    @recorded_by_proxy_async
-    async def test_read_only(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
-            kv = self.create_config_setting_no_label()
-            await self.add_for_test(client, kv)
-            read_only_kv = await client.set_read_only(kv)
-            assert read_only_kv.read_only
-            readable_kv = await client.set_read_only(read_only_kv, False)
-            assert not readable_kv.read_only
-            await client.delete_configuration_setting(kv.key)
+            to_list_kv = self.create_config_setting()
+            await self.add_for_test(client, to_list_kv)
+            to_list_kv = await client.get_configuration_setting(to_list_kv.key, to_list_kv.label)
+            custom_headers = {"If-Match": to_list_kv.etag}
+            items = await self.convert_to_list(
+                client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
+            )
+            assert len(items) >= 1
+            assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
 
-    @app_config_decorator_async
-    @recorded_by_proxy_async
-    async def test_delete_read_only(self, appconfiguration_connection_string):
-        async with self.create_client(appconfiguration_connection_string) as client:
-            to_delete_kv = self.create_config_setting_no_label()
-            await self.add_for_test(client, to_delete_kv)
-            read_only_kv = await client.set_read_only(to_delete_kv)
-            with pytest.raises(ResourceReadOnlyError):
-                await client.delete_configuration_setting(to_delete_kv.key)
-            await client.set_read_only(read_only_kv, False)
-            await client.delete_configuration_setting(to_delete_kv.key)
-            with pytest.raises(ResourceNotFoundError):
-                await client.get_configuration_setting(to_delete_kv.key)
+            await client.delete_configuration_setting(to_list_kv.key)
 
+    # method: set_read_only
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_set_read_only(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
-            to_set_kv = self.create_config_setting_no_label()
+            to_set_kv = self.create_config_setting()
             await self.add_for_test(client, to_set_kv)
-            to_set_kv.value = to_set_kv.value + "a"
-            to_set_kv.tags = {"a": "b", "c": "d"}
+            to_set_kv = await client.get_configuration_setting(to_set_kv.key, to_set_kv.label)
+
             read_only_kv = await client.set_read_only(to_set_kv)
+            assert read_only_kv.read_only
             with pytest.raises(ResourceReadOnlyError):
                 await client.set_configuration_setting(read_only_kv)
-            readable_kv = await client.set_read_only(read_only_kv, False)
-            readable_kv.value = to_set_kv.value
-            readable_kv.tags = to_set_kv.tags
-            set_kv = await client.set_configuration_setting(readable_kv)
-            assert (
-                to_set_kv.key == set_kv.key
-                and to_set_kv.label == to_set_kv.label
-                and to_set_kv.value == set_kv.value
-                and to_set_kv.content_type == set_kv.content_type
-                and to_set_kv.tags == set_kv.tags
-                and to_set_kv.etag != set_kv.etag
-            )
-            set_kv.etag = "bad"
-            with pytest.raises(ResourceModifiedError):
-                await client.set_read_only(set_kv, True, match_condition=MatchConditions.IfNotModified)
+            with pytest.raises(ResourceReadOnlyError):
+                await client.delete_configuration_setting(read_only_kv.key, read_only_kv.label)
+
+            writable_kv = await client.set_read_only(read_only_kv, False)
+            assert not writable_kv.read_only
+            await client.set_configuration_setting(writable_kv)
             await client.delete_configuration_setting(to_set_kv.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
+    async def test_set_read_only_with_wrong_etag(self, appconfiguration_connection_string):
+        async with self.create_client(appconfiguration_connection_string) as client:
+            to_set_kv = self.create_config_setting()
+            await self.add_for_test(client, to_set_kv)
+            to_set_kv = await client.get_configuration_setting(to_set_kv.key, to_set_kv.label)
+
+            to_set_kv.etag = "wrong etag"
+            with pytest.raises(ResourceModifiedError):
+                await client.set_read_only(to_set_kv, False, match_condition=MatchConditions.IfNotModified)
+
+            await client.delete_configuration_setting(to_set_kv)
+
+    @app_config_decorator_async
+    @recorded_by_proxy_async
     async def test_sync_tokens_with_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             sync_tokens = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header = self._order_dict(sync_tokens)
             sync_token_header = ",".join(str(x) for x in sync_token_header.values())
 
             new = ConfigurationSetting(
@@ -520,15 +478,16 @@
 
             await client.set_configuration_setting(new)
             sync_tokens3 = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header3 = self._order_dict(sync_tokens3)
             sync_token_header3 = ",".join(str(x) for x in sync_token_header3.values())
             assert sync_token_header2 != sync_token_header3
 
-            await client.delete_configuration_setting(new.key)
+            await client.delete_configuration_setting("KEY1")
+            await client.delete_configuration_setting("KEY2")
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_sync_tokens_with_feature_flag_configuration_setting(self, appconfiguration_connection_string):
         await self.set_up(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
             "custom",
@@ -590,37 +549,51 @@
         await self.client.close()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_config_setting_feature_flag(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             feature_flag = FeatureFlagConfigurationSetting("test_feature", enabled=True)
-            set_flag = await client.set_configuration_setting(feature_flag)
 
+            set_flag = await client.set_configuration_setting(feature_flag)
             self._assert_same_keys(feature_flag, set_flag)
+            set_flag_value = json.loads(set_flag.value)
+            assert set_flag_value["id"] == "test_feature"
+            assert set_flag_value["enabled"] == True
+            assert set_flag_value["conditions"] != None
 
             set_flag.enabled = not set_flag.enabled
             changed_flag = await client.set_configuration_setting(set_flag)
-
-            changed_flag.enabled = False
+            assert changed_flag.enabled == False
             temp = json.loads(changed_flag.value)
+            assert temp["id"] == set_flag_value["id"]
             assert temp["enabled"] == False
+            assert temp["conditions"] == set_flag_value["conditions"]
 
             c = json.loads(copy.deepcopy(changed_flag.value))
             c["enabled"] = True
             changed_flag.value = json.dumps(c)
             assert changed_flag.enabled == True
+            temp = json.loads(changed_flag.value)
+            assert temp["id"] == set_flag_value["id"]
+            assert temp["enabled"] == True
+            assert temp["conditions"] == set_flag_value["conditions"]
 
             changed_flag.value = json.dumps({})
             assert changed_flag.enabled == None
-            assert changed_flag.value == json.dumps({"enabled": None, "conditions": {"client_filters": None}})
+            temp = json.loads(changed_flag.value)
+            assert temp["id"] == set_flag_value["id"]
+            assert temp["enabled"] == None
+            assert temp["conditions"] != None
+            assert temp["conditions"]["client_filters"] == None
 
             set_flag.value = "bad_value"
             assert set_flag.enabled == None
             assert set_flag.filters == None
+            assert set_flag.value == "bad_value"
 
             await client.delete_configuration_setting(changed_flag.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_config_setting_secret_reference(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
@@ -893,14 +866,16 @@
     @recorded_by_proxy_async
     async def test_breaking_with_secret_reference_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             new = SecretReferenceConfigurationSetting("aref", "notaurl")  # cspell:disable-line
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
+            await client.delete_configuration_setting(new.key)
+
             new = SecretReferenceConfigurationSetting("aref1", "notaurl")  # cspell:disable-line
             new.content_type = "fkaeyjfdkal;"  # cspell:disable-line
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
             await client.delete_configuration_setting(new.key)
 
@@ -939,14 +914,34 @@
         recovered_snapshot = await self.client.recover_snapshot(name=snapshot_name)
         assert recovered_snapshot.status == "ready"
 
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
+    async def test_update_snapshot_status_with_etag(self, appconfiguration_connection_string):
+        await self.set_up(appconfiguration_connection_string)
+        snapshot_name = self.get_resource_name("snapshot")
+        filters = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response = await self.client.begin_create_snapshot(name=snapshot_name, filters=filters)
+        created_snapshot = await response.result()
+
+        # test update with wrong etag
+        with pytest.raises(ResourceModifiedError):
+            await self.client.archive_snapshot(
+                name=snapshot_name, etag="wrong etag", match_condition=MatchConditions.IfNotModified
+            )
+        # test update with correct etag
+        archived_snapshot = await self.client.archive_snapshot(name=snapshot_name, etag=created_snapshot.etag)
+        assert archived_snapshot.status == "archived"
+
+        await self.tear_down()
+
+    @app_config_decorator_async
+    @recorded_by_proxy_async
     async def test_list_snapshots(self, appconfiguration_connection_string):
         await self.set_up(appconfiguration_connection_string)
 
         result = await self.convert_to_list(self.client.list_snapshots())
         initial_snapshots = len(result)
 
         snapshot_name1 = self.get_resource_name("snapshot1")
```

## Comparing `azure-appconfiguration-1.5.0b1/tests/async_preparers.py` & `azure-appconfiguration-1.5.0b2/tests/async_preparers.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/tests/perfstress_tests/get.py` & `azure-appconfiguration-1.5.0b2/tests/perfstress_tests/get.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/tests/perfstress_tests/set.py` & `azure-appconfiguration-1.5.0b2/tests/perfstress_tests/set.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_client.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,339 +3,306 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 import binascii
 import sys
 from typing import Any, Dict, List, Mapping, Optional, Union, cast
 from azure.core import MatchConditions
-from azure.core.paging import ItemPaged
-from azure.core.credentials import TokenCredential
-from azure.core.pipeline import Pipeline
-from azure.core.pipeline.transport import (
-    RequestsTransport,
-)  # pylint:disable=non-abstract-transport-import,no-name-in-module
+from azure.core.async_paging import AsyncItemPaged
+from azure.core.credentials_async import AsyncTokenCredential
 from azure.core.pipeline.policies import (
     UserAgentPolicy,
-    DistributedTracingPolicy,
-    HttpLoggingPolicy,
-    BearerTokenCredentialPolicy,
-    ContentDecodePolicy,
-    RequestIdPolicy,
+    AsyncBearerTokenCredentialPolicy,
 )
-from azure.core.polling import LROPoller
+from azure.core.polling import AsyncLROPoller
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.exceptions import (
-    HttpResponseError,
-    ClientAuthenticationError,
     ResourceExistsError,
-    ResourceNotFoundError,
     ResourceModifiedError,
+    ResourceNotFoundError,
     ResourceNotModifiedError,
 )
 from azure.core.utils import CaseInsensitiveDict
-from ._azure_appconfiguration_error import ResourceReadOnlyError
-from ._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
-from ._azure_appconfiguration_credential import AppConfigConnectionStringCredential
-from ._generated import AzureAppConfiguration
-from ._generated._configuration import AzureAppConfigurationConfiguration
-from ._generated.models import SnapshotStatus, SnapshotUpdateParameters
-from ._models import ConfigurationSetting, ConfigurationSettingFilter, Snapshot
-from ._utils import (
+from ._sync_token_async import AsyncSyncTokenPolicy
+from .._azure_appconfiguration_error import ResourceReadOnlyError
+from .._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
+from .._azure_appconfiguration_credential import AppConfigConnectionStringCredential
+from .._generated.aio import AzureAppConfiguration
+from .._generated.models import SnapshotStatus, SnapshotUpdateParameters
+from .._models import ConfigurationSetting, ConfigurationSettingFilter, Snapshot
+from .._user_agent import USER_AGENT
+from .._utils import (
     get_endpoint_from_connection_string,
     prep_if_match,
     prep_if_none_match,
 )
-from ._sync_token import SyncTokenPolicy
-from ._user_agent import USER_AGENT
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 
 class AzureAppConfigurationClient:
     """Represents a client that calls restful API of Azure App Configuration service.
 
-    :param str base_url: Base url of the service.
-    :param credential: An object which can provide secrets for the app configuration service
-    :type credential: ~azure.appconfiguration.AppConfigConnectionStringCredential
-        or ~azure.core.credentials.TokenCredential
-    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding this default
-        value may result in unsupported behavior.
-    :paramtype api_version: str
+        :param str base_url: Base url of the service.
+        :param credential: An object which can provide secrets for the app configuration service
+        :type credential: ~azure.appconfiguration.AppConfigConnectionStringCredential
+            or ~azure.core.credentials_async.AsyncTokenCredential
+        :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding this default
+            value may result in unsupported behavior.
+        :paramtype api_version: str
+
+    This is the async version of :class:`~azure.appconfiguration.AzureAppConfigurationClient`
 
     """
 
     # pylint:disable=protected-access
-    def __init__(self, base_url: str, credential: TokenCredential, **kwargs) -> None:
+
+    def __init__(self, base_url: str, credential: AsyncTokenCredential, **kwargs) -> None:
         try:
             if not base_url.lower().startswith("http"):
                 base_url = "https://" + base_url
         except AttributeError as exc:
             raise ValueError("Base URL must be a string.") from exc
 
         if not credential:
             raise ValueError("Missing credential")
 
-        self._credential_scopes = base_url.strip("/") + "/.default"
+        credential_scopes = base_url.strip("/") + "/.default"
 
-        self._config = AzureAppConfigurationConfiguration(base_url, credential_scopes=self._credential_scopes, **kwargs)
-        self._config.user_agent_policy = UserAgentPolicy(base_user_agent=USER_AGENT, **kwargs)
-        self._sync_token_policy = SyncTokenPolicy()
-
-        pipeline = kwargs.get("pipeline")
-
-        if pipeline is None:
-            aad_mode = not isinstance(credential, AppConfigConnectionStringCredential)
-            pipeline = self._create_appconfig_pipeline(
-                credential=credential, aad_mode=aad_mode, base_url=base_url, **kwargs
-            )
+        user_agent_policy = UserAgentPolicy(base_user_agent=USER_AGENT, **kwargs)
+
+        self._sync_token_policy = AsyncSyncTokenPolicy()
+
+        aad_mode = not isinstance(credential, AppConfigConnectionStringCredential)
+        if aad_mode:
+            if hasattr(credential, "get_token"):
+                credential_policy = AsyncBearerTokenCredentialPolicy(
+                    credential,  # type: ignore
+                    credential_scopes,
+                )
+            else:
+                raise TypeError(
+                    "Please provide an instance from azure-identity or a class that implements the 'get_token' protocol"
+                )
+        else:
+            credential_policy = AppConfigRequestsCredentialsPolicy(credential)  # type: ignore
 
         self._impl = AzureAppConfiguration(
-            base_url, pipeline=pipeline, credential_scopes=self._credential_scopes, **kwargs
+            base_url,
+            credential_scopes=credential_scopes,
+            authentication_policy=credential_policy,
+            user_agent_policy=user_agent_policy,
+            per_call_policies=self._sync_token_policy,
+            **kwargs
         )
 
     @classmethod
     def from_connection_string(cls, connection_string: str, **kwargs) -> "AzureAppConfigurationClient":
         """Create AzureAppConfigurationClient from a Connection String.
+        This is the async version of :class:`~azure.appconfiguration.AzureAppConfigurationClient`
 
         :param str connection_string: Connection String
             (one of the access keys of the Azure App Configuration resource)
             used to access the Azure App Configuration.
         :return: An AzureAppConfigurationClient authenticated with the connection string
         :rtype: ~azure.appconfiguration.AzureAppConfigurationClient
 
         Example
 
         .. code-block:: python
 
-            from azure.appconfiguration import AzureAppConfigurationClient
+            from azure.appconfiguration.aio import AzureAppConfigurationClient
             connection_str = "<my connection string>"
-            client = AzureAppConfigurationClient.from_connection_string(connection_str)
+            async_client = AzureAppConfigurationClient.from_connection_string(connection_str)
         """
         base_url = "https://" + get_endpoint_from_connection_string(connection_string)
         return cls(
             credential=AppConfigConnectionStringCredential(connection_string),  # type: ignore
             base_url=base_url,
             **kwargs
         )
 
-    def _create_appconfig_pipeline(self, credential, base_url=None, aad_mode=False, **kwargs):
-        transport = kwargs.get("transport")
-        policies = kwargs.get("policies")
-
-        if policies is None:  # [] is a valid policy list
-            if aad_mode:
-                scope = base_url.strip("/") + "/.default"
-                if hasattr(credential, "get_token"):
-                    credential_policy = BearerTokenCredentialPolicy(credential, scope)
-                else:
-                    raise TypeError(
-                        "Please provide an instance from azure-identity "
-                        "or a class that implements the 'get_token protocol"
-                    )
-            else:
-                credential_policy = AppConfigRequestsCredentialsPolicy(credential)
-            policies = [
-                RequestIdPolicy(**kwargs),
-                self._config.headers_policy,
-                self._config.user_agent_policy,
-                self._config.retry_policy,
-                self._sync_token_policy,
-                credential_policy,
-                self._config.logging_policy,  # HTTP request/response log
-                DistributedTracingPolicy(**kwargs),
-                HttpLoggingPolicy(**kwargs),
-                ContentDecodePolicy(**kwargs),
-            ]
-
-        if not transport:
-            transport = RequestsTransport(**kwargs)
-
-        return Pipeline(transport, policies)
-
     @distributed_trace
     def list_configuration_settings(
         self, key_filter: Optional[str] = None, label_filter: Optional[str] = None, **kwargs
-    ) -> ItemPaged[ConfigurationSetting]:
+    ) -> AsyncItemPaged[ConfigurationSetting]:
+
         """List the configuration settings stored in the configuration service, optionally filtered by
         key, label and accept_datetime.
 
         :param key_filter: filter results based on their keys. '*' can be
             used as wildcard in the beginning or end of the filter
         :type key_filter: str
         :param label_filter: filter results based on their label. '*' can be
             used as wildcard in the beginning or end of the filter
         :type label_filter: str
         :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
         :keyword list[str] fields: specify which fields to include in the results. Leave None to include all fields
-        :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
-        :rtype: ~azure.core.paging.ItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :return: An async iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
         :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`
 
         Example
 
         .. code-block:: python
 
             from datetime import datetime, timedelta
 
             accept_datetime = datetime.utcnow() + timedelta(days=-1)
 
-            all_listed = client.list_configuration_settings()
-            for item in all_listed:
+            all_listed = async_client.list_configuration_settings()
+            async for item in all_listed:
                 pass  # do something
 
-            filtered_listed = client.list_configuration_settings(
+            filtered_listed = async_client.list_configuration_settings(
                 label_filter="Labe*", key_filter="Ke*", accept_datetime=str(accept_datetime)
             )
-            for item in filtered_listed:
+            async for item in filtered_listed:
                 pass  # do something
         """
         select = kwargs.pop("fields", None)
         if select:
             select = ["locked" if x == "read_only" else x for x in select]
-        error_map = {401: ClientAuthenticationError}
 
         try:
             return self._impl.get_key_values(  # type: ignore
                 label=label_filter,
                 key=key_filter,
                 select=select,
                 cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
-                error_map=error_map,
                 **kwargs
             )
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace
-    def get_configuration_setting(
+    @distributed_trace_async
+    async def get_configuration_setting(
         self,
         key: str,
         label: Optional[str] = None,
         etag: Optional[str] = "*",
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         **kwargs
     ) -> Union[None, ConfigurationSetting]:
+
         """Get the matched ConfigurationSetting from Azure App Configuration service
 
         :param key: key of the ConfigurationSetting
         :type key: str
         :param label: label used to identify the ConfigurationSetting. Default is `None`.
         :type label: str
         :param etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :type etag: str or None
         :param match_condition: The match condition to use upon the etag
         :type match_condition: ~azure.core.MatchConditions
         :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
         :return: The matched ConfigurationSetting object
-        :rtype: ~azure.appconfiguration.ConfigurationSetting
+        :rtype: ~azure.appconfiguration.ConfigurationSetting or None
         :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceModifiedError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
-            fetched_config_setting = client.get_configuration_setting(
+            # in async function
+            fetched_config_setting = await async_client.get_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
         """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError}
+        error_map = {}  # type: Dict[int, Any]
         if match_condition == MatchConditions.IfNotModified:
-            error_map[412] = ResourceModifiedError
-        if match_condition == MatchConditions.IfModified:
-            error_map[304] = ResourceNotModifiedError
+            error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfPresent:
-            error_map[412] = ResourceNotFoundError
+            error_map.update({412: ResourceNotFoundError})
         if match_condition == MatchConditions.IfMissing:
-            error_map[412] = ResourceExistsError
+            error_map.update({412: ResourceExistsError})
 
         try:
-            key_value = self._impl.get_key_value(
+            key_value = await self._impl.get_key_value(
                 key=key,
                 label=label,
                 if_match=prep_if_match(etag, match_condition),
                 if_none_match=prep_if_none_match(etag, match_condition),
                 error_map=error_map,
                 **kwargs
             )
             return ConfigurationSetting._from_generated(key_value)
         except ResourceNotModifiedError:
             return None
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace
-    def add_configuration_setting(self, configuration_setting: ConfigurationSetting, **kwargs) -> ConfigurationSetting:
+    @distributed_trace_async
+    async def add_configuration_setting(
+        self, configuration_setting: ConfigurationSetting, **kwargs
+    ) -> ConfigurationSetting:
+
         """Add a ConfigurationSetting instance into the Azure App Configuration service.
 
         :param configuration_setting: the ConfigurationSetting object to be added
         :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :return: The ConfigurationSetting object returned from the App Configuration service
         :rtype: ~azure.appconfiguration.ConfigurationSetting
         :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
+            # in async function
             config_setting = ConfigurationSetting(
                 key="MyKey",
                 label="MyLabel",
                 value="my value",
                 content_type="my content type",
                 tags={"my tag": "my tag value"}
             )
-            added_config_setting = client.add_configuration_setting(config_setting)
+            added_config_setting = await async_client.add_configuration_setting(config_setting)
         """
         key_value = configuration_setting._to_generated()
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
-        error_map = {401: ClientAuthenticationError, 412: ResourceExistsError}
+        error_map = {412: ResourceExistsError}
+
         try:
-            key_value_added = self._impl.put_key_value(
+            key_value_added = await self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_none_match="*",
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_added)
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace
-    def set_configuration_setting(
+    @distributed_trace_async
+    async def set_configuration_setting(
         self,
         configuration_setting: ConfigurationSetting,
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         **kwargs
     ) -> ConfigurationSetting:
+
         """Add or update a ConfigurationSetting.
         If the configuration setting identified by key and label does not exist, this is a create.
         Otherwise this is an update.
 
-        :param configuration_setting: the ConfigurationSetting to be added (if not exists) \
+        :param configuration_setting: the ConfigurationSetting to be added (if not exists)
             or updated (if exists) to the service
         :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :param match_condition: The match condition to use upon the etag
         :type match_condition: ~azure.core.MatchConditions
         :keyword str etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :return: The ConfigurationSetting returned from the service
         :rtype: ~azure.appconfiguration.ConfigurationSetting
@@ -347,56 +314,56 @@
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
+            # in async function
             config_setting = ConfigurationSetting(
                 key="MyKey",
                 label="MyLabel",
                 value="my set value",
                 content_type="my set content type",
                 tags={"my set tag": "my set tag value"}
             )
-            returned_config_setting = client.set_configuration_setting(config_setting)
+            returned_config_setting = await async_client.set_configuration_setting(config_setting)
         """
+        etag = kwargs.get("etag", configuration_setting.etag)
+
         key_value = configuration_setting._to_generated()
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
-        error_map = {401: ClientAuthenticationError, 409: ResourceReadOnlyError}
+        error_map = {409: ResourceReadOnlyError}  # type: Dict[int, Any]
         if match_condition == MatchConditions.IfNotModified:
-            error_map[412] = ResourceModifiedError
+            error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
-            error_map[412] = ResourceNotModifiedError
+            error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
-            error_map[412] = ResourceNotFoundError
+            error_map.update({412: ResourceNotFoundError})
         if match_condition == MatchConditions.IfMissing:
-            error_map[412] = ResourceExistsError
+            error_map.update({412: ResourceExistsError})
 
         try:
-            key_value_set = self._impl.put_key_value(
+            key_value_set = await self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_match=prep_if_match(configuration_setting.etag, match_condition),
-                if_none_match=prep_if_none_match(configuration_setting.etag, match_condition),
+                if_none_match=prep_if_none_match(etag, match_condition),
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_set)
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace
-    def delete_configuration_setting(
+    @distributed_trace_async
+    async def delete_configuration_setting(
         self, key: str, label: Optional[str] = None, **kwargs
-    ) -> ConfigurationSetting:  # pylint:disable=delete-operation-wrong-return-type
+    ) -> ConfigurationSetting:
         """Delete a ConfigurationSetting if it exists
 
         :param key: key used to identify the ConfigurationSetting
         :type key: str
         :param label: label used to identify the ConfigurationSetting. Default is `None`.
         :type label: str
         :keyword str etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
@@ -412,108 +379,104 @@
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
-            deleted_config_setting = client.delete_configuration_setting(
+            # in async function
+            deleted_config_setting = await async_client.delete_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
         """
         etag = kwargs.pop("etag", None)
         match_condition = kwargs.pop("match_condition", MatchConditions.Unconditionally)
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
-        error_map = {401: ClientAuthenticationError, 409: ResourceReadOnlyError}
+        error_map = {409: ResourceReadOnlyError}  # type: Dict[int, Any]
         if match_condition == MatchConditions.IfNotModified:
-            error_map[412] = ResourceModifiedError
+            error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
-            error_map[412] = ResourceNotModifiedError
+            error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
-            error_map[412] = ResourceNotFoundError
+            error_map.update({412: ResourceNotFoundError})
         if match_condition == MatchConditions.IfMissing:
-            error_map[412] = ResourceExistsError
+            error_map.update({412: ResourceExistsError})
 
         try:
-            key_value_deleted = self._impl.delete_key_value(
+            key_value_deleted = await self._impl.delete_key_value(
                 key=key,
                 label=label,
                 if_match=prep_if_match(etag, match_condition),
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_deleted)  # type: ignore
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace
     def list_revisions(
         self, key_filter: Optional[str] = None, label_filter: Optional[str] = None, **kwargs
-    ) -> ItemPaged[ConfigurationSetting]:
+    ) -> AsyncItemPaged[ConfigurationSetting]:
+
         """
         Find the ConfigurationSetting revision history, optionally filtered by key, label and accept_datetime.
 
         :param key_filter: filter results based on their keys. '*' can be
             used as wildcard in the beginning or end of the filter
         :type key_filter: str
         :param label_filter: filter results based on their label. '*' can be
             used as wildcard in the beginning or end of the filter
         :type label_filter: str
         :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
         :keyword list[str] fields: specify which fields to include in the results. Leave None to include all fields
-        :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
-        :rtype: ~azure.core.paging.ItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :return: An async iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
         :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`
 
         Example
 
         .. code-block:: python
 
+            # in async function
             from datetime import datetime, timedelta
 
             accept_datetime = datetime.utcnow() + timedelta(days=-1)
 
-            all_revisions = client.list_revisions()
-            for item in all_revisions:
+            all_revisions = async_client.list_revisions()
+            async for item in all_revisions:
                 pass  # do something
 
-            filtered_revisions = client.list_revisions(
+            filtered_revisions = async_client.list_revisions(
                 label_filter="Labe*", key_filter="Ke*", accept_datetime=str(accept_datetime)
             )
-            for item in filtered_revisions:
+            async for item in filtered_revisions:
                 pass  # do something
         """
         select = kwargs.pop("fields", None)
         if select:
             select = ["locked" if x == "read_only" else x for x in select]
-        error_map = {401: ClientAuthenticationError}
 
         try:
             return self._impl.get_revisions(  # type: ignore
                 label=label_filter,
                 key=key_filter,
                 select=select,
                 cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
-                error_map=error_map,
                 **kwargs
             )
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace
-    def set_read_only(
+    @distributed_trace_async
+    async def set_read_only(
         self, configuration_setting: ConfigurationSetting, read_only: bool = True, **kwargs
     ) -> ConfigurationSetting:
+
         """Set a configuration setting read only
 
         :param configuration_setting: the ConfigurationSetting to be set read only
         :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :param read_only: set the read only setting if true, else clear the read only setting
         :type read_only: bool
         :keyword match_condition: The match condition to use upon the etag
@@ -525,70 +488,66 @@
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
             :class:`~azure.core.exceptions.ResourceNotFoundError`
 
         Example
 
         .. code-block:: python
 
-            config_setting = client.get_configuration_setting(
+            config_setting = await async_client.get_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
 
-            read_only_config_setting = client.set_read_only(config_setting)
-            read_only_config_setting = client.set_read_only(config_setting, read_only=False)
+            read_only_config_setting = await async_client.set_read_only(config_setting)
+            read_only_config_setting = await client.set_read_only(config_setting, read_only=False)
         """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError}
-
+        error_map = {}  # type: Dict[int, Any]
         match_condition = kwargs.pop("match_condition", MatchConditions.Unconditionally)
         if match_condition == MatchConditions.IfNotModified:
-            error_map[412] = ResourceModifiedError
+            error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
-            error_map[412] = ResourceNotModifiedError
+            error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
-            error_map[412] = ResourceNotFoundError
+            error_map.update({412: ResourceNotFoundError})
         if match_condition == MatchConditions.IfMissing:
-            error_map[412] = ResourceExistsError
+            error_map.update({412: ResourceExistsError})
 
         try:
             if read_only:
-                key_value = self._impl.put_lock(
+                key_value = await self._impl.put_lock(
                     key=configuration_setting.key,
                     label=configuration_setting.label,
                     if_match=prep_if_match(configuration_setting.etag, match_condition),
                     if_none_match=prep_if_none_match(configuration_setting.etag, match_condition),
                     error_map=error_map,
                     **kwargs
                 )
             else:
-                key_value = self._impl.delete_lock(
+                key_value = await self._impl.delete_lock(
                     key=configuration_setting.key,
                     label=configuration_setting.label,
                     if_match=prep_if_match(configuration_setting.etag, match_condition),
                     if_none_match=prep_if_none_match(configuration_setting.etag, match_condition),
                     error_map=error_map,
                     **kwargs
                 )
             return ConfigurationSetting._from_generated(key_value)
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace
-    def begin_create_snapshot(
+    @distributed_trace_async
+    async def begin_create_snapshot(
         self,
         name: str,
         filters: List[ConfigurationSettingFilter],
         *,
         composition_type: Optional[Literal["key", "key_label"]] = None,
         retention_period: Optional[int] = None,
         tags: Optional[Dict[str, str]] = None,
         **kwargs
-    ) -> LROPoller[Snapshot]:
+    ) -> AsyncLROPoller[Snapshot]:
         """Create a snapshot of the configuration settings.
 
         :param name: The name of the snapshot to create.
         :type name: str
         :param filters: A list of filters used to filter the configuration settings by key field and label field
             included in the snapshot.
         :type filters: list[~azure.appconfiguration.ConfigurationSettingFilter]
@@ -597,33 +556,34 @@
             ensures there are no two key-values containing the same key. The 'key_label' composition type ensures
             there are no two key-values containing the same key and label.
         :keyword int retention_period: The amount of time, in seconds, that a snapshot will remain in the
             archived state before expiring. This property is only writable during the creation of a
             snapshot. If not specified, will set to 2592000(30 days). If specified, should be
             in range 3600(1 hour) to 7776000(90 days).
         :keyword dict[str, str] tags: The tags of the snapshot.
-        :return: A poller for create snapshot operation. Call `result()` on this object to wait for the
+        :return: An async poller for create snapshot operation. Call `result()` on this object to wait for the
             operation to complete and get the created snapshot.
-        :rtype: ~azure.core.polling.LROPoller[~azure.appconfiguration.Snapshot]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.appconfiguration.Snapshot]
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         snapshot = Snapshot(
             filters=filters, composition_type=composition_type, retention_period=retention_period, tags=tags
         )
         try:
             return cast(
-                LROPoller[Snapshot],
-                self._impl.begin_create_snapshot(
+                AsyncLROPoller[Snapshot],
+                await self._impl.begin_create_snapshot(
                     name=name, entity=snapshot._to_generated(), cls=Snapshot._from_deserialized, **kwargs
                 ),
             )
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
-    @distributed_trace
-    def archive_snapshot(
+    @distributed_trace_async
+    async def archive_snapshot(
         self,
         name: str,
         *,
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         etag: Optional[str] = None,
         **kwargs
     ) -> Snapshot:
@@ -633,29 +593,40 @@
         :param name: The name of the configuration setting snapshot to archive.
         :type name: str
         :keyword match_condition: The match condition to use upon the etag.
         :type match_condition: ~azure.core.MatchConditions
         :keyword str etag: Check if the Snapshot is changed. Set None to skip checking etag.
         :return: The Snapshot returned from the service.
         :rtype: ~azure.appconfiguration.Snapshot
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
+        error_map = {}  # type: Dict[int, Any]
+        if match_condition == MatchConditions.IfNotModified:
+            error_map.update({412: ResourceModifiedError})
+        if match_condition == MatchConditions.IfModified:
+            error_map.update({412: ResourceNotModifiedError})
+        if match_condition == MatchConditions.IfPresent:
+            error_map.update({412: ResourceNotFoundError})
+        if match_condition == MatchConditions.IfMissing:
+            error_map.update({412: ResourceExistsError})
         try:
-            generated_snapshot = self._impl.update_snapshot(
+            generated_snapshot = await self._impl.update_snapshot(
                 name=name,
                 entity=SnapshotUpdateParameters(status=SnapshotStatus.ARCHIVED),
                 if_match=prep_if_match(etag, match_condition),
                 if_none_match=prep_if_none_match(etag, match_condition),
+                error_map=error_map,
                 **kwargs
             )
             return Snapshot._from_generated(generated_snapshot)
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
-    @distributed_trace
-    def recover_snapshot(
+    @distributed_trace_async
+    async def recover_snapshot(
         self,
         name: str,
         *,
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         etag: Optional[str] = None,
         **kwargs
     ) -> Snapshot:
@@ -664,115 +635,128 @@
         :param name: The name of the configuration setting snapshot to recover.
         :type name: str
         :keyword match_condition: The match condition to use upon the etag.
         :type match_condition: ~azure.core.MatchConditions
         :keyword str etag: Check if the Snapshot is changed. Set None to skip checking etag.
         :return: The Snapshot returned from the service.
         :rtype: ~azure.appconfiguration.Snapshot
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
+        error_map = {}  # type: Dict[int, Any]
+        if match_condition == MatchConditions.IfNotModified:
+            error_map.update({412: ResourceModifiedError})
+        if match_condition == MatchConditions.IfModified:
+            error_map.update({412: ResourceNotModifiedError})
+        if match_condition == MatchConditions.IfPresent:
+            error_map.update({412: ResourceNotFoundError})
+        if match_condition == MatchConditions.IfMissing:
+            error_map.update({412: ResourceExistsError})
         try:
-            generated_snapshot = self._impl.update_snapshot(
+            generated_snapshot = await self._impl.update_snapshot(
                 name=name,
                 entity=SnapshotUpdateParameters(status=SnapshotStatus.READY),
                 if_match=prep_if_match(etag, match_condition),
                 if_none_match=prep_if_none_match(etag, match_condition),
+                error_map=error_map,
                 **kwargs
             )
             return Snapshot._from_generated(generated_snapshot)
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
-    @distributed_trace
-    def get_snapshot(self, name: str, *, fields: Optional[List[str]] = None, **kwargs) -> Snapshot:
+    @distributed_trace_async
+    async def get_snapshot(self, name: str, *, fields: Optional[List[str]] = None, **kwargs) -> Snapshot:
         """Get a configuration setting snapshot.
 
         :param name: The name of the configuration setting snapshot to retrieve.
         :type name: str
         :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
         :return: The Snapshot returned from the service.
         :rtype: ~azure.appconfiguration.Snapshot
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         try:
-            generated_snapshot = self._impl.get_snapshot(
+            generated_snapshot = await self._impl.get_snapshot(
                 name=name, if_match=None, if_none_match=None, select=fields, **kwargs
             )
             return Snapshot._from_generated(generated_snapshot)
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
     @distributed_trace
     def list_snapshots(
         self,
         *,
         name: Optional[str] = None,
         fields: Optional[List[str]] = None,
         status: Optional[List[str]] = None,
         **kwargs
-    ) -> ItemPaged[Snapshot]:
+    ) -> AsyncItemPaged[Snapshot]:
         """List the configuration setting snapshots stored in the configuration service, optionally filtered by
         snapshot name, snapshot status and fields to present in return.
 
         :keyword str name: Filter results based on snapshot name.
         :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
         :keyword list[str] status: Filter results based on snapshot keys.
-        :return: An iterator of :class:`~azure.appconfiguration.Snapshot`
-        :rtype: ~azure.core.paging.ItemPaged[~azure.appconfiguration.Snapshot]
+        :return: An async iterator of :class:`~azure.appconfiguration.Snapshot`
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.Snapshot]
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         try:
             return self._impl.get_snapshots(  # type: ignore
                 name=name,
                 select=fields,
                 status=status,
                 cls=lambda objs: [Snapshot._from_generated(x) for x in objs],
                 **kwargs
             )
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
     @distributed_trace
     def list_snapshot_configuration_settings(
         self, name: str, *, accept_datetime: Optional[str] = None, fields: Optional[List[str]] = None, **kwargs
-    ) -> ItemPaged[ConfigurationSetting]:
+    ) -> AsyncItemPaged[ConfigurationSetting]:
         """List the configuration settings stored under a snapshot in the configuration service, optionally filtered by
         accept_datetime and fields to present in return.
 
         :param str name: The snapshot name.
-        :keyword str accept_datetime: Filter out ConfigurationSetting created after this datetime
-        :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields
-        :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
-        :rtype: ~azure.core.paging.ItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :keyword str accept_datetime: Filter out ConfigurationSetting created after this datetime.
+        :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
+        :return: An async iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
+        :rtype: ~azure.core.paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         if fields:
             fields = ["locked" if x == "read_only" else x for x in fields]
 
         try:
             return self._impl.get_key_values(  # type: ignore
                 select=fields,
                 snapshot=name,
                 accept_datetime=accept_datetime,
                 cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
                 **kwargs
             )
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
+
+    async def update_sync_token(self, token: str) -> None:
 
-    def update_sync_token(self, token: str) -> None:
         """Add a sync token to the internal list of tokens.
 
         :param str token: The sync token to be added to the internal list of tokens
         """
-        if not self._sync_token_policy:
-            raise AttributeError(
-                "Client has no sync token policy, possibly because it was not provided during instantiation."
-            )
-        self._sync_token_policy.add_token(token)
 
-    def close(self) -> None:
+        await self._sync_token_policy.add_token(token)
+
+    async def close(self) -> None:
+
         """Close all connections made by the client"""
-        self._impl._client.close()
+        await self._impl._client.close()
 
-    def __enter__(self):
-        self._impl.__enter__()
+    async def __aenter__(self):
+        await self._impl.__aenter__()
         return self
 
-    def __exit__(self, *args):
-        self._impl.__exit__(*args)
+    async def __aexit__(self, *args):
+        await self._impl.__aexit__(*args)
```

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/__init__.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_utils.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_models.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 ]
 
 
 class ConfigurationSetting(Model):
     """A configuration value.
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar value: The value of the configuration setting
+    :ivar value: The value of the configuration setting.
     :vartype value: str
-    :ivar etag: Entity tag (etag) of the object
+    :ivar etag: Entity tag (etag) of the object.
     :vartype etag: str
-    :ivar key:
+    :ivar key: The key of the configuration setting.
     :vartype key: str
-    :ivar label:
+    :ivar label: The label of the configuration setting.
     :vartype label: str
-    :ivar content_type:
+    :ivar content_type: The content_type of the configuration setting.
     :vartype content_type: str
     :ivar last_modified:
     :vartype last_modified: datetime
     :ivar read_only:
     :vartype read_only: bool
-    :ivar tags:
+    :ivar tags: The tags assigned to the configuration setting.
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "etag": {"key": "etag", "type": "str"},
         "key": {"key": "key", "type": "str"},
         "label": {"key": "label", "type": "str"},
@@ -119,37 +119,39 @@
         )
 
 
 class FeatureFlagConfigurationSetting(ConfigurationSetting):  # pylint: disable=too-many-instance-attributes
     """A feature flag configuration value.
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar etag: Entity tag (etag) of the object
+    :ivar etag: Entity tag (etag) of the object.
     :vartype etag: str
-    :param feature_id:
+    :param feature_id: The identity of the configuration setting.
     :type feature_id: str
-    :ivar value: The value of the configuration setting
+    :ivar value: The value of the configuration setting.
     :vartype value: str
-    :keyword enabled:
+    :keyword enabled: The value indicating whether the feature flag is enabled. A feature is OFF if enabled is false.
+        If enabled is true, then the feature is ON if there are no conditions or if all conditions are satisfied.
     :paramtype enabled: bool
-    :keyword filters:
+    :keyword filters: Filters that must run on the client and be evaluated as true for the feature
+        to be considered enabled.
     :paramtype filters: list[dict[str, Any]]
-    :ivar label:
+    :ivar label: The label used to group this configuration setting with others.
     :vartype label: str
-    :ivar display_name:
+    :ivar display_name: The name for the feature to use for display rather than the ID.
     :vartype display_name: str
-    :ivar description:
+    :ivar description: The description of the feature.
     :vartype description: str
-    :ivar content_type:
+    :ivar content_type: The content_type of the configuration setting.
     :vartype content_type: str
     :ivar last_modified:
     :vartype last_modified: datetime
     :ivar read_only:
     :vartype read_only: bool
-    :ivar tags:
+    :ivar tags: The tags assigned to the configuration setting.
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "etag": {"key": "etag", "type": "str"},
         "feature_id": {"key": "feature_id", "type": "str"},
         "label": {"key": "label", "type": "str"},
@@ -181,35 +183,38 @@
         self.tags = kwargs.get("tags", {})
         self.read_only = kwargs.get("read_only", None)
         self.etag = kwargs.get("etag", None)
         self.description = kwargs.get("description", None)
         self.display_name = kwargs.get("display_name", None)
         self.filters = [] if filters is None else filters
         self.enabled = enabled
-        self._value = json.dumps({"enabled": self.enabled, "conditions": {"client_filters": self.filters}})
+        self._value = json.dumps(
+            {"id": self.feature_id, "enabled": self.enabled, "conditions": {"client_filters": self.filters}}
+        )
 
     @property
     def value(self):
         try:
             temp = json.loads(self._value)
+            temp["id"] = self.feature_id
             temp["enabled"] = self.enabled
-
             if "conditions" not in temp.keys():
                 temp["conditions"] = {}
             temp["conditions"]["client_filters"] = self.filters
             self._value = json.dumps(temp)
             return self._value
         except (json.JSONDecodeError, ValueError):
             return self._value
 
     @value.setter
     def value(self, new_value):
         try:
             temp = json.loads(new_value)
-            self._value = new_value
+            temp["id"] = self.feature_id
+            self._value = json.dumps(temp)
             self.enabled = temp.get("enabled", None)
             self.filters = None
             conditions = temp.get("conditions", None)
             if conditions:
                 self.filters = conditions.get("client_filters", None)
         except (json.JSONDecodeError, ValueError):
             self._value = new_value
@@ -257,31 +262,31 @@
 
 
 class SecretReferenceConfigurationSetting(ConfigurationSetting):
     """A configuration value that references a KeyVault Secret
     Variables are only populated by the server, and will be ignored when
     sending a request.
 
-    :ivar etag: Entity tag (etag) of the object
+    :ivar etag: Entity tag (etag) of the object.
     :vartype etag: str
-    :param key:
+    :param key: The key of the configuration setting.
     :type key: str
-    :param secret_id:
+    :param secret_id: The identity of the configuration setting.
     :type secret_id: str
-    :ivar label:
+    :ivar label: The label used to group this configuration setting with others.
     :vartype label: str
-    :ivar content_type:
+    :ivar content_type: The content_type of the configuration setting.
     :vartype content_type: str
     :ivar value: The value of the configuration setting
     :vartype value: dict[str, Any]
     :ivar last_modified:
     :vartype last_modified: datetime
     :ivar read_only:
     :vartype read_only: bool
-    :ivar tags:
+    :ivar tags: The tags assigned to the configuration setting.
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "etag": {"key": "etag", "type": "str"},
         "key": {"key": "key", "type": "str"},
         "label": {"key": "label", "type": "str"},
@@ -461,16 +466,19 @@
 
     @classmethod
     def _from_generated(cls, generated: GeneratedSnapshot) -> "Snapshot":
         if generated is None:
             return generated
 
         filters = []
-        for config_setting_filter in generated.filters:
-            filters.append(ConfigurationSettingFilter(key=config_setting_filter.key, label=config_setting_filter.label))
+        if generated.filters:
+            for config_setting_filter in generated.filters:
+                filters.append(
+                    ConfigurationSettingFilter(key=config_setting_filter.key, label=config_setting_filter.label)
+                )
         snapshot = cls(
             filters=filters,
             composition_type=cast(Optional[Literal["key", "key_label"]], generated.composition_type),
             retention_period=generated.retention_period,
             tags=generated.tags,
         )
         snapshot.name = generated.name
@@ -489,16 +497,19 @@
         response: HttpResponse,
         deserialized: GeneratedSnapshot,
         response_headers: Dict,
     ) -> "Snapshot":
         if deserialized is None:
             return deserialized
         filters = []
-        for config_setting_filter in deserialized.filters:
-            filters.append(ConfigurationSettingFilter(key=config_setting_filter.key, label=config_setting_filter.label))
+        if deserialized.filters:
+            for config_setting_filter in deserialized.filters:
+                filters.append(
+                    ConfigurationSettingFilter(key=config_setting_filter.key, label=config_setting_filter.label)
+                )
         snapshot = cls(
             filters=filters,
             composition_type=cast(Optional[Literal["key", "key_label"]], deserialized.composition_type),
             retention_period=deserialized.retention_period,
             tags=deserialized.tags,
         )
         snapshot.name = deserialized.name
```

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_credential.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_error.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_error.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
         # Get the path and query from url, which looks like https://host/path/query
         query_url = str(request.http_request.url[len(self._credentials.host) + 8 :])
         # Need URL() to get a correct encoded key value, from "%2A" to "*", when transport is in type AioHttpTransport.
         # There's a similar scenario in azure-storage-blob, the check logic is from there.
         try:
             from yarl import URL
-            from azure.core.pipeline.transport import (
+            from azure.core.pipeline.transport import (  # pylint:disable=non-abstract-transport-import,no-name-in-module
                 AioHttpTransport,
-            )  # pylint:disable=non-abstract-transport-import,no-name-in-module
+            )
 
             if (
                 isinstance(request.context.transport, AioHttpTransport)
                 or isinstance(getattr(request.context.transport, "_transport", None), AioHttpTransport)
                 or isinstance(
                     getattr(getattr(request.context.transport, "_transport", None), "_transport", None),
                     AioHttpTransport,
```

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_sync_token.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_sync_token.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/__init__.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_azure_appconfiguration_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,316 +3,319 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 import binascii
 import sys
 from typing import Any, Dict, List, Mapping, Optional, Union, cast
 from azure.core import MatchConditions
-from azure.core.async_paging import AsyncItemPaged
-from azure.core.credentials_async import AsyncTokenCredential
+from azure.core.paging import ItemPaged
+from azure.core.credentials import TokenCredential
+from azure.core.pipeline import Pipeline
+from azure.core.pipeline.transport import (  # pylint:disable=non-abstract-transport-import,no-name-in-module
+    RequestsTransport,
+)
 from azure.core.pipeline.policies import (
     UserAgentPolicy,
-    AsyncBearerTokenCredentialPolicy,
+    DistributedTracingPolicy,
+    HttpLoggingPolicy,
+    BearerTokenCredentialPolicy,
+    ContentDecodePolicy,
+    RequestIdPolicy,
 )
-from azure.core.polling import AsyncLROPoller
+from azure.core.polling import LROPoller
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.exceptions import (
-    HttpResponseError,
-    ClientAuthenticationError,
     ResourceExistsError,
-    ResourceModifiedError,
     ResourceNotFoundError,
+    ResourceModifiedError,
     ResourceNotModifiedError,
 )
 from azure.core.utils import CaseInsensitiveDict
-from ._sync_token_async import AsyncSyncTokenPolicy
-from .._azure_appconfiguration_error import ResourceReadOnlyError
-from .._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
-from .._azure_appconfiguration_credential import AppConfigConnectionStringCredential
-from .._generated.aio import AzureAppConfiguration
-from .._generated.models import SnapshotStatus, SnapshotUpdateParameters
-from .._models import ConfigurationSetting, ConfigurationSettingFilter, Snapshot
-from .._user_agent import USER_AGENT
-from .._utils import (
+from ._azure_appconfiguration_error import ResourceReadOnlyError
+from ._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
+from ._azure_appconfiguration_credential import AppConfigConnectionStringCredential
+from ._generated import AzureAppConfiguration
+from ._generated._configuration import AzureAppConfigurationConfiguration
+from ._generated.models import SnapshotStatus, SnapshotUpdateParameters
+from ._models import ConfigurationSetting, ConfigurationSettingFilter, Snapshot
+from ._utils import (
     get_endpoint_from_connection_string,
     prep_if_match,
     prep_if_none_match,
 )
+from ._sync_token import SyncTokenPolicy
+from ._user_agent import USER_AGENT
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 
 class AzureAppConfigurationClient:
     """Represents a client that calls restful API of Azure App Configuration service.
 
-        :param str base_url: Base url of the service.
-        :param credential: An object which can provide secrets for the app configuration service
-        :type credential: ~azure.appconfiguration.AppConfigConnectionStringCredential
-            or ~azure.core.credentials_async.AsyncTokenCredential
-        :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding this default
-            value may result in unsupported behavior.
-        :paramtype api_version: str
-
-    This is the async version of :class:`~azure.appconfiguration.AzureAppConfigurationClient`
+    :param str base_url: Base url of the service.
+    :param credential: An object which can provide secrets for the app configuration service
+    :type credential: ~azure.appconfiguration.AppConfigConnectionStringCredential
+        or ~azure.core.credentials.TokenCredential
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding this default
+        value may result in unsupported behavior.
+    :paramtype api_version: str
 
     """
 
     # pylint:disable=protected-access
-
-    def __init__(self, base_url: str, credential: AsyncTokenCredential, **kwargs) -> None:
+    def __init__(self, base_url: str, credential: TokenCredential, **kwargs) -> None:
         try:
             if not base_url.lower().startswith("http"):
                 base_url = "https://" + base_url
         except AttributeError as exc:
             raise ValueError("Base URL must be a string.") from exc
 
         if not credential:
             raise ValueError("Missing credential")
 
-        credential_scopes = base_url.strip("/") + "/.default"
-
-        user_agent_policy = UserAgentPolicy(base_user_agent=USER_AGENT, **kwargs)
-
-        self._sync_token_policy = AsyncSyncTokenPolicy()
+        self._credential_scopes = base_url.strip("/") + "/.default"
 
-        aad_mode = not isinstance(credential, AppConfigConnectionStringCredential)
-        if aad_mode:
-            if hasattr(credential, "get_token"):
-                credential_policy = AsyncBearerTokenCredentialPolicy(
-                    credential,  # type: ignore
-                    credential_scopes,
-                )
-            else:
-                raise TypeError(
-                    "Please provide an instance from azure-identity or a class that implements the 'get_token' protocol"
-                )
-        else:
-            credential_policy = AppConfigRequestsCredentialsPolicy(credential)  # type: ignore
+        self._config = AzureAppConfigurationConfiguration(base_url, credential_scopes=self._credential_scopes, **kwargs)
+        self._config.user_agent_policy = UserAgentPolicy(base_user_agent=USER_AGENT, **kwargs)
+        self._sync_token_policy = SyncTokenPolicy()
+
+        pipeline = kwargs.get("pipeline")
+
+        if pipeline is None:
+            aad_mode = not isinstance(credential, AppConfigConnectionStringCredential)
+            pipeline = self._create_appconfig_pipeline(
+                credential=credential, aad_mode=aad_mode, base_url=base_url, **kwargs
+            )
 
         self._impl = AzureAppConfiguration(
-            base_url,
-            credential_scopes=credential_scopes,
-            authentication_policy=credential_policy,
-            user_agent_policy=user_agent_policy,
-            per_call_policies=self._sync_token_policy,
-            **kwargs
+            base_url, pipeline=pipeline, credential_scopes=self._credential_scopes, **kwargs
         )
 
     @classmethod
     def from_connection_string(cls, connection_string: str, **kwargs) -> "AzureAppConfigurationClient":
         """Create AzureAppConfigurationClient from a Connection String.
-        This is the async version of :class:`~azure.appconfiguration.AzureAppConfigurationClient`
 
         :param str connection_string: Connection String
             (one of the access keys of the Azure App Configuration resource)
             used to access the Azure App Configuration.
         :return: An AzureAppConfigurationClient authenticated with the connection string
         :rtype: ~azure.appconfiguration.AzureAppConfigurationClient
 
         Example
 
         .. code-block:: python
 
-            from azure.appconfiguration.aio import AzureAppConfigurationClient
+            from azure.appconfiguration import AzureAppConfigurationClient
             connection_str = "<my connection string>"
-            async_client = AzureAppConfigurationClient.from_connection_string(connection_str)
+            client = AzureAppConfigurationClient.from_connection_string(connection_str)
         """
         base_url = "https://" + get_endpoint_from_connection_string(connection_string)
         return cls(
             credential=AppConfigConnectionStringCredential(connection_string),  # type: ignore
             base_url=base_url,
             **kwargs
         )
 
+    def _create_appconfig_pipeline(self, credential, base_url=None, aad_mode=False, **kwargs):
+        transport = kwargs.get("transport")
+        policies = kwargs.get("policies")
+
+        if policies is None:  # [] is a valid policy list
+            if aad_mode:
+                scope = base_url.strip("/") + "/.default"
+                if hasattr(credential, "get_token"):
+                    credential_policy = BearerTokenCredentialPolicy(credential, scope)
+                else:
+                    raise TypeError(
+                        "Please provide an instance from azure-identity "
+                        "or a class that implements the 'get_token protocol"
+                    )
+            else:
+                credential_policy = AppConfigRequestsCredentialsPolicy(credential)
+            policies = [
+                RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.retry_policy,
+                self._sync_token_policy,
+                credential_policy,
+                self._config.logging_policy,  # HTTP request/response log
+                DistributedTracingPolicy(**kwargs),
+                HttpLoggingPolicy(**kwargs),
+                ContentDecodePolicy(**kwargs),
+            ]
+
+        if not transport:
+            transport = RequestsTransport(**kwargs)
+
+        return Pipeline(transport, policies)
+
     @distributed_trace
     def list_configuration_settings(
         self, key_filter: Optional[str] = None, label_filter: Optional[str] = None, **kwargs
-    ) -> AsyncItemPaged[ConfigurationSetting]:
-
+    ) -> ItemPaged[ConfigurationSetting]:
         """List the configuration settings stored in the configuration service, optionally filtered by
         key, label and accept_datetime.
 
         :param key_filter: filter results based on their keys. '*' can be
             used as wildcard in the beginning or end of the filter
         :type key_filter: str
         :param label_filter: filter results based on their label. '*' can be
             used as wildcard in the beginning or end of the filter
         :type label_filter: str
         :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
         :keyword list[str] fields: specify which fields to include in the results. Leave None to include all fields
         :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.appconfiguration.ConfigurationSetting]
         :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`
 
         Example
 
         .. code-block:: python
 
             from datetime import datetime, timedelta
 
             accept_datetime = datetime.utcnow() + timedelta(days=-1)
 
-            all_listed = async_client.list_configuration_settings()
-            async for item in all_listed:
+            all_listed = client.list_configuration_settings()
+            for item in all_listed:
                 pass  # do something
 
-            filtered_listed = async_client.list_configuration_settings(
+            filtered_listed = client.list_configuration_settings(
                 label_filter="Labe*", key_filter="Ke*", accept_datetime=str(accept_datetime)
             )
-            async for item in filtered_listed:
+            for item in filtered_listed:
                 pass  # do something
         """
         select = kwargs.pop("fields", None)
         if select:
             select = ["locked" if x == "read_only" else x for x in select]
-        error_map = {401: ClientAuthenticationError}
 
         try:
             return self._impl.get_key_values(  # type: ignore
                 label=label_filter,
                 key=key_filter,
                 select=select,
                 cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
-                error_map=error_map,
                 **kwargs
             )
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace_async
-    async def get_configuration_setting(
+    @distributed_trace
+    def get_configuration_setting(
         self,
         key: str,
         label: Optional[str] = None,
         etag: Optional[str] = "*",
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         **kwargs
     ) -> Union[None, ConfigurationSetting]:
-
         """Get the matched ConfigurationSetting from Azure App Configuration service
 
         :param key: key of the ConfigurationSetting
         :type key: str
         :param label: label used to identify the ConfigurationSetting. Default is `None`.
         :type label: str
         :param etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :type etag: str or None
         :param match_condition: The match condition to use upon the etag
         :type match_condition: ~azure.core.MatchConditions
         :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
         :return: The matched ConfigurationSetting object
-        :rtype: ~azure.appconfiguration.ConfigurationSetting
+        :rtype: ~azure.appconfiguration.ConfigurationSetting or None
         :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceModifiedError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
-            # in async function
-            fetched_config_setting = await async_client.get_configuration_setting(
+            fetched_config_setting = client.get_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
         """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError}
+        error_map = {}  # type: Dict[int, Any]
         if match_condition == MatchConditions.IfNotModified:
-            error_map[412] = ResourceModifiedError
-        if match_condition == MatchConditions.IfModified:
-            error_map[304] = ResourceNotModifiedError
+            error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfPresent:
-            error_map[412] = ResourceNotFoundError
+            error_map.update({412: ResourceNotFoundError})
         if match_condition == MatchConditions.IfMissing:
-            error_map[412] = ResourceExistsError
+            error_map.update({412: ResourceExistsError})
 
         try:
-            key_value = await self._impl.get_key_value(
+            key_value = self._impl.get_key_value(
                 key=key,
                 label=label,
                 if_match=prep_if_match(etag, match_condition),
                 if_none_match=prep_if_none_match(etag, match_condition),
                 error_map=error_map,
                 **kwargs
             )
             return ConfigurationSetting._from_generated(key_value)
         except ResourceNotModifiedError:
             return None
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace_async
-    async def add_configuration_setting(
-        self, configuration_setting: ConfigurationSetting, **kwargs
-    ) -> ConfigurationSetting:
-
+    @distributed_trace
+    def add_configuration_setting(self, configuration_setting: ConfigurationSetting, **kwargs) -> ConfigurationSetting:
         """Add a ConfigurationSetting instance into the Azure App Configuration service.
 
         :param configuration_setting: the ConfigurationSetting object to be added
         :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :return: The ConfigurationSetting object returned from the App Configuration service
         :rtype: ~azure.appconfiguration.ConfigurationSetting
         :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
-            # in async function
             config_setting = ConfigurationSetting(
                 key="MyKey",
                 label="MyLabel",
                 value="my value",
                 content_type="my content type",
                 tags={"my tag": "my tag value"}
             )
-            added_config_setting = await async_client.add_configuration_setting(config_setting)
+            added_config_setting = client.add_configuration_setting(config_setting)
         """
         key_value = configuration_setting._to_generated()
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
-        error_map = {401: ClientAuthenticationError, 412: ResourceExistsError}
-
+        error_map = {412: ResourceExistsError}
         try:
-            key_value_added = await self._impl.put_key_value(
+            key_value_added = self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_none_match="*",
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_added)
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace_async
-    async def set_configuration_setting(
+    @distributed_trace
+    def set_configuration_setting(
         self,
         configuration_setting: ConfigurationSetting,
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         **kwargs
     ) -> ConfigurationSetting:
-
         """Add or update a ConfigurationSetting.
         If the configuration setting identified by key and label does not exist, this is a create.
         Otherwise this is an update.
 
         :param configuration_setting: the ConfigurationSetting to be added (if not exists) \
             or updated (if exists) to the service
         :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
@@ -329,57 +332,51 @@
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
-            # in async function
             config_setting = ConfigurationSetting(
                 key="MyKey",
                 label="MyLabel",
                 value="my set value",
                 content_type="my set content type",
                 tags={"my set tag": "my set tag value"}
             )
-            returned_config_setting = await async_client.set_configuration_setting(config_setting)
+            returned_config_setting = client.set_configuration_setting(config_setting)
         """
-        etag = kwargs.get("etag", configuration_setting.etag)
-
         key_value = configuration_setting._to_generated()
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
-        error_map = {401: ClientAuthenticationError, 409: ResourceReadOnlyError}
+        error_map = {409: ResourceReadOnlyError}  # type: Dict[int, Any]
         if match_condition == MatchConditions.IfNotModified:
-            error_map[412] = ResourceModifiedError
+            error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
-            error_map[412] = ResourceNotModifiedError
+            error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
-            error_map[412] = ResourceNotFoundError
+            error_map.update({412: ResourceNotFoundError})
         if match_condition == MatchConditions.IfMissing:
-            error_map[412] = ResourceExistsError
+            error_map.update({412: ResourceExistsError})
 
         try:
-            key_value_set = await self._impl.put_key_value(
+            key_value_set = self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_match=prep_if_match(configuration_setting.etag, match_condition),
-                if_none_match=prep_if_none_match(etag, match_condition),
+                if_none_match=prep_if_none_match(configuration_setting.etag, match_condition),
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_set)
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace_async
-    async def delete_configuration_setting(
+    @distributed_trace
+    def delete_configuration_setting(  # pylint:disable=delete-operation-wrong-return-type
         self, key: str, label: Optional[str] = None, **kwargs
     ) -> ConfigurationSetting:
         """Delete a ConfigurationSetting if it exists
 
         :param key: key used to identify the ConfigurationSetting
         :type key: str
         :param label: label used to identify the ConfigurationSetting. Default is `None`.
@@ -397,112 +394,100 @@
             :class:`~azure.core.exceptions.ResourceNotFoundError`, \
             :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
-            # in async function
-            deleted_config_setting = await async_client.delete_configuration_setting(
+            deleted_config_setting = client.delete_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
         """
         etag = kwargs.pop("etag", None)
         match_condition = kwargs.pop("match_condition", MatchConditions.Unconditionally)
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
-        error_map = {401: ClientAuthenticationError, 409: ResourceReadOnlyError}
+        error_map = {409: ResourceReadOnlyError}  # type: Dict[int, Any]
         if match_condition == MatchConditions.IfNotModified:
-            error_map[412] = ResourceModifiedError
+            error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
-            error_map[412] = ResourceNotModifiedError
+            error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
-            error_map[412] = ResourceNotFoundError
+            error_map.update({412: ResourceNotFoundError})
         if match_condition == MatchConditions.IfMissing:
-            error_map[412] = ResourceExistsError
+            error_map.update({412: ResourceExistsError})
 
         try:
-            key_value_deleted = await self._impl.delete_key_value(
+            key_value_deleted = self._impl.delete_key_value(
                 key=key,
                 label=label,
                 if_match=prep_if_match(etag, match_condition),
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_deleted)  # type: ignore
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace
     def list_revisions(
         self, key_filter: Optional[str] = None, label_filter: Optional[str] = None, **kwargs
-    ) -> AsyncItemPaged[ConfigurationSetting]:
-
+    ) -> ItemPaged[ConfigurationSetting]:
         """
         Find the ConfigurationSetting revision history, optionally filtered by key, label and accept_datetime.
 
         :param key_filter: filter results based on their keys. '*' can be
             used as wildcard in the beginning or end of the filter
         :type key_filter: str
         :param label_filter: filter results based on their label. '*' can be
             used as wildcard in the beginning or end of the filter
         :type label_filter: str
         :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
         :keyword list[str] fields: specify which fields to include in the results. Leave None to include all fields
         :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.appconfiguration.ConfigurationSetting]
         :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
             :class:`~azure.core.exceptions.ClientAuthenticationError`
 
         Example
 
         .. code-block:: python
 
-            # in async function
             from datetime import datetime, timedelta
 
             accept_datetime = datetime.utcnow() + timedelta(days=-1)
 
-            all_revisions = async_client.list_revisions()
-            async for item in all_revisions:
+            all_revisions = client.list_revisions()
+            for item in all_revisions:
                 pass  # do something
 
-            filtered_revisions = async_client.list_revisions(
+            filtered_revisions = client.list_revisions(
                 label_filter="Labe*", key_filter="Ke*", accept_datetime=str(accept_datetime)
             )
-            async for item in filtered_revisions:
+            for item in filtered_revisions:
                 pass  # do something
         """
         select = kwargs.pop("fields", None)
         if select:
             select = ["locked" if x == "read_only" else x for x in select]
-        error_map = {401: ClientAuthenticationError}
 
         try:
             return self._impl.get_revisions(  # type: ignore
                 label=label_filter,
                 key=key_filter,
                 select=select,
                 cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
-                error_map=error_map,
                 **kwargs
             )
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace_async
-    async def set_read_only(
+    @distributed_trace
+    def set_read_only(
         self, configuration_setting: ConfigurationSetting, read_only: bool = True, **kwargs
     ) -> ConfigurationSetting:
-
         """Set a configuration setting read only
 
         :param configuration_setting: the ConfigurationSetting to be set read only
         :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :param read_only: set the read only setting if true, else clear the read only setting
         :type read_only: bool
         :keyword match_condition: The match condition to use upon the etag
@@ -514,70 +499,66 @@
             :class:`~azure.core.exceptions.ClientAuthenticationError`, \
             :class:`~azure.core.exceptions.ResourceNotFoundError`
 
         Example
 
         .. code-block:: python
 
-            config_setting = await async_client.get_configuration_setting(
+            config_setting = client.get_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
 
-            read_only_config_setting = await async_client.set_read_only(config_setting)
-            read_only_config_setting = await client.set_read_only(config_setting, read_only=False)
+            read_only_config_setting = client.set_read_only(config_setting)
+            read_only_config_setting = client.set_read_only(config_setting, read_only=False)
         """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError}
-
+        error_map = {}  # type: Dict[int, Any]
         match_condition = kwargs.pop("match_condition", MatchConditions.Unconditionally)
         if match_condition == MatchConditions.IfNotModified:
-            error_map[412] = ResourceModifiedError
+            error_map.update({412: ResourceModifiedError})
         if match_condition == MatchConditions.IfModified:
-            error_map[412] = ResourceNotModifiedError
+            error_map.update({412: ResourceNotModifiedError})
         if match_condition == MatchConditions.IfPresent:
-            error_map[412] = ResourceNotFoundError
+            error_map.update({412: ResourceNotFoundError})
         if match_condition == MatchConditions.IfMissing:
-            error_map[412] = ResourceExistsError
+            error_map.update({412: ResourceExistsError})
 
         try:
             if read_only:
-                key_value = await self._impl.put_lock(
+                key_value = self._impl.put_lock(
                     key=configuration_setting.key,
                     label=configuration_setting.label,
                     if_match=prep_if_match(configuration_setting.etag, match_condition),
                     if_none_match=prep_if_none_match(configuration_setting.etag, match_condition),
                     error_map=error_map,
                     **kwargs
                 )
             else:
-                key_value = await self._impl.delete_lock(
+                key_value = self._impl.delete_lock(
                     key=configuration_setting.key,
                     label=configuration_setting.label,
                     if_match=prep_if_match(configuration_setting.etag, match_condition),
                     if_none_match=prep_if_none_match(configuration_setting.etag, match_condition),
                     error_map=error_map,
                     **kwargs
                 )
             return ConfigurationSetting._from_generated(key_value)
-        except HttpResponseError as error:
-            e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response) from error
         except binascii.Error as exc:
             raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace_async
-    async def begin_create_snapshot(
+    @distributed_trace
+    def begin_create_snapshot(
         self,
         name: str,
         filters: List[ConfigurationSettingFilter],
         *,
         composition_type: Optional[Literal["key", "key_label"]] = None,
         retention_period: Optional[int] = None,
         tags: Optional[Dict[str, str]] = None,
         **kwargs
-    ) -> AsyncLROPoller[Snapshot]:
+    ) -> LROPoller[Snapshot]:
         """Create a snapshot of the configuration settings.
 
         :param name: The name of the snapshot to create.
         :type name: str
         :param filters: A list of filters used to filter the configuration settings by key field and label field
             included in the snapshot.
         :type filters: list[~azure.appconfiguration.ConfigurationSettingFilter]
@@ -588,31 +569,32 @@
         :keyword int retention_period: The amount of time, in seconds, that a snapshot will remain in the
             archived state before expiring. This property is only writable during the creation of a
             snapshot. If not specified, will set to 2592000(30 days). If specified, should be
             in range 3600(1 hour) to 7776000(90 days).
         :keyword dict[str, str] tags: The tags of the snapshot.
         :return: A poller for create snapshot operation. Call `result()` on this object to wait for the
             operation to complete and get the created snapshot.
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.appconfiguration.Snapshot]
+        :rtype: ~azure.core.polling.LROPoller[~azure.appconfiguration.Snapshot]
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         snapshot = Snapshot(
             filters=filters, composition_type=composition_type, retention_period=retention_period, tags=tags
         )
         try:
             return cast(
-                AsyncLROPoller[Snapshot],
-                await self._impl.begin_create_snapshot(
+                LROPoller[Snapshot],
+                self._impl.begin_create_snapshot(
                     name=name, entity=snapshot._to_generated(), cls=Snapshot._from_deserialized, **kwargs
                 ),
             )
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
-    @distributed_trace_async
-    async def archive_snapshot(
+    @distributed_trace
+    def archive_snapshot(
         self,
         name: str,
         *,
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         etag: Optional[str] = None,
         **kwargs
     ) -> Snapshot:
@@ -622,29 +604,40 @@
         :param name: The name of the configuration setting snapshot to archive.
         :type name: str
         :keyword match_condition: The match condition to use upon the etag.
         :type match_condition: ~azure.core.MatchConditions
         :keyword str etag: Check if the Snapshot is changed. Set None to skip checking etag.
         :return: The Snapshot returned from the service.
         :rtype: ~azure.appconfiguration.Snapshot
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
+        error_map = {}  # type: Dict[int, Any]
+        if match_condition == MatchConditions.IfNotModified:
+            error_map.update({412: ResourceModifiedError})
+        if match_condition == MatchConditions.IfModified:
+            error_map.update({412: ResourceNotModifiedError})
+        if match_condition == MatchConditions.IfPresent:
+            error_map.update({412: ResourceNotFoundError})
+        if match_condition == MatchConditions.IfMissing:
+            error_map.update({412: ResourceExistsError})
         try:
-            generated_snapshot = await self._impl.update_snapshot(
+            generated_snapshot = self._impl.update_snapshot(
                 name=name,
                 entity=SnapshotUpdateParameters(status=SnapshotStatus.ARCHIVED),
                 if_match=prep_if_match(etag, match_condition),
                 if_none_match=prep_if_none_match(etag, match_condition),
+                error_map=error_map,
                 **kwargs
             )
             return Snapshot._from_generated(generated_snapshot)
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
-    @distributed_trace_async
-    async def recover_snapshot(
+    @distributed_trace
+    def recover_snapshot(
         self,
         name: str,
         *,
         match_condition: MatchConditions = MatchConditions.Unconditionally,
         etag: Optional[str] = None,
         **kwargs
     ) -> Snapshot:
@@ -653,114 +646,129 @@
         :param name: The name of the configuration setting snapshot to recover.
         :type name: str
         :keyword match_condition: The match condition to use upon the etag.
         :type match_condition: ~azure.core.MatchConditions
         :keyword str etag: Check if the Snapshot is changed. Set None to skip checking etag.
         :return: The Snapshot returned from the service.
         :rtype: ~azure.appconfiguration.Snapshot
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
+        error_map = {}  # type: Dict[int, Any]
+        if match_condition == MatchConditions.IfNotModified:
+            error_map.update({412: ResourceModifiedError})
+        if match_condition == MatchConditions.IfModified:
+            error_map.update({412: ResourceNotModifiedError})
+        if match_condition == MatchConditions.IfPresent:
+            error_map.update({412: ResourceNotFoundError})
+        if match_condition == MatchConditions.IfMissing:
+            error_map.update({412: ResourceExistsError})
         try:
-            generated_snapshot = await self._impl.update_snapshot(
+            generated_snapshot = self._impl.update_snapshot(
                 name=name,
                 entity=SnapshotUpdateParameters(status=SnapshotStatus.READY),
                 if_match=prep_if_match(etag, match_condition),
                 if_none_match=prep_if_none_match(etag, match_condition),
+                error_map=error_map,
                 **kwargs
             )
             return Snapshot._from_generated(generated_snapshot)
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
-    @distributed_trace_async
-    async def get_snapshot(self, name: str, *, fields: Optional[List[str]] = None, **kwargs) -> Snapshot:
+    @distributed_trace
+    def get_snapshot(self, name: str, *, fields: Optional[List[str]] = None, **kwargs) -> Snapshot:
         """Get a configuration setting snapshot.
 
         :param name: The name of the configuration setting snapshot to retrieve.
         :type name: str
         :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
         :return: The Snapshot returned from the service.
         :rtype: ~azure.appconfiguration.Snapshot
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         try:
-            generated_snapshot = await self._impl.get_snapshot(
+            generated_snapshot = self._impl.get_snapshot(
                 name=name, if_match=None, if_none_match=None, select=fields, **kwargs
             )
             return Snapshot._from_generated(generated_snapshot)
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
     @distributed_trace
     def list_snapshots(
         self,
         *,
         name: Optional[str] = None,
         fields: Optional[List[str]] = None,
         status: Optional[List[str]] = None,
         **kwargs
-    ) -> AsyncItemPaged[Snapshot]:
+    ) -> ItemPaged[Snapshot]:
         """List the configuration setting snapshots stored in the configuration service, optionally filtered by
         snapshot name, snapshot status and fields to present in return.
 
         :keyword str name: Filter results based on snapshot name.
         :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
         :keyword list[str] status: Filter results based on snapshot keys.
         :return: An iterator of :class:`~azure.appconfiguration.Snapshot`
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.Snapshot]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.appconfiguration.Snapshot]
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         try:
             return self._impl.get_snapshots(  # type: ignore
                 name=name,
                 select=fields,
                 status=status,
                 cls=lambda objs: [Snapshot._from_generated(x) for x in objs],
                 **kwargs
             )
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
     @distributed_trace
     def list_snapshot_configuration_settings(
         self, name: str, *, accept_datetime: Optional[str] = None, fields: Optional[List[str]] = None, **kwargs
-    ) -> AsyncItemPaged[ConfigurationSetting]:
+    ) -> ItemPaged[ConfigurationSetting]:
         """List the configuration settings stored under a snapshot in the configuration service, optionally filtered by
         accept_datetime and fields to present in return.
 
         :param str name: The snapshot name.
-        :keyword str accept_datetime: Filter out ConfigurationSetting created after this datetime.
-        :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
+        :keyword str accept_datetime: Filter out ConfigurationSetting created after this datetime
+        :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields
         :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
-        :rtype: ~azure.core.paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         if fields:
             fields = ["locked" if x == "read_only" else x for x in fields]
 
         try:
             return self._impl.get_key_values(  # type: ignore
                 select=fields,
                 snapshot=name,
                 accept_datetime=accept_datetime,
                 cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
                 **kwargs
             )
         except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
-
-    async def update_sync_token(self, token: str) -> None:
+            raise binascii.Error("Connection string secret has incorrect padding")  # pylint: disable=raise-missing-from
 
+    def update_sync_token(self, token: str) -> None:
         """Add a sync token to the internal list of tokens.
 
         :param str token: The sync token to be added to the internal list of tokens
         """
+        if not self._sync_token_policy:
+            raise AttributeError(
+                "Client has no sync token policy, possibly because it was not provided during instantiation."
+            )
+        self._sync_token_policy.add_token(token)
 
-        await self._sync_token_policy.add_token(token)
-
-    async def close(self) -> None:
-
+    def close(self) -> None:
         """Close all connections made by the client"""
-        await self._impl._client.close()
+        self._impl._client.close()
 
-    async def __aenter__(self):
-        await self._impl.__aenter__()
+    def __enter__(self):
+        self._impl.__enter__()
         return self
 
-    async def __aexit__(self, *args):
-        await self._impl.__aexit__(*args)
+    def __exit__(self, *args):
+        self._impl.__exit__(*args)
```

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_sync_token_async.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/aio/_sync_token_async.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_serialization.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/__init__.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_patch.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_vendor.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_azure_app_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_configuration.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/__init__.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_patch.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_vendor.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_azure_app_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_configuration.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/__init__.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_patch.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/__init__.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_patch.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_models_py3.py` & `azure-appconfiguration-1.5.0b2/azure/appconfiguration/_generated/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/PKG-INFO` & `azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-appconfiguration
-Version: 1.5.0b1
+Version: 1.5.0b2
 Summary: Microsoft App Configuration Data Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/appconfiguration/azure-appconfiguration
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -274,48 +274,48 @@
 
 <!-- SNIPPET:snapshot_samples.create_snapshot -->
 
 ```python
 from azure.appconfiguration import ConfigurationSettingFilter
 
 filters = [ConfigurationSettingFilter(key="my_key1", label="my_label1")]
-response = client.begin_create_snapshot(name="my_snapshot_name", filters=filters)
+response = client.begin_create_snapshot(name=snapshot_name, filters=filters)
 created_snapshot = response.result()
 print_snapshot(created_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### Get a Snapshot
 
 <!-- SNIPPET:snapshot_samples.get_snapshot -->
 
 ```python
-received_snapshot = client.get_snapshot(name="my_snapshot_name")
+received_snapshot = client.get_snapshot(name=snapshot_name)
 ```
 
 <!-- END SNIPPET -->
 
 ### Archive a Snapshot
 
 <!-- SNIPPET:snapshot_samples.archive_snapshot -->
 
 ```python
-archived_snapshot = client.archive_snapshot(name="my_snapshot_name")
+archived_snapshot = client.archive_snapshot(name=snapshot_name)
 print_snapshot(archived_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### Recover a Snapshot
 
 <!-- SNIPPET:snapshot_samples.recover_snapshot -->
 
 ```python
-recovered_snapshot = client.recover_snapshot(name="my_snapshot_name")
+recovered_snapshot = client.recover_snapshot(name=snapshot_name)
 print_snapshot(recovered_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 ### List Snapshots
 
@@ -329,15 +329,15 @@
 <!-- END SNIPPET -->
 
 ### List Configuration Settings of a Snapshot
 
 <!-- SNIPPET:snapshot_samples.list_snapshot_configuration_settings -->
 
 ```python
-for config_setting in client.list_snapshot_configuration_settings(name="my_snapshot_name"):
+for config_setting in client.list_snapshot_configuration_settings(name=snapshot_name):
     print_configuration_setting(config_setting)
 ```
 
 <!-- END SNIPPET -->
 
 ### Async APIs
 
@@ -383,42 +383,42 @@
 
 <!-- SNIPPET:snapshot_samples_async.create_snapshot -->
 
 ```python
 from azure.appconfiguration import ConfigurationSettingFilter
 
 filters = [ConfigurationSettingFilter(key="my_key1", label="my_label1")]
-response = await client.begin_create_snapshot(name="my_snapshot_name", filters=filters)
+response = await client.begin_create_snapshot(name=snapshot_name, filters=filters)
 created_snapshot = await response.result()
 print_snapshot(created_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.get_snapshot -->
 
 ```python
-received_snapshot = await client.get_snapshot(name="my_snapshot_name")
+received_snapshot = await client.get_snapshot(name=snapshot_name)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.archive_snapshot -->
 
 ```python
-archived_snapshot = await client.archive_snapshot(name="my_snapshot_name")
+archived_snapshot = await client.archive_snapshot(name=snapshot_name)
 print_snapshot(archived_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.recover_snapshot -->
 
 ```python
-recovered_snapshot = await client.recover_snapshot(name="my_snapshot_name")
+recovered_snapshot = await client.recover_snapshot(name=snapshot_name)
 print_snapshot(recovered_snapshot)
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.list_snapshots -->
 
@@ -428,15 +428,15 @@
 ```
 
 <!-- END SNIPPET -->
 
 <!-- SNIPPET:snapshot_samples_async.list_snapshot_configuration_settings -->
 
 ```python
-async for config_setting in client.list_snapshot_configuration_settings(name="my_snapshot_name"):
+async for config_setting in client.list_snapshot_configuration_settings(name=snapshot_name):
     print_configuration_setting(config_setting)
 ```
 
 <!-- END SNIPPET -->
 
 ## Troubleshooting
 
@@ -489,14 +489,20 @@
 [coc_contact]: mailto:opencode@microsoft.com
 [troubleshooting_guide]: https://aka.ms/azsdk/python/appconfiguration/troubleshoot
 [label_concept]: https://docs.microsoft.com/azure/azure-app-configuration/concept-key-value#label-keys
 
 
 # Release History
 
+## 1.5.0b2 (2023-08-02)
+
+### Bugs Fixed
+- Fixed a bug in deserializing and serializing Snapshot when `filters` property is `None`.
+- Fixed a bug when creating `FeatureFlagConfigurationSetting` from SDK but having an error in portal.([#31326](https://github.com/Azure/azure-sdk-for-python/issues/31326))
+
 ## 1.5.0b1 (2023-07-11)
 
 ### Features Added
 - Added support for `Snapshot` CRUD operations.
 
 ### Bugs Fixed
 - Fixed async `update_sync_token` to use async/await keywords
```

## Comparing `azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/SOURCES.txt` & `azure-appconfiguration-1.5.0b2/azure_appconfiguration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample.py` & `azure-appconfiguration-1.5.0b2/samples/hello_world_advanced_sample.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/snapshot_samples.py` & `azure-appconfiguration-1.5.0b2/samples/snapshot_samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,58 +16,60 @@
 
     Set the environment variables with your own values before running the sample:
     1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
 """
 import os
 from azure.appconfiguration import AzureAppConfigurationClient, ConfigurationSetting
 from util import print_configuration_setting, print_snapshot
+from uuid import uuid4
 
 
 def main():
     CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
     config_setting1 = ConfigurationSetting(key="my_key1", label="my_label1")
     config_setting2 = ConfigurationSetting(key="my_key2", label="my_label2")
+    snapshot_name = uuid4()
     with AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING) as client:
         client.add_configuration_setting(config_setting1)
         client.add_configuration_setting(config_setting2)
 
         # [START create_snapshot]
         from azure.appconfiguration import ConfigurationSettingFilter
 
         filters = [ConfigurationSettingFilter(key="my_key1", label="my_label1")]
-        response = client.begin_create_snapshot(name="my_snapshot_name", filters=filters)
+        response = client.begin_create_snapshot(name=snapshot_name, filters=filters)
         created_snapshot = response.result()
         print_snapshot(created_snapshot)
         # [END create_snapshot]
         print("")
 
         # [START get_snapshot]
-        received_snapshot = client.get_snapshot(name="my_snapshot_name")
+        received_snapshot = client.get_snapshot(name=snapshot_name)
         # [END get_snapshot]
 
         # [START archive_snapshot]
-        archived_snapshot = client.archive_snapshot(name="my_snapshot_name")
+        archived_snapshot = client.archive_snapshot(name=snapshot_name)
         print_snapshot(archived_snapshot)
         # [END archive_snapshot]
         print("")
 
         # [START recover_snapshot]
-        recovered_snapshot = client.recover_snapshot(name="my_snapshot_name")
+        recovered_snapshot = client.recover_snapshot(name=snapshot_name)
         print_snapshot(recovered_snapshot)
         # [END recover_snapshot]
         print("")
 
         # [START list_snapshots]
         for snapshot in client.list_snapshots():
             print_snapshot(snapshot)
         # [END list_snapshots]
         print("")
 
         # [START list_snapshot_configuration_settings]
-        for config_setting in client.list_snapshot_configuration_settings(name="my_snapshot_name"):
+        for config_setting in client.list_snapshot_configuration_settings(name=snapshot_name):
             print_configuration_setting(config_setting)
         # [END list_snapshot_configuration_settings]
 
         client.delete_configuration_setting(key=config_setting1.key, label=config_setting1.label)
         client.delete_configuration_setting(key=config_setting2.key, label=config_setting2.label)
```

## Comparing `azure-appconfiguration-1.5.0b1/samples/sync_token_samples.py` & `azure-appconfiguration-1.5.0b2/samples/sync_token_samples.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/hello_world_sample.py` & `azure-appconfiguration-1.5.0b2/samples/hello_world_sample.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample_async.py` & `azure-appconfiguration-1.5.0b2/samples/conditional_operation_sample_async.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/hello_world_sample_async.py` & `azure-appconfiguration-1.5.0b2/samples/hello_world_sample_async.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/README.md` & `azure-appconfiguration-1.5.0b2/samples/README.md`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/read_only_sample_async.py` & `azure-appconfiguration-1.5.0b2/samples/read_only_sample_async.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/read_only_sample.py` & `azure-appconfiguration-1.5.0b2/samples/read_only_sample.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample_async.py` & `azure-appconfiguration-1.5.0b2/samples/hello_world_advanced_sample_async.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/list_revision_sample_async.py` & `azure-appconfiguration-1.5.0b2/samples/list_revision_sample_async.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/util.py` & `azure-appconfiguration-1.5.0b2/samples/util.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample.py` & `azure-appconfiguration-1.5.0b2/samples/conditional_operation_sample.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/snapshot_samples_async.py` & `azure-appconfiguration-1.5.0b2/samples/snapshot_samples_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,59 +18,61 @@
     1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
 """
 import asyncio
 import os
 from azure.appconfiguration import ConfigurationSetting
 from azure.appconfiguration.aio import AzureAppConfigurationClient
 from util import print_configuration_setting, print_snapshot
+from uuid import uuid4
 
 
 async def main():
     CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
     config_setting1 = ConfigurationSetting(key="my_key1", label="my_label1")
     config_setting2 = ConfigurationSetting(key="my_key1", label="my_label2")
+    snapshot_name = uuid4()
     async with AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING) as client:
         await client.add_configuration_setting(config_setting1)
         await client.add_configuration_setting(config_setting2)
 
         # [START create_snapshot]
         from azure.appconfiguration import ConfigurationSettingFilter
 
         filters = [ConfigurationSettingFilter(key="my_key1", label="my_label1")]
-        response = await client.begin_create_snapshot(name="my_snapshot_name", filters=filters)
+        response = await client.begin_create_snapshot(name=snapshot_name, filters=filters)
         created_snapshot = await response.result()
         print_snapshot(created_snapshot)
         # [END create_snapshot]
         print("")
 
         # [START get_snapshot]
-        received_snapshot = await client.get_snapshot(name="my_snapshot_name")
+        received_snapshot = await client.get_snapshot(name=snapshot_name)
         # [END get_snapshot]
         print("")
 
         # [START archive_snapshot]
-        archived_snapshot = await client.archive_snapshot(name="my_snapshot_name")
+        archived_snapshot = await client.archive_snapshot(name=snapshot_name)
         print_snapshot(archived_snapshot)
         # [END archive_snapshot]
         print("")
 
         # [START recover_snapshot]
-        recovered_snapshot = await client.recover_snapshot(name="my_snapshot_name")
+        recovered_snapshot = await client.recover_snapshot(name=snapshot_name)
         print_snapshot(recovered_snapshot)
         # [END recover_snapshot]
         print("")
 
         # [START list_snapshots]
         async for snapshot in client.list_snapshots():
             print_snapshot(snapshot)
         # [END list_snapshots]
         print("")
 
         # [START list_snapshot_configuration_settings]
-        async for config_setting in client.list_snapshot_configuration_settings(name="my_snapshot_name"):
+        async for config_setting in client.list_snapshot_configuration_settings(name=snapshot_name):
             print_configuration_setting(config_setting)
         # [END list_snapshot_configuration_settings]
 
         await client.delete_configuration_setting(key=config_setting1.key, label=config_setting1.label)
         await client.delete_configuration_setting(key=config_setting2.key, label=config_setting2.label)
```

## Comparing `azure-appconfiguration-1.5.0b1/samples/list_revision_sample.py` & `azure-appconfiguration-1.5.0b2/samples/list_revision_sample.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.5.0b1/samples/sync_token_samples_async.py` & `azure-appconfiguration-1.5.0b2/samples/sync_token_samples_async.py`

 * *Files identical despite different names*

