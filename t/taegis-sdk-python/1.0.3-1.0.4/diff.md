# Comparing `tmp/taegis-sdk-python-1.0.3.tar.gz` & `tmp/taegis-sdk-python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.0.3.tar", last modified: Mon Jul 31 14:20:42 2023, max compression
+gzip compressed data, was "taegis-sdk-python-1.0.4.tar", last modified: Thu Aug  3 16:39:13 2023, max compression
```

## Comparing `taegis-sdk-python-1.0.3.tar` & `taegis-sdk-python-1.0.4.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.386678 taegis-sdk-python-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6228 2023-07-31 14:20:42.386678 taegis-sdk-python-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5793 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 14:20:42.386678 taegis-sdk-python-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.358678 taegis-sdk-python-1.0.3/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-31 14:20:41.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8618 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10654 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.362678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    14015 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.362678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.362678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4740 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.362678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3900 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78106 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.366678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6375 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14954 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.366678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12807 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    26822 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.366678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10314 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.366678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.370678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15823 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    24262 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    31817 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.370678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7300 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.370678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.370678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7325 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8546 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.370678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7782 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.374678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.374678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.374678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10901 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.374678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12999 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10457 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24620 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.374678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.374678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    28008 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    37546 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.378678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12204 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7214 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    42368 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.378678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9291 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.378678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.378678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6858 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.378678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5923 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5961 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    12949 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.382678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6660 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    13046 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.382678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14207 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16097 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22172 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.382678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.382678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17210 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9170 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    19048 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.382678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12659 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5913 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    34203 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.386678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3443 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13781 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53278 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.386678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.386678 taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11558 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7075 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25732 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-07-31 14:20:18.000000 taegis-sdk-python-1.0.3/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:20:42.362678 taegis-sdk-python-1.0.3/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6228 2023-07-31 14:20:42.000000 taegis-sdk-python-1.0.3/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8488 2023-07-31 14:20:42.000000 taegis-sdk-python-1.0.3/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 14:20:42.000000 taegis-sdk-python-1.0.3/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-31 14:20:42.000000 taegis-sdk-python-1.0.3/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-31 14:20:42.000000 taegis-sdk-python-1.0.3/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5793 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.738347 taegis-sdk-python-1.0.4/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10654 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    14015 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4740 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3900 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    78106 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.746347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6375 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14954 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.746347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12807 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    26822 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.746347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10314 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.746347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.750346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15823 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    24262 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31817 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.750346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.750346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.750346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8546 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.754346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7782 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.754346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.754346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.754346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10901 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.758346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12999 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10457 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24620 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.758346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.758346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    28008 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    37546 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.758346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12204 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7214 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    42368 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.762346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.762346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.762346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6858 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.762346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5923 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12949 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6660 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13046 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14207 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16097 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22172 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17210 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9170 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    19048 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12659 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    34203 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3443 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13781 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    53278 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7993 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11558 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7075 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25732 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8488 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.0.3/LICENSE` & `taegis-sdk-python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/PKG-INFO` & `taegis-sdk-python-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.3/README.md` & `taegis-sdk-python-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/setup.py` & `taegis-sdk-python-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/config.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/service_core.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/detector_registry/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/entity_profile/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-""""FastIoc Service."""
+""""Trip Service."""
 from taegis_sdk_python.service_core import ServiceCore
