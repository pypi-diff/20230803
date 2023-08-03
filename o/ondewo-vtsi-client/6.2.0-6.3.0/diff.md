# Comparing `tmp/ondewo-vtsi-client-6.2.0.tar.gz` & `tmp/ondewo-vtsi-client-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-vtsi-client-6.2.0.tar", last modified: Sun May 21 21:03:21 2023, max compression
+gzip compressed data, was "ondewo-vtsi-client-6.3.0.tar", last modified: Thu Aug  3 17:12:42 2023, max compression
```

## Comparing `ondewo-vtsi-client-6.2.0.tar` & `ondewo-vtsi-client-6.3.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8516 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.461773 ondewo-vtsi-client-6.2.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.464773 ondewo-vtsi-client-6.2.0/ondewo/nlu/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    73579 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/agent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    87204 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/agent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    28729 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/aiservices_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16826 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/aiservices_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     1600 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/common_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/common_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    10375 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/context_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14789 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/context_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    29954 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/entity_type_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    36069 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/entity_type_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    72044 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/intent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59591 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/intent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3366 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/operation_metadata_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/operation_metadata_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7908 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/operations_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    11374 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/operations_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     9554 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/project_role_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    10478 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/project_role_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7470 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/project_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16562 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/project_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3009 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/server_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6634 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/server_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    66065 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/session_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59122 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/session_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    19689 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/user_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    27124 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/user_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    20239 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/utility_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16902 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/utility_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     6369 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/webhook_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6508 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/webhook_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.465772 ondewo-vtsi-client-6.2.0/ondewo/qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/qa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11457 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/qa/qa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    13389 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/qa/qa_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.465772 ondewo-vtsi-client-6.2.0/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/s2t/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38634 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    30933 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.465772 ondewo-vtsi-client-6.2.0/ondewo/sip/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/sip/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11001 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/sip/sip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    21323 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/sip/sip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.466772 ondewo-vtsi-client-6.2.0/ondewo/t2s/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/t2s/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31414 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/t2s/text_to_speech_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    33144 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/t2s/text_to_speech_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.466772 ondewo-vtsi-client-6.2.0/ondewo/vtsi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    42878 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/calls_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    29068 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/calls_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      735 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      263 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3734 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/calls.py
--rw-rw-r--   0 root         (0) root         (0)     2153 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/projects.py
--rw-rw-r--   0 root         (0) root         (0)      317 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    13169 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/projects_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    12545 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/projects_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-05-21 21:03:21.468772 ondewo-vtsi-client-6.2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1586 2023-05-21 21:03:09.000000 ondewo-vtsi-client-6.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.880974 ondewo-vtsi-client-6.3.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-08-03 17:12:42.881974 ondewo-vtsi-client-6.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8516 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.875974 ondewo-vtsi-client-6.3.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.878974 ondewo-vtsi-client-6.3.0/ondewo/nlu/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    73267 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/agent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    87204 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/agent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    28593 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/aiservices_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16826 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/aiservices_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     1592 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/common_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    10331 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/context_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14789 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/context_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    29810 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/entity_type_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    36069 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/entity_type_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    71700 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/intent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59591 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/intent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3354 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/operation_metadata_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/operation_metadata_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7876 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/operations_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11374 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     9514 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/project_role_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    10478 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/project_role_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7450 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/project_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16562 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/project_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3001 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/server_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6634 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/server_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    65793 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/session_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59122 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/session_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    19597 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/user_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    27124 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/user_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    20143 2023-08-03 17:11:23.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/utility_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16902 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/utility_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     6345 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/webhook_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6508 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/nlu/webhook_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.878974 ondewo-vtsi-client-6.3.0/ondewo/qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11401 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/qa/qa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    13389 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/qa/qa_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.879974 ondewo-vtsi-client-6.3.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/s2t/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38422 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    30933 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.879974 ondewo-vtsi-client-6.3.0/ondewo/sip/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/sip/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10949 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/sip/sip_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    21323 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/sip/sip_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.879974 ondewo-vtsi-client-6.3.0/ondewo/t2s/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/t2s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31234 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/t2s/text_to_speech_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    33144 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/t2s/text_to_speech_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.880974 ondewo-vtsi-client-6.3.0/ondewo/vtsi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    42646 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/calls_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    29068 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/calls_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.880974 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      735 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.880974 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3734 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/services/calls.py
+-rw-rw-r--   0 root         (0) root         (0)     2153 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/services/projects.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-08-03 17:10:17.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    17004 2023-08-03 17:11:22.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/projects_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14451 2023-08-03 17:11:21.000000 ondewo-vtsi-client-6.3.0/ondewo/vtsi/projects_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 17:12:42.880974 ondewo-vtsi-client-6.3.0/ondewo_vtsi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-08-03 17:12:42.000000 ondewo-vtsi-client-6.3.0/ondewo_vtsi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-08-03 17:12:42.000000 ondewo-vtsi-client-6.3.0/ondewo_vtsi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 17:12:42.000000 ondewo-vtsi-client-6.3.0/ondewo_vtsi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2023-08-03 17:12:42.000000 ondewo-vtsi-client-6.3.0/ondewo_vtsi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-03 17:12:42.000000 ondewo-vtsi-client-6.3.0/ondewo_vtsi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-08-03 17:12:42.881974 ondewo-vtsi-client-6.3.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1586 2023-08-03 17:11:25.000000 ondewo-vtsi-client-6.3.0/setup.py
```

### Comparing `ondewo-vtsi-client-6.2.0/LICENSE` & `ondewo-vtsi-client-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/PKG-INFO` & `ondewo-vtsi-client-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.2.0
+Version: 6.3.0
 Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.2.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.3.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.2.0/README.md` & `ondewo-vtsi-client-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/agent_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/agent_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -676,164 +676,164 @@
     _AGENTS.methods_by_name['SetAgentStatus']._serialized_options = b'\202\323\344\223\002)\"$/v2/{parent=projects/*/agent}:status:\001*'
     _AGENTS.methods_by_name['SetResources']._options = None
     _AGENTS.methods_by_name['SetResources']._serialized_options = b'\202\323\344\223\002,\"\'/v2/{parent=projects/*/agent}:resources:\001*'
     _AGENTS.methods_by_name['DeleteResources']._options = None
     _AGENTS.methods_by_name['DeleteResources']._serialized_options = b'\202\323\344\223\002)*\'/v2/{parent=projects/*/agent}:resources'
     _AGENTS.methods_by_name['ExportResources']._options = None
     _AGENTS.methods_by_name['ExportResources']._serialized_options = b'\202\323\344\223\002,\"\'/v2/{parent=projects/*/agent}:resources:\001*'
-    _AGENTVIEW._serialized_start = 10464
-    _AGENTVIEW._serialized_end = 10572
-    _INITIATIONPROTOCOL._serialized_start = 10574
-    _INITIATIONPROTOCOL._serialized_end = 10648
-    _REPORTTYPE._serialized_start = 10650
-    _REPORTTYPE._serialized_end = 10763
-    _SESSIONSREPORTTYPE._serialized_start = 10766
-    _SESSIONSREPORTTYPE._serialized_end = 11272
-    _REPORTFORMAT._serialized_start = 11274
-    _REPORTFORMAT._serialized_end = 11317
-    _AGENTSTATUS._serialized_start = 11319
-    _AGENTSTATUS._serialized_end = 11358
-    _AGENT._serialized_start = 354
-    _AGENT._serialized_end = 627
-    _AGENTWITHOWNER._serialized_start = 629
-    _AGENTWITHOWNER._serialized_end = 712
-    _AGENTOFUSERWITHOWNER._serialized_start = 714
-    _AGENTOFUSERWITHOWNER._serialized_end = 837
-    _CREATEAGENTREQUEST._serialized_start = 839
-    _CREATEAGENTREQUEST._serialized_end = 936
-    _UPDATEAGENTREQUEST._serialized_start = 939
-    _UPDATEAGENTREQUEST._serialized_end = 1085
-    _DELETEAGENTREQUEST._serialized_start = 1087
-    _DELETEAGENTREQUEST._serialized_end = 1123
-    _GETAGENTREQUEST._serialized_start = 1125
-    _GETAGENTREQUEST._serialized_end = 1201
-    _LISTAGENTSREQUEST._serialized_start = 1204
-    _LISTAGENTSREQUEST._serialized_end = 1335
-    _LISTAGENTSRESPONSE._serialized_start = 1337
-    _LISTAGENTSRESPONSE._serialized_end = 1438
-    _LISTAGENTSOFUSERRESPONSE._serialized_start = 1440
-    _LISTAGENTSOFUSERRESPONSE._serialized_end = 1561
-    _TRAINAGENTREQUEST._serialized_start = 1563
-    _TRAINAGENTREQUEST._serialized_end = 1675
-    _BUILDCACHEREQUEST._serialized_start = 1677
-    _BUILDCACHEREQUEST._serialized_end = 1728
-    _EXPORTAGENTREQUEST._serialized_start = 1730
-    _EXPORTAGENTREQUEST._serialized_end = 1812
-    _EXPORTAGENTRESPONSE._serialized_start = 1814
-    _EXPORTAGENTRESPONSE._serialized_end = 1890
-    _EXPORTBENCHMARKAGENTREQUEST._serialized_start = 1893
-    _EXPORTBENCHMARKAGENTREQUEST._serialized_end = 2026
-    _EXPORTBENCHMARKAGENTRESPONSE._serialized_start = 2029
-    _EXPORTBENCHMARKAGENTRESPONSE._serialized_end = 2268
-    _EXPORTBENCHMARKAGENTRESPONSE_TRAININGPHRASESENTRY._serialized_start = 2173
-    _EXPORTBENCHMARKAGENTRESPONSE_TRAININGPHRASESENTRY._serialized_end = 2268
-    _OPTIMIZERANKINGMATCHREQUEST._serialized_start = 2271
-    _OPTIMIZERANKINGMATCHREQUEST._serialized_end = 2432
-    _RANKINGMATCHOPTIMIZATIONCONFIG._serialized_start = 2435
-    _RANKINGMATCHOPTIMIZATIONCONFIG._serialized_end = 2582
-    _OPTIMIZERANKINGMATCHRESPONSE._serialized_start = 2585
-    _OPTIMIZERANKINGMATCHRESPONSE._serialized_end = 2725
-    _IMPORTAGENTREQUEST._serialized_start = 2727
-    _IMPORTAGENTREQUEST._serialized_end = 2818
-    _RESTOREAGENTREQUEST._serialized_start = 2820
-    _RESTOREAGENTREQUEST._serialized_end = 2912
-    _GETAGENTSTATISTICSREQUEST._serialized_start = 2915
-    _GETAGENTSTATISTICSREQUEST._serialized_end = 3061
-    _GETAGENTSTATISTICSRESPONSE._serialized_start = 3063
-    _GETAGENTSTATISTICSRESPONSE._serialized_end = 3188
-    _GETSESSIONSSTATISTICSREQUEST._serialized_start = 3191
-    _GETSESSIONSSTATISTICSREQUEST._serialized_end = 3548
-    _GETSESSIONSSTATISTICSRESPONSE._serialized_start = 3551
-    _GETSESSIONSSTATISTICSRESPONSE._serialized_end = 3687
-    _ADDUSERTOPROJECTREQUEST._serialized_start = 3689
-    _ADDUSERTOPROJECTREQUEST._serialized_end = 3772
-    _REMOVEUSERFROMPROJECTREQUEST._serialized_start = 3774
-    _REMOVEUSERFROMPROJECTREQUEST._serialized_end = 3837
-    _LISTUSERSINPROJECTREQUEST._serialized_start = 3839
-    _LISTUSERSINPROJECTREQUEST._serialized_end = 3902
-    _USERINPROJECT._serialized_start = 3904
-    _USERINPROJECT._serialized_end = 3984
-    _LISTUSERSINPROJECTRESPONSE._serialized_start = 3986
-    _LISTUSERSINPROJECTRESPONSE._serialized_end = 4081
-    _GETPLATFORMINFORESPONSE._serialized_start = 4083
-    _GETPLATFORMINFORESPONSE._serialized_end = 4146
-    _LISTPROJECTPERMISSIONSREQUEST._serialized_start = 4148
-    _LISTPROJECTPERMISSIONSREQUEST._serialized_end = 4199
-    _LISTPROJECTPERMISSIONSRESPONSE._serialized_start = 4201
-    _LISTPROJECTPERMISSIONSRESPONSE._serialized_end = 4279
-    _SETAGENTSTATUSREQUEST._serialized_start = 4281
-    _SETAGENTSTATUSREQUEST._serialized_end = 4404
-    _AGENTSORTING._serialized_start = 4407
-    _AGENTSORTING._serialized_end = 4698
-    _AGENTSORTING_AGENTSORTINGFIELD._serialized_start = 4538
-    _AGENTSORTING_AGENTSORTINGFIELD._serialized_end = 4698
-    _SETRESOURCESREQUEST._serialized_start = 4700
-    _SETRESOURCESREQUEST._serialized_end = 4811
-    _DELETERESOURCESREQUEST._serialized_start = 4813
-    _DELETERESOURCESREQUEST._serialized_end = 4904
-    _EXPORTRESOURCESREQUEST._serialized_start = 4906
-    _EXPORTRESOURCESREQUEST._serialized_end = 4997
-    _EXPORTRESOURCESRESPONSE._serialized_start = 4999
-    _EXPORTRESOURCESRESPONSE._serialized_end = 5114
-    _GETMODELSTATUSESREQUEST._serialized_start = 5116
-    _GETMODELSTATUSESREQUEST._serialized_end = 5223
-    _MODELSTATUS._serialized_start = 5226
-    _MODELSTATUS._serialized_end = 5546
-    _MODELSTATUS_STATUSNAME._serialized_start = 5428
-    _MODELSTATUS_STATUSNAME._serialized_end = 5546
-    _GETMODELSTATUSESRESPONSE._serialized_start = 5548
-    _GETMODELSTATUSESRESPONSE._serialized_end = 5623
-    _CUSTOMPLATFORMINFO._serialized_start = 5625
-    _CUSTOMPLATFORMINFO._serialized_end = 5740
-    _GETPLATFORMMAPPINGREQUEST._serialized_start = 5742
-    _GETPLATFORMMAPPINGREQUEST._serialized_end = 5785
-    _PLATFORMMAPPING._serialized_start = 5787
-    _PLATFORMMAPPING._serialized_end = 5875
-    _FULLTEXTSEARCHREQUEST._serialized_start = 5878
-    _FULLTEXTSEARCHREQUEST._serialized_end = 6287
-    _FULLTEXTSEARCHREQUEST_QUERYTYPE._serialized_start = 5977
-    _FULLTEXTSEARCHREQUEST_QUERYTYPE._serialized_end = 6287
-    _FULLTEXTSEARCHRESPONSEENTITYTYPE._serialized_start = 6290
-    _FULLTEXTSEARCHRESPONSEENTITYTYPE._serialized_end = 6617
-    _FULLTEXTSEARCHRESPONSEENTITYTYPE_ENTITYTYPESEARCHRESULT._serialized_start = 6539
-    _FULLTEXTSEARCHRESPONSEENTITYTYPE_ENTITYTYPESEARCHRESULT._serialized_end = 6617
-    _FULLTEXTSEARCHRESPONSEENTITY._serialized_start = 6620
-    _FULLTEXTSEARCHRESPONSEENTITY._serialized_end = 6987
-    _FULLTEXTSEARCHRESPONSEENTITY_ENTITYSEARCHRESULT._serialized_start = 6853
-    _FULLTEXTSEARCHRESPONSEENTITY_ENTITYSEARCHRESULT._serialized_end = 6987
-    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM._serialized_start = 6990
-    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM._serialized_end = 7443
-    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM_ENTITYSYNONYMSEARCHRESULT._serialized_start = 7252
-    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM_ENTITYSYNONYMSEARCHRESULT._serialized_end = 7443
-    _FULLTEXTSEARCHRESPONSEINTENT._serialized_start = 7446
-    _FULLTEXTSEARCHRESPONSEINTENT._serialized_end = 7787
-    _FULLTEXTSEARCHRESPONSEINTENT_INTENTSEARCHRESULT._serialized_start = 7678
-    _FULLTEXTSEARCHRESPONSEINTENT_INTENTSEARCHRESULT._serialized_end = 7787
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN._serialized_start = 7790
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN._serialized_end = 8185
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN_INTENTCONTEXTINSEARCHRESULT._serialized_start = 8060
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN_INTENTCONTEXTINSEARCHRESULT._serialized_end = 8185
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT._serialized_start = 8188
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT._serialized_end = 8588
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT_INTENTCONTEXTOUTSEARCHRESULT._serialized_start = 8462
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT_INTENTCONTEXTOUTSEARCHRESULT._serialized_end = 8588
-    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS._serialized_start = 8591
-    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS._serialized_end = 9070
-    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS_INTENTUSERSAYSSEARCHRESULT._serialized_start = 8857
-    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS_INTENTUSERSAYSSEARCHRESULT._serialized_end = 9070
-    _FULLTEXTSEARCHRESPONSEINTENTTAGS._serialized_start = 9073
-    _FULLTEXTSEARCHRESPONSEINTENTTAGS._serialized_end = 9457
-    _FULLTEXTSEARCHRESPONSEINTENTTAGS_INTENTTAGSSEARCHRESULT._serialized_start = 9323
-    _FULLTEXTSEARCHRESPONSEINTENTTAGS_INTENTTAGSSEARCHRESULT._serialized_end = 9457
-    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE._serialized_start = 9460
-    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE._serialized_end = 9891
-    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE_INTENTRESPONSESEARCHRESULT._serialized_start = 9726
-    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE_INTENTRESPONSESEARCHRESULT._serialized_end = 9891
-    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS._serialized_start = 9894
-    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS._serialized_end = 10336
-    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS_INTENTPARAMETERSSEARCHRESULT._serialized_start = 10168
-    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS_INTENTPARAMETERSSEARCHRESULT._serialized_end = 10336
-    _REINDEXAGENTREQUEST._serialized_start = 10338
-    _REINDEXAGENTREQUEST._serialized_end = 10462
-    _AGENTS._serialized_start = 11361
-    _AGENTS._serialized_end = 16111
+    _AGENTVIEW._serialized_start=10464
+    _AGENTVIEW._serialized_end=10572
+    _INITIATIONPROTOCOL._serialized_start=10574
+    _INITIATIONPROTOCOL._serialized_end=10648
+    _REPORTTYPE._serialized_start=10650
+    _REPORTTYPE._serialized_end=10763
+    _SESSIONSREPORTTYPE._serialized_start=10766
+    _SESSIONSREPORTTYPE._serialized_end=11272
+    _REPORTFORMAT._serialized_start=11274
+    _REPORTFORMAT._serialized_end=11317
+    _AGENTSTATUS._serialized_start=11319
+    _AGENTSTATUS._serialized_end=11358
+    _AGENT._serialized_start=354
+    _AGENT._serialized_end=627
+    _AGENTWITHOWNER._serialized_start=629
+    _AGENTWITHOWNER._serialized_end=712
+    _AGENTOFUSERWITHOWNER._serialized_start=714
+    _AGENTOFUSERWITHOWNER._serialized_end=837
+    _CREATEAGENTREQUEST._serialized_start=839
+    _CREATEAGENTREQUEST._serialized_end=936
+    _UPDATEAGENTREQUEST._serialized_start=939
+    _UPDATEAGENTREQUEST._serialized_end=1085
+    _DELETEAGENTREQUEST._serialized_start=1087
+    _DELETEAGENTREQUEST._serialized_end=1123
+    _GETAGENTREQUEST._serialized_start=1125
+    _GETAGENTREQUEST._serialized_end=1201
+    _LISTAGENTSREQUEST._serialized_start=1204
+    _LISTAGENTSREQUEST._serialized_end=1335
+    _LISTAGENTSRESPONSE._serialized_start=1337
+    _LISTAGENTSRESPONSE._serialized_end=1438
+    _LISTAGENTSOFUSERRESPONSE._serialized_start=1440
+    _LISTAGENTSOFUSERRESPONSE._serialized_end=1561
+    _TRAINAGENTREQUEST._serialized_start=1563
+    _TRAINAGENTREQUEST._serialized_end=1675
+    _BUILDCACHEREQUEST._serialized_start=1677
+    _BUILDCACHEREQUEST._serialized_end=1728
+    _EXPORTAGENTREQUEST._serialized_start=1730
+    _EXPORTAGENTREQUEST._serialized_end=1812
+    _EXPORTAGENTRESPONSE._serialized_start=1814
+    _EXPORTAGENTRESPONSE._serialized_end=1890
+    _EXPORTBENCHMARKAGENTREQUEST._serialized_start=1893
+    _EXPORTBENCHMARKAGENTREQUEST._serialized_end=2026
+    _EXPORTBENCHMARKAGENTRESPONSE._serialized_start=2029
+    _EXPORTBENCHMARKAGENTRESPONSE._serialized_end=2268
+    _EXPORTBENCHMARKAGENTRESPONSE_TRAININGPHRASESENTRY._serialized_start=2173
+    _EXPORTBENCHMARKAGENTRESPONSE_TRAININGPHRASESENTRY._serialized_end=2268
+    _OPTIMIZERANKINGMATCHREQUEST._serialized_start=2271
+    _OPTIMIZERANKINGMATCHREQUEST._serialized_end=2432
+    _RANKINGMATCHOPTIMIZATIONCONFIG._serialized_start=2435
+    _RANKINGMATCHOPTIMIZATIONCONFIG._serialized_end=2582
+    _OPTIMIZERANKINGMATCHRESPONSE._serialized_start=2585
+    _OPTIMIZERANKINGMATCHRESPONSE._serialized_end=2725
+    _IMPORTAGENTREQUEST._serialized_start=2727
+    _IMPORTAGENTREQUEST._serialized_end=2818
+    _RESTOREAGENTREQUEST._serialized_start=2820
+    _RESTOREAGENTREQUEST._serialized_end=2912
+    _GETAGENTSTATISTICSREQUEST._serialized_start=2915
+    _GETAGENTSTATISTICSREQUEST._serialized_end=3061
+    _GETAGENTSTATISTICSRESPONSE._serialized_start=3063
+    _GETAGENTSTATISTICSRESPONSE._serialized_end=3188
+    _GETSESSIONSSTATISTICSREQUEST._serialized_start=3191
+    _GETSESSIONSSTATISTICSREQUEST._serialized_end=3548
+    _GETSESSIONSSTATISTICSRESPONSE._serialized_start=3551
+    _GETSESSIONSSTATISTICSRESPONSE._serialized_end=3687
+    _ADDUSERTOPROJECTREQUEST._serialized_start=3689
+    _ADDUSERTOPROJECTREQUEST._serialized_end=3772
+    _REMOVEUSERFROMPROJECTREQUEST._serialized_start=3774
+    _REMOVEUSERFROMPROJECTREQUEST._serialized_end=3837
+    _LISTUSERSINPROJECTREQUEST._serialized_start=3839
+    _LISTUSERSINPROJECTREQUEST._serialized_end=3902
+    _USERINPROJECT._serialized_start=3904
+    _USERINPROJECT._serialized_end=3984
+    _LISTUSERSINPROJECTRESPONSE._serialized_start=3986
+    _LISTUSERSINPROJECTRESPONSE._serialized_end=4081
+    _GETPLATFORMINFORESPONSE._serialized_start=4083
+    _GETPLATFORMINFORESPONSE._serialized_end=4146
+    _LISTPROJECTPERMISSIONSREQUEST._serialized_start=4148
+    _LISTPROJECTPERMISSIONSREQUEST._serialized_end=4199
+    _LISTPROJECTPERMISSIONSRESPONSE._serialized_start=4201
+    _LISTPROJECTPERMISSIONSRESPONSE._serialized_end=4279
+    _SETAGENTSTATUSREQUEST._serialized_start=4281
+    _SETAGENTSTATUSREQUEST._serialized_end=4404
+    _AGENTSORTING._serialized_start=4407
+    _AGENTSORTING._serialized_end=4698
+    _AGENTSORTING_AGENTSORTINGFIELD._serialized_start=4538
+    _AGENTSORTING_AGENTSORTINGFIELD._serialized_end=4698
+    _SETRESOURCESREQUEST._serialized_start=4700
+    _SETRESOURCESREQUEST._serialized_end=4811
+    _DELETERESOURCESREQUEST._serialized_start=4813
+    _DELETERESOURCESREQUEST._serialized_end=4904
+    _EXPORTRESOURCESREQUEST._serialized_start=4906
+    _EXPORTRESOURCESREQUEST._serialized_end=4997
+    _EXPORTRESOURCESRESPONSE._serialized_start=4999
+    _EXPORTRESOURCESRESPONSE._serialized_end=5114
+    _GETMODELSTATUSESREQUEST._serialized_start=5116
+    _GETMODELSTATUSESREQUEST._serialized_end=5223
+    _MODELSTATUS._serialized_start=5226
+    _MODELSTATUS._serialized_end=5546
+    _MODELSTATUS_STATUSNAME._serialized_start=5428
+    _MODELSTATUS_STATUSNAME._serialized_end=5546
+    _GETMODELSTATUSESRESPONSE._serialized_start=5548
+    _GETMODELSTATUSESRESPONSE._serialized_end=5623
+    _CUSTOMPLATFORMINFO._serialized_start=5625
+    _CUSTOMPLATFORMINFO._serialized_end=5740
+    _GETPLATFORMMAPPINGREQUEST._serialized_start=5742
+    _GETPLATFORMMAPPINGREQUEST._serialized_end=5785
+    _PLATFORMMAPPING._serialized_start=5787
+    _PLATFORMMAPPING._serialized_end=5875
+    _FULLTEXTSEARCHREQUEST._serialized_start=5878
+    _FULLTEXTSEARCHREQUEST._serialized_end=6287
+    _FULLTEXTSEARCHREQUEST_QUERYTYPE._serialized_start=5977
+    _FULLTEXTSEARCHREQUEST_QUERYTYPE._serialized_end=6287
+    _FULLTEXTSEARCHRESPONSEENTITYTYPE._serialized_start=6290
+    _FULLTEXTSEARCHRESPONSEENTITYTYPE._serialized_end=6617
+    _FULLTEXTSEARCHRESPONSEENTITYTYPE_ENTITYTYPESEARCHRESULT._serialized_start=6539
+    _FULLTEXTSEARCHRESPONSEENTITYTYPE_ENTITYTYPESEARCHRESULT._serialized_end=6617
+    _FULLTEXTSEARCHRESPONSEENTITY._serialized_start=6620
+    _FULLTEXTSEARCHRESPONSEENTITY._serialized_end=6987
+    _FULLTEXTSEARCHRESPONSEENTITY_ENTITYSEARCHRESULT._serialized_start=6853
+    _FULLTEXTSEARCHRESPONSEENTITY_ENTITYSEARCHRESULT._serialized_end=6987
+    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM._serialized_start=6990
+    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM._serialized_end=7443
+    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM_ENTITYSYNONYMSEARCHRESULT._serialized_start=7252
+    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM_ENTITYSYNONYMSEARCHRESULT._serialized_end=7443
+    _FULLTEXTSEARCHRESPONSEINTENT._serialized_start=7446
+    _FULLTEXTSEARCHRESPONSEINTENT._serialized_end=7787
+    _FULLTEXTSEARCHRESPONSEINTENT_INTENTSEARCHRESULT._serialized_start=7678
+    _FULLTEXTSEARCHRESPONSEINTENT_INTENTSEARCHRESULT._serialized_end=7787
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN._serialized_start=7790
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN._serialized_end=8185
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN_INTENTCONTEXTINSEARCHRESULT._serialized_start=8060
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN_INTENTCONTEXTINSEARCHRESULT._serialized_end=8185
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT._serialized_start=8188
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT._serialized_end=8588
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT_INTENTCONTEXTOUTSEARCHRESULT._serialized_start=8462
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT_INTENTCONTEXTOUTSEARCHRESULT._serialized_end=8588
+    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS._serialized_start=8591
+    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS._serialized_end=9070
+    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS_INTENTUSERSAYSSEARCHRESULT._serialized_start=8857
+    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS_INTENTUSERSAYSSEARCHRESULT._serialized_end=9070
+    _FULLTEXTSEARCHRESPONSEINTENTTAGS._serialized_start=9073
+    _FULLTEXTSEARCHRESPONSEINTENTTAGS._serialized_end=9457
+    _FULLTEXTSEARCHRESPONSEINTENTTAGS_INTENTTAGSSEARCHRESULT._serialized_start=9323
+    _FULLTEXTSEARCHRESPONSEINTENTTAGS_INTENTTAGSSEARCHRESULT._serialized_end=9457
+    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE._serialized_start=9460
+    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE._serialized_end=9891
+    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE_INTENTRESPONSESEARCHRESULT._serialized_start=9726
+    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE_INTENTRESPONSESEARCHRESULT._serialized_end=9891
+    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS._serialized_start=9894
+    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS._serialized_end=10336
+    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS_INTENTPARAMETERSSEARCHRESULT._serialized_start=10168
+    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS_INTENTPARAMETERSSEARCHRESULT._serialized_end=10336
+    _REINDEXAGENTREQUEST._serialized_start=10338
+    _REINDEXAGENTREQUEST._serialized_end=10462
+    _AGENTS._serialized_start=11361
+    _AGENTS._serialized_end=16111
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/agent_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/aiservices_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/aiservices_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -294,76 +294,76 @@
     _AISERVICES.methods_by_name['GetAlternativeSentences']._serialized_options = b'\202\323\344\223\002;\"6/v2/{parent=projects/*/agent}/get_alternative:sentence:\001*'
     _AISERVICES.methods_by_name['GetAlternativeTrainingPhrases']._options = None
     _AISERVICES.methods_by_name['GetAlternativeTrainingPhrases']._serialized_options = b'\202\323\344\223\002C\">/v2/{parent=projects/*/agent}/get_alternative:training_phrases:\001*'
     _AISERVICES.methods_by_name['GetSynonyms']._options = None
     _AISERVICES.methods_by_name['GetSynonyms']._serialized_options = b'\202\323\344\223\002/\"*/v2/{parent=projects/*/agent}/get_synonyms:\001*'
     _AISERVICES.methods_by_name['ClassifyIntents']._options = None
     _AISERVICES.methods_by_name['ClassifyIntents']._serialized_options = b'\202\323\344\223\0022\"-/v2/{parent=projects/*/agent}/classify_intent:\001*'
