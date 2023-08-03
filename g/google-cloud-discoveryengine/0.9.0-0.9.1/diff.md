# Comparing `tmp/google-cloud-discoveryengine-0.9.0.tar.gz` & `tmp/google-cloud-discoveryengine-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-discoveryengine-0.9.0.tar", last modified: Tue Jun 20 13:27:20 2023, max compression
+gzip compressed data, was "google-cloud-discoveryengine-0.9.1.tar", last modified: Wed Jul  5 15:52:32 2023, max compression
```

## Comparing `google-cloud-discoveryengine-0.9.0.tar` & `google-cloud-discoveryengine-0.9.1.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.875496 google-cloud-discoveryengine-0.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4587 2023-06-20 13:27:20.875496 google-cloud-discoveryengine-0.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3663 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.835491 google-cloud-discoveryengine-0.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.839492 google-cloud-discoveryengine-0.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/
--rw-rw-r--   0 root         (0)     1003     5697 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/
--rw-rw-r--   0 root         (0)     1003     4020 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8490 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17074 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26167 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6703 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13608 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13816 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23102 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.843492 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47501 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58096 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5885 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.847493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10026 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22476 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22924 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    60840 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.847493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38042 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48349 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     5793 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.847493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8545 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18663 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19066 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    49720 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.847493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17593 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28224 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/client.py
--rw-rw-r--   0 root         (0)     1003     5721 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.851493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6595 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13393 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13611 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22989 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.851493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27405 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37270 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.851493 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8157 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17214 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17552 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41428 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/
--rw-rw-r--   0 root         (0)     1003     3050 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3977 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     4614 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     6357 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/document.py
--rw-rw-r--   0 root         (0)     1003     9309 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    21849 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/import_config.py
--rw-rw-r--   0 root         (0)     1003     4073 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/purge_config.py
--rw-rw-r--   0 root         (0)     1003     2392 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/schema.py
--rw-rw-r--   0 root         (0)     1003     8915 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/schema_service.py
--rw-rw-r--   0 root         (0)     1003    16487 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/search_service.py
--rw-rw-r--   0 root         (0)     1003    27255 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3424 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003     4372 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     9266 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17110 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26203 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6711 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13616 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13824 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22926 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.855494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47829 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58424 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5921 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.859494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10042 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23048 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    60520 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.859494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17422 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27322 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.859494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6712 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13617 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13829 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23083 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.859494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38222 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48529 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     5829 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.863494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8553 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18711 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19114 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    49372 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.863494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17633 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28264 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py
--rw-rw-r--   0 root         (0)     1003     5757 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.863494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6603 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13401 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13619 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22813 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.863494 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27473 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37338 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.867495 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8165 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17230 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17568 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41036 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.867495 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     3197 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5368 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/common.py
--rw-rw-r--   0 root         (0)     1003     4809 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     6716 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/document.py
--rw-rw-r--   0 root         (0)     1003     9481 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    22350 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/import_config.py
--rw-rw-r--   0 root         (0)     1003     4085 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/purge_config.py
--rw-rw-r--   0 root         (0)     1003    10788 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
--rw-rw-r--   0 root         (0)     1003     2396 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/schema.py
--rw-rw-r--   0 root         (0)     1003     9031 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/schema_service.py
--rw-rw-r--   0 root         (0)     1003    40476 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/search_service.py
--rw-rw-r--   0 root         (0)     1003    27718 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3436 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/
--rw-r--r--   0 root         (0)     1003     4587 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    10665 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-20 13:27:20.000000 google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-20 13:27:20.875496 google-cloud-discoveryengine-0.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.871495 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    83160 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_completion_service.py
--rw-rw-r--   0 root         (0)     1003   201237 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_document_service.py
--rw-rw-r--   0 root         (0)     1003   168146 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_schema_service.py
--rw-rw-r--   0 root         (0)     1003    93087 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_search_service.py
--rw-rw-r--   0 root         (0)     1003   119289 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-20 13:27:20.875496 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    83584 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
--rw-rw-r--   0 root         (0)     1003   201685 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
--rw-rw-r--   0 root         (0)     1003    86195 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
--rw-rw-r--   0 root         (0)     1003   168594 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
--rw-rw-r--   0 root         (0)     1003    94203 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
--rw-rw-r--   0 root         (0)     1003   119544 2023-06-20 13:23:48.000000 google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.925343 google-cloud-discoveryengine-0.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4587 2023-07-05 15:52:32.925343 google-cloud-discoveryengine-0.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3663 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.889342 google-cloud-discoveryengine-0.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.893342 google-cloud-discoveryengine-0.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.893342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine/
+-rw-rw-r--   0 root         (0)     1003     5697 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.893342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/
+-rw-rw-r--   0 root         (0)     1003     4020 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8490 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.893342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.897343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17108 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26167 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.897343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6703 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13608 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13816 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23102 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.897343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47533 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58096 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5885 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.897343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10026 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22476 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22924 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    60840 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.897343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38072 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48349 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5793 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.901342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8545 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18663 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19066 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    49720 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.901342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17623 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28224 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5721 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.901342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6595 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13393 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13611 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22989 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.901342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27438 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37270 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.901342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8157 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17214 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17552 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41428 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.905342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3050 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3977 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4614 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6357 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9309 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    21849 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003     4073 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/purge_config.py
+-rw-rw-r--   0 root         (0)     1003     2392 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     8915 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    16487 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27255 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3424 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.905342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4372 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9266 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.905342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.905342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17144 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26203 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.905342 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6711 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13616 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13824 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22926 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.909343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47861 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58424 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5921 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.909343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10042 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22600 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23048 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    60520 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.909343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17460 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27322 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.909343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6712 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13617 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13829 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23083 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.909343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38252 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48529 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5829 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.913343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8553 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18711 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19114 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    49372 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.913343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17663 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28264 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5757 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.913343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6603 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13401 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13619 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22813 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.913343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27506 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37338 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.917343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8165 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17230 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17568 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41036 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.917343 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     3197 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5368 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4809 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6716 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9481 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    22350 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003     4085 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/purge_config.py
+-rw-rw-r--   0 root         (0)     1003    10788 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003     2396 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     9031 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    40476 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27718 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3436 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.921343 google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     4587 2023-07-05 15:52:32.000000 google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    10665 2023-07-05 15:52:32.000000 google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:32.000000 google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:32.000000 google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:32.000000 google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:52:32.000000 google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:32.000000 google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:52:32.925343 google-cloud-discoveryengine-0.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.921343 google-cloud-discoveryengine-0.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.921343 google-cloud-discoveryengine-0.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.921343 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.921343 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83160 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   200236 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003   167949 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    93286 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119289 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:32.925343 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83584 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   200684 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003    86195 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003   168397 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    94402 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119544 2023-07-05 15:46:58.000000 google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
```

### Comparing `google-cloud-discoveryengine-0.9.0/LICENSE` & `google-cloud-discoveryengine-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/MANIFEST.in` & `google-cloud-discoveryengine-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/PKG-INFO` & `google-cloud-discoveryengine-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.9.0
+Version: 0.9.1
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.9.0/README.rst` & `google-cloud-discoveryengine-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine/gapic_version.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.9.0"  # {x-release-please-version}
+__version__ = "0.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/gapic_metadata.json` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/gapic_version.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.9.0"  # {x-release-please-version}
+__version__ = "0.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CompletionServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1134,15 +1134,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DocumentServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -925,15 +925,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "SchemaServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/pagers.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "SearchServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/pagers.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,15 +664,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "UserEventServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/common.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/completion_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/document.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/document_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/import_config.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/import_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/purge_config.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/purge_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/schema.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/schema_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/search_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/user_event.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/user_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1/types/user_event_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1/types/user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/gapic_version.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.9.0"  # {x-release-please-version}
+__version__ = "0.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CompletionServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1137,15 +1137,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DocumentServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,15 +413,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RecommendationServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -925,15 +925,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "SchemaServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "SearchServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,15 +664,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "UserEventServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/__init__.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/common.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/completion_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/document.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/document_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/import_config.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/import_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/purge_config.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/purge_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/schema.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/schema_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/search_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/user_event.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/user_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py` & `google-cloud-discoveryengine-0.9.1/google/cloud/discoveryengine_v1beta/types/user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/PKG-INFO` & `google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.9.0
+Version: 0.9.1
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.9.0/google_cloud_discoveryengine.egg-info/SOURCES.txt` & `google-cloud-discoveryengine-0.9.1/google_cloud_discoveryengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/setup.py` & `google-cloud-discoveryengine-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/__init__.py` & `google-cloud-discoveryengine-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/__init__.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/__init__.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/__init__.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_completion_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_document_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,27 +50,27 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.discoveryengine_v1.services.document_service import (
+from google.cloud.discoveryengine_v1beta.services.document_service import (
     DocumentServiceAsyncClient,
     DocumentServiceClient,
     pagers,
     transports,
 )
-from google.cloud.discoveryengine_v1.types import (
+from google.cloud.discoveryengine_v1beta.types import (
     document_service,
     import_config,
     purge_config,
 )
-from google.cloud.discoveryengine_v1.types import document
-from google.cloud.discoveryengine_v1.types import document as gcd_document
+from google.cloud.discoveryengine_v1beta.types import document
+from google.cloud.discoveryengine_v1beta.types import document as gcd_document
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -654,15 +654,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_document_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.discoveryengine_v1.services.document_service.transports.DocumentServiceGrpcTransport.__init__"
+        "google.cloud.discoveryengine_v1beta.services.document_service.transports.DocumentServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = DocumentServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -765,21 +765,15 @@
     with mock.patch.object(type(client.transport.get_document), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
         response = client.get_document(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == document_service.GetDocumentRequest()
@@ -1399,17 +1393,19 @@
                     document.Document(),
                     document.Document(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_documents(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1432,21 +1428,15 @@
     with mock.patch.object(type(client.transport.create_document), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcd_document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
         response = client.create_document(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == document_service.CreateDocumentRequest()
@@ -1751,21 +1741,15 @@
     with mock.patch.object(type(client.transport.update_document), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
         response = client.update_document(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == document_service.UpdateDocumentRequest()
@@ -2428,21 +2412,15 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = document.Document.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -2659,15 +2637,15 @@
         client.get_document(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/dataStores/*/branches/*/documents/*}"
+            "%s/v1beta/{name=projects/*/locations/*/dataStores/*/branches/*/documents/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_document_rest_flattened_error(transport: str = "rest"):
     client = DocumentServiceClient(
@@ -2948,15 +2926,15 @@
         client.list_documents(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents"
+            "%s/v1beta/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_documents_rest_flattened_error(transport: str = "rest"):
     client = DocumentServiceClient(
@@ -3075,21 +3053,15 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcd_document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcd_document.Document.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3357,15 +3329,15 @@
         client.create_document(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents"
+            "%s/v1beta/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_document_rest_flattened_error(transport: str = "rest"):
     client = DocumentServiceClient(
@@ -3437,21 +3409,15 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = document.Document.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3883,15 +3849,15 @@
         client.delete_document(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/dataStores/*/branches/*/documents/*}"
+            "%s/v1beta/{name=projects/*/locations/*/dataStores/*/branches/*/documents/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_document_rest_flattened_error(transport: str = "rest"):
     client = DocumentServiceClient(
@@ -4477,15 +4443,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_document_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.discoveryengine_v1.services.document_service.transports.DocumentServiceTransport.__init__"
+        "google.cloud.discoveryengine_v1beta.services.document_service.transports.DocumentServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.DocumentServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -4523,15 +4489,15 @@
 
 
 def test_document_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.discoveryengine_v1.services.document_service.transports.DocumentServiceTransport._prep_wrapped_messages"
+        "google.cloud.discoveryengine_v1beta.services.document_service.transports.DocumentServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.DocumentServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -4542,15 +4508,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_document_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.discoveryengine_v1.services.document_service.transports.DocumentServiceTransport._prep_wrapped_messages"
+        "google.cloud.discoveryengine_v1beta.services.document_service.transports.DocumentServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.DocumentServiceTransport()
         adc.assert_called_once()
 
 
@@ -5172,15 +5138,18 @@
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     request = request_type()
     request = json_format.ParseDict(
-        {"name": "projects/sample1/operations/sample2"}, request
+        {
+            "name": "projects/sample1/locations/sample2/collections/sample3/dataStores/sample4/branches/sample5/operations/sample6"
+        },
+        request,
     )
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
         # Wrap the value into a proper Response obj
@@ -5199,15 +5168,17 @@
     ],
 )
 def test_get_operation_rest(request_type):
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="rest",
     )
-    request_init = {"name": "projects/sample1/operations/sample2"}
+    request_init = {
+        "name": "projects/sample1/locations/sample2/collections/sample3/dataStores/sample4/branches/sample5/operations/sample6"
+    }
     request = request_type(**request_init)
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation()
 
         # Wrap the value into a proper Response obj
@@ -5229,15 +5200,20 @@
 ):
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     request = request_type()
-    request = json_format.ParseDict({"name": "projects/sample1"}, request)
+    request = json_format.ParseDict(
+        {
+            "name": "projects/sample1/locations/sample2/collections/sample3/dataStores/sample4/branches/sample5"
+        },
+        request,
+    )
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
         # Wrap the value into a proper Response obj
         response_value = Response()
@@ -5255,15 +5231,17 @@
     ],
 )
 def test_list_operations_rest(request_type):
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="rest",
     )
-    request_init = {"name": "projects/sample1"}
+    request_init = {
+        "name": "projects/sample1/locations/sample2/collections/sample3/dataStores/sample4/branches/sample5"
+    }
     request = request_type(**request_init)
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.ListOperationsResponse()
 
         # Wrap the value into a proper Response obj
```

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_schema_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_schema_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -734,21 +734,15 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_schema), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = schema.Schema(
             name="name_value",
-            struct_schema=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_schema="json_schema_value",
         )
         response = client.get_schema(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == schema_service.GetSchemaRequest()
@@ -1359,17 +1353,19 @@
                     schema.Schema(),
                     schema.Schema(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_schemas(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2055,21 +2051,15 @@
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = schema.Schema(
             name="name_value",
-            struct_schema=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_schema="json_schema_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = schema.Schema.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_search_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_search_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1046,14 +1046,16 @@
                     search_service.SearchResponse.SearchResult(),
                     search_service.SearchResponse.SearchResult(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
         async for page_ in (await client.search(request={})).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
```

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1/test_document_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,27 +50,27 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.discoveryengine_v1beta.services.document_service import (
+from google.cloud.discoveryengine_v1.services.document_service import (
     DocumentServiceAsyncClient,
     DocumentServiceClient,
     pagers,
     transports,
 )
-from google.cloud.discoveryengine_v1beta.types import (
+from google.cloud.discoveryengine_v1.types import (
     document_service,
     import_config,
     purge_config,
 )
-from google.cloud.discoveryengine_v1beta.types import document
-from google.cloud.discoveryengine_v1beta.types import document as gcd_document
+from google.cloud.discoveryengine_v1.types import document
+from google.cloud.discoveryengine_v1.types import document as gcd_document
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -654,15 +654,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_document_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.discoveryengine_v1beta.services.document_service.transports.DocumentServiceGrpcTransport.__init__"
+        "google.cloud.discoveryengine_v1.services.document_service.transports.DocumentServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = DocumentServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -765,21 +765,15 @@
     with mock.patch.object(type(client.transport.get_document), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
         response = client.get_document(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == document_service.GetDocumentRequest()
@@ -1399,17 +1393,19 @@
                     document.Document(),
                     document.Document(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_documents(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1432,21 +1428,15 @@
     with mock.patch.object(type(client.transport.create_document), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gcd_document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
         response = client.create_document(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == document_service.CreateDocumentRequest()
@@ -1751,21 +1741,15 @@
     with mock.patch.object(type(client.transport.update_document), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
         response = client.update_document(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == document_service.UpdateDocumentRequest()
@@ -2428,21 +2412,15 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = document.Document.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -2659,15 +2637,15 @@
         client.get_document(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/dataStores/*/branches/*/documents/*}"
+            "%s/v1/{name=projects/*/locations/*/dataStores/*/branches/*/documents/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_document_rest_flattened_error(transport: str = "rest"):
     client = DocumentServiceClient(
@@ -2948,15 +2926,15 @@
         client.list_documents(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents"
+            "%s/v1/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_documents_rest_flattened_error(transport: str = "rest"):
     client = DocumentServiceClient(
@@ -3075,21 +3053,15 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcd_document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gcd_document.Document.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3357,15 +3329,15 @@
         client.create_document(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents"
+            "%s/v1/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_document_rest_flattened_error(transport: str = "rest"):
     client = DocumentServiceClient(
@@ -3437,21 +3409,15 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = document.Document(
             name="name_value",
             id="id_value",
             schema_id="schema_id_value",
             parent_document_id="parent_document_id_value",
-            struct_data=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_data="json_data_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = document.Document.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3883,15 +3849,15 @@
         client.delete_document(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/dataStores/*/branches/*/documents/*}"
+            "%s/v1/{name=projects/*/locations/*/dataStores/*/branches/*/documents/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_document_rest_flattened_error(transport: str = "rest"):
     client = DocumentServiceClient(
@@ -4477,15 +4443,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_document_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.discoveryengine_v1beta.services.document_service.transports.DocumentServiceTransport.__init__"
+        "google.cloud.discoveryengine_v1.services.document_service.transports.DocumentServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.DocumentServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -4523,15 +4489,15 @@
 
 
 def test_document_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.discoveryengine_v1beta.services.document_service.transports.DocumentServiceTransport._prep_wrapped_messages"
+        "google.cloud.discoveryengine_v1.services.document_service.transports.DocumentServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.DocumentServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -4542,15 +4508,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_document_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.discoveryengine_v1beta.services.document_service.transports.DocumentServiceTransport._prep_wrapped_messages"
+        "google.cloud.discoveryengine_v1.services.document_service.transports.DocumentServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.DocumentServiceTransport()
         adc.assert_called_once()
 
 
@@ -5172,18 +5138,15 @@
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     request = request_type()
     request = json_format.ParseDict(
-        {
-            "name": "projects/sample1/locations/sample2/collections/sample3/dataStores/sample4/branches/sample5/operations/sample6"
-        },
-        request,
+        {"name": "projects/sample1/operations/sample2"}, request
     )
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
         # Wrap the value into a proper Response obj
@@ -5202,17 +5165,15 @@
     ],
 )
 def test_get_operation_rest(request_type):
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="rest",
     )
-    request_init = {
-        "name": "projects/sample1/locations/sample2/collections/sample3/dataStores/sample4/branches/sample5/operations/sample6"
-    }
+    request_init = {"name": "projects/sample1/operations/sample2"}
     request = request_type(**request_init)
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation()
 
         # Wrap the value into a proper Response obj
@@ -5234,20 +5195,15 @@
 ):
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     request = request_type()
-    request = json_format.ParseDict(
-        {
-            "name": "projects/sample1/locations/sample2/collections/sample3/dataStores/sample4/branches/sample5"
-        },
-        request,
-    )
+    request = json_format.ParseDict({"name": "projects/sample1"}, request)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
         # Wrap the value into a proper Response obj
         response_value = Response()
@@ -5265,17 +5221,15 @@
     ],
 )
 def test_list_operations_rest(request_type):
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="rest",
     )
-    request_init = {
-        "name": "projects/sample1/locations/sample2/collections/sample3/dataStores/sample4/branches/sample5"
-    }
+    request_init = {"name": "projects/sample1"}
     request = request_type(**request_init)
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.ListOperationsResponse()
 
         # Wrap the value into a proper Response obj
```

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,21 +734,15 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_schema), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = schema.Schema(
             name="name_value",
-            struct_schema=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_schema="json_schema_value",
         )
         response = client.get_schema(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == schema_service.GetSchemaRequest()
@@ -1359,17 +1353,19 @@
                     schema.Schema(),
                     schema.Schema(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_schemas(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2055,21 +2051,15 @@
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = schema.Schema(
             name="name_value",
-            struct_schema=struct_pb2.Struct(
-                fields={
-                    "key_value": struct_pb2.Value(
-                        null_value=struct_pb2.NullValue.NULL_VALUE
-                    )
-                }
-            ),
+            json_schema="json_schema_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = schema.Schema.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1054,14 +1054,16 @@
                     search_service.SearchResponse.SearchResult(),
                     search_service.SearchResponse.SearchResult(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
         async for page_ in (await client.search(request={})).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
```

### Comparing `google-cloud-discoveryengine-0.9.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py` & `google-cloud-discoveryengine-0.9.1/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py`

 * *Files identical despite different names*