-from taegis_sdk_python.services.fast_ioc.mutations import TaegisSDKFastIocMutation
-from taegis_sdk_python.services.fast_ioc.queries import TaegisSDKFastIocQuery
-from taegis_sdk_python.services.fast_ioc.subscriptions import (
-    TaegisSDKFastIocSubscription,
+from taegis_sdk_python.services.trip.mutations import TaegisSDKTripMutation
+from taegis_sdk_python.services.trip.queries import TaegisSDKTripQuery
+from taegis_sdk_python.services.trip.subscriptions import (
+    TaegisSDKTripSubscription,
 )
 
 
-class FastIocService(ServiceCore):
-    """Taegis FastIoc Service."""
+class TripService(ServiceCore):
+    """Taegis Trip Service."""
 
     @property
     def query(self):
         if not self._queries:
-            self._queries = TaegisSDKFastIocQuery(self)
+            self._queries = TaegisSDKTripQuery(self)
         return self._queries
 
     @property
     def mutation(self):
         if not self._mutations:
-            self._mutations = TaegisSDKFastIocMutation(self)
+            self._mutations = TaegisSDKTripMutation(self)
         return self._mutations
 
     @property
     def subscription(self):
         if not self._subscriptions:
-            self._subscriptions = TaegisSDKFastIocSubscription(self)
+            self._subscriptions = TaegisSDKTripSubscription(self)
         return self._subscriptions
```

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/fast_ioc/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/investigations2/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/preferences/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/roadrunner/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenant_profiles/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-""""Trip Service."""
+""""Users Service."""
 from taegis_sdk_python.service_core import ServiceCore
-from taegis_sdk_python.services.trip.mutations import TaegisSDKTripMutation
-from taegis_sdk_python.services.trip.queries import TaegisSDKTripQuery
-from taegis_sdk_python.services.trip.subscriptions import (
-    TaegisSDKTripSubscription,
+from taegis_sdk_python.services.users.mutations import TaegisSDKUsersMutation
+from taegis_sdk_python.services.users.queries import TaegisSDKUsersQuery
+from taegis_sdk_python.services.users.subscriptions import (
+    TaegisSDKUsersSubscription,
 )
 
 
-class TripService(ServiceCore):
-    """Taegis Trip Service."""
+class UsersService(ServiceCore):
+    """Taegis Users Service."""
 
     @property
     def query(self):
         if not self._queries:
-            self._queries = TaegisSDKTripQuery(self)
+            self._queries = TaegisSDKUsersQuery(self)
         return self._queries
 
     @property
     def mutation(self):
         if not self._mutations:
-            self._mutations = TaegisSDKTripMutation(self)
+            self._mutations = TaegisSDKUsersMutation(self)
         return self._mutations
 
     @property
     def subscription(self):
         if not self._subscriptions:
-            self._subscriptions = TaegisSDKTripSubscription(self)
+            self._subscriptions = TaegisSDKUsersSubscription(self)
         return self._subscriptions
```

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,40 @@
-""""Users Service."""
+""""FastIoc Service."""
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from taegis_sdk_python.service_core import ServiceCore
-from taegis_sdk_python.services.users.mutations import TaegisSDKUsersMutation
-from taegis_sdk_python.services.users.queries import TaegisSDKUsersQuery
-from taegis_sdk_python.services.users.subscriptions import (
-    TaegisSDKUsersSubscription,
+from taegis_sdk_python.services.fast_ioc.mutations import TaegisSDKFastIocMutation
+from taegis_sdk_python.services.fast_ioc.queries import TaegisSDKFastIocQuery
+from taegis_sdk_python.services.fast_ioc.subscriptions import (
+    TaegisSDKFastIocSubscription,
 )
 
+if TYPE_CHECKING:  # pragma: no cover
+    from taegis_sdk_python.services import GraphQLService
+
+
+class FastIocService(ServiceCore):
+    """Taegis FastIoc Service."""
 
-class UsersService(ServiceCore):
-    """Taegis Users Service."""
+    def __init__(self, service: GraphQLService):
+        super().__init__(service)
+        self._gateway = "/fast-ioc/query"
 
     @property
     def query(self):
         if not self._queries:
-            self._queries = TaegisSDKUsersQuery(self)
+            self._queries = TaegisSDKFastIocQuery(self)
         return self._queries
 
     @property
     def mutation(self):
         if not self._mutations:
-            self._mutations = TaegisSDKUsersMutation(self)
+            self._mutations = TaegisSDKFastIocMutation(self)
         return self._mutations
 
     @property
     def subscription(self):
         if not self._subscriptions:
-            self._subscriptions = TaegisSDKUsersSubscription(self)
+            self._subscriptions = TaegisSDKFastIocSubscription(self)
         return self._subscriptions
```

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/subscriptions.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.0.4/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.3/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