-    _MODE._serialized_start = 4135
-    _MODE._serialized_end = 4188
-    _INTENTALGORITHMS._serialized_start = 4191
-    _INTENTALGORITHMS._serialized_end = 4587
-    _EXTRACTENTITIESREQUEST._serialized_start = 128
-    _EXTRACTENTITIESREQUEST._serialized_end = 226
-    _EXTRACTENTITIESFUZZYREQUEST._serialized_start = 229
-    _EXTRACTENTITIESFUZZYREQUEST._serialized_end = 401
-    _ENTITYTYPEFUZZYNERCONFIG._serialized_start = 404
-    _ENTITYTYPEFUZZYNERCONFIG._serialized_end = 687
-    _ENTITYTYPEFUZZYNERCONFIG_FUZZYNERALGORITHM._serialized_start = 622
-    _ENTITYTYPEFUZZYNERCONFIG_FUZZYNERALGORITHM._serialized_end = 687
-    _ENTITYDETECTED._serialized_start = 689
-    _ENTITYDETECTED._serialized_end = 805
-    _EXTRACTENTITIESRESPONSE._serialized_start = 807
-    _EXTRACTENTITIESRESPONSE._serialized_end = 901
-    _GETALTERNATIVESENTENCESREQUEST._serialized_start = 904
-    _GETALTERNATIVESENTENCESREQUEST._serialized_end = 1093
-    _GENERATEUSERSAYSREQUEST._serialized_start = 1095
-    _GENERATEUSERSAYSREQUEST._serialized_end = 1201
-    _GENERATERESPONSESREQUEST._serialized_start = 1204
-    _GENERATERESPONSESREQUEST._serialized_end = 1344
-    _GETALTERNATIVETRAININGPHRASESREQUEST._serialized_start = 1347
-    _GETALTERNATIVETRAININGPHRASESREQUEST._serialized_end = 1676
-    _GETSYNONYMSREQUEST._serialized_start = 1678
-    _GETSYNONYMSREQUEST._serialized_end = 1801
-    _GETSYNONYMSRESPONSE._serialized_start = 1803
-    _GETSYNONYMSRESPONSE._serialized_end = 1863
-    _SYNONYM._serialized_start = 1865
-    _SYNONYM._serialized_end = 1906
-    _GETALTERNATIVESENTENCESRESPONSE._serialized_start = 1908
-    _GETALTERNATIVESENTENCESRESPONSE._serialized_end = 1997
-    _GENERATERESPONSESRESPONSE._serialized_start = 1999
-    _GENERATERESPONSESRESPONSE._serialized_end = 2045
-    _GENERATEUSERSAYSRESPONSE._serialized_start = 2047
-    _GENERATEUSERSAYSRESPONSE._serialized_end = 2092
-    _GETALTERNATIVETRAININGPHRASESRESPONSE._serialized_start = 2094
-    _GETALTERNATIVETRAININGPHRASESRESPONSE._serialized_end = 2202
-    _ALTSENTENCE._serialized_start = 2204
-    _ALTSENTENCE._serialized_end = 2250
-    _ALTTRAININGPHRASE._serialized_start = 2252
-    _ALTTRAININGPHRASE._serialized_end = 2346
-    _DATAENRICHMENTCONFIG._serialized_start = 2349
-    _DATAENRICHMENTCONFIG._serialized_end = 2885
-    _ENTITYENRICHMENTCONFIG._serialized_start = 2887
-    _ENTITYENRICHMENTCONFIG._serialized_end = 2982
-    _THESAURUSENRICHMENTCONFIG._serialized_start = 2984
-    _THESAURUSENRICHMENTCONFIG._serialized_end = 3082
-    _BERTAUGENRICHMENTCONFIG._serialized_start = 3084
-    _BERTAUGENRICHMENTCONFIG._serialized_end = 3180
-    _GLOVEENRICHMENTCONFIG._serialized_start = 3182
-    _GLOVEENRICHMENTCONFIG._serialized_end = 3276
-    _GPT2ENRICHMENTCONFIG._serialized_start = 3278
-    _GPT2ENRICHMENTCONFIG._serialized_end = 3371
-    _WORD2VECENRICHMENTCONFIG._serialized_start = 3373
-    _WORD2VECENRICHMENTCONFIG._serialized_end = 3470
-    _WORDNETAUGENRICHMENTCONFIG._serialized_start = 3472
-    _WORDNETAUGENRICHMENTCONFIG._serialized_end = 3571
-    _XLNETAUGENRICHMENTCONFIG._serialized_start = 3573
-    _XLNETAUGENRICHMENTCONFIG._serialized_end = 3670
-    _CLASSIFYINTENTSREQUEST._serialized_start = 3673
-    _CLASSIFYINTENTSREQUEST._serialized_end = 3880
-    _INTENTCLASSIFIED._serialized_start = 3882
-    _INTENTCLASSIFIED._serialized_end = 3985
-    _CLASSIFYINTENTSRESPONSE._serialized_start = 3988
-    _CLASSIFYINTENTSRESPONSE._serialized_end = 4133
-    _AISERVICES._serialized_start = 4590
-    _AISERVICES._serialized_end = 5854
+    _MODE._serialized_start=4135
+    _MODE._serialized_end=4188
+    _INTENTALGORITHMS._serialized_start=4191
+    _INTENTALGORITHMS._serialized_end=4587
+    _EXTRACTENTITIESREQUEST._serialized_start=128
+    _EXTRACTENTITIESREQUEST._serialized_end=226
+    _EXTRACTENTITIESFUZZYREQUEST._serialized_start=229
+    _EXTRACTENTITIESFUZZYREQUEST._serialized_end=401
+    _ENTITYTYPEFUZZYNERCONFIG._serialized_start=404
+    _ENTITYTYPEFUZZYNERCONFIG._serialized_end=687
+    _ENTITYTYPEFUZZYNERCONFIG_FUZZYNERALGORITHM._serialized_start=622
+    _ENTITYTYPEFUZZYNERCONFIG_FUZZYNERALGORITHM._serialized_end=687
+    _ENTITYDETECTED._serialized_start=689
+    _ENTITYDETECTED._serialized_end=805
+    _EXTRACTENTITIESRESPONSE._serialized_start=807
+    _EXTRACTENTITIESRESPONSE._serialized_end=901
+    _GETALTERNATIVESENTENCESREQUEST._serialized_start=904
+    _GETALTERNATIVESENTENCESREQUEST._serialized_end=1093
+    _GENERATEUSERSAYSREQUEST._serialized_start=1095
+    _GENERATEUSERSAYSREQUEST._serialized_end=1201
+    _GENERATERESPONSESREQUEST._serialized_start=1204
+    _GENERATERESPONSESREQUEST._serialized_end=1344
+    _GETALTERNATIVETRAININGPHRASESREQUEST._serialized_start=1347
+    _GETALTERNATIVETRAININGPHRASESREQUEST._serialized_end=1676
+    _GETSYNONYMSREQUEST._serialized_start=1678
+    _GETSYNONYMSREQUEST._serialized_end=1801
+    _GETSYNONYMSRESPONSE._serialized_start=1803
+    _GETSYNONYMSRESPONSE._serialized_end=1863
+    _SYNONYM._serialized_start=1865
+    _SYNONYM._serialized_end=1906
+    _GETALTERNATIVESENTENCESRESPONSE._serialized_start=1908
+    _GETALTERNATIVESENTENCESRESPONSE._serialized_end=1997
+    _GENERATERESPONSESRESPONSE._serialized_start=1999
+    _GENERATERESPONSESRESPONSE._serialized_end=2045
+    _GENERATEUSERSAYSRESPONSE._serialized_start=2047
+    _GENERATEUSERSAYSRESPONSE._serialized_end=2092
+    _GETALTERNATIVETRAININGPHRASESRESPONSE._serialized_start=2094
+    _GETALTERNATIVETRAININGPHRASESRESPONSE._serialized_end=2202
+    _ALTSENTENCE._serialized_start=2204
+    _ALTSENTENCE._serialized_end=2250
+    _ALTTRAININGPHRASE._serialized_start=2252
+    _ALTTRAININGPHRASE._serialized_end=2346
+    _DATAENRICHMENTCONFIG._serialized_start=2349
+    _DATAENRICHMENTCONFIG._serialized_end=2885
+    _ENTITYENRICHMENTCONFIG._serialized_start=2887
+    _ENTITYENRICHMENTCONFIG._serialized_end=2982
+    _THESAURUSENRICHMENTCONFIG._serialized_start=2984
+    _THESAURUSENRICHMENTCONFIG._serialized_end=3082
+    _BERTAUGENRICHMENTCONFIG._serialized_start=3084
+    _BERTAUGENRICHMENTCONFIG._serialized_end=3180
+    _GLOVEENRICHMENTCONFIG._serialized_start=3182
+    _GLOVEENRICHMENTCONFIG._serialized_end=3276
+    _GPT2ENRICHMENTCONFIG._serialized_start=3278
+    _GPT2ENRICHMENTCONFIG._serialized_end=3371
+    _WORD2VECENRICHMENTCONFIG._serialized_start=3373
+    _WORD2VECENRICHMENTCONFIG._serialized_end=3470
+    _WORDNETAUGENRICHMENTCONFIG._serialized_start=3472
+    _WORDNETAUGENRICHMENTCONFIG._serialized_end=3571
+    _XLNETAUGENRICHMENTCONFIG._serialized_start=3573
+    _XLNETAUGENRICHMENTCONFIG._serialized_end=3670
+    _CLASSIFYINTENTSREQUEST._serialized_start=3673
+    _CLASSIFYINTENTSREQUEST._serialized_end=3880
+    _INTENTCLASSIFIED._serialized_start=3882
+    _INTENTCLASSIFIED._serialized_end=3985
+    _CLASSIFYINTENTSRESPONSE._serialized_start=3988
+    _CLASSIFYINTENTSRESPONSE._serialized_end=4133
+    _AISERVICES._serialized_start=4590
+    _AISERVICES._serialized_end=5854
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/aiservices_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/aiservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/common_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/common_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     # @@protoc_insertion_point(class_scope:ondewo.nlu.StatResponse)
 })
 _sym_db.RegisterMessage(StatResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _SORTINGMODE._serialized_start = 70
-    _SORTINGMODE._serialized_end = 114
-    _STATRESPONSE._serialized_start = 39
-    _STATRESPONSE._serialized_end = 68
+    _SORTINGMODE._serialized_start=70
+    _SORTINGMODE._serialized_end=114
+    _STATRESPONSE._serialized_start=39
+    _STATRESPONSE._serialized_end=68
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/context_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/context_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -113,30 +113,30 @@
     _CONTEXTS.methods_by_name['CreateContext']._serialized_options = b'\202\323\344\223\002<\"1/v2/{parent=projects/*/agent/sessions/*}/contexts:\007context'
     _CONTEXTS.methods_by_name['UpdateContext']._options = None
     _CONTEXTS.methods_by_name['UpdateContext']._serialized_options = b'\202\323\344\223\002D29/v2/{context.name=projects/*/agent/sessions/*/contexts/*}:\007context'
     _CONTEXTS.methods_by_name['DeleteContext']._options = None
     _CONTEXTS.methods_by_name['DeleteContext']._serialized_options = b'\202\323\344\223\0023*1/v2/{name=projects/*/agent/sessions/*/contexts/*}'
     _CONTEXTS.methods_by_name['DeleteAllContexts']._options = None
     _CONTEXTS.methods_by_name['DeleteAllContexts']._serialized_options = b'\202\323\344\223\0023*1/v2/{parent=projects/*/agent/sessions/*}/contexts'
-    _CONTEXT._serialized_start = 134
-    _CONTEXT._serialized_end = 431
-    _CONTEXT_PARAMETER._serialized_start = 263
-    _CONTEXT_PARAMETER._serialized_end = 349
-    _CONTEXT_PARAMETERSENTRY._serialized_start = 351
-    _CONTEXT_PARAMETERSENTRY._serialized_end = 431
-    _LISTCONTEXTSREQUEST._serialized_start = 433
-    _LISTCONTEXTSREQUEST._serialized_end = 494
-    _LISTCONTEXTSRESPONSE._serialized_start = 496
-    _LISTCONTEXTSRESPONSE._serialized_end = 582
-    _GETCONTEXTREQUEST._serialized_start = 584
-    _GETCONTEXTREQUEST._serialized_end = 617
-    _CREATECONTEXTREQUEST._serialized_start = 619
-    _CREATECONTEXTREQUEST._serialized_end = 699
-    _UPDATECONTEXTREQUEST._serialized_start = 701
-    _UPDATECONTEXTREQUEST._serialized_end = 810
-    _DELETECONTEXTREQUEST._serialized_start = 812
-    _DELETECONTEXTREQUEST._serialized_end = 848
-    _DELETEALLCONTEXTSREQUEST._serialized_start = 850
-    _DELETEALLCONTEXTSREQUEST._serialized_end = 896
-    _CONTEXTS._serialized_start = 899
-    _CONTEXTS._serialized_end = 1745
+    _CONTEXT._serialized_start=134
+    _CONTEXT._serialized_end=431
+    _CONTEXT_PARAMETER._serialized_start=263
+    _CONTEXT_PARAMETER._serialized_end=349
+    _CONTEXT_PARAMETERSENTRY._serialized_start=351
+    _CONTEXT_PARAMETERSENTRY._serialized_end=431
+    _LISTCONTEXTSREQUEST._serialized_start=433
+    _LISTCONTEXTSREQUEST._serialized_end=494
+    _LISTCONTEXTSRESPONSE._serialized_start=496
+    _LISTCONTEXTSRESPONSE._serialized_end=582
+    _GETCONTEXTREQUEST._serialized_start=584
+    _GETCONTEXTREQUEST._serialized_end=617
+    _CREATECONTEXTREQUEST._serialized_start=619
+    _CREATECONTEXTREQUEST._serialized_end=699
+    _UPDATECONTEXTREQUEST._serialized_start=701
+    _UPDATECONTEXTREQUEST._serialized_end=810
+    _DELETECONTEXTREQUEST._serialized_start=812
+    _DELETECONTEXTREQUEST._serialized_end=848
+    _DELETEALLCONTEXTSREQUEST._serialized_start=850
+    _DELETEALLCONTEXTSREQUEST._serialized_end=896
+    _CONTEXTS._serialized_start=899
+    _CONTEXTS._serialized_end=1745
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/context_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/context_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/entity_type_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/entity_type_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -286,80 +286,80 @@
     _ENTITYTYPES.methods_by_name['GetEntity']._serialized_options = b'\202\323\344\223\0026\0224/v2/{name=projects/*/agent/entityTypes/*/entities/*}'
     _ENTITYTYPES.methods_by_name['CreateEntity']._options = None
     _ENTITYTYPES.methods_by_name['CreateEntity']._serialized_options = b'\202\323\344\223\002:\"5/v2/{parent=projects/*/agent}/entityTypes/*/entities/:\001*'
     _ENTITYTYPES.methods_by_name['UpdateEntity']._options = None
     _ENTITYTYPES.methods_by_name['UpdateEntity']._serialized_options = b'\202\323\344\223\002A2</v2/{entity_.name=projects/*/agent/entityTypes/*/entities/*}:\001*'
     _ENTITYTYPES.methods_by_name['DeleteEntity']._options = None
     _ENTITYTYPES.methods_by_name['DeleteEntity']._serialized_options = b'\202\323\344\223\0026*4/v2/{name=projects/*/agent/entityTypes/*/entities/*}'
-    _ENTITYTYPEVIEW._serialized_start = 4123
-    _ENTITYTYPEVIEW._serialized_end = 4290
-    _ENTITYTYPECATEGORY._serialized_start = 4292
-    _ENTITYTYPECATEGORY._serialized_end = 4391
-    _ENTITYTYPE._serialized_start = 192
-    _ENTITYTYPE._serialized_end = 851
-    _ENTITYTYPE_ENTITY._serialized_start = 532
-    _ENTITYTYPE_ENTITY._serialized_end = 655
-    _ENTITYTYPE_KIND._serialized_start = 657
-    _ENTITYTYPE_KIND._serialized_end = 714
-    _ENTITYTYPE_ENTITYTYPESTATUS._serialized_start = 716
-    _ENTITYTYPE_ENTITYTYPESTATUS._serialized_end = 760
-    _ENTITYTYPE_AUTOEXPANSIONMODE._serialized_start = 762
-    _ENTITYTYPE_AUTOEXPANSIONMODE._serialized_end = 851
-    _LISTENTITYTYPESREQUEST._serialized_start = 854
-    _LISTENTITYTYPESREQUEST._serialized_end = 1105
-    _LISTENTITYTYPESRESPONSE._serialized_start = 1107
-    _LISTENTITYTYPESRESPONSE._serialized_end = 1203
-    _GETENTITYTYPEREQUEST._serialized_start = 1206
-    _GETENTITYTYPEREQUEST._serialized_end = 1339
-    _CREATEENTITYTYPEREQUEST._serialized_start = 1342
-    _CREATEENTITYTYPEREQUEST._serialized_end = 1505
-    _UPDATEENTITYTYPEREQUEST._serialized_start = 1508
-    _UPDATEENTITYTYPEREQUEST._serialized_end = 1704
-    _DELETEENTITYTYPEREQUEST._serialized_start = 1706
-    _DELETEENTITYTYPEREQUEST._serialized_end = 1745
-    _BATCHUPDATEENTITYTYPESREQUEST._serialized_start = 1748
-    _BATCHUPDATEENTITYTYPESREQUEST._serialized_end = 1986
-    _BATCHUPDATEENTITYTYPESRESPONSE._serialized_start = 1988
-    _BATCHUPDATEENTITYTYPESRESPONSE._serialized_end = 2066
-    _BATCHDELETEENTITYTYPESREQUEST._serialized_start = 2068
-    _BATCHDELETEENTITYTYPESREQUEST._serialized_end = 2142
-    _ENTITYTYPEBATCH._serialized_start = 2144
-    _ENTITYTYPEBATCH._serialized_end = 2207
-    _ENTITYTYPESORTING._serialized_start = 2210
-    _ENTITYTYPESORTING._serialized_end = 2598
-    _ENTITYTYPESORTING_ENTITYTYPESORTINGFIELD._serialized_start = 2356
-    _ENTITYTYPESORTING_ENTITYTYPESORTINGFIELD._serialized_end = 2598
-    _ENTITYSTATUS._serialized_start = 2600
-    _ENTITYSTATUS._serialized_end = 2708
-    _BATCHENTITIESRESPONSE._serialized_start = 2710
-    _BATCHENTITIESRESPONSE._serialized_end = 2804
-    _CREATEENTITYREQUEST._serialized_start = 2806
-    _CREATEENTITYREQUEST._serialized_end = 2900
-    _BATCHCREATEENTITIESREQUEST._serialized_start = 2902
-    _BATCHCREATEENTITIESREQUEST._serialized_end = 2995
-    _BATCHUPDATEENTITIESREQUEST._serialized_start = 2997
-    _BATCHUPDATEENTITIESREQUEST._serialized_end = 3074
-    _UPDATEENTITYREQUEST._serialized_start = 3076
-    _UPDATEENTITYREQUEST._serialized_end = 3144
-    _GETENTITYREQUEST._serialized_start = 3146
-    _GETENTITYREQUEST._serialized_end = 3178
-    _BATCHGETENTITIESREQUEST._serialized_start = 3180
-    _BATCHGETENTITIESREQUEST._serialized_end = 3220
-    _BATCHDELETEENTITIESREQUEST._serialized_start = 3222
-    _BATCHDELETEENTITIESREQUEST._serialized_end = 3265
-    _DELETEENTITYREQUEST._serialized_start = 3267
-    _DELETEENTITYREQUEST._serialized_end = 3302
-    _DELETEENTITYSTATUS._serialized_start = 3304
-    _DELETEENTITYSTATUS._serialized_end = 3422
-    _BATCHDELETEENTITIESRESPONSE._serialized_start = 3424
-    _BATCHDELETEENTITIESRESPONSE._serialized_end = 3530
-    _LISTENTITIESREQUEST._serialized_start = 3533
-    _LISTENTITIESREQUEST._serialized_end = 3705
-    _LISTENTITIESRESPONSE._serialized_start = 3707
-    _LISTENTITIESRESPONSE._serialized_end = 3803
-    _ENTITYVALUESORTING._serialized_start = 3806
-    _ENTITYVALUESORTING._serialized_end = 4120
-    _ENTITYVALUESORTING_ENTITYVALUESORTINGFIELD._serialized_start = 3955
-    _ENTITYVALUESORTING_ENTITYVALUESORTINGFIELD._serialized_end = 4120
-    _ENTITYTYPES._serialized_start = 4394
-    _ENTITYTYPES._serialized_end = 6469
+    _ENTITYTYPEVIEW._serialized_start=4123
+    _ENTITYTYPEVIEW._serialized_end=4290
+    _ENTITYTYPECATEGORY._serialized_start=4292
+    _ENTITYTYPECATEGORY._serialized_end=4391
+    _ENTITYTYPE._serialized_start=192
+    _ENTITYTYPE._serialized_end=851
+    _ENTITYTYPE_ENTITY._serialized_start=532
+    _ENTITYTYPE_ENTITY._serialized_end=655
+    _ENTITYTYPE_KIND._serialized_start=657
+    _ENTITYTYPE_KIND._serialized_end=714
+    _ENTITYTYPE_ENTITYTYPESTATUS._serialized_start=716
+    _ENTITYTYPE_ENTITYTYPESTATUS._serialized_end=760
+    _ENTITYTYPE_AUTOEXPANSIONMODE._serialized_start=762
+    _ENTITYTYPE_AUTOEXPANSIONMODE._serialized_end=851
+    _LISTENTITYTYPESREQUEST._serialized_start=854
+    _LISTENTITYTYPESREQUEST._serialized_end=1105
+    _LISTENTITYTYPESRESPONSE._serialized_start=1107
+    _LISTENTITYTYPESRESPONSE._serialized_end=1203
+    _GETENTITYTYPEREQUEST._serialized_start=1206
+    _GETENTITYTYPEREQUEST._serialized_end=1339
+    _CREATEENTITYTYPEREQUEST._serialized_start=1342
+    _CREATEENTITYTYPEREQUEST._serialized_end=1505
+    _UPDATEENTITYTYPEREQUEST._serialized_start=1508
+    _UPDATEENTITYTYPEREQUEST._serialized_end=1704
+    _DELETEENTITYTYPEREQUEST._serialized_start=1706
+    _DELETEENTITYTYPEREQUEST._serialized_end=1745
+    _BATCHUPDATEENTITYTYPESREQUEST._serialized_start=1748
+    _BATCHUPDATEENTITYTYPESREQUEST._serialized_end=1986
+    _BATCHUPDATEENTITYTYPESRESPONSE._serialized_start=1988
+    _BATCHUPDATEENTITYTYPESRESPONSE._serialized_end=2066
+    _BATCHDELETEENTITYTYPESREQUEST._serialized_start=2068
+    _BATCHDELETEENTITYTYPESREQUEST._serialized_end=2142
+    _ENTITYTYPEBATCH._serialized_start=2144
+    _ENTITYTYPEBATCH._serialized_end=2207
+    _ENTITYTYPESORTING._serialized_start=2210
+    _ENTITYTYPESORTING._serialized_end=2598
+    _ENTITYTYPESORTING_ENTITYTYPESORTINGFIELD._serialized_start=2356
+    _ENTITYTYPESORTING_ENTITYTYPESORTINGFIELD._serialized_end=2598
+    _ENTITYSTATUS._serialized_start=2600
+    _ENTITYSTATUS._serialized_end=2708
+    _BATCHENTITIESRESPONSE._serialized_start=2710
+    _BATCHENTITIESRESPONSE._serialized_end=2804
+    _CREATEENTITYREQUEST._serialized_start=2806
+    _CREATEENTITYREQUEST._serialized_end=2900
+    _BATCHCREATEENTITIESREQUEST._serialized_start=2902
+    _BATCHCREATEENTITIESREQUEST._serialized_end=2995
+    _BATCHUPDATEENTITIESREQUEST._serialized_start=2997
+    _BATCHUPDATEENTITIESREQUEST._serialized_end=3074
+    _UPDATEENTITYREQUEST._serialized_start=3076
+    _UPDATEENTITYREQUEST._serialized_end=3144
+    _GETENTITYREQUEST._serialized_start=3146
+    _GETENTITYREQUEST._serialized_end=3178
+    _BATCHGETENTITIESREQUEST._serialized_start=3180
+    _BATCHGETENTITIESREQUEST._serialized_end=3220
+    _BATCHDELETEENTITIESREQUEST._serialized_start=3222
+    _BATCHDELETEENTITIESREQUEST._serialized_end=3265
+    _DELETEENTITYREQUEST._serialized_start=3267
+    _DELETEENTITYREQUEST._serialized_end=3302
+    _DELETEENTITYSTATUS._serialized_start=3304
+    _DELETEENTITYSTATUS._serialized_end=3422
+    _BATCHDELETEENTITIESRESPONSE._serialized_start=3424
+    _BATCHDELETEENTITIESRESPONSE._serialized_end=3530
+    _LISTENTITIESREQUEST._serialized_start=3533
+    _LISTENTITIESREQUEST._serialized_end=3705
+    _LISTENTITIESRESPONSE._serialized_start=3707
+    _LISTENTITIESRESPONSE._serialized_end=3803
+    _ENTITYVALUESORTING._serialized_start=3806
+    _ENTITYVALUESORTING._serialized_end=4120
+    _ENTITYVALUESORTING_ENTITYVALUESORTINGFIELD._serialized_start=3955
+    _ENTITYVALUESORTING_ENTITYVALUESORTINGFIELD._serialized_end=4120
+    _ENTITYTYPES._serialized_start=4394
+    _ENTITYTYPES._serialized_end=6469
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/entity_type_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/entity_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/intent_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/intent_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -687,180 +687,180 @@
     _INTENTS.methods_by_name['BatchUpdateIntents']._serialized_options = b'\202\323\344\223\0026\"1/v2/{parent=projects/*/agent}/intents:batchUpdate:\001*'
     _INTENTS.methods_by_name['BatchDeleteIntents']._options = None
     _INTENTS.methods_by_name['BatchDeleteIntents']._serialized_options = b'\202\323\344\223\0026\"1/v2/{parent=projects/*/agent}/intents:batchDelete:\001*'
     _INTENTS.methods_by_name['TagIntent']._options = None
     _INTENTS.methods_by_name['TagIntent']._serialized_options = b'\202\323\344\223\0024\"//v2/{parent=projects/*/agent}/intents:tagIntent:\001*'
     _INTENTS.methods_by_name['DeleteIntentTag']._options = None
     _INTENTS.methods_by_name['DeleteIntentTag']._serialized_options = b'\202\323\344\223\002:\"5/v2/{parent=projects/*/agent}/intents:deleteIntentTag:\001*'
-    _INTENTVIEW._serialized_start = 10996
-    _INTENTVIEW._serialized_end = 11134
-    _INTENTCATEGORY._serialized_start = 11137
-    _INTENTCATEGORY._serialized_end = 11295
-    _INTENT._serialized_start = 276
-    _INTENT._serialized_end = 5347
-    _INTENT_TRAININGPHRASE._serialized_start = 1235
-    _INTENT_TRAININGPHRASE._serialized_end = 1717
-    _INTENT_TRAININGPHRASE_ENTITY._serialized_start = 1446
-    _INTENT_TRAININGPHRASE_ENTITY._serialized_end = 1660
-    _INTENT_TRAININGPHRASE_TYPE._serialized_start = 1662
-    _INTENT_TRAININGPHRASE_TYPE._serialized_end = 1717
-    _INTENT_PARAMETER._serialized_start = 1720
-    _INTENT_PARAMETER._serialized_end = 2016
-    _INTENT_PARAMETER_PROMPT._serialized_start = 1957
-    _INTENT_PARAMETER_PROMPT._serialized_end = 2016
-    _INTENT_MESSAGE._serialized_start = 2019
-    _INTENT_MESSAGE._serialized_end = 5098
-    _INTENT_MESSAGE_TEXT._serialized_start = 2964
-    _INTENT_MESSAGE_TEXT._serialized_end = 2984
-    _INTENT_MESSAGE_IMAGE._serialized_start = 2986
-    _INTENT_MESSAGE_IMAGE._serialized_end = 3040
-    _INTENT_MESSAGE_QUICKREPLIES._serialized_start = 3042
-    _INTENT_MESSAGE_QUICKREPLIES._serialized_end = 3094
-    _INTENT_MESSAGE_CARD._serialized_start = 3097
-    _INTENT_MESSAGE_CARD._serialized_end = 3254
-    _INTENT_MESSAGE_CARD_BUTTON._serialized_start = 3214
-    _INTENT_MESSAGE_CARD_BUTTON._serialized_end = 3254
-    _INTENT_MESSAGE_SIMPLERESPONSE._serialized_start = 3256
-    _INTENT_MESSAGE_SIMPLERESPONSE._serialized_end = 3332
-    _INTENT_MESSAGE_SIMPLERESPONSES._serialized_start = 3334
-    _INTENT_MESSAGE_SIMPLERESPONSES._serialized_end = 3420
-    _INTENT_MESSAGE_BASICCARD._serialized_start = 3423
-    _INTENT_MESSAGE_BASICCARD._serialized_end = 3742
-    _INTENT_MESSAGE_BASICCARD_BUTTON._serialized_start = 3605
-    _INTENT_MESSAGE_BASICCARD_BUTTON._serialized_end = 3742
-    _INTENT_MESSAGE_BASICCARD_BUTTON_OPENURIACTION._serialized_start = 3714
-    _INTENT_MESSAGE_BASICCARD_BUTTON_OPENURIACTION._serialized_end = 3742
-    _INTENT_MESSAGE_SUGGESTION._serialized_start = 3744
-    _INTENT_MESSAGE_SUGGESTION._serialized_end = 3771
-    _INTENT_MESSAGE_SUGGESTIONS._serialized_start = 3773
-    _INTENT_MESSAGE_SUGGESTIONS._serialized_end = 3846
-    _INTENT_MESSAGE_LINKOUTSUGGESTION._serialized_start = 3848
-    _INTENT_MESSAGE_LINKOUTSUGGESTION._serialized_end = 3906
-    _INTENT_MESSAGE_LISTSELECT._serialized_start = 3909
-    _INTENT_MESSAGE_LISTSELECT._serialized_end = 4146
-    _INTENT_MESSAGE_LISTSELECT_ITEM._serialized_start = 3998
-    _INTENT_MESSAGE_LISTSELECT_ITEM._serialized_end = 4146
-    _INTENT_MESSAGE_CAROUSELSELECT._serialized_start = 4149
-    _INTENT_MESSAGE_CAROUSELSELECT._serialized_end = 4379
-    _INTENT_MESSAGE_CAROUSELSELECT_ITEM._serialized_start = 3998
-    _INTENT_MESSAGE_CAROUSELSELECT_ITEM._serialized_end = 4146
-    _INTENT_MESSAGE_HTMLTEXT._serialized_start = 4381
-    _INTENT_MESSAGE_HTMLTEXT._serialized_end = 4405
-    _INTENT_MESSAGE_VIDEO._serialized_start = 4407
-    _INTENT_MESSAGE_VIDEO._serialized_end = 4455
-    _INTENT_MESSAGE_AUDIO._serialized_start = 4457
-    _INTENT_MESSAGE_AUDIO._serialized_end = 4505
-    _INTENT_MESSAGE_SELECTITEMINFO._serialized_start = 4507
-    _INTENT_MESSAGE_SELECTITEMINFO._serialized_end = 4554
-    _INTENT_MESSAGE_PLATFORM._serialized_start = 4557
-    _INTENT_MESSAGE_PLATFORM._serialized_end = 5087
-    _INTENT_FOLLOWUPINTENTINFO._serialized_start = 5100
-    _INTENT_FOLLOWUPINTENTINFO._serialized_end = 5187
-    _INTENT_INTENTSTATUS._serialized_start = 5189
-    _INTENT_INTENTSTATUS._serialized_end = 5229
-    _INTENT_WEBHOOKSTATE._serialized_start = 5231
-    _INTENT_WEBHOOKSTATE._serialized_end = 5347
-    _LISTINTENTSREQUEST._serialized_start = 5350
-    _LISTINTENTSREQUEST._serialized_end = 5604
-    _LISTINTENTSRESPONSE._serialized_start = 5606
-    _LISTINTENTSRESPONSE._serialized_end = 5689
-    _GETINTENTREQUEST._serialized_start = 5691
-    _GETINTENTREQUEST._serialized_end = 5811
-    _CREATEINTENTREQUEST._serialized_start = 5814
-    _CREATEINTENTREQUEST._serialized_end = 5955
-    _UPDATEINTENTREQUEST._serialized_start = 5958
-    _UPDATEINTENTREQUEST._serialized_end = 6132
-    _DELETEINTENTREQUEST._serialized_start = 6134
-    _DELETEINTENTREQUEST._serialized_end = 6169
-    _BATCHUPDATEINTENTSREQUEST._serialized_start = 6172
-    _BATCHUPDATEINTENTSREQUEST._serialized_end = 6432
-    _BATCHUPDATEINTENTSRESPONSE._serialized_start = 6434
-    _BATCHUPDATEINTENTSRESPONSE._serialized_end = 6499
-    _BATCHDELETEINTENTSREQUEST._serialized_start = 6501
-    _BATCHDELETEINTENTSREQUEST._serialized_end = 6581
-    _INTENTBATCH._serialized_start = 6583
-    _INTENTBATCH._serialized_end = 6633
-    _INTENTSORTING._serialized_start = 6636
-    _INTENTSORTING._serialized_end = 7000
-    _INTENTSORTING_INTENTSORTINGFIELD._serialized_start = 6770
-    _INTENTSORTING_INTENTSORTINGFIELD._serialized_end = 7000
-    _INTENTTAGREQUEST._serialized_start = 7002
-    _INTENTTAGREQUEST._serialized_end = 7055
-    _GETINTENTTAGSREQUEST._serialized_start = 7057
-    _GETINTENTTAGSREQUEST._serialized_end = 7100
-    _GETINTENTTAGSRESPONSE._serialized_start = 7102
-    _GETINTENTTAGSRESPONSE._serialized_end = 7146
-    _GETALLINTENTTAGSREQUEST._serialized_start = 7148
-    _GETALLINTENTTAGSREQUEST._serialized_end = 7189
-    _BATCHUPDATETRAININGPHRASESREQUEST._serialized_start = 7191
-    _BATCHUPDATETRAININGPHRASESREQUEST._serialized_end = 7287
-    _TRAININGPHRASESTATUS._serialized_start = 7290
-    _TRAININGPHRASESTATUS._serialized_end = 7419
-    _BATCHTRAININGPHRASESSTATUSRESPONSE._serialized_start = 7421
-    _BATCHTRAININGPHRASESSTATUSRESPONSE._serialized_end = 7545
-    _BATCHCREATETRAININGPHRASESREQUEST._serialized_start = 7548
-    _BATCHCREATETRAININGPHRASESREQUEST._serialized_end = 7804
-    _BATCHCREATETRAININGPHRASESREQUEST_CREATETRAININGPHRASEREQUEST._serialized_start = 7694
-    _BATCHCREATETRAININGPHRASESREQUEST_CREATETRAININGPHRASEREQUEST._serialized_end = 7804
-    _BATCHGETTRAININGPHRASESREQUEST._serialized_start = 7806
-    _BATCHGETTRAININGPHRASESREQUEST._serialized_end = 7853
-    _BATCHDELETETRAININGPHRASESREQUEST._serialized_start = 7855
-    _BATCHDELETETRAININGPHRASESREQUEST._serialized_end = 7905
-    _BATCHDELETETRAININGPHRASESRESPONSE._serialized_start = 7908
-    _BATCHDELETETRAININGPHRASESRESPONSE._serialized_end = 8192
-    _BATCHDELETETRAININGPHRASESRESPONSE_DELETETRAININGPHRASESTATUS._serialized_start = 8066
-    _BATCHDELETETRAININGPHRASESRESPONSE_DELETETRAININGPHRASESTATUS._serialized_end = 8192
-    _LISTTRAININGPHRASESREQUEST._serialized_start = 8194
-    _LISTTRAININGPHRASESREQUEST._serialized_end = 8286
-    _LISTTRAININGPHRASESRESPONSE._serialized_start = 8288
-    _LISTTRAININGPHRASESRESPONSE._serialized_end = 8403
-    _BATCHRESPONSEMESSAGESSTATUSRESPONSE._serialized_start = 8406
-    _BATCHRESPONSEMESSAGESSTATUSRESPONSE._serialized_end = 8695
-    _BATCHRESPONSEMESSAGESSTATUSRESPONSE_RESPONSEMESSAGESTATUS._serialized_start = 8571
-    _BATCHRESPONSEMESSAGESSTATUSRESPONSE_RESPONSEMESSAGESTATUS._serialized_end = 8695
-    _BATCHCREATERESPONSEMESSAGESREQUEST._serialized_start = 8698
-    _BATCHCREATERESPONSEMESSAGESREQUEST._serialized_end = 8953
-    _BATCHCREATERESPONSEMESSAGESREQUEST_CREATERESPONSEMESSAGEREQUEST._serialized_start = 8848
-    _BATCHCREATERESPONSEMESSAGESREQUEST_CREATERESPONSEMESSAGEREQUEST._serialized_end = 8953
-    _BATCHUPDATERESPONSEMESSAGESREQUEST._serialized_start = 8955
-    _BATCHUPDATERESPONSEMESSAGESREQUEST._serialized_end = 9046
-    _BATCHGETRESPONSEMESSAGESREQUEST._serialized_start = 9048
-    _BATCHGETRESPONSEMESSAGESREQUEST._serialized_end = 9096
-    _BATCHDELETERESPONSEMESSAGESREQUEST._serialized_start = 9098
-    _BATCHDELETERESPONSEMESSAGESREQUEST._serialized_end = 9149
-    _BATCHDELETERESPONSEMESSAGESRESPONSE._serialized_start = 9152
-    _BATCHDELETERESPONSEMESSAGESRESPONSE._serialized_end = 9440
-    _BATCHDELETERESPONSEMESSAGESRESPONSE_DELETERESPONSEMESSAGESTATUS._serialized_start = 9313
-    _BATCHDELETERESPONSEMESSAGESRESPONSE_DELETERESPONSEMESSAGESTATUS._serialized_end = 9440
-    _LISTRESPONSEMESSAGESREQUEST._serialized_start = 9442
-    _LISTRESPONSEMESSAGESREQUEST._serialized_end = 9535
-    _LISTRESPONSEMESSAGESRESPONSE._serialized_start = 9537
-    _LISTRESPONSEMESSAGESRESPONSE._serialized_end = 9647
-    _BATCHPARAMETERSSTATUSRESPONSE._serialized_start = 9650
-    _BATCHPARAMETERSSTATUSRESPONSE._serialized_end = 9903
-    _BATCHPARAMETERSSTATUSRESPONSE_PARAMETERSTATUS._serialized_start = 9790
-    _BATCHPARAMETERSSTATUSRESPONSE_PARAMETERSTATUS._serialized_end = 9903
-    _BATCHCREATEPARAMETERSREQUEST._serialized_start = 9906
-    _BATCHCREATEPARAMETERSREQUEST._serialized_end = 10125
-    _BATCHCREATEPARAMETERSREQUEST_CREATEPARAMETERREQUEST._serialized_start = 10031
-    _BATCHCREATEPARAMETERSREQUEST_CREATEPARAMETERREQUEST._serialized_end = 10125
-    _BATCHUPDATEPARAMETERSREQUEST._serialized_start = 10127
-    _BATCHUPDATEPARAMETERSREQUEST._serialized_end = 10207
-    _BATCHGETPARAMETERSREQUEST._serialized_start = 10209
-    _BATCHGETPARAMETERSREQUEST._serialized_end = 10251
-    _BATCHDELETEPARAMETERSREQUEST._serialized_start = 10253
-    _BATCHDELETEPARAMETERSREQUEST._serialized_end = 10298
-    _BATCHDELETEPARAMETERSRESPONSE._serialized_start = 10301
-    _BATCHDELETEPARAMETERSRESPONSE._serialized_end = 10565
-    _BATCHDELETEPARAMETERSRESPONSE_DELETEPARAMETERSTATUS._serialized_start = 10444
-    _BATCHDELETEPARAMETERSRESPONSE_DELETEPARAMETERSTATUS._serialized_end = 10565
-    _LISTPARAMETERSREQUEST._serialized_start = 10567
-    _LISTPARAMETERSREQUEST._serialized_end = 10654
-    _LISTPARAMETERSRESPONSE._serialized_start = 10656
-    _LISTPARAMETERSRESPONSE._serialized_end = 10755
-    _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTREQUEST._serialized_start = 10758
-    _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTREQUEST._serialized_end = 10888
-    _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTRESPONSE._serialized_start = 10890
-    _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTRESPONSE._serialized_end = 10993
-    _INTENTS._serialized_start = 11298
-    _INTENTS._serialized_end = 14560
+    _INTENTVIEW._serialized_start=10996
+    _INTENTVIEW._serialized_end=11134
+    _INTENTCATEGORY._serialized_start=11137
+    _INTENTCATEGORY._serialized_end=11295
+    _INTENT._serialized_start=276
+    _INTENT._serialized_end=5347
+    _INTENT_TRAININGPHRASE._serialized_start=1235
+    _INTENT_TRAININGPHRASE._serialized_end=1717
+    _INTENT_TRAININGPHRASE_ENTITY._serialized_start=1446
+    _INTENT_TRAININGPHRASE_ENTITY._serialized_end=1660
+    _INTENT_TRAININGPHRASE_TYPE._serialized_start=1662
+    _INTENT_TRAININGPHRASE_TYPE._serialized_end=1717
+    _INTENT_PARAMETER._serialized_start=1720
+    _INTENT_PARAMETER._serialized_end=2016
+    _INTENT_PARAMETER_PROMPT._serialized_start=1957
+    _INTENT_PARAMETER_PROMPT._serialized_end=2016
+    _INTENT_MESSAGE._serialized_start=2019
+    _INTENT_MESSAGE._serialized_end=5098
+    _INTENT_MESSAGE_TEXT._serialized_start=2964
+    _INTENT_MESSAGE_TEXT._serialized_end=2984
+    _INTENT_MESSAGE_IMAGE._serialized_start=2986
+    _INTENT_MESSAGE_IMAGE._serialized_end=3040
+    _INTENT_MESSAGE_QUICKREPLIES._serialized_start=3042
+    _INTENT_MESSAGE_QUICKREPLIES._serialized_end=3094
+    _INTENT_MESSAGE_CARD._serialized_start=3097
+    _INTENT_MESSAGE_CARD._serialized_end=3254
+    _INTENT_MESSAGE_CARD_BUTTON._serialized_start=3214
+    _INTENT_MESSAGE_CARD_BUTTON._serialized_end=3254
+    _INTENT_MESSAGE_SIMPLERESPONSE._serialized_start=3256
+    _INTENT_MESSAGE_SIMPLERESPONSE._serialized_end=3332
+    _INTENT_MESSAGE_SIMPLERESPONSES._serialized_start=3334
+    _INTENT_MESSAGE_SIMPLERESPONSES._serialized_end=3420
+    _INTENT_MESSAGE_BASICCARD._serialized_start=3423
+    _INTENT_MESSAGE_BASICCARD._serialized_end=3742
+    _INTENT_MESSAGE_BASICCARD_BUTTON._serialized_start=3605
+    _INTENT_MESSAGE_BASICCARD_BUTTON._serialized_end=3742
+    _INTENT_MESSAGE_BASICCARD_BUTTON_OPENURIACTION._serialized_start=3714
+    _INTENT_MESSAGE_BASICCARD_BUTTON_OPENURIACTION._serialized_end=3742
+    _INTENT_MESSAGE_SUGGESTION._serialized_start=3744
+    _INTENT_MESSAGE_SUGGESTION._serialized_end=3771
+    _INTENT_MESSAGE_SUGGESTIONS._serialized_start=3773
+    _INTENT_MESSAGE_SUGGESTIONS._serialized_end=3846
+    _INTENT_MESSAGE_LINKOUTSUGGESTION._serialized_start=3848
+    _INTENT_MESSAGE_LINKOUTSUGGESTION._serialized_end=3906
+    _INTENT_MESSAGE_LISTSELECT._serialized_start=3909
+    _INTENT_MESSAGE_LISTSELECT._serialized_end=4146
+    _INTENT_MESSAGE_LISTSELECT_ITEM._serialized_start=3998
+    _INTENT_MESSAGE_LISTSELECT_ITEM._serialized_end=4146
+    _INTENT_MESSAGE_CAROUSELSELECT._serialized_start=4149
+    _INTENT_MESSAGE_CAROUSELSELECT._serialized_end=4379
+    _INTENT_MESSAGE_CAROUSELSELECT_ITEM._serialized_start=3998
+    _INTENT_MESSAGE_CAROUSELSELECT_ITEM._serialized_end=4146
+    _INTENT_MESSAGE_HTMLTEXT._serialized_start=4381
+    _INTENT_MESSAGE_HTMLTEXT._serialized_end=4405
+    _INTENT_MESSAGE_VIDEO._serialized_start=4407
+    _INTENT_MESSAGE_VIDEO._serialized_end=4455
+    _INTENT_MESSAGE_AUDIO._serialized_start=4457
+    _INTENT_MESSAGE_AUDIO._serialized_end=4505
+    _INTENT_MESSAGE_SELECTITEMINFO._serialized_start=4507
+    _INTENT_MESSAGE_SELECTITEMINFO._serialized_end=4554
+    _INTENT_MESSAGE_PLATFORM._serialized_start=4557
+    _INTENT_MESSAGE_PLATFORM._serialized_end=5087
+    _INTENT_FOLLOWUPINTENTINFO._serialized_start=5100
+    _INTENT_FOLLOWUPINTENTINFO._serialized_end=5187
+    _INTENT_INTENTSTATUS._serialized_start=5189
+    _INTENT_INTENTSTATUS._serialized_end=5229
+    _INTENT_WEBHOOKSTATE._serialized_start=5231
+    _INTENT_WEBHOOKSTATE._serialized_end=5347
+    _LISTINTENTSREQUEST._serialized_start=5350
+    _LISTINTENTSREQUEST._serialized_end=5604
+    _LISTINTENTSRESPONSE._serialized_start=5606
+    _LISTINTENTSRESPONSE._serialized_end=5689
+    _GETINTENTREQUEST._serialized_start=5691
+    _GETINTENTREQUEST._serialized_end=5811
+    _CREATEINTENTREQUEST._serialized_start=5814
+    _CREATEINTENTREQUEST._serialized_end=5955
+    _UPDATEINTENTREQUEST._serialized_start=5958
+    _UPDATEINTENTREQUEST._serialized_end=6132
+    _DELETEINTENTREQUEST._serialized_start=6134
+    _DELETEINTENTREQUEST._serialized_end=6169
+    _BATCHUPDATEINTENTSREQUEST._serialized_start=6172
+    _BATCHUPDATEINTENTSREQUEST._serialized_end=6432
+    _BATCHUPDATEINTENTSRESPONSE._serialized_start=6434
+    _BATCHUPDATEINTENTSRESPONSE._serialized_end=6499
+    _BATCHDELETEINTENTSREQUEST._serialized_start=6501
+    _BATCHDELETEINTENTSREQUEST._serialized_end=6581
+    _INTENTBATCH._serialized_start=6583
+    _INTENTBATCH._serialized_end=6633
+    _INTENTSORTING._serialized_start=6636
+    _INTENTSORTING._serialized_end=7000
+    _INTENTSORTING_INTENTSORTINGFIELD._serialized_start=6770
+    _INTENTSORTING_INTENTSORTINGFIELD._serialized_end=7000
+    _INTENTTAGREQUEST._serialized_start=7002
+    _INTENTTAGREQUEST._serialized_end=7055
+    _GETINTENTTAGSREQUEST._serialized_start=7057
+    _GETINTENTTAGSREQUEST._serialized_end=7100
+    _GETINTENTTAGSRESPONSE._serialized_start=7102
+    _GETINTENTTAGSRESPONSE._serialized_end=7146
+    _GETALLINTENTTAGSREQUEST._serialized_start=7148
+    _GETALLINTENTTAGSREQUEST._serialized_end=7189
+    _BATCHUPDATETRAININGPHRASESREQUEST._serialized_start=7191
+    _BATCHUPDATETRAININGPHRASESREQUEST._serialized_end=7287
+    _TRAININGPHRASESTATUS._serialized_start=7290
+    _TRAININGPHRASESTATUS._serialized_end=7419
+    _BATCHTRAININGPHRASESSTATUSRESPONSE._serialized_start=7421
+    _BATCHTRAININGPHRASESSTATUSRESPONSE._serialized_end=7545
+    _BATCHCREATETRAININGPHRASESREQUEST._serialized_start=7548
+    _BATCHCREATETRAININGPHRASESREQUEST._serialized_end=7804
+    _BATCHCREATETRAININGPHRASESREQUEST_CREATETRAININGPHRASEREQUEST._serialized_start=7694
+    _BATCHCREATETRAININGPHRASESREQUEST_CREATETRAININGPHRASEREQUEST._serialized_end=7804
+    _BATCHGETTRAININGPHRASESREQUEST._serialized_start=7806
+    _BATCHGETTRAININGPHRASESREQUEST._serialized_end=7853
+    _BATCHDELETETRAININGPHRASESREQUEST._serialized_start=7855
+    _BATCHDELETETRAININGPHRASESREQUEST._serialized_end=7905
+    _BATCHDELETETRAININGPHRASESRESPONSE._serialized_start=7908
+    _BATCHDELETETRAININGPHRASESRESPONSE._serialized_end=8192
+    _BATCHDELETETRAININGPHRASESRESPONSE_DELETETRAININGPHRASESTATUS._serialized_start=8066
+    _BATCHDELETETRAININGPHRASESRESPONSE_DELETETRAININGPHRASESTATUS._serialized_end=8192
+    _LISTTRAININGPHRASESREQUEST._serialized_start=8194
+    _LISTTRAININGPHRASESREQUEST._serialized_end=8286
+    _LISTTRAININGPHRASESRESPONSE._serialized_start=8288
+    _LISTTRAININGPHRASESRESPONSE._serialized_end=8403
+    _BATCHRESPONSEMESSAGESSTATUSRESPONSE._serialized_start=8406
+    _BATCHRESPONSEMESSAGESSTATUSRESPONSE._serialized_end=8695
+    _BATCHRESPONSEMESSAGESSTATUSRESPONSE_RESPONSEMESSAGESTATUS._serialized_start=8571
+    _BATCHRESPONSEMESSAGESSTATUSRESPONSE_RESPONSEMESSAGESTATUS._serialized_end=8695
+    _BATCHCREATERESPONSEMESSAGESREQUEST._serialized_start=8698
+    _BATCHCREATERESPONSEMESSAGESREQUEST._serialized_end=8953
+    _BATCHCREATERESPONSEMESSAGESREQUEST_CREATERESPONSEMESSAGEREQUEST._serialized_start=8848
+    _BATCHCREATERESPONSEMESSAGESREQUEST_CREATERESPONSEMESSAGEREQUEST._serialized_end=8953
+    _BATCHUPDATERESPONSEMESSAGESREQUEST._serialized_start=8955
+    _BATCHUPDATERESPONSEMESSAGESREQUEST._serialized_end=9046
+    _BATCHGETRESPONSEMESSAGESREQUEST._serialized_start=9048
+    _BATCHGETRESPONSEMESSAGESREQUEST._serialized_end=9096
+    _BATCHDELETERESPONSEMESSAGESREQUEST._serialized_start=9098
+    _BATCHDELETERESPONSEMESSAGESREQUEST._serialized_end=9149
+    _BATCHDELETERESPONSEMESSAGESRESPONSE._serialized_start=9152
+    _BATCHDELETERESPONSEMESSAGESRESPONSE._serialized_end=9440
+    _BATCHDELETERESPONSEMESSAGESRESPONSE_DELETERESPONSEMESSAGESTATUS._serialized_start=9313
+    _BATCHDELETERESPONSEMESSAGESRESPONSE_DELETERESPONSEMESSAGESTATUS._serialized_end=9440
+    _LISTRESPONSEMESSAGESREQUEST._serialized_start=9442
+    _LISTRESPONSEMESSAGESREQUEST._serialized_end=9535
+    _LISTRESPONSEMESSAGESRESPONSE._serialized_start=9537
+    _LISTRESPONSEMESSAGESRESPONSE._serialized_end=9647
+    _BATCHPARAMETERSSTATUSRESPONSE._serialized_start=9650
+    _BATCHPARAMETERSSTATUSRESPONSE._serialized_end=9903
+    _BATCHPARAMETERSSTATUSRESPONSE_PARAMETERSTATUS._serialized_start=9790
+    _BATCHPARAMETERSSTATUSRESPONSE_PARAMETERSTATUS._serialized_end=9903
+    _BATCHCREATEPARAMETERSREQUEST._serialized_start=9906
+    _BATCHCREATEPARAMETERSREQUEST._serialized_end=10125
+    _BATCHCREATEPARAMETERSREQUEST_CREATEPARAMETERREQUEST._serialized_start=10031
+    _BATCHCREATEPARAMETERSREQUEST_CREATEPARAMETERREQUEST._serialized_end=10125
+    _BATCHUPDATEPARAMETERSREQUEST._serialized_start=10127
+    _BATCHUPDATEPARAMETERSREQUEST._serialized_end=10207
+    _BATCHGETPARAMETERSREQUEST._serialized_start=10209
+    _BATCHGETPARAMETERSREQUEST._serialized_end=10251
+    _BATCHDELETEPARAMETERSREQUEST._serialized_start=10253
+    _BATCHDELETEPARAMETERSREQUEST._serialized_end=10298
+    _BATCHDELETEPARAMETERSRESPONSE._serialized_start=10301
+    _BATCHDELETEPARAMETERSRESPONSE._serialized_end=10565
+    _BATCHDELETEPARAMETERSRESPONSE_DELETEPARAMETERSTATUS._serialized_start=10444
+    _BATCHDELETEPARAMETERSRESPONSE_DELETEPARAMETERSTATUS._serialized_end=10565
+    _LISTPARAMETERSREQUEST._serialized_start=10567
+    _LISTPARAMETERSREQUEST._serialized_end=10654
+    _LISTPARAMETERSRESPONSE._serialized_start=10656
+    _LISTPARAMETERSRESPONSE._serialized_end=10755
+    _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTREQUEST._serialized_start=10758
+    _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTREQUEST._serialized_end=10888
+    _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTRESPONSE._serialized_start=10890
+    _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTRESPONSE._serialized_end=10993
+    _INTENTS._serialized_start=11298
+    _INTENTS._serialized_end=14560
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/intent_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/intent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/operation_metadata_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/operation_metadata_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     # @@protoc_insertion_point(class_scope:ondewo.nlu.OperationMetadata)
 })
 _sym_db.RegisterMessage(OperationMetadata)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _OPERATIONMETADATA._serialized_start = 85
-    _OPERATIONMETADATA._serialized_end = 995
-    _OPERATIONMETADATA_STATUS._serialized_start = 683
-    _OPERATIONMETADATA_STATUS._serialized_end = 786
-    _OPERATIONMETADATA_OPERATIONTYPE._serialized_start = 789
-    _OPERATIONMETADATA_OPERATIONTYPE._serialized_end = 995
+    _OPERATIONMETADATA._serialized_start=85
+    _OPERATIONMETADATA._serialized_end=995
+    _OPERATIONMETADATA_STATUS._serialized_start=683
+    _OPERATIONMETADATA_STATUS._serialized_end=786
+    _OPERATIONMETADATA_OPERATIONTYPE._serialized_start=789
+    _OPERATIONMETADATA_OPERATIONTYPE._serialized_end=995
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/operations_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/operations_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,24 +85,24 @@
     _OPERATIONS.methods_by_name['ListOperations']._serialized_options = b'\202\323\344\223\002\027\022\025/v1/{name=operations}'
     _OPERATIONS.methods_by_name['GetOperation']._options = None
     _OPERATIONS.methods_by_name['GetOperation']._serialized_options = b'\202\323\344\223\002\032\022\030/v1/{name=operations/**}'
     _OPERATIONS.methods_by_name['DeleteOperation']._options = None
     _OPERATIONS.methods_by_name['DeleteOperation']._serialized_options = b'\202\323\344\223\002\032*\030/v1/{name=operations/**}'
     _OPERATIONS.methods_by_name['CancelOperation']._options = None
     _OPERATIONS.methods_by_name['CancelOperation']._serialized_options = b'\202\323\344\223\002$\"\037/v1/{name=operations/**}:cancel:\001*'
-    _OPERATION._serialized_start = 225
-    _OPERATION._serialized_end = 402
-    _GETOPERATIONREQUEST._serialized_start = 404
-    _GETOPERATIONREQUEST._serialized_end = 439
-    _LISTOPERATIONSREQUEST._serialized_start = 442
-    _LISTOPERATIONSREQUEST._serialized_end = 589
-    _OPERATIONFILTER._serialized_start = 592
-    _OPERATIONFILTER._serialized_end = 904
-    _LISTOPERATIONSRESPONSE._serialized_start = 906
-    _LISTOPERATIONSRESPONSE._serialized_end = 998
-    _CANCELOPERATIONREQUEST._serialized_start = 1000
-    _CANCELOPERATIONREQUEST._serialized_end = 1038
-    _DELETEOPERATIONREQUEST._serialized_start = 1040
-    _DELETEOPERATIONREQUEST._serialized_end = 1078
-    _OPERATIONS._serialized_start = 1081
-    _OPERATIONS._serialized_end = 1555
+    _OPERATION._serialized_start=225
+    _OPERATION._serialized_end=402
+    _GETOPERATIONREQUEST._serialized_start=404
+    _GETOPERATIONREQUEST._serialized_end=439
+    _LISTOPERATIONSREQUEST._serialized_start=442
+    _LISTOPERATIONSREQUEST._serialized_end=589
+    _OPERATIONFILTER._serialized_start=592
+    _OPERATIONFILTER._serialized_end=904
+    _LISTOPERATIONSRESPONSE._serialized_start=906
+    _LISTOPERATIONSRESPONSE._serialized_end=998
+    _CANCELOPERATIONREQUEST._serialized_start=1000
+    _CANCELOPERATIONREQUEST._serialized_end=1038
+    _DELETEOPERATIONREQUEST._serialized_start=1040
+    _DELETEOPERATIONREQUEST._serialized_end=1078
+    _OPERATIONS._serialized_start=1081
+    _OPERATIONS._serialized_end=1555
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/operations_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/project_role_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/project_role_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,28 +99,28 @@
     _PROJECTROLES.methods_by_name['GetProjectRole']._serialized_options = b'\202\323\344\223\0029\0227/v2/{parent=projects/*/agent}/project_roles/{role_id=*}'
     _PROJECTROLES.methods_by_name['DeleteProjectRole']._options = None
     _PROJECTROLES.methods_by_name['DeleteProjectRole']._serialized_options = b'\202\323\344\223\0029*7/v2/{parent=projects/*/agent}/project_roles/{role_id=*}'
     _PROJECTROLES.methods_by_name['UpdateProjectRole']._options = None
     _PROJECTROLES.methods_by_name['UpdateProjectRole']._serialized_options = b'\202\323\344\223\00202+/v2/{parent=projects/*/agent}/project_roles:\001*'
     _PROJECTROLES.methods_by_name['ListProjectRoles']._options = None
     _PROJECTROLES.methods_by_name['ListProjectRoles']._serialized_options = b'\202\323\344\223\002-\022+/v2/{parent=projects/*/agent}/project_roles'
-    _DEFAULTPROJECTROLE._serialized_start = 981
-    _DEFAULTPROJECTROLE._serialized_end = 1130
-    _PROJECTROLEVIEW._serialized_start = 1132
-    _PROJECTROLEVIEW._serialized_end = 1243
-    _PROJECTROLE._serialized_start = 138
-    _PROJECTROLE._serialized_end = 203
-    _CREATEPROJECTROLEREQUEST._serialized_start = 206
-    _CREATEPROJECTROLEREQUEST._serialized_end = 343
-    _UPDATEPROJECTROLEREQUEST._serialized_start = 346
-    _UPDATEPROJECTROLEREQUEST._serialized_end = 532
-    _GETPROJECTROLEREQUEST._serialized_start = 535
-    _GETPROJECTROLEREQUEST._serialized_end = 697
-    _DELETEPROJECTROLEREQUEST._serialized_start = 699
-    _DELETEPROJECTROLEREQUEST._serialized_end = 758
-    _LISTPROJECTROLESREQUEST._serialized_start = 760
-    _LISTPROJECTROLESREQUEST._serialized_end = 877
-    _LISTPROJECTROLESRESPONSE._serialized_start = 879
-    _LISTPROJECTROLESRESPONSE._serialized_end = 978
-    _PROJECTROLES._serialized_start = 1246
-    _PROJECTROLES._serialized_end = 1984
+    _DEFAULTPROJECTROLE._serialized_start=981
+    _DEFAULTPROJECTROLE._serialized_end=1130
+    _PROJECTROLEVIEW._serialized_start=1132
+    _PROJECTROLEVIEW._serialized_end=1243
+    _PROJECTROLE._serialized_start=138
+    _PROJECTROLE._serialized_end=203
+    _CREATEPROJECTROLEREQUEST._serialized_start=206
+    _CREATEPROJECTROLEREQUEST._serialized_end=343
+    _UPDATEPROJECTROLEREQUEST._serialized_start=346
+    _UPDATEPROJECTROLEREQUEST._serialized_end=532
+    _GETPROJECTROLEREQUEST._serialized_start=535
+    _GETPROJECTROLEREQUEST._serialized_end=697
+    _DELETEPROJECTROLEREQUEST._serialized_start=699
+    _DELETEPROJECTROLEREQUEST._serialized_end=758
+    _LISTPROJECTROLESREQUEST._serialized_start=760
+    _LISTPROJECTROLESREQUEST._serialized_end=877
+    _LISTPROJECTROLESRESPONSE._serialized_start=879
+    _LISTPROJECTROLESRESPONSE._serialized_end=978
+    _PROJECTROLES._serialized_start=1246
+    _PROJECTROLES._serialized_end=1984
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/project_role_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/project_role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/project_statistics_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/project_statistics_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,18 @@
     _PROJECTSTATISTICS.methods_by_name['GetTrainingPhraseCount']._serialized_options = b'\202\323\344\223\002:\0228/{name=projects/*/agent/intents/*}/trainingPhrases:count'
     _PROJECTSTATISTICS.methods_by_name['GetResponseCount']._options = None
     _PROJECTSTATISTICS.methods_by_name['GetResponseCount']._serialized_options = b'\202\323\344\223\0024\0222/{name=projects/*/agent/intents/*}/responses:count'
     _PROJECTSTATISTICS.methods_by_name['GetEntityValueCount']._options = None
     _PROJECTSTATISTICS.methods_by_name['GetEntityValueCount']._serialized_options = b'\202\323\344\223\0027\0225/{name=projects/*/agent/entityTypes/*}/entities:count'
     _PROJECTSTATISTICS.methods_by_name['GetEntitySynonymCount']._options = None
     _PROJECTSTATISTICS.methods_by_name['GetEntitySynonymCount']._serialized_options = b'\202\323\344\223\002L\022J/{name=projects/*/agent/entityTypes/*/entityValues/*}/entitySynonyms:count'
-    _GETINTENTCOUNTREQUEST._serialized_start = 161
-    _GETINTENTCOUNTREQUEST._serialized_end = 256
-    _GETENTITYTYPECOUNTREQUEST._serialized_start = 258
-    _GETENTITYTYPECOUNTREQUEST._serialized_end = 361
-    _GETPROJECTSTATREQUEST._serialized_start = 363
-    _GETPROJECTSTATREQUEST._serialized_end = 402
-    _GETPROJECTELEMENTSTATREQUEST._serialized_start = 404
-    _GETPROJECTELEMENTSTATREQUEST._serialized_end = 471
-    _PROJECTSTATISTICS._serialized_start = 474
-    _PROJECTSTATISTICS._serialized_end = 1664
+    _GETINTENTCOUNTREQUEST._serialized_start=161
+    _GETINTENTCOUNTREQUEST._serialized_end=256
+    _GETENTITYTYPECOUNTREQUEST._serialized_start=258
+    _GETENTITYTYPECOUNTREQUEST._serialized_end=361
+    _GETPROJECTSTATREQUEST._serialized_start=363
+    _GETPROJECTSTATREQUEST._serialized_end=402
+    _GETPROJECTELEMENTSTATREQUEST._serialized_start=404
+    _GETPROJECTELEMENTSTATREQUEST._serialized_end=471
+    _PROJECTSTATISTICS._serialized_start=474
+    _PROJECTSTATISTICS._serialized_end=1664
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/project_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/project_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/server_statistics_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/server_statistics_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,12 @@
     DESCRIPTOR._options = None
     _SERVERSTATISTICS.methods_by_name['GetProjectCount']._options = None
     _SERVERSTATISTICS.methods_by_name['GetProjectCount']._serialized_options = b'\202\323\344\223\002\021\022\017/projects:count'
     _SERVERSTATISTICS.methods_by_name['GetUserProjectCount']._options = None
     _SERVERSTATISTICS.methods_by_name['GetUserProjectCount']._serialized_options = b'\202\323\344\223\002+\022)/users/{user_identifier=*}/projects:count'
     _SERVERSTATISTICS.methods_by_name['GetUserCount']._options = None
     _SERVERSTATISTICS.methods_by_name['GetUserCount']._serialized_options = b'\202\323\344\223\002\016\022\014/users:count'
-    _GETUSERPROJECTCOUNTREQUEST._serialized_start = 134
-    _GETUSERPROJECTCOUNTREQUEST._serialized_end = 179
-    _SERVERSTATISTICS._serialized_start = 182
-    _SERVERSTATISTICS._serialized_end = 523
+    _GETUSERPROJECTCOUNTREQUEST._serialized_start=134
+    _GETUSERPROJECTCOUNTREQUEST._serialized_end=179
+    _SERVERSTATISTICS._serialized_start=182
+    _SERVERSTATISTICS._serialized_end=523
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/server_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/server_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/session_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/session_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -600,144 +600,144 @@
     _SESSIONS.methods_by_name['ListSessionReviews']._serialized_options = b'\202\323\344\223\0026\0224/v2/{session_id=projects/*/agent/sessions/*}/reviews'
     _SESSIONS.methods_by_name['GetSessionReview']._options = None
     _SESSIONS.methods_by_name['GetSessionReview']._serialized_options = b'\202\323\344\223\002?\022=/v2/{session_review_id=projects/*/agent/sessions/*/reviews/*}'
     _SESSIONS.methods_by_name['GetLatestSessionReview']._options = None
     _SESSIONS.methods_by_name['GetLatestSessionReview']._serialized_options = b'\202\323\344\223\002M\022K/v2/{session_id=projects/*/agent/sessions/*}/reviews:getLatestSessionReview'
     _SESSIONS.methods_by_name['CreateSessionReview']._options = None
     _SESSIONS.methods_by_name['CreateSessionReview']._serialized_options = b'\202\323\344\223\002E\"@/v2/{session_id=projects/*/agent/sessions/*}:createSessionReview:\001*'
-    _AUDIOENCODING._serialized_start = 10586
-    _AUDIOENCODING._serialized_end = 10837
-    _COMPARISONOPERATOR._serialized_start = 10840
-    _COMPARISONOPERATOR._serialized_end = 10971
-    _DETECTINTENTREQUEST._serialized_start = 329
-    _DETECTINTENTREQUEST._serialized_end = 484
-    _DETECTINTENTRESPONSE._serialized_start = 487
-    _DETECTINTENTRESPONSE._serialized_end = 621
-    _QUERYPARAMETERS._serialized_start = 624
-    _QUERYPARAMETERS._serialized_end = 991
-    _QUERYINPUT._serialized_start = 994
-    _QUERYINPUT._serialized_end = 1149
-    _QUERYRESULT._serialized_start = 1152
-    _QUERYRESULT._serialized_end = 1701
-    _STREAMINGDETECTINTENTREQUEST._serialized_start = 1704
-    _STREAMINGDETECTINTENTREQUEST._serialized_end = 1894
-    _STREAMINGDETECTINTENTRESPONSE._serialized_start = 1897
-    _STREAMINGDETECTINTENTRESPONSE._serialized_end = 2108
-    _STREAMINGRECOGNITIONRESULT._serialized_start = 2111
-    _STREAMINGRECOGNITIONRESULT._serialized_end = 2361
-    _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_start = 2273
-    _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_end = 2361
-    _INPUTAUDIOCONFIG._serialized_start = 2364
-    _INPUTAUDIOCONFIG._serialized_end = 2505
-    _TEXTINPUT._serialized_start = 2507
-    _TEXTINPUT._serialized_end = 2555
-    _EVENTINPUT._serialized_start = 2557
-    _EVENTINPUT._serialized_end = 2651
-    _SESSION._serialized_start = 2654
-    _SESSION._serialized_end = 2834
-    _SESSION_VIEW._serialized_start = 2774
-    _SESSION_VIEW._serialized_end = 2834
-    _SESSIONSTEP._serialized_start = 2837
-    _SESSIONSTEP._serialized_end = 3080
-    _TRACKSESSIONSTEPREQUEST._serialized_start = 3083
-    _TRACKSESSIONSTEPREQUEST._serialized_end = 3223
-    _LISTSESSIONSREQUEST._serialized_start = 3226
-    _LISTSESSIONSREQUEST._serialized_end = 3430
-    _CONTEXTFILTER._serialized_start = 3432
-    _CONTEXTFILTER._serialized_end = 3547
-    _SESSIONFILTER._serialized_start = 3550
-    _SESSIONFILTER._serialized_end = 5299
-    _SESSIONINFO._serialized_start = 5302
-    _SESSIONINFO._serialized_end = 6444
-    _SESSIONINFO_CONTEXTSTEPS._serialized_start = 6391
-    _SESSIONINFO_CONTEXTSTEPS._serialized_end = 6444
-    _LISTSESSIONSRESPONSE._serialized_start = 6446
-    _LISTSESSIONSRESPONSE._serialized_end = 6532
-    _GETSESSIONREQUEST._serialized_start = 6535
-    _GETSESSIONREQUEST._serialized_end = 6670
-    _CREATESESSIONREQUEST._serialized_start = 6672
-    _CREATESESSIONREQUEST._serialized_end = 6787
-    _DELETESESSIONREQUEST._serialized_start = 6789
-    _DELETESESSIONREQUEST._serialized_end = 6831
-    _CREATESESSIONREVIEWREQUEST._serialized_start = 6834
-    _CREATESESSIONREVIEWREQUEST._serialized_end = 7020
-    _SESSIONREVIEW._serialized_start = 7023
-    _SESSIONREVIEW._serialized_end = 7175
-    _SESSIONREVIEW_VIEW._serialized_start = 2774
-    _SESSIONREVIEW_VIEW._serialized_end = 2834
-    _SESSIONREVIEWSTEP._serialized_start = 7178
-    _SESSIONREVIEWSTEP._serialized_end = 7565
-    _DETECTEDINTENT._serialized_start = 7568
-    _DETECTEDINTENT._serialized_end = 7744
-    _LISTSESSIONLABELSREQUEST._serialized_start = 7746
-    _LISTSESSIONLABELSREQUEST._serialized_end = 7792
-    _LISTSESSIONLABELSOFALLSESSIONSREQUEST._serialized_start = 7794
-    _LISTSESSIONLABELSOFALLSESSIONSREQUEST._serialized_end = 7900
-    _LISTSESSIONLABELSRESPONSE._serialized_start = 7902
-    _LISTSESSIONLABELSRESPONSE._serialized_end = 7945
-    _LISTLANGUAGECODESOFALLSESSIONSREQUEST._serialized_start = 7947
-    _LISTLANGUAGECODESOFALLSESSIONSREQUEST._serialized_end = 8053
-    _LISTLANGUAGECODESRESPONSE._serialized_start = 8055
-    _LISTLANGUAGECODESRESPONSE._serialized_end = 8106
-    _LISTMATCHEDINTENTSOFALLSESSIONSREQUEST._serialized_start = 8108
-    _LISTMATCHEDINTENTSOFALLSESSIONSREQUEST._serialized_end = 8215
-    _LISTMATCHEDINTENTSRESPONSE._serialized_start = 8217
-    _LISTMATCHEDINTENTSRESPONSE._serialized_end = 8270
-    _LISTMATCHEDENTITYTYPESOFALLSESSIONSREQUEST._serialized_start = 8272
-    _LISTMATCHEDENTITYTYPESOFALLSESSIONSREQUEST._serialized_end = 8383
-    _LISTMATCHEDENTITYTYPESRESPONSE._serialized_start = 8385
-    _LISTMATCHEDENTITYTYPESRESPONSE._serialized_end = 8447
-    _LISTUSERIDSOFALLSESSIONSREQUEST._serialized_start = 8449
-    _LISTUSERIDSOFALLSESSIONSREQUEST._serialized_end = 8549
-    _LISTUSERIDSRESPONSE._serialized_start = 8551
-    _LISTUSERIDSRESPONSE._serialized_end = 8590
-    _LISTIDENTIFIEDUSERIDSOFALLSESSIONSREQUEST._serialized_start = 8592
-    _LISTIDENTIFIEDUSERIDSOFALLSESSIONSREQUEST._serialized_end = 8702
-    _LISTIDENTIFIEDUSERIDSRESPONSE._serialized_start = 8704
-    _LISTIDENTIFIEDUSERIDSRESPONSE._serialized_end = 8764
-    _LISTTAGSOFALLSESSIONSREQUEST._serialized_start = 8766
-    _LISTTAGSOFALLSESSIONSREQUEST._serialized_end = 8863
-    _LISTTAGSRESPONSE._serialized_start = 8865
-    _LISTTAGSRESPONSE._serialized_end = 8897
-    _LISTINPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_start = 8899
-    _LISTINPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_end = 9005
-    _LISTINPUTCONTEXTSRESPONSE._serialized_start = 9007
-    _LISTINPUTCONTEXTSRESPONSE._serialized_end = 9058
-    _LISTOUTPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_start = 9060
-    _LISTOUTPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_end = 9167
-    _LISTOUTPUTCONTEXTSRESPONSE._serialized_start = 9169
-    _LISTOUTPUTCONTEXTSRESPONSE._serialized_end = 9222
-    _LISTPLATFORMSOFALLSESSIONSREQUEST._serialized_start = 9224
-    _LISTPLATFORMSOFALLSESSIONSREQUEST._serialized_end = 9326
-    _LISTPLATFORMSRESPONSE._serialized_start = 9328
-    _LISTPLATFORMSRESPONSE._serialized_end = 9370
-    _LISTACCOUNTIDSOFALLSESSIONSREQUEST._serialized_start = 9372
-    _LISTACCOUNTIDSOFALLSESSIONSREQUEST._serialized_end = 9475
-    _LISTACCOUNTIDSRESPONSE._serialized_start = 9477
-    _LISTACCOUNTIDSRESPONSE._serialized_end = 9522
-    _LISTPROPERTYIDSOFALLSESSIONSREQUEST._serialized_start = 9524
-    _LISTPROPERTYIDSOFALLSESSIONSREQUEST._serialized_end = 9628
-    _LISTPROPERTYIDSRESPONSE._serialized_start = 9630
-    _LISTPROPERTYIDSRESPONSE._serialized_end = 9677
-    _LISTDATASTREAMIDSOFALLSESSIONSREQUEST._serialized_start = 9679
-    _LISTDATASTREAMIDSOFALLSESSIONSREQUEST._serialized_end = 9785
-    _LISTDATASTREAMIDSRESPONSE._serialized_start = 9787
-    _LISTDATASTREAMIDSRESPONSE._serialized_end = 9838
-    _LISTORIGINIDSOFALLSESSIONSREQUEST._serialized_start = 9840
-    _LISTORIGINIDSOFALLSESSIONSREQUEST._serialized_end = 9942
-    _LISTORIGINIDSRESPONSE._serialized_start = 9944
-    _LISTORIGINIDSRESPONSE._serialized_end = 9987
-    _ADDSESSIONLABELSREQUEST._serialized_start = 9989
-    _ADDSESSIONLABELSREQUEST._serialized_end = 10050
-    _DELETESESSIONLABELSREQUEST._serialized_start = 10052
-    _DELETESESSIONLABELSREQUEST._serialized_end = 10116
-    _LISTSESSIONREVIEWSREQUEST._serialized_start = 10119
-    _LISTSESSIONREVIEWSREQUEST._serialized_end = 10247
-    _LISTSESSIONREVIEWSRESPONSE._serialized_start = 10249
-    _LISTSESSIONREVIEWSRESPONSE._serialized_end = 10354
-    _GETSESSIONREVIEWREQUEST._serialized_start = 10356
-    _GETSESSIONREVIEWREQUEST._serialized_end = 10469
-    _GETLATESTSESSIONREVIEWREQUEST._serialized_start = 10471
-    _GETLATESTSESSIONREVIEWREQUEST._serialized_end = 10583
-    _SESSIONS._serialized_start = 10974
-    _SESSIONS._serialized_end = 15595
+    _AUDIOENCODING._serialized_start=10586
+    _AUDIOENCODING._serialized_end=10837
+    _COMPARISONOPERATOR._serialized_start=10840
+    _COMPARISONOPERATOR._serialized_end=10971
+    _DETECTINTENTREQUEST._serialized_start=329
+    _DETECTINTENTREQUEST._serialized_end=484
+    _DETECTINTENTRESPONSE._serialized_start=487
+    _DETECTINTENTRESPONSE._serialized_end=621
+    _QUERYPARAMETERS._serialized_start=624
+    _QUERYPARAMETERS._serialized_end=991
+    _QUERYINPUT._serialized_start=994
+    _QUERYINPUT._serialized_end=1149
+    _QUERYRESULT._serialized_start=1152
+    _QUERYRESULT._serialized_end=1701
+    _STREAMINGDETECTINTENTREQUEST._serialized_start=1704
+    _STREAMINGDETECTINTENTREQUEST._serialized_end=1894
+    _STREAMINGDETECTINTENTRESPONSE._serialized_start=1897
+    _STREAMINGDETECTINTENTRESPONSE._serialized_end=2108
+    _STREAMINGRECOGNITIONRESULT._serialized_start=2111
+    _STREAMINGRECOGNITIONRESULT._serialized_end=2361
+    _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_start=2273
+    _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_end=2361
+    _INPUTAUDIOCONFIG._serialized_start=2364
+    _INPUTAUDIOCONFIG._serialized_end=2505
+    _TEXTINPUT._serialized_start=2507
+    _TEXTINPUT._serialized_end=2555
+    _EVENTINPUT._serialized_start=2557
+    _EVENTINPUT._serialized_end=2651
+    _SESSION._serialized_start=2654
+    _SESSION._serialized_end=2834
+    _SESSION_VIEW._serialized_start=2774
+    _SESSION_VIEW._serialized_end=2834
+    _SESSIONSTEP._serialized_start=2837
+    _SESSIONSTEP._serialized_end=3080
+    _TRACKSESSIONSTEPREQUEST._serialized_start=3083
+    _TRACKSESSIONSTEPREQUEST._serialized_end=3223
+    _LISTSESSIONSREQUEST._serialized_start=3226
+    _LISTSESSIONSREQUEST._serialized_end=3430
+    _CONTEXTFILTER._serialized_start=3432
+    _CONTEXTFILTER._serialized_end=3547
+    _SESSIONFILTER._serialized_start=3550
+    _SESSIONFILTER._serialized_end=5299
+    _SESSIONINFO._serialized_start=5302
+    _SESSIONINFO._serialized_end=6444
+    _SESSIONINFO_CONTEXTSTEPS._serialized_start=6391
+    _SESSIONINFO_CONTEXTSTEPS._serialized_end=6444
+    _LISTSESSIONSRESPONSE._serialized_start=6446
+    _LISTSESSIONSRESPONSE._serialized_end=6532
+    _GETSESSIONREQUEST._serialized_start=6535
+    _GETSESSIONREQUEST._serialized_end=6670
+    _CREATESESSIONREQUEST._serialized_start=6672
+    _CREATESESSIONREQUEST._serialized_end=6787
+    _DELETESESSIONREQUEST._serialized_start=6789
+    _DELETESESSIONREQUEST._serialized_end=6831
+    _CREATESESSIONREVIEWREQUEST._serialized_start=6834
+    _CREATESESSIONREVIEWREQUEST._serialized_end=7020
+    _SESSIONREVIEW._serialized_start=7023
+    _SESSIONREVIEW._serialized_end=7175
+    _SESSIONREVIEW_VIEW._serialized_start=2774
+    _SESSIONREVIEW_VIEW._serialized_end=2834
+    _SESSIONREVIEWSTEP._serialized_start=7178
+    _SESSIONREVIEWSTEP._serialized_end=7565
+    _DETECTEDINTENT._serialized_start=7568
+    _DETECTEDINTENT._serialized_end=7744
+    _LISTSESSIONLABELSREQUEST._serialized_start=7746
+    _LISTSESSIONLABELSREQUEST._serialized_end=7792
+    _LISTSESSIONLABELSOFALLSESSIONSREQUEST._serialized_start=7794
+    _LISTSESSIONLABELSOFALLSESSIONSREQUEST._serialized_end=7900
+    _LISTSESSIONLABELSRESPONSE._serialized_start=7902
+    _LISTSESSIONLABELSRESPONSE._serialized_end=7945
+    _LISTLANGUAGECODESOFALLSESSIONSREQUEST._serialized_start=7947
+    _LISTLANGUAGECODESOFALLSESSIONSREQUEST._serialized_end=8053
+    _LISTLANGUAGECODESRESPONSE._serialized_start=8055
+    _LISTLANGUAGECODESRESPONSE._serialized_end=8106
+    _LISTMATCHEDINTENTSOFALLSESSIONSREQUEST._serialized_start=8108
+    _LISTMATCHEDINTENTSOFALLSESSIONSREQUEST._serialized_end=8215
+    _LISTMATCHEDINTENTSRESPONSE._serialized_start=8217
+    _LISTMATCHEDINTENTSRESPONSE._serialized_end=8270
+    _LISTMATCHEDENTITYTYPESOFALLSESSIONSREQUEST._serialized_start=8272
+    _LISTMATCHEDENTITYTYPESOFALLSESSIONSREQUEST._serialized_end=8383
+    _LISTMATCHEDENTITYTYPESRESPONSE._serialized_start=8385
+    _LISTMATCHEDENTITYTYPESRESPONSE._serialized_end=8447
+    _LISTUSERIDSOFALLSESSIONSREQUEST._serialized_start=8449
+    _LISTUSERIDSOFALLSESSIONSREQUEST._serialized_end=8549
+    _LISTUSERIDSRESPONSE._serialized_start=8551
+    _LISTUSERIDSRESPONSE._serialized_end=8590
+    _LISTIDENTIFIEDUSERIDSOFALLSESSIONSREQUEST._serialized_start=8592
+    _LISTIDENTIFIEDUSERIDSOFALLSESSIONSREQUEST._serialized_end=8702
+    _LISTIDENTIFIEDUSERIDSRESPONSE._serialized_start=8704
+    _LISTIDENTIFIEDUSERIDSRESPONSE._serialized_end=8764
+    _LISTTAGSOFALLSESSIONSREQUEST._serialized_start=8766
+    _LISTTAGSOFALLSESSIONSREQUEST._serialized_end=8863
+    _LISTTAGSRESPONSE._serialized_start=8865
+    _LISTTAGSRESPONSE._serialized_end=8897
+    _LISTINPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_start=8899
+    _LISTINPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_end=9005
+    _LISTINPUTCONTEXTSRESPONSE._serialized_start=9007
+    _LISTINPUTCONTEXTSRESPONSE._serialized_end=9058
+    _LISTOUTPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_start=9060
+    _LISTOUTPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_end=9167
+    _LISTOUTPUTCONTEXTSRESPONSE._serialized_start=9169
+    _LISTOUTPUTCONTEXTSRESPONSE._serialized_end=9222
+    _LISTPLATFORMSOFALLSESSIONSREQUEST._serialized_start=9224
+    _LISTPLATFORMSOFALLSESSIONSREQUEST._serialized_end=9326
+    _LISTPLATFORMSRESPONSE._serialized_start=9328
+    _LISTPLATFORMSRESPONSE._serialized_end=9370
+    _LISTACCOUNTIDSOFALLSESSIONSREQUEST._serialized_start=9372
+    _LISTACCOUNTIDSOFALLSESSIONSREQUEST._serialized_end=9475
+    _LISTACCOUNTIDSRESPONSE._serialized_start=9477
+    _LISTACCOUNTIDSRESPONSE._serialized_end=9522
+    _LISTPROPERTYIDSOFALLSESSIONSREQUEST._serialized_start=9524
+    _LISTPROPERTYIDSOFALLSESSIONSREQUEST._serialized_end=9628
+    _LISTPROPERTYIDSRESPONSE._serialized_start=9630
+    _LISTPROPERTYIDSRESPONSE._serialized_end=9677
+    _LISTDATASTREAMIDSOFALLSESSIONSREQUEST._serialized_start=9679
+    _LISTDATASTREAMIDSOFALLSESSIONSREQUEST._serialized_end=9785
+    _LISTDATASTREAMIDSRESPONSE._serialized_start=9787
+    _LISTDATASTREAMIDSRESPONSE._serialized_end=9838
+    _LISTORIGINIDSOFALLSESSIONSREQUEST._serialized_start=9840
+    _LISTORIGINIDSOFALLSESSIONSREQUEST._serialized_end=9942
+    _LISTORIGINIDSRESPONSE._serialized_start=9944
+    _LISTORIGINIDSRESPONSE._serialized_end=9987
+    _ADDSESSIONLABELSREQUEST._serialized_start=9989
+    _ADDSESSIONLABELSREQUEST._serialized_end=10050
+    _DELETESESSIONLABELSREQUEST._serialized_start=10052
+    _DELETESESSIONLABELSREQUEST._serialized_end=10116
+    _LISTSESSIONREVIEWSREQUEST._serialized_start=10119
+    _LISTSESSIONREVIEWSREQUEST._serialized_end=10247
+    _LISTSESSIONREVIEWSRESPONSE._serialized_start=10249
+    _LISTSESSIONREVIEWSRESPONSE._serialized_end=10354
+    _GETSESSIONREVIEWREQUEST._serialized_start=10356
+    _GETSESSIONREVIEWREQUEST._serialized_end=10469
+    _GETLATESTSESSIONREVIEWREQUEST._serialized_start=10471
+    _GETLATESTSESSIONREVIEWREQUEST._serialized_end=10583
+    _SESSIONS._serialized_start=10974
+    _SESSIONS._serialized_end=15595
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/session_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/user_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/user_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -228,54 +228,54 @@
     _USERS.methods_by_name['ListServerRoles']._serialized_options = b'\202\323\344\223\002\022\022\020/v2/server_roles'
     _USERS.methods_by_name['ListServerPermissions']._options = None
     _USERS.methods_by_name['ListServerPermissions']._serialized_options = b'\202\323\344\223\002\030\022\026/v2/server_permissions'
     _USERS.methods_by_name['Login']._options = None
     _USERS.methods_by_name['Login']._serialized_options = b'\202\323\344\223\002\016\"\t/v2/login:\001*'
     _USERS.methods_by_name['CheckLogin']._options = None
     _USERS.methods_by_name['CheckLogin']._serialized_options = b'\202\323\344\223\002\021*\017/v2/check_login'
-    _DEFAULTSERVERROLE._serialized_start = 1728
-    _DEFAULTSERVERROLE._serialized_end = 1847
-    _USER._serialized_start = 161
-    _USER._serialized_end = 250
-    _USERINFO._serialized_start = 253
-    _USERINFO._serialized_end = 436
-    _USERINFO_PROJECTROLESENTRY._serialized_start = 360
-    _USERINFO_PROJECTROLESENTRY._serialized_end = 436
-    _CREATEUSERREQUEST._serialized_start = 438
-    _CREATEUSERREQUEST._serialized_end = 507
-    _UPDATEUSERREQUEST._serialized_start = 509
-    _UPDATEUSERREQUEST._serialized_end = 627
-    _GETUSERREQUEST._serialized_start = 629
-    _GETUSERREQUEST._serialized_end = 705
-    _DELETEUSERREQUEST._serialized_start = 707
-    _DELETEUSERREQUEST._serialized_end = 743
-    _LISTUSERSREQUEST._serialized_start = 745
-    _LISTUSERSREQUEST._serialized_end = 783
-    _LISTUSERSRESPONSE._serialized_start = 785
-    _LISTUSERSRESPONSE._serialized_end = 862
-    _LISTUSERINFOSRESPONSE._serialized_start = 864
-    _LISTUSERINFOSRESPONSE._serialized_end = 949
-    _SERVERROLE._serialized_start = 951
-    _SERVERROLE._serialized_end = 1015
-    _CREATESERVERROLEREQUEST._serialized_start = 1017
-    _CREATESERVERROLEREQUEST._serialized_end = 1080
-    _UPDATESERVERROLEREQUEST._serialized_start = 1082
-    _UPDATESERVERROLEREQUEST._serialized_end = 1194
-    _DELETESERVERROLEREQUEST._serialized_start = 1196
-    _DELETESERVERROLEREQUEST._serialized_end = 1238
-    _GETSERVERROLEREQUEST._serialized_start = 1240
-    _GETSERVERROLEREQUEST._serialized_end = 1328
-    _LISTSERVERROLESREQUEST._serialized_start = 1330
-    _LISTSERVERROLESREQUEST._serialized_end = 1374
-    _LISTSERVERROLESRESPONSE._serialized_start = 1376
-    _LISTSERVERROLESRESPONSE._serialized_end = 1472
-    _LISTSERVERPERMISSIONSREQUEST._serialized_start = 1474
-    _LISTSERVERPERMISSIONSREQUEST._serialized_end = 1524
-    _LISTSERVERPERMISSIONSRESPONSE._serialized_start = 1526
-    _LISTSERVERPERMISSIONSRESPONSE._serialized_end = 1603
-    _LOGINREQUEST._serialized_start = 1605
-    _LOGINREQUEST._serialized_end = 1657
-    _LOGINRESPONSE._serialized_start = 1659
-    _LOGINRESPONSE._serialized_end = 1726
-    _USERS._serialized_start = 1850
-    _USERS._serialized_end = 3421
+    _DEFAULTSERVERROLE._serialized_start=1728
+    _DEFAULTSERVERROLE._serialized_end=1847
+    _USER._serialized_start=161
+    _USER._serialized_end=250
+    _USERINFO._serialized_start=253
+    _USERINFO._serialized_end=436
+    _USERINFO_PROJECTROLESENTRY._serialized_start=360
+    _USERINFO_PROJECTROLESENTRY._serialized_end=436
+    _CREATEUSERREQUEST._serialized_start=438
+    _CREATEUSERREQUEST._serialized_end=507
+    _UPDATEUSERREQUEST._serialized_start=509
+    _UPDATEUSERREQUEST._serialized_end=627
+    _GETUSERREQUEST._serialized_start=629
+    _GETUSERREQUEST._serialized_end=705
+    _DELETEUSERREQUEST._serialized_start=707
+    _DELETEUSERREQUEST._serialized_end=743
+    _LISTUSERSREQUEST._serialized_start=745
+    _LISTUSERSREQUEST._serialized_end=783
+    _LISTUSERSRESPONSE._serialized_start=785
+    _LISTUSERSRESPONSE._serialized_end=862
+    _LISTUSERINFOSRESPONSE._serialized_start=864
+    _LISTUSERINFOSRESPONSE._serialized_end=949
+    _SERVERROLE._serialized_start=951
+    _SERVERROLE._serialized_end=1015
+    _CREATESERVERROLEREQUEST._serialized_start=1017
+    _CREATESERVERROLEREQUEST._serialized_end=1080
+    _UPDATESERVERROLEREQUEST._serialized_start=1082
+    _UPDATESERVERROLEREQUEST._serialized_end=1194
+    _DELETESERVERROLEREQUEST._serialized_start=1196
+    _DELETESERVERROLEREQUEST._serialized_end=1238
+    _GETSERVERROLEREQUEST._serialized_start=1240
+    _GETSERVERROLEREQUEST._serialized_end=1328
+    _LISTSERVERROLESREQUEST._serialized_start=1330
+    _LISTSERVERROLESREQUEST._serialized_end=1374
+    _LISTSERVERROLESRESPONSE._serialized_start=1376
+    _LISTSERVERROLESRESPONSE._serialized_end=1472
+    _LISTSERVERPERMISSIONSREQUEST._serialized_start=1474
+    _LISTSERVERPERMISSIONSREQUEST._serialized_end=1524
+    _LISTSERVERPERMISSIONSRESPONSE._serialized_start=1526
+    _LISTSERVERPERMISSIONSRESPONSE._serialized_end=1603
+    _LOGINREQUEST._serialized_start=1605
+    _LOGINREQUEST._serialized_end=1657
+    _LOGINRESPONSE._serialized_start=1659
+    _LOGINRESPONSE._serialized_end=1726
+    _USERS._serialized_start=1850
+    _USERS._serialized_end=3421
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/user_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/utility_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/utility_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,56 +202,56 @@
 })
 _sym_db.RegisterMessage(AddTrainingPhrasesFromCSVRequest)
 
 _UTILITIES = DESCRIPTOR.services_by_name['Utilities']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _REANNOTATEENTITIESOPTIONS._serialized_start = 3640
-    _REANNOTATEENTITIESOPTIONS._serialized_end = 3811
-    _VALIDATEREGEXREQUEST._serialized_start = 95
-    _VALIDATEREGEXREQUEST._serialized_end = 132
-    _VALIDATEREGEXRESPONSE._serialized_start = 134
-    _VALIDATEREGEXRESPONSE._serialized_end = 181
-    _VALIDATEEMBEDDEDREGEXREQUEST._serialized_start = 183
-    _VALIDATEEMBEDDEDREGEXREQUEST._serialized_end = 265
-    _VALIDATEEMBEDDEDREGEXRESPONSE._serialized_start = 267
-    _VALIDATEEMBEDDEDREGEXRESPONSE._serialized_end = 322
-    _CLEANALLINTENTSREQUEST._serialized_start = 325
-    _CLEANALLINTENTSREQUEST._serialized_end = 649
-    _CLEANALLINTENTSRESPONSE._serialized_start = 651
-    _CLEANALLINTENTSRESPONSE._serialized_end = 775
-    _CLEANINTENTREQUEST._serialized_start = 778
-    _CLEANINTENTREQUEST._serialized_end = 1092
-    _CLEANINTENTRESPONSE._serialized_start = 1094
-    _CLEANINTENTRESPONSE._serialized_end = 1208
-    _TRAININGPHRASECLEANEROPTIONS._serialized_start = 1211
-    _TRAININGPHRASECLEANEROPTIONS._serialized_end = 1365
-    _STRINGUPDATE._serialized_start = 1367
-    _STRINGUPDATE._serialized_end = 1407
-    _INTENTUPDATE._serialized_start = 1410
-    _INTENTUPDATE._serialized_end = 1762
-    _INTENTUPDATE_TRAININGPHRASEUPDATE._serialized_start = 1568
-    _INTENTUPDATE_TRAININGPHRASEUPDATE._serialized_end = 1762
-    _ENTITYTYPEUPDATE._serialized_start = 1765
-    _ENTITYTYPEUPDATE._serialized_end = 2009
-    _ENTITYTYPEUPDATE_ENTITYUPDATE._serialized_start = 1882
-    _ENTITYTYPEUPDATE_ENTITYUPDATE._serialized_end = 2009
-    _CLEANALLENTITYTYPESREQUEST._serialized_start = 2012
-    _CLEANALLENTITYTYPESREQUEST._serialized_end = 2254
-    _CLEANALLENTITYTYPESRESPONSE._serialized_start = 2257
-    _CLEANALLENTITYTYPESRESPONSE._serialized_end = 2514
-    _CLEANENTITYTYPEREQUEST._serialized_start = 2517
-    _CLEANENTITYTYPEREQUEST._serialized_end = 2714
-    _CLEANENTITYTYPERESPONSE._serialized_start = 2717
-    _CLEANENTITYTYPERESPONSE._serialized_end = 2853
-    _ADDTRAININGPHRASESREQUEST._serialized_start = 2856
-    _ADDTRAININGPHRASESREQUEST._serialized_end = 3321
-    _ADDTRAININGPHRASESREQUEST_TRAININGPHRASEFORINTENT._serialized_start = 3182
-    _ADDTRAININGPHRASESREQUEST_TRAININGPHRASEFORINTENT._serialized_end = 3321
-    _ADDTRAININGPHRASESRESPONSE._serialized_start = 3323
-    _ADDTRAININGPHRASESRESPONSE._serialized_end = 3375
-    _ADDTRAININGPHRASESFROMCSVREQUEST._serialized_start = 3378
-    _ADDTRAININGPHRASESFROMCSVREQUEST._serialized_end = 3637
-    _UTILITIES._serialized_start = 3814
-    _UTILITIES._serialized_end = 4605
+    _REANNOTATEENTITIESOPTIONS._serialized_start=3640
+    _REANNOTATEENTITIESOPTIONS._serialized_end=3811
+    _VALIDATEREGEXREQUEST._serialized_start=95
+    _VALIDATEREGEXREQUEST._serialized_end=132
+    _VALIDATEREGEXRESPONSE._serialized_start=134
+    _VALIDATEREGEXRESPONSE._serialized_end=181
+    _VALIDATEEMBEDDEDREGEXREQUEST._serialized_start=183
+    _VALIDATEEMBEDDEDREGEXREQUEST._serialized_end=265
+    _VALIDATEEMBEDDEDREGEXRESPONSE._serialized_start=267
+    _VALIDATEEMBEDDEDREGEXRESPONSE._serialized_end=322
+    _CLEANALLINTENTSREQUEST._serialized_start=325
+    _CLEANALLINTENTSREQUEST._serialized_end=649
+    _CLEANALLINTENTSRESPONSE._serialized_start=651
+    _CLEANALLINTENTSRESPONSE._serialized_end=775
+    _CLEANINTENTREQUEST._serialized_start=778
+    _CLEANINTENTREQUEST._serialized_end=1092
+    _CLEANINTENTRESPONSE._serialized_start=1094
+    _CLEANINTENTRESPONSE._serialized_end=1208
+    _TRAININGPHRASECLEANEROPTIONS._serialized_start=1211
+    _TRAININGPHRASECLEANEROPTIONS._serialized_end=1365
+    _STRINGUPDATE._serialized_start=1367
+    _STRINGUPDATE._serialized_end=1407
+    _INTENTUPDATE._serialized_start=1410
+    _INTENTUPDATE._serialized_end=1762
+    _INTENTUPDATE_TRAININGPHRASEUPDATE._serialized_start=1568
+    _INTENTUPDATE_TRAININGPHRASEUPDATE._serialized_end=1762
+    _ENTITYTYPEUPDATE._serialized_start=1765
+    _ENTITYTYPEUPDATE._serialized_end=2009
+    _ENTITYTYPEUPDATE_ENTITYUPDATE._serialized_start=1882
+    _ENTITYTYPEUPDATE_ENTITYUPDATE._serialized_end=2009
+    _CLEANALLENTITYTYPESREQUEST._serialized_start=2012
+    _CLEANALLENTITYTYPESREQUEST._serialized_end=2254
+    _CLEANALLENTITYTYPESRESPONSE._serialized_start=2257
+    _CLEANALLENTITYTYPESRESPONSE._serialized_end=2514
+    _CLEANENTITYTYPEREQUEST._serialized_start=2517
+    _CLEANENTITYTYPEREQUEST._serialized_end=2714
+    _CLEANENTITYTYPERESPONSE._serialized_start=2717
+    _CLEANENTITYTYPERESPONSE._serialized_end=2853
+    _ADDTRAININGPHRASESREQUEST._serialized_start=2856
+    _ADDTRAININGPHRASESREQUEST._serialized_end=3321
+    _ADDTRAININGPHRASESREQUEST_TRAININGPHRASEFORINTENT._serialized_start=3182
+    _ADDTRAININGPHRASESREQUEST_TRAININGPHRASEFORINTENT._serialized_end=3321
+    _ADDTRAININGPHRASESRESPONSE._serialized_start=3323
+    _ADDTRAININGPHRASESRESPONSE._serialized_end=3375
+    _ADDTRAININGPHRASESFROMCSVREQUEST._serialized_start=3378
+    _ADDTRAININGPHRASESFROMCSVREQUEST._serialized_end=3637
+    _UTILITIES._serialized_start=3814
+    _UTILITIES._serialized_end=4605
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/utility_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/utility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/webhook_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/webhook_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,20 @@
     DESCRIPTOR._serialized_options = b'\n\036com.google.cloud.dialogflow.v2B\014WebhookProtoP\001ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\370\001\001\242\002\002DF\252\002\032Google.Cloud.Dialogflow.V2'
     _WEBHOOK.methods_by_name['ResponseRefinement']._options = None
     _WEBHOOK.methods_by_name['ResponseRefinement']._serialized_options = b'\202\323\344\223\002>\"9/{session=projects/*/agent/sessions/*}:responseRefinement:\001*'
     _WEBHOOK.methods_by_name['SlotFilling']._options = None
     _WEBHOOK.methods_by_name['SlotFilling']._serialized_options = b'\202\323\344\223\0027\"2/{session=projects/*/agent/sessions/*}:slotFilling:\001*'
     _WEBHOOK.methods_by_name['Ping']._options = None
     _WEBHOOK.methods_by_name['Ping']._serialized_options = b'\202\323\344\223\002 \022\036/projects/*/agent/webhook:ping'
-    _PINGREQUEST._serialized_start = 177
-    _PINGREQUEST._serialized_end = 207
-    _WEBHOOKREQUEST._serialized_start = 210
-    _WEBHOOKREQUEST._serialized_end = 434
-    _WEBHOOKRESPONSE._serialized_start = 437
-    _WEBHOOKRESPONSE._serialized_end = 696
-    _ORIGINALDETECTINTENTREQUEST._serialized_start = 698
-    _ORIGINALDETECTINTENTREQUEST._serialized_end = 785
-    _PINGRESPONSE._serialized_start = 787
-    _PINGRESPONSE._serialized_end = 823
-    _WEBHOOK._serialized_start = 826
-    _WEBHOOK._serialized_end = 1220
+    _PINGREQUEST._serialized_start=177
+    _PINGREQUEST._serialized_end=207
+    _WEBHOOKREQUEST._serialized_start=210
+    _WEBHOOKREQUEST._serialized_end=434
+    _WEBHOOKRESPONSE._serialized_start=437
+    _WEBHOOKRESPONSE._serialized_end=696
+    _ORIGINALDETECTINTENTREQUEST._serialized_start=698
+    _ORIGINALDETECTINTENTREQUEST._serialized_end=785
+    _PINGRESPONSE._serialized_start=787
+    _PINGRESPONSE._serialized_end=823
+    _WEBHOOK._serialized_start=826
+    _WEBHOOK._serialized_end=1220
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/nlu/webhook_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/nlu/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/qa/qa_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/qa/qa_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,36 +136,36 @@
     _QA.methods_by_name['RunTraining']._serialized_options = b'\202\323\344\223\002\021\022\017/qa:RunTraining'
     _QA.methods_by_name['GetServerState']._options = None
     _QA.methods_by_name['GetServerState']._serialized_options = b'\202\323\344\223\002\024\022\022/qa:GetServerState'
     _QA.methods_by_name['ListProjectIds']._options = None
     _QA.methods_by_name['ListProjectIds']._serialized_options = b'\202\323\344\223\002\024\022\022/qa:ListProjectIds'
     _QA.methods_by_name['GetProjectConfig']._options = None
     _QA.methods_by_name['GetProjectConfig']._serialized_options = b'\202\323\344\223\002\027\022\025/qa:ListProjectConfig'
-    _GETANSWERREQUEST._serialized_start = 119
-    _GETANSWERREQUEST._serialized_end = 370
-    _GETANSWERRESPONSE._serialized_start = 372
-    _GETANSWERRESPONSE._serialized_end = 447
-    _RUNSCRAPERREQUEST._serialized_start = 449
-    _RUNSCRAPERREQUEST._serialized_end = 489
-    _RUNSCRAPERRESPONSE._serialized_start = 492
-    _RUNSCRAPERRESPONSE._serialized_end = 654
-    _RUNSCRAPERRESPONSE_SCRAPERCONTAINER._serialized_start = 590
-    _RUNSCRAPERRESPONSE_SCRAPERCONTAINER._serialized_end = 654
-    _RUNTRAININGRESPONSE._serialized_start = 656
-    _RUNTRAININGRESPONSE._serialized_end = 707
-    _URLFILTER._serialized_start = 709
-    _URLFILTER._serialized_end = 804
-    _GETSERVERSTATERESPONSE._serialized_start = 806
-    _GETSERVERSTATERESPONSE._serialized_end = 855
-    _LISTPROJECTIDSRESPONSE._serialized_start = 857
-    _LISTPROJECTIDSRESPONSE._serialized_end = 902
-    _GETPROJECTCONFIGREQUEST._serialized_start = 904
-    _GETPROJECTCONFIGREQUEST._serialized_end = 949
-    _GETPROJECTCONFIGRESPONSE._serialized_start = 951
-    _GETPROJECTCONFIGRESPONSE._serialized_end = 1004
-    _UPDATEDATABASEREQUEST._serialized_start = 1006
-    _UPDATEDATABASEREQUEST._serialized_end = 1050
-    _UPDATEDATABASERESPONSE._serialized_start = 1052
-    _UPDATEDATABASERESPONSE._serialized_end = 1100
-    _QA._serialized_start = 1103
-    _QA._serialized_end = 1839
+    _GETANSWERREQUEST._serialized_start=119
+    _GETANSWERREQUEST._serialized_end=370
+    _GETANSWERRESPONSE._serialized_start=372
+    _GETANSWERRESPONSE._serialized_end=447
+    _RUNSCRAPERREQUEST._serialized_start=449
+    _RUNSCRAPERREQUEST._serialized_end=489
+    _RUNSCRAPERRESPONSE._serialized_start=492
+    _RUNSCRAPERRESPONSE._serialized_end=654
+    _RUNSCRAPERRESPONSE_SCRAPERCONTAINER._serialized_start=590
+    _RUNSCRAPERRESPONSE_SCRAPERCONTAINER._serialized_end=654
+    _RUNTRAININGRESPONSE._serialized_start=656
+    _RUNTRAININGRESPONSE._serialized_end=707
+    _URLFILTER._serialized_start=709
+    _URLFILTER._serialized_end=804
+    _GETSERVERSTATERESPONSE._serialized_start=806
+    _GETSERVERSTATERESPONSE._serialized_end=855
+    _LISTPROJECTIDSRESPONSE._serialized_start=857
+    _LISTPROJECTIDSRESPONSE._serialized_end=902
+    _GETPROJECTCONFIGREQUEST._serialized_start=904
+    _GETPROJECTCONFIGREQUEST._serialized_end=949
+    _GETPROJECTCONFIGRESPONSE._serialized_start=951
+    _GETPROJECTCONFIGRESPONSE._serialized_end=1004
+    _UPDATEDATABASEREQUEST._serialized_start=1006
+    _UPDATEDATABASEREQUEST._serialized_end=1050
+    _UPDATEDATABASERESPONSE._serialized_start=1052
+    _UPDATEDATABASERESPONSE._serialized_end=1100
+    _QA._serialized_start=1103
+    _QA._serialized_end=1839
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/qa/qa_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/qa/qa_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -429,114 +429,114 @@
 })
 _sym_db.RegisterMessage(TrainUserLanguageModelRequest)
 
 _SPEECH2TEXT = DESCRIPTOR.services_by_name['Speech2Text']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _DECODING._serialized_start = 6230
-    _DECODING._serialized_end = 6307
-    _INFERENCEBACKEND._serialized_start = 6309
-    _INFERENCEBACKEND._serialized_end = 6417
-    _TRANSCRIBEREQUESTCONFIG._serialized_start = 77
-    _TRANSCRIBEREQUESTCONFIG._serialized_end = 615
-    _TRANSCRIPTIONRETURNOPTIONS._serialized_start = 618
-    _TRANSCRIPTIONRETURNOPTIONS._serialized_end = 921
-    _UTTERANCEDETECTIONOPTIONS._serialized_start = 924
-    _UTTERANCEDETECTIONOPTIONS._serialized_end = 1115
-    _POSTPROCESSINGOPTIONS._serialized_start = 1117
-    _POSTPROCESSINGOPTIONS._serialized_end = 1232
-    _TRANSCRIPTION._serialized_start = 1235
-    _TRANSCRIPTION._serialized_end = 1398
-    _TRANSCRIPTIONALTERNATIVE._serialized_start = 1400
-    _TRANSCRIPTIONALTERNATIVE._serialized_end = 1505
-    _WORDDETAIL._serialized_start = 1508
-    _WORDDETAIL._serialized_end = 1648
-    _WORDALTERNATIVE._serialized_start = 1650
-    _WORDALTERNATIVE._serialized_end = 1701
-    _TRANSCRIBESTREAMREQUEST._serialized_start = 1704
-    _TRANSCRIBESTREAMREQUEST._serialized_end = 1846
-    _TRANSCRIBESTREAMRESPONSE._serialized_start = 1849
-    _TRANSCRIBESTREAMRESPONSE._serialized_end = 2108
-    _TRANSCRIBEFILEREQUEST._serialized_start = 2110
-    _TRANSCRIBEFILEREQUEST._serialized_end = 2206
-    _TRANSCRIBEFILERESPONSE._serialized_start = 2208
-    _TRANSCRIBEFILERESPONSE._serialized_end = 2317
-    _S2TPIPELINEID._serialized_start = 2319
-    _S2TPIPELINEID._serialized_end = 2346
-    _LISTS2TPIPELINESREQUEST._serialized_start = 2348
-    _LISTS2TPIPELINESREQUEST._serialized_end = 2459
-    _LISTS2TPIPELINESRESPONSE._serialized_start = 2461
-    _LISTS2TPIPELINESRESPONSE._serialized_end = 2544
-    _LISTS2TLANGUAGESREQUEST._serialized_start = 2546
-    _LISTS2TLANGUAGESREQUEST._serialized_end = 2613
-    _LISTS2TLANGUAGESRESPONSE._serialized_start = 2615
-    _LISTS2TLANGUAGESRESPONSE._serialized_end = 2660
-    _LISTS2TDOMAINSREQUEST._serialized_start = 2662
-    _LISTS2TDOMAINSREQUEST._serialized_end = 2729
-    _LISTS2TDOMAINSRESPONSE._serialized_start = 2731
-    _LISTS2TDOMAINSRESPONSE._serialized_end = 2772
-    _S2TGETSERVICEINFORESPONSE._serialized_start = 2774
-    _S2TGETSERVICEINFORESPONSE._serialized_end = 2818
-    _SPEECH2TEXTCONFIG._serialized_start = 2821
-    _SPEECH2TEXTCONFIG._serialized_end = 3178
-    _S2TDESCRIPTION._serialized_start = 3180
-    _S2TDESCRIPTION._serialized_end = 3272
-    _S2TINFERENCE._serialized_start = 3275
-    _S2TINFERENCE._serialized_end = 3452
-    _ACOUSTICMODELS._serialized_start = 3455
-    _ACOUSTICMODELS._serialized_end = 3760
-    _WHISPER._serialized_start = 3762
-    _WHISPER._serialized_end = 3826
-    _WHISPERTRITON._serialized_start = 3828
-    _WHISPERTRITON._serialized_end = 3954
-    _WAV2VEC._serialized_start = 3956
-    _WAV2VEC._serialized_end = 4002
-    _WAV2VECTRITON._serialized_start = 4004
-    _WAV2VECTRITON._serialized_end = 4130
-    _QUARTZNET._serialized_start = 4133
-    _QUARTZNET._serialized_end = 4281
-    _PTFILES._serialized_start = 4283
-    _PTFILES._serialized_end = 4320
-    _CKPTFILE._serialized_start = 4322
-    _CKPTFILE._serialized_end = 4346
-    _QUARTZNETTRITON._serialized_start = 4348
-    _QUARTZNETTRITON._serialized_end = 4428
-    _LANGUAGEMODELS._serialized_start = 4431
-    _LANGUAGEMODELS._serialized_end = 4567
-    _STREAMINGSERVER._serialized_start = 4570
-    _STREAMINGSERVER._serialized_end = 4715
-    _STREAMINGSPEECHRECOGNITION._serialized_start = 4718
-    _STREAMINGSPEECHRECOGNITION._serialized_end = 4956
-    _VOICEACTIVITYDETECTION._serialized_start = 4959
-    _VOICEACTIVITYDETECTION._serialized_end = 5102
-    _PYANNOTE._serialized_start = 5105
-    _PYANNOTE._serialized_end = 5281
-    _MATCHBOX._serialized_start = 5283
-    _MATCHBOX._serialized_end = 5359
-    _POSTPROCESSING._serialized_start = 5361
-    _POSTPROCESSING._serialized_end = 5448
-    _POSTPROCESSORS._serialized_start = 5450
-    _POSTPROCESSORS._serialized_end = 5560
-    _SYMSPELL._serialized_start = 5562
-    _SYMSPELL._serialized_end = 5652
-    _S2TNORMALIZATION._serialized_start = 5654
-    _S2TNORMALIZATION._serialized_end = 5690
-    _LOGGING._serialized_start = 5692
-    _LOGGING._serialized_end = 5729
-    _LISTS2TLANGUAGEMODELSREQUEST._serialized_start = 5731
-    _LISTS2TLANGUAGEMODELSREQUEST._serialized_end = 5774
-    _LANGUAGEMODELPIPELINEID._serialized_start = 5776
-    _LANGUAGEMODELPIPELINEID._serialized_end = 5843
-    _LISTS2TLANGUAGEMODELSRESPONSE._serialized_start = 5845
-    _LISTS2TLANGUAGEMODELSRESPONSE._serialized_end = 5938
-    _CREATEUSERLANGUAGEMODELREQUEST._serialized_start = 5940
-    _CREATEUSERLANGUAGEMODELREQUEST._serialized_end = 6001
-    _DELETEUSERLANGUAGEMODELREQUEST._serialized_start = 6003
-    _DELETEUSERLANGUAGEMODELREQUEST._serialized_end = 6064
-    _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_start = 6066
-    _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_end = 6151
-    _TRAINUSERLANGUAGEMODELREQUEST._serialized_start = 6153
-    _TRAINUSERLANGUAGEMODELREQUEST._serialized_end = 6228
-    _SPEECH2TEXT._serialized_start = 6420
-    _SPEECH2TEXT._serialized_end = 7808
+    _DECODING._serialized_start=6230
+    _DECODING._serialized_end=6307
+    _INFERENCEBACKEND._serialized_start=6309
+    _INFERENCEBACKEND._serialized_end=6417
+    _TRANSCRIBEREQUESTCONFIG._serialized_start=77
+    _TRANSCRIBEREQUESTCONFIG._serialized_end=615
+    _TRANSCRIPTIONRETURNOPTIONS._serialized_start=618
+    _TRANSCRIPTIONRETURNOPTIONS._serialized_end=921
+    _UTTERANCEDETECTIONOPTIONS._serialized_start=924
+    _UTTERANCEDETECTIONOPTIONS._serialized_end=1115
+    _POSTPROCESSINGOPTIONS._serialized_start=1117
+    _POSTPROCESSINGOPTIONS._serialized_end=1232
+    _TRANSCRIPTION._serialized_start=1235
+    _TRANSCRIPTION._serialized_end=1398
+    _TRANSCRIPTIONALTERNATIVE._serialized_start=1400
+    _TRANSCRIPTIONALTERNATIVE._serialized_end=1505
+    _WORDDETAIL._serialized_start=1508
+    _WORDDETAIL._serialized_end=1648
+    _WORDALTERNATIVE._serialized_start=1650
+    _WORDALTERNATIVE._serialized_end=1701
+    _TRANSCRIBESTREAMREQUEST._serialized_start=1704
+    _TRANSCRIBESTREAMREQUEST._serialized_end=1846
+    _TRANSCRIBESTREAMRESPONSE._serialized_start=1849
+    _TRANSCRIBESTREAMRESPONSE._serialized_end=2108
+    _TRANSCRIBEFILEREQUEST._serialized_start=2110
+    _TRANSCRIBEFILEREQUEST._serialized_end=2206
+    _TRANSCRIBEFILERESPONSE._serialized_start=2208
+    _TRANSCRIBEFILERESPONSE._serialized_end=2317
+    _S2TPIPELINEID._serialized_start=2319
+    _S2TPIPELINEID._serialized_end=2346
+    _LISTS2TPIPELINESREQUEST._serialized_start=2348
+    _LISTS2TPIPELINESREQUEST._serialized_end=2459
+    _LISTS2TPIPELINESRESPONSE._serialized_start=2461
+    _LISTS2TPIPELINESRESPONSE._serialized_end=2544
+    _LISTS2TLANGUAGESREQUEST._serialized_start=2546
+    _LISTS2TLANGUAGESREQUEST._serialized_end=2613
+    _LISTS2TLANGUAGESRESPONSE._serialized_start=2615
+    _LISTS2TLANGUAGESRESPONSE._serialized_end=2660
+    _LISTS2TDOMAINSREQUEST._serialized_start=2662
+    _LISTS2TDOMAINSREQUEST._serialized_end=2729
+    _LISTS2TDOMAINSRESPONSE._serialized_start=2731
+    _LISTS2TDOMAINSRESPONSE._serialized_end=2772
+    _S2TGETSERVICEINFORESPONSE._serialized_start=2774
+    _S2TGETSERVICEINFORESPONSE._serialized_end=2818
+    _SPEECH2TEXTCONFIG._serialized_start=2821
+    _SPEECH2TEXTCONFIG._serialized_end=3178
+    _S2TDESCRIPTION._serialized_start=3180
+    _S2TDESCRIPTION._serialized_end=3272
+    _S2TINFERENCE._serialized_start=3275
+    _S2TINFERENCE._serialized_end=3452
+    _ACOUSTICMODELS._serialized_start=3455
+    _ACOUSTICMODELS._serialized_end=3760
+    _WHISPER._serialized_start=3762
+    _WHISPER._serialized_end=3826
+    _WHISPERTRITON._serialized_start=3828
+    _WHISPERTRITON._serialized_end=3954
+    _WAV2VEC._serialized_start=3956
+    _WAV2VEC._serialized_end=4002
+    _WAV2VECTRITON._serialized_start=4004
+    _WAV2VECTRITON._serialized_end=4130
+    _QUARTZNET._serialized_start=4133
+    _QUARTZNET._serialized_end=4281
+    _PTFILES._serialized_start=4283
+    _PTFILES._serialized_end=4320
+    _CKPTFILE._serialized_start=4322
+    _CKPTFILE._serialized_end=4346
+    _QUARTZNETTRITON._serialized_start=4348
+    _QUARTZNETTRITON._serialized_end=4428
+    _LANGUAGEMODELS._serialized_start=4431
+    _LANGUAGEMODELS._serialized_end=4567
+    _STREAMINGSERVER._serialized_start=4570
+    _STREAMINGSERVER._serialized_end=4715
+    _STREAMINGSPEECHRECOGNITION._serialized_start=4718
+    _STREAMINGSPEECHRECOGNITION._serialized_end=4956
+    _VOICEACTIVITYDETECTION._serialized_start=4959
+    _VOICEACTIVITYDETECTION._serialized_end=5102
+    _PYANNOTE._serialized_start=5105
+    _PYANNOTE._serialized_end=5281
+    _MATCHBOX._serialized_start=5283
+    _MATCHBOX._serialized_end=5359
+    _POSTPROCESSING._serialized_start=5361
+    _POSTPROCESSING._serialized_end=5448
+    _POSTPROCESSORS._serialized_start=5450
+    _POSTPROCESSORS._serialized_end=5560
+    _SYMSPELL._serialized_start=5562
+    _SYMSPELL._serialized_end=5652
+    _S2TNORMALIZATION._serialized_start=5654
+    _S2TNORMALIZATION._serialized_end=5690
+    _LOGGING._serialized_start=5692
+    _LOGGING._serialized_end=5729
+    _LISTS2TLANGUAGEMODELSREQUEST._serialized_start=5731
+    _LISTS2TLANGUAGEMODELSREQUEST._serialized_end=5774
+    _LANGUAGEMODELPIPELINEID._serialized_start=5776
+    _LANGUAGEMODELPIPELINEID._serialized_end=5843
+    _LISTS2TLANGUAGEMODELSRESPONSE._serialized_start=5845
+    _LISTS2TLANGUAGEMODELSRESPONSE._serialized_end=5938
+    _CREATEUSERLANGUAGEMODELREQUEST._serialized_start=5940
+    _CREATEUSERLANGUAGEMODELREQUEST._serialized_end=6001
+    _DELETEUSERLANGUAGEMODELREQUEST._serialized_start=6003
+    _DELETEUSERLANGUAGEMODELREQUEST._serialized_end=6064
+    _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_start=6066
+    _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_end=6151
+    _TRAINUSERLANGUAGEMODELREQUEST._serialized_start=6153
+    _TRAINUSERLANGUAGEMODELREQUEST._serialized_end=6228
+    _SPEECH2TEXT._serialized_start=6420
+    _SPEECH2TEXT._serialized_end=7808
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/s2t/speech_to_text_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/sip/sip_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/sip/sip_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,34 +112,34 @@
     DESCRIPTOR._options = None
     _SIPSTARTCALLREQUEST_HEADERSENTRY._options = None
     _SIPSTARTCALLREQUEST_HEADERSENTRY._serialized_options = b'8\001'
     _SIPTRANSFERCALLREQUEST_HEADERSENTRY._options = None
     _SIPTRANSFERCALLREQUEST_HEADERSENTRY._serialized_options = b'8\001'
     _SIPSTATUS_HEADERSENTRY._options = None
     _SIPSTATUS_HEADERSENTRY._serialized_options = b'8\001'
-    _SIPENDCALLREQUEST._serialized_start = 98
-    _SIPENDCALLREQUEST._serialized_end = 138
-    _SIPSTARTCALLREQUEST._serialized_start = 141
-    _SIPSTARTCALLREQUEST._serialized_end = 292
-    _SIPSTARTCALLREQUEST_HEADERSENTRY._serialized_start = 246
-    _SIPSTARTCALLREQUEST_HEADERSENTRY._serialized_end = 292
-    _SIPREGISTERACCOUNTREQUEST._serialized_start = 294
-    _SIPREGISTERACCOUNTREQUEST._serialized_end = 408
-    _SIPSTARTSESSIONREQUEST._serialized_start = 410
-    _SIPSTARTSESSIONREQUEST._serialized_end = 486
-    _SIPTRANSFERCALLREQUEST._serialized_start = 489
-    _SIPTRANSFERCALLREQUEST._serialized_end = 648
-    _SIPTRANSFERCALLREQUEST_HEADERSENTRY._serialized_start = 246
-    _SIPTRANSFERCALLREQUEST_HEADERSENTRY._serialized_end = 292
-    _SIPSTATUS._serialized_start = 651
-    _SIPSTATUS._serialized_end = 1570
-    _SIPSTATUS_HEADERSENTRY._serialized_start = 246
-    _SIPSTATUS_HEADERSENTRY._serialized_end = 292
-    _SIPSTATUS_STATUSTYPE._serialized_start = 1009
-    _SIPSTATUS_STATUSTYPE._serialized_end = 1570
-    _SIPSTATUSHISTORYRESPONSE._serialized_start = 1572
-    _SIPSTATUSHISTORYRESPONSE._serialized_end = 1645
-    _SIPPLAYWAVFILESREQUEST._serialized_start = 1647
-    _SIPPLAYWAVFILESREQUEST._serialized_end = 1690
-    _SIP._serialized_start = 1693
-    _SIP._serialized_end = 2514
+    _SIPENDCALLREQUEST._serialized_start=98
+    _SIPENDCALLREQUEST._serialized_end=138
+    _SIPSTARTCALLREQUEST._serialized_start=141
+    _SIPSTARTCALLREQUEST._serialized_end=292
+    _SIPSTARTCALLREQUEST_HEADERSENTRY._serialized_start=246
+    _SIPSTARTCALLREQUEST_HEADERSENTRY._serialized_end=292
+    _SIPREGISTERACCOUNTREQUEST._serialized_start=294
+    _SIPREGISTERACCOUNTREQUEST._serialized_end=408
+    _SIPSTARTSESSIONREQUEST._serialized_start=410
+    _SIPSTARTSESSIONREQUEST._serialized_end=486
+    _SIPTRANSFERCALLREQUEST._serialized_start=489
+    _SIPTRANSFERCALLREQUEST._serialized_end=648
+    _SIPTRANSFERCALLREQUEST_HEADERSENTRY._serialized_start=246
+    _SIPTRANSFERCALLREQUEST_HEADERSENTRY._serialized_end=292
+    _SIPSTATUS._serialized_start=651
+    _SIPSTATUS._serialized_end=1570
+    _SIPSTATUS_HEADERSENTRY._serialized_start=246
+    _SIPSTATUS_HEADERSENTRY._serialized_end=292
+    _SIPSTATUS_STATUSTYPE._serialized_start=1009
+    _SIPSTATUS_STATUSTYPE._serialized_end=1570
+    _SIPSTATUSHISTORYRESPONSE._serialized_start=1572
+    _SIPSTATUSHISTORYRESPONSE._serialized_end=1645
+    _SIPPLAYWAVFILESREQUEST._serialized_start=1647
+    _SIPPLAYWAVFILESREQUEST._serialized_end=1690
+    _SIP._serialized_start=1693
+    _SIP._serialized_end=2514
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/sip/sip_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/sip/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/t2s/text_to_speech_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/t2s/text_to_speech_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -358,98 +358,98 @@
 _sym_db.RegisterMessage(CreateCustomPhonemizerRequest)
 
 _TEXT2SPEECH = DESCRIPTOR.services_by_name['Text2Speech']
 _CUSTOMPHONEMIZERS = DESCRIPTOR.services_by_name['CustomPhonemizers']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _PCM._serialized_start = 4624
-    _PCM._serialized_end = 4712
-    _AUDIOFORMAT._serialized_start = 4714
-    _AUDIOFORMAT._serialized_end = 4791
-    _SYNTHESIZEREQUEST._serialized_start = 76
-    _SYNTHESIZEREQUEST._serialized_end = 152
-    _BATCHSYNTHESIZEREQUEST._serialized_start = 154
-    _BATCHSYNTHESIZEREQUEST._serialized_end = 232
-    _BATCHSYNTHESIZERESPONSE._serialized_start = 234
-    _BATCHSYNTHESIZERESPONSE._serialized_end = 315
-    _REQUESTCONFIG._serialized_start = 318
-    _REQUESTCONFIG._serialized_end = 689
-    _SYNTHESIZERESPONSE._serialized_start = 692
-    _SYNTHESIZERESPONSE._serialized_end = 876
-    _NORMALIZETEXTREQUEST._serialized_start = 878
-    _NORMALIZETEXTREQUEST._serialized_end = 939
-    _NORMALIZETEXTRESPONSE._serialized_start = 941
-    _NORMALIZETEXTRESPONSE._serialized_end = 989
-    _T2SGETSERVICEINFORESPONSE._serialized_start = 991
-    _T2SGETSERVICEINFORESPONSE._serialized_end = 1035
-    _LISTT2SPIPELINESREQUEST._serialized_start = 1038
-    _LISTT2SPIPELINESREQUEST._serialized_end = 1170
-    _LISTT2SPIPELINESRESPONSE._serialized_start = 1172
-    _LISTT2SPIPELINESRESPONSE._serialized_end = 1248
-    _LISTT2SLANGUAGESREQUEST._serialized_start = 1250
-    _LISTT2SLANGUAGESREQUEST._serialized_end = 1363
-    _LISTT2SLANGUAGESRESPONSE._serialized_start = 1365
-    _LISTT2SLANGUAGESRESPONSE._serialized_end = 1410
-    _LISTT2SDOMAINSREQUEST._serialized_start = 1412
-    _LISTT2SDOMAINSREQUEST._serialized_end = 1525
-    _LISTT2SDOMAINSRESPONSE._serialized_start = 1527
-    _LISTT2SDOMAINSRESPONSE._serialized_end = 1568
-    _T2SPIPELINEID._serialized_start = 1570
-    _T2SPIPELINEID._serialized_end = 1597
-    _TEXT2SPEECHCONFIG._serialized_start = 1600
-    _TEXT2SPEECHCONFIG._serialized_end = 1846
-    _T2SDESCRIPTION._serialized_start = 1849
-    _T2SDESCRIPTION._serialized_end = 1984
-    _T2SINFERENCE._serialized_start = 1986
-    _T2SINFERENCE._serialized_end = 2113
-    _COMPOSITEINFERENCE._serialized_start = 2115
-    _COMPOSITEINFERENCE._serialized_end = 2217
-    _TEXT2MEL._serialized_start = 2219
-    _TEXT2MEL._serialized_end = 2334
-    _GLOWTTS._serialized_start = 2337
-    _GLOWTTS._serialized_end = 2485
-    _GLOWTTSTRITON._serialized_start = 2488
-    _GLOWTTSTRITON._serialized_end = 2663
-    _MEL2AUDIO._serialized_start = 2666
-    _MEL2AUDIO._serialized_end = 2836
-    _HIFIGAN._serialized_start = 2838
-    _HIFIGAN._serialized_end = 2925
-    _HIFIGANTRITON._serialized_start = 2927
-    _HIFIGANTRITON._serialized_end = 2990
-    _MBMELGANTRITON._serialized_start = 2992
-    _MBMELGANTRITON._serialized_end = 3096
-    _CACHING._serialized_start = 3099
-    _CACHING._serialized_end = 3242
-    _T2SNORMALIZATION._serialized_start = 3245
-    _T2SNORMALIZATION._serialized_end = 3471
-    _POSTPROCESSING._serialized_start = 3474
-    _POSTPROCESSING._serialized_end = 3650
-    _LOGMNSE._serialized_start = 3652
-    _LOGMNSE._serialized_end = 3730
-    _WIENER._serialized_start = 3732
-    _WIENER._serialized_end = 3829
-    _APODIZATION._serialized_start = 3831
-    _APODIZATION._serialized_end = 3870
-    _T2SCUSTOMLENGTHSCALES._serialized_start = 3873
-    _T2SCUSTOMLENGTHSCALES._serialized_end = 4041
-    _PHONEMIZERID._serialized_start = 4043
-    _PHONEMIZERID._serialized_end = 4069
-    _CUSTOMPHONEMIZERPROTO._serialized_start = 4071
-    _CUSTOMPHONEMIZERPROTO._serialized_end = 4137
-    _MAP._serialized_start = 4139
-    _MAP._serialized_end = 4182
-    _LISTCUSTOMPHONEMIZERRESPONSE._serialized_start = 4184
-    _LISTCUSTOMPHONEMIZERRESPONSE._serialized_end = 4270
-    _LISTCUSTOMPHONEMIZERREQUEST._serialized_start = 4272
-    _LISTCUSTOMPHONEMIZERREQUEST._serialized_end = 4323
-    _UPDATECUSTOMPHONEMIZERREQUEST._serialized_start = 4326
-    _UPDATECUSTOMPHONEMIZERREQUEST._serialized_end = 4542
-    _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_start = 4481
-    _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_end = 4542
-    _CREATECUSTOMPHONEMIZERREQUEST._serialized_start = 4544
-    _CREATECUSTOMPHONEMIZERREQUEST._serialized_end = 4622
-    _TEXT2SPEECH._serialized_start = 4794
-    _TEXT2SPEECH._serialized_end = 5747
-    _CUSTOMPHONEMIZERS._serialized_start = 5750
-    _CUSTOMPHONEMIZERS._serialized_end = 6245
+    _PCM._serialized_start=4624
+    _PCM._serialized_end=4712
+    _AUDIOFORMAT._serialized_start=4714
+    _AUDIOFORMAT._serialized_end=4791
+    _SYNTHESIZEREQUEST._serialized_start=76
+    _SYNTHESIZEREQUEST._serialized_end=152
+    _BATCHSYNTHESIZEREQUEST._serialized_start=154
+    _BATCHSYNTHESIZEREQUEST._serialized_end=232
+    _BATCHSYNTHESIZERESPONSE._serialized_start=234
+    _BATCHSYNTHESIZERESPONSE._serialized_end=315
+    _REQUESTCONFIG._serialized_start=318
+    _REQUESTCONFIG._serialized_end=689
+    _SYNTHESIZERESPONSE._serialized_start=692
+    _SYNTHESIZERESPONSE._serialized_end=876
+    _NORMALIZETEXTREQUEST._serialized_start=878
+    _NORMALIZETEXTREQUEST._serialized_end=939
+    _NORMALIZETEXTRESPONSE._serialized_start=941
+    _NORMALIZETEXTRESPONSE._serialized_end=989
+    _T2SGETSERVICEINFORESPONSE._serialized_start=991
+    _T2SGETSERVICEINFORESPONSE._serialized_end=1035
+    _LISTT2SPIPELINESREQUEST._serialized_start=1038
+    _LISTT2SPIPELINESREQUEST._serialized_end=1170
+    _LISTT2SPIPELINESRESPONSE._serialized_start=1172
+    _LISTT2SPIPELINESRESPONSE._serialized_end=1248
+    _LISTT2SLANGUAGESREQUEST._serialized_start=1250
+    _LISTT2SLANGUAGESREQUEST._serialized_end=1363
+    _LISTT2SLANGUAGESRESPONSE._serialized_start=1365
+    _LISTT2SLANGUAGESRESPONSE._serialized_end=1410
+    _LISTT2SDOMAINSREQUEST._serialized_start=1412
+    _LISTT2SDOMAINSREQUEST._serialized_end=1525
+    _LISTT2SDOMAINSRESPONSE._serialized_start=1527
+    _LISTT2SDOMAINSRESPONSE._serialized_end=1568
+    _T2SPIPELINEID._serialized_start=1570
+    _T2SPIPELINEID._serialized_end=1597
+    _TEXT2SPEECHCONFIG._serialized_start=1600
+    _TEXT2SPEECHCONFIG._serialized_end=1846
+    _T2SDESCRIPTION._serialized_start=1849
+    _T2SDESCRIPTION._serialized_end=1984
+    _T2SINFERENCE._serialized_start=1986
+    _T2SINFERENCE._serialized_end=2113
+    _COMPOSITEINFERENCE._serialized_start=2115
+    _COMPOSITEINFERENCE._serialized_end=2217
+    _TEXT2MEL._serialized_start=2219
+    _TEXT2MEL._serialized_end=2334
+    _GLOWTTS._serialized_start=2337
+    _GLOWTTS._serialized_end=2485
+    _GLOWTTSTRITON._serialized_start=2488
+    _GLOWTTSTRITON._serialized_end=2663
+    _MEL2AUDIO._serialized_start=2666
+    _MEL2AUDIO._serialized_end=2836
+    _HIFIGAN._serialized_start=2838
+    _HIFIGAN._serialized_end=2925
+    _HIFIGANTRITON._serialized_start=2927
+    _HIFIGANTRITON._serialized_end=2990
+    _MBMELGANTRITON._serialized_start=2992
+    _MBMELGANTRITON._serialized_end=3096
+    _CACHING._serialized_start=3099
+    _CACHING._serialized_end=3242
+    _T2SNORMALIZATION._serialized_start=3245
+    _T2SNORMALIZATION._serialized_end=3471
+    _POSTPROCESSING._serialized_start=3474
+    _POSTPROCESSING._serialized_end=3650
+    _LOGMNSE._serialized_start=3652
+    _LOGMNSE._serialized_end=3730
+    _WIENER._serialized_start=3732
+    _WIENER._serialized_end=3829
+    _APODIZATION._serialized_start=3831
+    _APODIZATION._serialized_end=3870
+    _T2SCUSTOMLENGTHSCALES._serialized_start=3873
+    _T2SCUSTOMLENGTHSCALES._serialized_end=4041
+    _PHONEMIZERID._serialized_start=4043
+    _PHONEMIZERID._serialized_end=4069
+    _CUSTOMPHONEMIZERPROTO._serialized_start=4071
+    _CUSTOMPHONEMIZERPROTO._serialized_end=4137
+    _MAP._serialized_start=4139
+    _MAP._serialized_end=4182
+    _LISTCUSTOMPHONEMIZERRESPONSE._serialized_start=4184
+    _LISTCUSTOMPHONEMIZERRESPONSE._serialized_end=4270
+    _LISTCUSTOMPHONEMIZERREQUEST._serialized_start=4272
+    _LISTCUSTOMPHONEMIZERREQUEST._serialized_end=4323
+    _UPDATECUSTOMPHONEMIZERREQUEST._serialized_start=4326
+    _UPDATECUSTOMPHONEMIZERREQUEST._serialized_end=4542
+    _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_start=4481
+    _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_end=4542
+    _CREATECUSTOMPHONEMIZERREQUEST._serialized_start=4544
+    _CREATECUSTOMPHONEMIZERREQUEST._serialized_end=4622
+    _TEXT2SPEECH._serialized_start=4794
+    _TEXT2SPEECH._serialized_end=5747
+    _CUSTOMPHONEMIZERS._serialized_start=5750
+    _CUSTOMPHONEMIZERS._serialized_end=6245
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/t2s/text_to_speech_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/t2s/text_to_speech_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/vtsi/calls_pb2.py` & `ondewo-vtsi-client-6.3.0/ondewo/vtsi/calls_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -475,124 +475,124 @@
 
 _CALLS = DESCRIPTOR.services_by_name['Calls']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
     _SIPCALLERCONFIG_SIPHEADERSENTRY._options = None
     _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_options = b'8\001'
-    _CALLINFOVIEW._serialized_start = 7594
-    _CALLINFOVIEW._serialized_end = 7631
-    _CALLTYPE._serialized_start = 7633
-    _CALLTYPE._serialized_end = 7679
-    _BASESERVICECONFIG._serialized_start = 246
-    _BASESERVICECONFIG._serialized_end = 312
-    _CREDENTIALS._serialized_start = 314
-    _CREDENTIALS._serialized_end = 367
-    _NLUVTSICONFIG._serialized_start = 370
-    _NLUVTSICONFIG._serialized_end = 668
-    _T2SVTSICONFIG._serialized_start = 670
-    _T2SVTSICONFIG._serialized_end = 797
-    _S2TVTSICONFIG._serialized_start = 800
-    _S2TVTSICONFIG._serialized_end = 948
-    _ASTERISKCONFIG._serialized_start = 950
-    _ASTERISKCONFIG._serialized_end = 1028
-    _COMMONSERVICESCONFIG._serialized_start = 1031
-    _COMMONSERVICESCONFIG._serialized_end = 1265
-    _SIPBASECONFIG._serialized_start = 1267
-    _SIPBASECONFIG._serialized_end = 1307
-    _SIPCALLERCONFIG._serialized_start = 1310
-    _SIPCALLERCONFIG._serialized_end = 1517
-    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_start = 1468
-    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_end = 1517
-    _CSIVTSICONFIG._serialized_start = 1520
-    _CSIVTSICONFIG._serialized_end = 1886
-    _AUDIOOBJECTSTORAGECONFIG._serialized_start = 1889
-    _AUDIOOBJECTSTORAGECONFIG._serialized_end = 2142
-    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_start = 2144
-    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_end = 2232
-    _MESSAGEBROKERCONFIG._serialized_start = 2235
-    _MESSAGEBROKERCONFIG._serialized_end = 2474
-    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_start = 2476
-    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_end = 2603
-    _RABBITMQCONFIG._serialized_start = 2605
-    _RABBITMQCONFIG._serialized_end = 2697
-    _MINIOCONFIG._serialized_start = 2699
-    _MINIOCONFIG._serialized_end = 2819
-    _S2TVTSICALLBACKS._serialized_start = 2821
-    _S2TVTSICALLBACKS._serialized_end = 2894
-    _NLUVTSICALLBACKS._serialized_start = 2896
-    _NLUVTSICALLBACKS._serialized_end = 2969
-    _T2SVTSICALLBACKS._serialized_start = 2971
-    _T2SVTSICALLBACKS._serialized_end = 3044
-    _LISTENER._serialized_start = 3047
-    _LISTENER._serialized_end = 3210
-    _CALLER._serialized_start = 3213
-    _CALLER._serialized_end = 3378
-    _STARTLISTENERREQUEST._serialized_start = 3381
-    _STARTLISTENERREQUEST._serialized_end = 3550
-    _STARTLISTENERRESPONSE._serialized_start = 3552
-    _STARTLISTENERRESPONSE._serialized_end = 3666
-    _STARTLISTENERSREQUEST._serialized_start = 3668
-    _STARTLISTENERSREQUEST._serialized_end = 3780
-    _STARTLISTENERSRESPONSE._serialized_start = 3783
-    _STARTLISTENERSRESPONSE._serialized_end = 3921
-    _STARTCALLERREQUEST._serialized_start = 3924
-    _STARTCALLERREQUEST._serialized_end = 4095
-    _STARTCALLERRESPONSE._serialized_start = 4097
-    _STARTCALLERRESPONSE._serialized_end = 4205
-    _STARTCALLERSREQUEST._serialized_start = 4207
-    _STARTCALLERSREQUEST._serialized_end = 4313
-    _STARTCALLERSRESPONSE._serialized_start = 4316
-    _STARTCALLERSRESPONSE._serialized_end = 4448
-    _STARTSCHEDULEDCALLERREQUEST._serialized_start = 4451
-    _STARTSCHEDULEDCALLERREQUEST._serialized_end = 4609
-    _STARTSCHEDULEDCALLERSREQUEST._serialized_start = 4612
-    _STARTSCHEDULEDCALLERSREQUEST._serialized_end = 4746
-    _STARTSCHEDULEDCALLERSRESPONSE._serialized_start = 4749
-    _STARTSCHEDULEDCALLERSRESPONSE._serialized_end = 4886
-    _STARTSCHEDULEDCALLERRESPONSE._serialized_start = 4889
-    _STARTSCHEDULEDCALLERRESPONSE._serialized_end = 5025
-    _SCHEDULEDCALLER._serialized_start = 5028
-    _SCHEDULEDCALLER._serialized_end = 5245
-    _STOPCALLREQUEST._serialized_start = 5247
-    _STOPCALLREQUEST._serialized_end = 5310
-    _STOPCALLRESPONSE._serialized_start = 5312
-    _STOPCALLRESPONSE._serialized_end = 5399
-    _STOPCALLSREQUEST._serialized_start = 5401
-    _STOPCALLSREQUEST._serialized_end = 5466
-    _STOPCALLSRESPONSE._serialized_start = 5468
-    _STOPCALLSRESPONSE._serialized_end = 5570
-    _STOPALLCALLSREQUEST._serialized_start = 5572
-    _STOPALLCALLSREQUEST._serialized_end = 5620
-    _TRANSFERCALLREQUEST._serialized_start = 5622
-    _TRANSFERCALLREQUEST._serialized_end = 5710
-    _TRANSFERCALLRESPONSE._serialized_start = 5712
-    _TRANSFERCALLRESPONSE._serialized_end = 5824
-    _TRANSFERCALLSREQUEST._serialized_start = 5826
-    _TRANSFERCALLSREQUEST._serialized_end = 5941
-    _TRANSFERCALLSRESPONSE._serialized_start = 5944
-    _TRANSFERCALLSRESPONSE._serialized_end = 6085
-    _GETCALLINFOREQUEST._serialized_start = 6087
-    _GETCALLINFOREQUEST._serialized_end = 6204
-    _GETCALLINFORESPONSE._serialized_start = 6206
-    _GETCALLINFORESPONSE._serialized_end = 6312
-    _CALLINFO._serialized_start = 6315
-    _CALLINFO._serialized_end = 6717
-    _LISTCALLINFOREQUEST._serialized_start = 6720
-    _LISTCALLINFOREQUEST._serialized_end = 6861
-    _LISTCALLINFORESPONSE._serialized_start = 6863
-    _LISTCALLINFORESPONSE._serialized_end = 6928
-    _ALLSERVICESSTATUSES._serialized_start = 6931
-    _ALLSERVICESSTATUSES._serialized_end = 7197
-    _SERVICESTATUS._serialized_start = 7199
-    _SERVICESTATUS._serialized_end = 7254
-    _GETAUDIOFILEREQUEST._serialized_start = 7256
-    _GETAUDIOFILEREQUEST._serialized_end = 7367
-    _GETAUDIOFILERESPONSE._serialized_start = 7369
-    _GETAUDIOFILERESPONSE._serialized_end = 7406
-    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_start = 7409
-    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_end = 7537
-    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_start = 7539
-    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_end = 7592
-    _CALLS._serialized_start = 7682
-    _CALLS._serialized_end = 9048
+    _CALLINFOVIEW._serialized_start=7594
+    _CALLINFOVIEW._serialized_end=7631
+    _CALLTYPE._serialized_start=7633
+    _CALLTYPE._serialized_end=7679
+    _BASESERVICECONFIG._serialized_start=246
+    _BASESERVICECONFIG._serialized_end=312
+    _CREDENTIALS._serialized_start=314
+    _CREDENTIALS._serialized_end=367
+    _NLUVTSICONFIG._serialized_start=370
+    _NLUVTSICONFIG._serialized_end=668
+    _T2SVTSICONFIG._serialized_start=670
+    _T2SVTSICONFIG._serialized_end=797
+    _S2TVTSICONFIG._serialized_start=800
+    _S2TVTSICONFIG._serialized_end=948
+    _ASTERISKCONFIG._serialized_start=950
+    _ASTERISKCONFIG._serialized_end=1028
+    _COMMONSERVICESCONFIG._serialized_start=1031
+    _COMMONSERVICESCONFIG._serialized_end=1265
+    _SIPBASECONFIG._serialized_start=1267
+    _SIPBASECONFIG._serialized_end=1307
+    _SIPCALLERCONFIG._serialized_start=1310
+    _SIPCALLERCONFIG._serialized_end=1517
+    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_start=1468
+    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_end=1517
+    _CSIVTSICONFIG._serialized_start=1520
+    _CSIVTSICONFIG._serialized_end=1886
+    _AUDIOOBJECTSTORAGECONFIG._serialized_start=1889
+    _AUDIOOBJECTSTORAGECONFIG._serialized_end=2142
+    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_start=2144
+    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_end=2232
+    _MESSAGEBROKERCONFIG._serialized_start=2235
+    _MESSAGEBROKERCONFIG._serialized_end=2474
+    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_start=2476
+    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_end=2603
+    _RABBITMQCONFIG._serialized_start=2605
+    _RABBITMQCONFIG._serialized_end=2697
+    _MINIOCONFIG._serialized_start=2699
+    _MINIOCONFIG._serialized_end=2819
+    _S2TVTSICALLBACKS._serialized_start=2821
+    _S2TVTSICALLBACKS._serialized_end=2894
+    _NLUVTSICALLBACKS._serialized_start=2896
+    _NLUVTSICALLBACKS._serialized_end=2969
+    _T2SVTSICALLBACKS._serialized_start=2971
+    _T2SVTSICALLBACKS._serialized_end=3044
+    _LISTENER._serialized_start=3047
+    _LISTENER._serialized_end=3210
+    _CALLER._serialized_start=3213
+    _CALLER._serialized_end=3378
+    _STARTLISTENERREQUEST._serialized_start=3381
+    _STARTLISTENERREQUEST._serialized_end=3550
+    _STARTLISTENERRESPONSE._serialized_start=3552
+    _STARTLISTENERRESPONSE._serialized_end=3666
+    _STARTLISTENERSREQUEST._serialized_start=3668
+    _STARTLISTENERSREQUEST._serialized_end=3780
+    _STARTLISTENERSRESPONSE._serialized_start=3783
+    _STARTLISTENERSRESPONSE._serialized_end=3921
+    _STARTCALLERREQUEST._serialized_start=3924
+    _STARTCALLERREQUEST._serialized_end=4095
+    _STARTCALLERRESPONSE._serialized_start=4097
+    _STARTCALLERRESPONSE._serialized_end=4205
+    _STARTCALLERSREQUEST._serialized_start=4207
+    _STARTCALLERSREQUEST._serialized_end=4313
+    _STARTCALLERSRESPONSE._serialized_start=4316
+    _STARTCALLERSRESPONSE._serialized_end=4448
+    _STARTSCHEDULEDCALLERREQUEST._serialized_start=4451
+    _STARTSCHEDULEDCALLERREQUEST._serialized_end=4609
+    _STARTSCHEDULEDCALLERSREQUEST._serialized_start=4612
+    _STARTSCHEDULEDCALLERSREQUEST._serialized_end=4746
+    _STARTSCHEDULEDCALLERSRESPONSE._serialized_start=4749
+    _STARTSCHEDULEDCALLERSRESPONSE._serialized_end=4886
+    _STARTSCHEDULEDCALLERRESPONSE._serialized_start=4889
+    _STARTSCHEDULEDCALLERRESPONSE._serialized_end=5025
+    _SCHEDULEDCALLER._serialized_start=5028
+    _SCHEDULEDCALLER._serialized_end=5245
+    _STOPCALLREQUEST._serialized_start=5247
+    _STOPCALLREQUEST._serialized_end=5310
+    _STOPCALLRESPONSE._serialized_start=5312
+    _STOPCALLRESPONSE._serialized_end=5399
+    _STOPCALLSREQUEST._serialized_start=5401
+    _STOPCALLSREQUEST._serialized_end=5466
+    _STOPCALLSRESPONSE._serialized_start=5468
+    _STOPCALLSRESPONSE._serialized_end=5570
+    _STOPALLCALLSREQUEST._serialized_start=5572
+    _STOPALLCALLSREQUEST._serialized_end=5620
+    _TRANSFERCALLREQUEST._serialized_start=5622
+    _TRANSFERCALLREQUEST._serialized_end=5710
+    _TRANSFERCALLRESPONSE._serialized_start=5712
+    _TRANSFERCALLRESPONSE._serialized_end=5824
+    _TRANSFERCALLSREQUEST._serialized_start=5826
+    _TRANSFERCALLSREQUEST._serialized_end=5941
+    _TRANSFERCALLSRESPONSE._serialized_start=5944
+    _TRANSFERCALLSRESPONSE._serialized_end=6085
+    _GETCALLINFOREQUEST._serialized_start=6087
+    _GETCALLINFOREQUEST._serialized_end=6204
+    _GETCALLINFORESPONSE._serialized_start=6206
+    _GETCALLINFORESPONSE._serialized_end=6312
+    _CALLINFO._serialized_start=6315
+    _CALLINFO._serialized_end=6717
+    _LISTCALLINFOREQUEST._serialized_start=6720
+    _LISTCALLINFOREQUEST._serialized_end=6861
+    _LISTCALLINFORESPONSE._serialized_start=6863
+    _LISTCALLINFORESPONSE._serialized_end=6928
+    _ALLSERVICESSTATUSES._serialized_start=6931
+    _ALLSERVICESSTATUSES._serialized_end=7197
+    _SERVICESTATUS._serialized_start=7199
+    _SERVICESTATUS._serialized_end=7254
+    _GETAUDIOFILEREQUEST._serialized_start=7256
+    _GETAUDIOFILEREQUEST._serialized_end=7367
+    _GETAUDIOFILERESPONSE._serialized_start=7369
+    _GETAUDIOFILERESPONSE._serialized_end=7406
+    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_start=7409
+    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_end=7537
+    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_start=7539
+    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_end=7592
+    _CALLS._serialized_start=7682
+    _CALLS._serialized_end=9048
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/vtsi/calls_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/vtsi/calls_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/client.py` & `ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/calls.py` & `ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/services/calls.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/projects.py` & `ondewo-vtsi-client-6.3.0/ondewo/vtsi/client/services/projects.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/ondewo/vtsi/projects_pb2_grpc.py` & `ondewo-vtsi-client-6.3.0/ondewo/vtsi/projects_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,19 @@
             response_deserializer=ondewo_dot_vtsi_dot_projects__pb2.DeployVtsiProjectResponse.FromString,
         )
         self.UndeployVtsiProject = channel.unary_unary(
             '/ondewo.vtsi.Projects/UndeployVtsiProject',
             request_serializer=ondewo_dot_vtsi_dot_projects__pb2.UndeployVtsiProjectRequest.SerializeToString,
             response_deserializer=ondewo_dot_vtsi_dot_projects__pb2.UndeployVtsiProjectResponse.FromString,
         )
+        self.ListVtsiProjects = channel.unary_unary(
+            '/ondewo.vtsi.Projects/ListVtsiProjects',
+            request_serializer=ondewo_dot_vtsi_dot_projects__pb2.ListVtsiProjectsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_projects__pb2.ListVtsiProjectsResponse.FromString,
+        )
 
 
 class ProjectsServicer(object):
     """ONDEWO VTSI API
     """
 
     def CreateVtsiProject(self, request, context):
@@ -93,14 +98,21 @@
     def UndeployVtsiProject(self, request, context):
         """Undeploy a VTSI project
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListVtsiProjects(self, request, context):
+        """Get a VTSI project with configs
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_ProjectsServicer_to_server(servicer, server):
     rpc_method_handlers = {
         'CreateVtsiProject': grpc.unary_unary_rpc_method_handler(
             servicer.CreateVtsiProject,
             request_deserializer=ondewo_dot_vtsi_dot_projects__pb2.CreateVtsiProjectRequest.FromString,
             response_serializer=ondewo_dot_vtsi_dot_projects__pb2.CreateVtsiProjectResponse.SerializeToString,
@@ -126,14 +138,19 @@
             response_serializer=ondewo_dot_vtsi_dot_projects__pb2.DeployVtsiProjectResponse.SerializeToString,
         ),
         'UndeployVtsiProject': grpc.unary_unary_rpc_method_handler(
             servicer.UndeployVtsiProject,
             request_deserializer=ondewo_dot_vtsi_dot_projects__pb2.UndeployVtsiProjectRequest.FromString,
             response_serializer=ondewo_dot_vtsi_dot_projects__pb2.UndeployVtsiProjectResponse.SerializeToString,
         ),
+        'ListVtsiProjects': grpc.unary_unary_rpc_method_handler(
+            servicer.ListVtsiProjects,
+            request_deserializer=ondewo_dot_vtsi_dot_projects__pb2.ListVtsiProjectsRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_projects__pb2.ListVtsiProjectsResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         'ondewo.vtsi.Projects', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
 
@@ -239,7 +256,24 @@
                             timeout=None,
                             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Projects/UndeployVtsiProject',
                                              ondewo_dot_vtsi_dot_projects__pb2.UndeployVtsiProjectRequest.SerializeToString,
                                              ondewo_dot_vtsi_dot_projects__pb2.UndeployVtsiProjectResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListVtsiProjects(request,
+                         target,
+                         options=(),
+                         channel_credentials=None,
+                         call_credentials=None,
+                         insecure=False,
+                         compression=None,
+                         wait_for_ready=None,
+                         timeout=None,
+                         metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Projects/ListVtsiProjects',
+                                             ondewo_dot_vtsi_dot_projects__pb2.ListVtsiProjectsRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_projects__pb2.ListVtsiProjectsResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/PKG-INFO` & `ondewo-vtsi-client-6.3.0/ondewo_vtsi_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.2.0
+Version: 6.3.0
 Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.2.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.3.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/SOURCES.txt` & `ondewo-vtsi-client-6.3.0/ondewo_vtsi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.2.0/setup.py` & `ondewo-vtsi-client-6.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             req_str = f"{req_name} @ {req_url}"
         else:
             req_str = req
         requires.append(req_str)
 
 setup(
     name="ondewo-vtsi-client",
-    version='6.2.0',
+    version='6.3.0',
     author="Ondewo GbmH",
     author_email="office@ondewo.com",
     description="exposes the ondewo-vtsi endpoints in a user-friendly way",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-vtsi-client-python",
     packages=[
```

