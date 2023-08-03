# Comparing `tmp/qdrant_client-1.3.1.tar.gz` & `tmp/qdrant_client-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.3.1.tar", max compression
+gzip compressed data, was "qdrant_client-1.3.2.tar", max compression
```

## Comparing `qdrant_client-1.3.1.tar` & `qdrant_client-1.3.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0    11357 2023-06-26 12:13:26.011897 qdrant_client-1.3.1/LICENSE
--rw-r--r--   0        0        0     6250 2023-06-26 12:13:26.011897 qdrant_client-1.3.1/README.md
--rw-r--r--   0        0        0     1440 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       56 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/__init__.py
--rw-r--r--   0        0        0    10034 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/client_base.py
--rw-r--r--   0        0        0     9742 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     3447 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0    72811 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      252 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    36463 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     2063 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    16916 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3395 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    54119 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     2907 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    30011 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7768 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      505 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10437 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    30407 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    38894 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9499 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    18850 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7577 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0    67870 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0     2979 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     1446 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/geo.py
--rw-r--r--   0        0        0    29728 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0     6371 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2922 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     4388 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    23964 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0        0 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/tests/__init__.py
--rw-r--r--   0        0        0     4210 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/tests/test_payload_filters.py
--rw-r--r--   0        0        0       40 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    13786 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1496 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1936 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    19848 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     2873 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      331 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1895 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/py.typed
--rw-r--r--   0        0        0    72285 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    81209 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     2758 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2160 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3200 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     7436 1970-01-01 00:00:00.000000 qdrant_client-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/LICENSE
+-rw-r--r--   0        0        0     6250 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/README.md
+-rw-r--r--   0        0        0     1351 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/qdrant_client/__init__.py
+-rw-r--r--   0        0        0     1085 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/qdrant_client/_pydantic_compat.py
+-rw-r--r--   0        0        0    10063 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/qdrant_client/client_base.py
+-rw-r--r--   0        0        0     9732 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     3447 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0    72838 2023-07-26 21:40:50.714630 qdrant_client-1.3.2/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      252 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    36463 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     2063 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    16916 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3395 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    54119 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     2907 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    30011 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7768 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      567 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    26898 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    36694 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     5395 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    14746 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7577 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0    70362 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0     2979 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     1446 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0    30185 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0     6371 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2922 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     4388 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    24615 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/tests/__init__.py
+-rw-r--r--   0        0        0     4210 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/local/tests/test_payload_filters.py
+-rw-r--r--   0        0        0       40 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    13786 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1496 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1936 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    19848 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     2873 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      331 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1895 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/py.typed
+-rw-r--r--   0        0        0    72298 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    81388 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     2758 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2243 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3264 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-26 21:40:50.718630 qdrant_client-1.3.2/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     7384 1970-01-01 00:00:00.000000 qdrant_client-1.3.2/PKG-INFO
```

### Comparing `qdrant_client-1.3.1/LICENSE` & `qdrant_client-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/README.md` & `qdrant_client-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/pyproject.toml` & `qdrant_client-1.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.3.1"
+version = "1.3.2"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
 license = "Apache-2.0"
@@ -16,16 +16,15 @@
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 httpx = { version = ">=0.14.0", extras = ["http2"] }
 numpy = [
     { version = "<1.21", python = "<3.8" },
     { version = ">=1.21", python = ">=3.8" }
 ]
-pydantic = "^1.8"
-typing-extensions = ">=4.0.0,<4.6.0"  # at the moment 4.6.0 breaks support for python3.8,3.9
+pydantic = ">=1.10.8"
 grpcio = { version = ">=1.41.0", allow-prereleases = true }
 grpcio-tools = ">=1.41.0"
 urllib3 = "^1.26.14"
 portalocker = "^2.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
```

### Comparing `qdrant_client-1.3.1/qdrant_client/client_base.py` & `qdrant_client-1.3.2/qdrant_client/client_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,17 @@
         **kwargs: Any,
     ) -> None:
         raise NotImplementedError()
 
     def upload_collection(
         self,
         collection_name: str,
-        vectors: Union[types.NumpyArray, Dict[str, types.NumpyArray], Iterable[List[float]]],
+        vectors: Union[
+            Dict[str, types.NumpyArray], types.NumpyArray, Iterable[types.VectorStruct]
+        ],
         payload: Optional[Iterable[Dict[Any, Any]]] = None,
         ids: Optional[Iterable[types.PointId]] = None,
         **kwargs: Any,
     ) -> None:
         raise NotImplementedError()
 
     def create_payload_index(
```

### Comparing `qdrant_client-1.3.1/qdrant_client/connection.py` & `qdrant_client-1.3.2/qdrant_client/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             creds = grpc.ssl_channel_credentials()
 
         # finally pass in the combined credentials when creating a channel
         return grpc.secure_channel(f"{host}:{port}", creds, options)
     else:
         if metadata:
             metadata_interceptor = header_adder_interceptor(metadata)
-            channel = grpc.insecure_channel(f"{host}:{port}", metadata, options)
+            channel = grpc.insecure_channel(f"{host}:{port}", options)
             return grpc.intercept_channel(channel, metadata_interceptor)
         else:
             return grpc.insecure_channel(f"{host}:{port}", options)
 
 
 def get_async_channel(
     host: str, port: int, ssl: bool, metadata: Optional[List[Tuple[str, str]]] = None
```

### Comparing `qdrant_client-1.3.1/qdrant_client/conversions/common_types.py` & `qdrant_client-1.3.2/qdrant_client/conversions/common_types.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/conversions/conversion.py` & `qdrant_client-1.3.2/qdrant_client/conversions/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.timestamp_pb2 import Timestamp
 
+from qdrant_client._pydantic_compat import construct
+
 try:
     from google.protobuf.pyext._message import MessageMapContainer  # type: ignore
 except ImportError:
     pass
 
 from qdrant_client import grpc as grpc
 from qdrant_client.grpc import ListValue, NullValue, Struct, Value
@@ -171,15 +173,15 @@
             return rest.OptimizersStatusOneOf.OK
         else:
             return rest.OptimizersStatusOneOf1(error=model.error)
 
     @classmethod
     def convert_collection_config(cls, model: grpc.CollectionConfig) -> rest.CollectionConfig:
         return rest.CollectionConfig(
-            hnsw_config=cls.convert_hnsw_config_diff(model.hnsw_config),
+            hnsw_config=cls.convert_hnsw_config(model.hnsw_config),
             optimizer_config=cls.convert_optimizer_config(model.optimizer_config),
             params=cls.convert_collection_params(model.params),
             wal_config=cls.convert_wal_config(model.wal_config),
             quantization_config=cls.convert_quantization_config(model.quantization_config)
             if model.HasField("quantization_config")
             else None,
         )
@@ -389,26 +391,26 @@
     @classmethod
     def convert_create_collection(cls, model: grpc.CreateCollection) -> rest.CreateCollection:
         return rest.CreateCollection(
             vectors=cls.convert_vectors_config(model.vectors_config)
             if model.HasField("vectors_config")
             else None,
             shard_number=model.shard_number,
-            collection_name=model.collection_name,
-            hnsw_config=cls.convert_hnsw_config(model.hnsw_config),
-            wal_config=cls.convert_wal_config(model.wal_config),
-            optimizers_config=cls.convert_optimizer_config(model.optimizers_config),
+            hnsw_config=cls.convert_hnsw_config_diff(model.hnsw_config),
+            wal_config=cls.convert_wal_config_diff(model.wal_config),
+            optimizers_config=cls.convert_optimizers_config_diff(model.optimizers_config),
             quantization_config=cls.convert_quantization_config(model.quantization_config)
             if model.HasField("quantization_config")
             else None,
         )
 
     @classmethod
     def convert_scored_point(cls, model: grpc.ScoredPoint) -> rest.ScoredPoint:
-        return rest.ScoredPoint.construct(
+        return construct(
+            rest.ScoredPoint,
             id=cls.convert_point_id(model.id),
             payload=cls.convert_payload(model.payload),
             score=model.score,
             vector=cls.convert_vectors(model.vectors) if model.HasField("vectors") else None,
             version=model.version,
         )
```

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.3.2/qdrant_client/grpc/collections_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.3.2/qdrant_client/grpc/collections_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.3.2/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.3.2/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.3.2/qdrant_client/grpc/points_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.3.2/qdrant_client/grpc/points_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.3.2/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.3.2/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.3.2/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.3.2/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.3.2/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.3.2/qdrant_client/local/qdrant_local.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1032 +1,656 @@
-# flake8: noqa E501
-from enum import Enum
-from pathlib import PurePath
-from types import GeneratorType
-from typing import IO, TYPE_CHECKING, Any, Callable, Dict, List, Set, Tuple, Union
-
-from pydantic.json import ENCODERS_BY_TYPE
-from pydantic.main import BaseModel
-from qdrant_client.http.models import *
-from qdrant_client.http.models import models as m
-
-SetIntStr = Set[Union[int, str]]
-DictIntStrAny = Dict[Union[int, str], Any]
-file = None
-
-
-def generate_encoders_by_class_tuples(type_encoder_map: Dict[Any, Callable]) -> Dict[Callable, Tuple]:
-    encoders_by_classes: Dict[Callable, List] = {}
-    for type_, encoder in type_encoder_map.items():
-        encoders_by_classes.setdefault(encoder, []).append(type_)
-    encoders_by_class_tuples: Dict[Callable, Tuple] = {}
-    for encoder, classes in encoders_by_classes.items():
-        encoders_by_class_tuples[encoder] = tuple(classes)
-    return encoders_by_class_tuples
-
-
-encoders_by_class_tuples = generate_encoders_by_class_tuples(ENCODERS_BY_TYPE)
-
-
-def jsonable_encoder(
-    obj: Any,
-    include: Union[SetIntStr, DictIntStrAny] = None,
-    exclude=None,
-    by_alias: bool = True,
-    skip_defaults: bool = None,
-    exclude_unset: bool = False,
-    include_none: bool = True,
-    custom_encoder=None,
-    sqlalchemy_safe: bool = True,
-) -> Any:
-    if exclude is None:
-        exclude = set()
-    if custom_encoder is None:
-        custom_encoder = {}
-    if include is not None and not isinstance(include, set):
-        include = set(include)
-    if exclude is not None and not isinstance(exclude, set):
-        exclude = set(exclude)
-    if isinstance(obj, BaseModel):
-        encoder = getattr(obj.Config, "json_encoders", {})
-        if custom_encoder:
-            encoder.update(custom_encoder)
-        obj_dict = obj.dict(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            exclude_unset=bool(exclude_unset or skip_defaults),
-        )
-
-        return jsonable_encoder(
-            obj_dict,
-            include_none=include_none,
-            custom_encoder=encoder,
-            sqlalchemy_safe=sqlalchemy_safe,
-        )
-    if isinstance(obj, Enum):
-        return obj.value
-    if isinstance(obj, PurePath):
-        return str(obj)
-    if isinstance(obj, (str, int, float, type(None))):
-        return obj
-    if isinstance(obj, dict):
-        encoded_dict = {}
-        for key, value in obj.items():
-            if (
-                (not sqlalchemy_safe or (not isinstance(key, str)) or (not key.startswith("_sa")))
-                and (value is not None or include_none)
-                and ((include and key in include) or key not in exclude)
-            ):
-                encoded_key = jsonable_encoder(
-                    key,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-                encoded_value = jsonable_encoder(
-                    value,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-                encoded_dict[encoded_key] = encoded_value
-        return encoded_dict
-    if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
-        encoded_list = []
-        for item in obj:
-            encoded_list.append(
-                jsonable_encoder(
-                    item,
-                    include=include,
-                    exclude=exclude,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-            )
-        return encoded_list
-
-    if custom_encoder:
-        if type(obj) in custom_encoder:
-            return custom_encoder[type(obj)](obj)
+import itertools
+import json
+import logging
+import os
+import shutil
+from io import TextIOWrapper
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
+
+import numpy as np
+import portalocker
+
+from qdrant_client._pydantic_compat import to_dict
+from qdrant_client.client_base import QdrantBase
+from qdrant_client.conversions import common_types as types
+from qdrant_client.http import models as rest_models
+from qdrant_client.local.local_collection import LocalCollection
+
+META_INFO_FILENAME = "meta.json"
+
+
+class QdrantLocal(QdrantBase):
+    """
+    Everything Qdrant server can do, but locally.
+
+    Use this implementation to run vector search without running a Qdrant server.
+    Everything that works with local Qdrant will work with server Qdrant as well.
+
+    Use for small-scale data, demos, and tests.
+    If you need more speed or size, use Qdrant server.
+    """
+
+    def __init__(self, location: str) -> None:
+        """
+        Initialize local Qdrant.
+
+        Args:
+            location: Where to store data. Can be a path to a directory or `:memory:` for in-memory storage.
+        """
+        self.location = location
+        self.persistent = location != ":memory:"
+        self.collections: Dict[str, LocalCollection] = {}
+        self.aliases: Dict[str, str] = {}
+        self._lock = None
+        self._flock_file: Optional[TextIOWrapper] = None
+        self._load()
+
+    def _load(self) -> None:
+        if not self.persistent:
+            return
+        meta_path = os.path.join(self.location, META_INFO_FILENAME)
+        if not os.path.exists(meta_path):
+            os.makedirs(self.location, exist_ok=True)
+            with open(meta_path, "w") as f:
+                f.write(json.dumps({"collections": {}, "aliases": {}}))
         else:
-            for encoder_type, encoder in custom_encoder.items():
-                if isinstance(obj, encoder_type):
-                    return encoder(obj)
-
-    if type(obj) in ENCODERS_BY_TYPE:
-        return ENCODERS_BY_TYPE[type(obj)](obj)
-    for encoder, classes_tuple in encoders_by_class_tuples.items():
-        if isinstance(obj, classes_tuple):
-            return encoder(obj)
-
-    errors: List[Exception] = []
-    try:
-        data = dict(obj)
-    except Exception as e:
-        errors.append(e)
+            with open(meta_path, "r") as f:
+                meta = json.load(f)
+                for collection_name, config_json in meta["collections"].items():
+                    config = rest_models.CreateCollection(**config_json)
+                    collection_path = self._collection_path(collection_name)
+                    self.collections[collection_name] = LocalCollection(config, collection_path)
+                self.aliases = meta["aliases"]
+
+        lock_file_path = os.path.join(self.location, ".lock")
+        if not os.path.exists(lock_file_path):
+            os.makedirs(self.location, exist_ok=True)
+            with open(lock_file_path, "w") as f:
+                f.write("tmp lock file")
+        self._flock_file = open(lock_file_path, "r+")
         try:
-            data = vars(obj)
-        except Exception as e:
-            errors.append(e)
-            raise ValueError(errors)
-    return jsonable_encoder(
-        data,
-        by_alias=by_alias,
-        exclude_unset=exclude_unset,
-        include_none=include_none,
-        custom_encoder=custom_encoder,
-        sqlalchemy_safe=sqlalchemy_safe,
-    )
-
-
-if TYPE_CHECKING:
-    from qdrant_client.http.api_client import ApiClient
-
-
-class _CollectionsApi:
-    def __init__(self, api_client: "Union[ApiClient, AsyncApiClient]"):
-        self.api_client = api_client
-
-    def _build_for_collection_cluster_info(
-        self,
-        collection_name: str,
-    ):
-        """
-        Get cluster information for a collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        return self.api_client.request(
-            type_=m.InlineResponse2007,
-            method="GET",
-            url="/collections/{collection_name}/cluster",
-            path_params=path_params,
-        )
-
-    def _build_for_create_collection(
-        self,
-        collection_name: str,
-        timeout: int = None,
-        create_collection: m.CreateCollection = None,
-    ):
-        """
-        Create new collection with given parameters
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        query_params = {}
-        if timeout is not None:
-            query_params["timeout"] = str(timeout)
-
-        body = jsonable_encoder(create_collection)
-
-        return self.api_client.request(
-            type_=m.InlineResponse2003,
-            method="PUT",
-            url="/collections/{collection_name}",
-            path_params=path_params,
-            params=query_params,
-            json=body,
-        )
-
-    def _build_for_create_field_index(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        ordering: WriteOrdering = None,
-        create_field_index: m.CreateFieldIndex = None,
-    ):
-        """
-        Create index for field in collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        query_params = {}
-        if wait is not None:
-            query_params["wait"] = str(wait).lower()
-        if ordering is not None:
-            query_params["ordering"] = str(ordering)
-
-        body = jsonable_encoder(create_field_index)
-
-        return self.api_client.request(
-            type_=m.InlineResponse2006,
-            method="PUT",
-            url="/collections/{collection_name}/index",
-            path_params=path_params,
-            params=query_params,
-            json=body,
-        )
-
-    def _build_for_create_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-    ):
-        """
-        Create new snapshot for a collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        query_params = {}
-        if wait is not None:
-            query_params["wait"] = str(wait).lower()
-
-        return self.api_client.request(
-            type_=m.InlineResponse20010,
-            method="POST",
-            url="/collections/{collection_name}/snapshots",
-            path_params=path_params,
-            params=query_params,
-        )
-
-    def _build_for_delete_collection(
-        self,
-        collection_name: str,
-        timeout: int = None,
-    ):
-        """
-        Drop collection and all associated data
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        query_params = {}
-        if timeout is not None:
-            query_params["timeout"] = str(timeout)
-
-        return self.api_client.request(
-            type_=m.InlineResponse2003,
-            method="DELETE",
-            url="/collections/{collection_name}",
-            path_params=path_params,
-            params=query_params,
-        )
-
-    def _build_for_delete_field_index(
-        self,
-        collection_name: str,
-        field_name: str,
-        wait: bool = None,
-        ordering: WriteOrdering = None,
-    ):
-        """
-        Delete field index for collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-            "field_name": str(field_name),
-        }
-
-        query_params = {}
-        if wait is not None:
-            query_params["wait"] = str(wait).lower()
-        if ordering is not None:
-            query_params["ordering"] = str(ordering)
-
-        return self.api_client.request(
-            type_=m.InlineResponse2006,
-            method="DELETE",
-            url="/collections/{collection_name}/index/{field_name}",
-            path_params=path_params,
-            params=query_params,
-        )
-
-    def _build_for_delete_snapshot(
-        self,
-        collection_name: str,
-        snapshot_name: str,
-        wait: bool = None,
-    ):
-        """
-        Delete snapshot for a collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-            "snapshot_name": str(snapshot_name),
-        }
-
-        query_params = {}
-        if wait is not None:
-            query_params["wait"] = str(wait).lower()
-
-        return self.api_client.request(
-            type_=m.InlineResponse2003,
-            method="DELETE",
-            url="/collections/{collection_name}/snapshots/{snapshot_name}",
-            path_params=path_params,
-            params=query_params,
-        )
-
-    def _build_for_get_collection(
-        self,
-        collection_name: str,
-    ):
-        """
-        Get detailed information about specified existing collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        return self.api_client.request(
-            type_=m.InlineResponse2005,
-            method="GET",
-            url="/collections/{collection_name}",
-            path_params=path_params,
-        )
-
-    def _build_for_get_collection_aliases(
-        self,
-        collection_name: str,
-    ):
-        """
-        Get list of all aliases for a collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        return self.api_client.request(
-            type_=m.InlineResponse2008,
-            method="GET",
-            url="/collections/{collection_name}/aliases",
-            path_params=path_params,
-        )
-
-    def _build_for_get_collections(
-        self,
-    ):
-        """
-        Get list name of all existing collections
-        """
-        return self.api_client.request(
-            type_=m.InlineResponse2004,
-            method="GET",
-            url="/collections",
-        )
-
-    def _build_for_get_collections_aliases(
-        self,
-    ):
-        """
-        Get list of all existing collections aliases
-        """
-        return self.api_client.request(
-            type_=m.InlineResponse2008,
-            method="GET",
-            url="/aliases",
-        )
-
-    def _build_for_get_snapshot(
-        self,
-        collection_name: str,
-        snapshot_name: str,
-    ):
-        """
-        Download specified snapshot from a collection as a file
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-            "snapshot_name": str(snapshot_name),
-        }
-
-        return self.api_client.request(
-            type_=file,
-            method="GET",
-            url="/collections/{collection_name}/snapshots/{snapshot_name}",
-            path_params=path_params,
-        )
-
-    def _build_for_list_snapshots(
-        self,
-        collection_name: str,
-    ):
-        """
-        Get list of snapshots for a collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        return self.api_client.request(
-            type_=m.InlineResponse2009,
-            method="GET",
-            url="/collections/{collection_name}/snapshots",
-            path_params=path_params,
-        )
-
-    def _build_for_recover_from_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        snapshot_recover: m.SnapshotRecover = None,
-    ):
-        """
-        Recover local collection data from a snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        query_params = {}
-        if wait is not None:
-            query_params["wait"] = str(wait).lower()
-
-        body = jsonable_encoder(snapshot_recover)
-
-        return self.api_client.request(
-            type_=m.InlineResponse2003,
-            method="PUT",
-            url="/collections/{collection_name}/snapshots/recover",
-            path_params=path_params,
-            params=query_params,
-            json=body,
-        )
-
-    def _build_for_recover_from_uploaded_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        priority: SnapshotPriority = None,
-        snapshot: IO[Any] = None,
-    ):
-        """
-        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        query_params = {}
-        if wait is not None:
-            query_params["wait"] = str(wait).lower()
-        if priority is not None:
-            query_params["priority"] = str(priority)
-
-        files: Dict[str, IO[Any]] = {}  # noqa F841
-        data: Dict[str, Any] = {}  # noqa F841
-        if snapshot is not None:
-            files["snapshot"] = snapshot
-
-        return self.api_client.request(
-            type_=m.InlineResponse2003,
-            method="POST",
-            url="/collections/{collection_name}/snapshots/upload",
-            path_params=path_params,
-            params=query_params,
-            data=data,
-            files=files,
-        )
-
-    def _build_for_update_aliases(
-        self,
-        timeout: int = None,
-        change_aliases_operation: m.ChangeAliasesOperation = None,
-    ):
-        query_params = {}
-        if timeout is not None:
-            query_params["timeout"] = str(timeout)
-
-        body = jsonable_encoder(change_aliases_operation)
-
-        return self.api_client.request(
-            type_=m.InlineResponse2003, method="POST", url="/collections/aliases", params=query_params, json=body
-        )
-
-    def _build_for_update_collection(
-        self,
-        collection_name: str,
-        timeout: int = None,
-        update_collection: m.UpdateCollection = None,
-    ):
-        """
-        Update parameters of the existing collection
-        """
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        query_params = {}
-        if timeout is not None:
-            query_params["timeout"] = str(timeout)
-
-        body = jsonable_encoder(update_collection)
-
-        return self.api_client.request(
-            type_=m.InlineResponse2003,
-            method="PATCH",
-            url="/collections/{collection_name}",
-            path_params=path_params,
-            params=query_params,
-            json=body,
-        )
-
-    def _build_for_update_collection_cluster(
-        self,
-        collection_name: str,
-        timeout: int = None,
-        cluster_operations: m.ClusterOperations = None,
-    ):
-        path_params = {
-            "collection_name": str(collection_name),
-        }
-
-        query_params = {}
-        if timeout is not None:
-            query_params["timeout"] = str(timeout)
-
-        body = jsonable_encoder(cluster_operations)
-
-        return self.api_client.request(
-            type_=m.InlineResponse2003,
-            method="POST",
-            url="/collections/{collection_name}/cluster",
-            path_params=path_params,
-            params=query_params,
-            json=body,
-        )
-
-
-class AsyncCollectionsApi(_CollectionsApi):
-    async def collection_cluster_info(
-        self,
-        collection_name: str,
-    ) -> m.InlineResponse2007:
-        """
-        Get cluster information for a collection
-        """
-        return await self._build_for_collection_cluster_info(
-            collection_name=collection_name,
-        )
-
-    async def create_collection(
-        self,
-        collection_name: str,
-        timeout: int = None,
-        create_collection: m.CreateCollection = None,
-    ) -> m.InlineResponse2003:
-        """
-        Create new collection with given parameters
-        """
-        return await self._build_for_create_collection(
-            collection_name=collection_name,
-            timeout=timeout,
-            create_collection=create_collection,
-        )
-
-    async def create_field_index(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        ordering: WriteOrdering = None,
-        create_field_index: m.CreateFieldIndex = None,
-    ) -> m.InlineResponse2006:
-        """
-        Create index for field in collection
-        """
-        return await self._build_for_create_field_index(
-            collection_name=collection_name,
-            wait=wait,
-            ordering=ordering,
-            create_field_index=create_field_index,
-        )
-
-    async def create_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-    ) -> m.InlineResponse20010:
-        """
-        Create new snapshot for a collection
-        """
-        return await self._build_for_create_snapshot(
-            collection_name=collection_name,
-            wait=wait,
-        )
-
-    async def delete_collection(
-        self,
-        collection_name: str,
-        timeout: int = None,
-    ) -> m.InlineResponse2003:
-        """
-        Drop collection and all associated data
-        """
-        return await self._build_for_delete_collection(
-            collection_name=collection_name,
-            timeout=timeout,
-        )
-
-    async def delete_field_index(
-        self,
-        collection_name: str,
-        field_name: str,
-        wait: bool = None,
-        ordering: WriteOrdering = None,
-    ) -> m.InlineResponse2006:
-        """
-        Delete field index for collection
-        """
-        return await self._build_for_delete_field_index(
-            collection_name=collection_name,
-            field_name=field_name,
-            wait=wait,
-            ordering=ordering,
-        )
-
-    async def delete_snapshot(
-        self,
-        collection_name: str,
-        snapshot_name: str,
-        wait: bool = None,
-    ) -> m.InlineResponse2003:
-        """
-        Delete snapshot for a collection
-        """
-        return await self._build_for_delete_snapshot(
-            collection_name=collection_name,
-            snapshot_name=snapshot_name,
-            wait=wait,
-        )
-
-    async def get_collection(
-        self,
-        collection_name: str,
-    ) -> m.InlineResponse2005:
-        """
-        Get detailed information about specified existing collection
-        """
-        return await self._build_for_get_collection(
-            collection_name=collection_name,
-        )
-
-    async def get_collection_aliases(
-        self,
-        collection_name: str,
-    ) -> m.InlineResponse2008:
-        """
-        Get list of all aliases for a collection
-        """
-        return await self._build_for_get_collection_aliases(
-            collection_name=collection_name,
-        )
+            self._flock = portalocker.lock(
+                self._flock_file,
+                portalocker.LockFlags.EXCLUSIVE | portalocker.LockFlags.NON_BLOCKING,
+            )
+        except portalocker.exceptions.LockException:
+            raise RuntimeError(
+                f"Storage folder {self.location} is already accessed by another instance of Qdrant client."
+                f" If you require concurrent access, use Qdrant server instead."
+            )
 
-    async def get_collections(
-        self,
-    ) -> m.InlineResponse2004:
-        """
-        Get list name of all existing collections
-        """
-        return await self._build_for_get_collections()
+    def _save(self) -> None:
+        if not self.persistent:
+            return
+        meta_path = os.path.join(self.location, META_INFO_FILENAME)
+        with open(meta_path, "w") as f:
+            f.write(
+                json.dumps(
+                    {
+                        "collections": {
+                            collection_name: to_dict(collection.config)
+                            for collection_name, collection in self.collections.items()
+                        },
+                        "aliases": self.aliases,
+                    }
+                )
+            )
 
-    async def get_collections_aliases(
-        self,
-    ) -> m.InlineResponse2008:
-        """
-        Get list of all existing collections aliases
-        """
-        return await self._build_for_get_collections_aliases()
+    def _get_collection(self, collection_name: str) -> LocalCollection:
+        if collection_name in self.collections:
+            return self.collections[collection_name]
+        if collection_name in self.aliases:
+            return self.collections[self.aliases[collection_name]]
+        raise ValueError(f"Collection {collection_name} not found")
+
+    def search_batch(
+        self,
+        collection_name: str,
+        requests: Sequence[types.SearchRequest],
+        **kwargs: Any,
+    ) -> List[List[types.ScoredPoint]]:
+        collection = self._get_collection(collection_name)
+
+        return [
+            collection.search(
+                query_vector=request.vector,
+                query_filter=request.filter,
+                limit=request.limit,
+                offset=request.offset,
+                with_payload=request.with_payload,
+                with_vectors=request.with_vector,
+                score_threshold=request.score_threshold,
+            )
+            for request in requests
+        ]
 
-    async def get_snapshot(
+    def search(
         self,
         collection_name: str,
-        snapshot_name: str,
-    ) -> file:
-        """
-        Download specified snapshot from a collection as a file
-        """
-        return await self._build_for_get_snapshot(
-            collection_name=collection_name,
-            snapshot_name=snapshot_name,
-        )
+        query_vector: Union[
+            types.NumpyArray,
+            Sequence[float],
+            Tuple[str, List[float]],
+            types.NamedVector,
+        ],
+        query_filter: Optional[types.Filter] = None,
+        search_params: Optional[types.SearchParams] = None,
+        limit: int = 10,
+        offset: int = 0,
+        with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        score_threshold: Optional[float] = None,
+        **kwargs: Any,
+    ) -> List[types.ScoredPoint]:
+        collection = self._get_collection(collection_name)
+        return collection.search(
+            query_vector=query_vector,
+            query_filter=query_filter,
+            limit=limit,
+            offset=offset,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+        )
+
+    def search_groups(
+        self,
+        collection_name: str,
+        query_vector: Union[
+            types.NumpyArray,
+            Sequence[float],
+            Tuple[str, List[float]],
+            types.NamedVector,
+        ],
+        group_by: str,
+        query_filter: Optional[rest_models.Filter] = None,
+        search_params: Optional[rest_models.SearchParams] = None,
+        limit: int = 10,
+        group_size: int = 1,
+        with_payload: Union[bool, Sequence[str], rest_models.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        score_threshold: Optional[float] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
+        **kwargs: Any,
+    ) -> types.GroupsResult:
+        collection = self._get_collection(collection_name)
+        with_lookup_collection = None
+        if with_lookup is not None:
+            if isinstance(with_lookup, str):
+                with_lookup_collection = self._get_collection(with_lookup)
+            else:
+                with_lookup_collection = self._get_collection(with_lookup.collection)
+
+        return collection.search_groups(
+            query_vector=query_vector,
+            query_filter=query_filter,
+            limit=limit,
+            group_by=group_by,
+            group_size=group_size,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+            with_lookup=with_lookup,
+            with_lookup_collection=with_lookup_collection,
+        )
+
+    def recommend_batch(
+        self,
+        collection_name: str,
+        requests: Sequence[types.RecommendRequest],
+        **kwargs: Any,
+    ) -> List[List[types.ScoredPoint]]:
+        collection = self._get_collection(collection_name)
+
+        return [
+            collection.recommend(
+                positive=request.positive,
+                negative=request.negative,
+                query_filter=request.filter,
+                limit=request.limit,
+                offset=request.offset,
+                with_payload=request.with_payload,
+                with_vectors=request.with_vector,
+                score_threshold=request.score_threshold,
+            )
+            for request in requests
+        ]
 
-    async def list_snapshots(
+    def recommend(
         self,
         collection_name: str,
-    ) -> m.InlineResponse2009:
-        """
-        Get list of snapshots for a collection
-        """
-        return await self._build_for_list_snapshots(
-            collection_name=collection_name,
-        )
+        positive: Sequence[types.PointId],
+        negative: Optional[Sequence[types.PointId]] = None,
+        query_filter: Optional[types.Filter] = None,
+        search_params: Optional[types.SearchParams] = None,
+        limit: int = 10,
+        offset: int = 0,
+        with_payload: Union[bool, List[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, List[str]] = False,
+        score_threshold: Optional[float] = None,
+        using: Optional[str] = None,
+        lookup_from: Optional[types.LookupLocation] = None,
+        **kwargs: Any,
+    ) -> List[types.ScoredPoint]:
+        collection = self._get_collection(collection_name)
+        return collection.recommend(
+            positive=positive,
+            negative=negative,
+            query_filter=query_filter,
+            limit=limit,
+            offset=offset,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+            using=using,
+            lookup_from_collection=self._get_collection(lookup_from.collection)
+            if lookup_from
+            else None,
+            lookup_from_vector_name=lookup_from.vector if lookup_from else None,
+        )
+
+    def recommend_groups(
+        self,
+        collection_name: str,
+        group_by: str,
+        positive: Sequence[types.PointId],
+        negative: Optional[Sequence[types.PointId]] = None,
+        query_filter: Optional[types.Filter] = None,
+        search_params: Optional[types.SearchParams] = None,
+        limit: int = 10,
+        group_size: int = 1,
+        score_threshold: Optional[float] = None,
+        with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        using: Optional[str] = None,
+        lookup_from: Optional[types.LookupLocation] = None,
+        with_lookup: Optional[types.WithLookupInterface] = None,
+        **kwargs: Any,
+    ) -> types.GroupsResult:
+        collection = self._get_collection(collection_name)
+        with_lookup_collection = None
+        if with_lookup is not None:
+            if isinstance(with_lookup, str):
+                with_lookup_collection = self._get_collection(with_lookup)
+            else:
+                with_lookup_collection = self._get_collection(with_lookup.collection)
+
+        return collection.recommend_groups(
+            positive=positive,
+            negative=negative,
+            group_by=group_by,
+            group_size=group_size,
+            query_filter=query_filter,
+            limit=limit,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+            score_threshold=score_threshold,
+            using=using,
+            lookup_from_collection=self._get_collection(lookup_from.collection)
+            if lookup_from
+            else None,
+            lookup_from_vector_name=lookup_from.vector if lookup_from else None,
+            with_lookup=with_lookup,
+            with_lookup_collection=with_lookup_collection,
+        )
+
+    def scroll(
+        self,
+        collection_name: str,
+        scroll_filter: Optional[types.Filter] = None,
+        limit: int = 10,
+        offset: Optional[types.PointId] = None,
+        with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        **kwargs: Any,
+    ) -> Tuple[List[types.Record], Optional[types.PointId]]:
+        collection = self._get_collection(collection_name)
+        return collection.scroll(
+            scroll_filter=scroll_filter,
+            limit=limit,
+            offset=offset,
+            with_payload=with_payload,
+            with_vectors=with_vectors,
+        )
+
+    def count(
+        self,
+        collection_name: str,
+        count_filter: Optional[types.Filter] = None,
+        exact: bool = True,
+        **kwargs: Any,
+    ) -> types.CountResult:
+        collection = self._get_collection(collection_name)
+        return collection.count(count_filter=count_filter)
+
+    def upsert(
+        self, collection_name: str, points: types.Points, **kwargs: Any
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.upsert(points)
+        return self._default_update_result()
+
+    def update_vectors(
+        self,
+        collection_name: str,
+        vectors: Sequence[types.PointVectors],
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.update_vectors(vectors)
+        return self._default_update_result()
+
+    def delete_vectors(
+        self,
+        collection_name: str,
+        vectors: Sequence[str],
+        points: types.PointsSelector,
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.delete_vectors(vectors, points)
+        return self._default_update_result()
+
+    def retrieve(
+        self,
+        collection_name: str,
+        ids: Sequence[types.PointId],
+        with_payload: Union[bool, Sequence[str], types.PayloadSelector] = True,
+        with_vectors: Union[bool, Sequence[str]] = False,
+        **kwargs: Any,
+    ) -> List[types.Record]:
+        collection = self._get_collection(collection_name)
+        return collection.retrieve(ids, with_payload, with_vectors)
+
+    @classmethod
+    def _default_update_result(cls, operation_id: int = 0) -> types.UpdateResult:
+        return types.UpdateResult(
+            operation_id=operation_id,
+            status=rest_models.UpdateStatus.COMPLETED,
+        )
+
+    def delete(
+        self, collection_name: str, points_selector: types.PointsSelector, **kwargs: Any
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.delete(points_selector)
+        return self._default_update_result()
+
+    def set_payload(
+        self,
+        collection_name: str,
+        payload: types.Payload,
+        points: types.PointsSelector,
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.set_payload(payload=payload, selector=points)
+        return self._default_update_result()
+
+    def overwrite_payload(
+        self,
+        collection_name: str,
+        payload: types.Payload,
+        points: types.PointsSelector,
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.overwrite_payload(payload=payload, selector=points)
+        return self._default_update_result()
+
+    def delete_payload(
+        self,
+        collection_name: str,
+        keys: Sequence[str],
+        points: types.PointsSelector,
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.delete_payload(keys=keys, selector=points)
+        return self._default_update_result()
+
+    def clear_payload(
+        self, collection_name: str, points_selector: types.PointsSelector, **kwargs: Any
+    ) -> types.UpdateResult:
+        collection = self._get_collection(collection_name)
+        collection.clear_payload(selector=points_selector)
+        return self._default_update_result()
+
+    def update_collection_aliases(
+        self, change_aliases_operations: Sequence[types.AliasOperations], **kwargs: Any
+    ) -> bool:
+        for operation in change_aliases_operations:
+            if isinstance(operation, rest_models.CreateAliasOperation):
+                self._get_collection(operation.create_alias.collection_name)
+                self.aliases[
+                    operation.create_alias.alias_name
+                ] = operation.create_alias.collection_name
+            elif isinstance(operation, rest_models.DeleteAliasOperation):
+                self.aliases.pop(operation.delete_alias.alias_name, None)
+            elif isinstance(operation, rest_models.RenameAliasOperation):
+                new_name = operation.rename_alias.new_alias_name
+                old_name = operation.rename_alias.old_alias_name
+                self.aliases[new_name] = self.aliases.pop(old_name)
+            else:
+                raise ValueError(f"Unknown operation: {operation}")
+        self._save()
+        return True
 
-    async def recover_from_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        snapshot_recover: m.SnapshotRecover = None,
-    ) -> m.InlineResponse2003:
-        """
-        Recover local collection data from a snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
-        """
-        return await self._build_for_recover_from_snapshot(
-            collection_name=collection_name,
-            wait=wait,
-            snapshot_recover=snapshot_recover,
+    def get_collection_aliases(
+        self, collection_name: str, **kwargs: Any
+    ) -> types.CollectionsAliasesResponse:
+        return types.CollectionsAliasesResponse(
+            aliases=[
+                rest_models.AliasDescription(
+                    alias_name=alias_name,
+                    collection_name=name,
+                )
+                for alias_name, name in self.aliases.items()
+                if name == collection_name
+            ]
         )
 
-    async def recover_from_uploaded_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        priority: SnapshotPriority = None,
-        snapshot: IO[Any] = None,
-    ) -> m.InlineResponse2003:
-        """
-        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
-        """
-        return await self._build_for_recover_from_uploaded_snapshot(
-            collection_name=collection_name,
-            wait=wait,
-            priority=priority,
-            snapshot=snapshot,
+    def get_aliases(self, **kwargs: Any) -> types.CollectionsAliasesResponse:
+        return types.CollectionsAliasesResponse(
+            aliases=[
+                rest_models.AliasDescription(
+                    alias_name=alias_name,
+                    collection_name=name,
+                )
+                for alias_name, name in self.aliases.items()
+            ]
         )
 
-    async def update_aliases(
-        self,
-        timeout: int = None,
-        change_aliases_operation: m.ChangeAliasesOperation = None,
-    ) -> m.InlineResponse2003:
-        return await self._build_for_update_aliases(
-            timeout=timeout,
-            change_aliases_operation=change_aliases_operation,
+    def get_collections(self, **kwargs: Any) -> types.CollectionsResponse:
+        return types.CollectionsResponse(
+            collections=[
+                rest_models.CollectionDescription(name=name)
+                for name, _ in self.collections.items()
+            ]
         )
 
-    async def update_collection(
-        self,
-        collection_name: str,
-        timeout: int = None,
-        update_collection: m.UpdateCollection = None,
-    ) -> m.InlineResponse2003:
-        """
-        Update parameters of the existing collection
-        """
-        return await self._build_for_update_collection(
-            collection_name=collection_name,
-            timeout=timeout,
-            update_collection=update_collection,
-        )
+    def get_collection(self, collection_name: str, **kwargs: Any) -> types.CollectionInfo:
+        collection = self._get_collection(collection_name)
+        return collection.info()
 
-    async def update_collection_cluster(
-        self,
-        collection_name: str,
-        timeout: int = None,
-        cluster_operations: m.ClusterOperations = None,
-    ) -> m.InlineResponse2003:
-        return await self._build_for_update_collection_cluster(
-            collection_name=collection_name,
-            timeout=timeout,
-            cluster_operations=cluster_operations,
-        )
+    def update_collection(self, collection_name: str, **kwargs: Any) -> bool:
+        _collection = self._get_collection(collection_name)
+        return False
 
+    def _collection_path(self, collection_name: str) -> Optional[str]:
+        if self.persistent:
+            return os.path.join(self.location, "collection", collection_name)
+        else:
+            return None
 
-class SyncCollectionsApi(_CollectionsApi):
-    def collection_cluster_info(
-        self,
-        collection_name: str,
-    ) -> m.InlineResponse2007:
-        """
-        Get cluster information for a collection
-        """
-        return self._build_for_collection_cluster_info(
-            collection_name=collection_name,
-        )
+    def delete_collection(self, collection_name: str, **kwargs: Any) -> bool:
+        _collection = self.collections.pop(collection_name, None)
+        del _collection
+        self.aliases = {
+            alias_name: name
+            for alias_name, name in self.aliases.items()
+            if name != collection_name
+        }
+        collection_path = self._collection_path(collection_name)
+        if collection_path is not None:
+            shutil.rmtree(collection_path, ignore_errors=True)
+        self._save()
+        return True
 
     def create_collection(
         self,
         collection_name: str,
-        timeout: int = None,
-        create_collection: m.CreateCollection = None,
-    ) -> m.InlineResponse2003:
-        """
-        Create new collection with given parameters
-        """
-        return self._build_for_create_collection(
-            collection_name=collection_name,
-            timeout=timeout,
-            create_collection=create_collection,
-        )
-
-    def create_field_index(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        ordering: WriteOrdering = None,
-        create_field_index: m.CreateFieldIndex = None,
-    ) -> m.InlineResponse2006:
-        """
-        Create index for field in collection
-        """
-        return self._build_for_create_field_index(
-            collection_name=collection_name,
-            wait=wait,
-            ordering=ordering,
-            create_field_index=create_field_index,
-        )
-
-    def create_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-    ) -> m.InlineResponse20010:
-        """
-        Create new snapshot for a collection
-        """
-        return self._build_for_create_snapshot(
-            collection_name=collection_name,
-            wait=wait,
+        vectors_config: Union[types.VectorParams, Mapping[str, types.VectorParams]],
+        init_from: Optional[types.InitFrom] = None,
+        **kwargs: Any,
+    ) -> bool:
+        if collection_name in self.collections:
+            raise ValueError(f"Collection {collection_name} already exists")
+        collection_path = self._collection_path(collection_name)
+        if collection_path is not None:
+            os.makedirs(collection_path, exist_ok=True)
+
+        collection = LocalCollection(
+            rest_models.CreateCollection(
+                vectors=vectors_config,
+            ),
+            location=collection_path,
+        )
+
+        self.collections[collection_name] = collection
+        self._save()
+        return True
+
+    def recreate_collection(
+        self,
+        collection_name: str,
+        vectors_config: Union[types.VectorParams, Mapping[str, types.VectorParams]],
+        init_from: Optional[types.InitFrom] = None,
+        **kwargs: Any,
+    ) -> bool:
+        self.delete_collection(collection_name)
+        return self.create_collection(collection_name, vectors_config, init_from)
+
+    def upload_records(
+        self, collection_name: str, records: Iterable[types.Record], **kwargs: Any
+    ) -> None:
+        collection = self._get_collection(collection_name)
+        collection.upsert(
+            [
+                rest_models.PointStruct(
+                    id=record.id,
+                    vector=record.vector or {},
+                    payload=record.payload or {},
+                )
+                for record in records
+            ]
         )
 
-    def delete_collection(
+    def upload_collection(
         self,
         collection_name: str,
-        timeout: int = None,
-    ) -> m.InlineResponse2003:
-        """
-        Drop collection and all associated data
-        """
-        return self._build_for_delete_collection(
-            collection_name=collection_name,
-            timeout=timeout,
+        vectors: Union[
+            Dict[str, types.NumpyArray], types.NumpyArray, Iterable[types.VectorStruct]
+        ],
+        payload: Optional[Iterable[Dict[Any, Any]]] = None,
+        ids: Optional[Iterable[types.PointId]] = None,
+        **kwargs: Any,
+    ) -> None:
+        collection = self._get_collection(collection_name)
+        if isinstance(vectors, dict) and any(isinstance(v, np.ndarray) for v in vectors.values()):
+            assert (
+                len(set([arr.shape[0] for arr in vectors.values()])) == 1
+            ), "Each named vector should have the same number of vectors"
+
+            num_vectors = next(iter(vectors.values())).shape[0]
+            # convert Dict[str, np.ndarray] to List[Dict[str, List[float]]]
+            vectors = [
+                {name: vectors[name][i].tolist() for name in vectors.keys()}
+                for i in range(num_vectors)
+            ]
+
+        collection.upsert(
+            [
+                rest_models.PointStruct(
+                    id=point_id,
+                    vector=(vector.tolist() if isinstance(vector, np.ndarray) else vector) or {},
+                    payload=payload or {},
+                )
+                for (point_id, vector, payload) in zip(
+                    ids or itertools.count(),
+                    iter(vectors),
+                    payload or itertools.cycle([{}]),
+                )
+            ]
         )
 
-    def delete_field_index(
+    def create_payload_index(
         self,
         collection_name: str,
         field_name: str,
-        wait: bool = None,
-        ordering: WriteOrdering = None,
-    ) -> m.InlineResponse2006:
-        """
-        Delete field index for collection
-        """
-        return self._build_for_delete_field_index(
-            collection_name=collection_name,
-            field_name=field_name,
-            wait=wait,
-            ordering=ordering,
+        field_schema: Optional[types.PayloadSchemaType] = None,
+        field_type: Optional[types.PayloadSchemaType] = None,
+        **kwargs: Any,
+    ) -> types.UpdateResult:
+        logging.warning(
+            "Payload indexes have no effect in the local Qdrant. Please use server Qdrant if you need payload indexes."
+        )
+        return self._default_update_result()
+
+    def delete_payload_index(
+        self, collection_name: str, field_name: str, **kwargs: Any
+    ) -> types.UpdateResult:
+        logging.warning(
+            "Payload indexes have no effect in the local Qdrant. Please use server Qdrant if you need payload indexes."
         )
+        return self._default_update_result()
 
-    def delete_snapshot(
-        self,
-        collection_name: str,
-        snapshot_name: str,
-        wait: bool = None,
-    ) -> m.InlineResponse2003:
-        """
-        Delete snapshot for a collection
-        """
-        return self._build_for_delete_snapshot(
-            collection_name=collection_name,
-            snapshot_name=snapshot_name,
-            wait=wait,
-        )
+    def list_snapshots(
+        self, collection_name: str, **kwargs: Any
+    ) -> List[types.SnapshotDescription]:
+        return []
 
-    def get_collection(
-        self,
-        collection_name: str,
-    ) -> m.InlineResponse2005:
-        """
-        Get detailed information about specified existing collection
-        """
-        return self._build_for_get_collection(
-            collection_name=collection_name,
+    def create_snapshot(
+        self, collection_name: str, **kwargs: Any
+    ) -> Optional[types.SnapshotDescription]:
+        raise NotImplementedError(
+            "Snapshots are not supported in the local Qdrant. Please use server Qdrant if you need full snapshots."
         )
 
-    def get_collection_aliases(
-        self,
-        collection_name: str,
-    ) -> m.InlineResponse2008:
-        """
-        Get list of all aliases for a collection
-        """
-        return self._build_for_get_collection_aliases(
-            collection_name=collection_name,
+    def delete_snapshot(self, collection_name: str, snapshot_name: str, **kwargs: Any) -> bool:
+        raise NotImplementedError(
+            "Snapshots are not supported in the local Qdrant. Please use server Qdrant if you need full snapshots."
         )
 
-    def get_collections(
-        self,
-    ) -> m.InlineResponse2004:
-        """
-        Get list name of all existing collections
-        """
-        return self._build_for_get_collections()
-
-    def get_collections_aliases(
-        self,
-    ) -> m.InlineResponse2008:
-        """
-        Get list of all existing collections aliases
-        """
-        return self._build_for_get_collections_aliases()
+    def list_full_snapshots(self, **kwargs: Any) -> List[types.SnapshotDescription]:
+        return []
 
-    def get_snapshot(
-        self,
-        collection_name: str,
-        snapshot_name: str,
-    ) -> file:
-        """
-        Download specified snapshot from a collection as a file
-        """
-        return self._build_for_get_snapshot(
-            collection_name=collection_name,
-            snapshot_name=snapshot_name,
+    def create_full_snapshot(self, **kwargs: Any) -> types.SnapshotDescription:
+        raise NotImplementedError(
+            "Snapshots are not supported in the local Qdrant. Please use server Qdrant if you need full snapshots."
         )
 
-    def list_snapshots(
-        self,
-        collection_name: str,
-    ) -> m.InlineResponse2009:
-        """
-        Get list of snapshots for a collection
-        """
-        return self._build_for_list_snapshots(
-            collection_name=collection_name,
+    def delete_full_snapshot(self, snapshot_name: str, **kwargs: Any) -> bool:
+        raise NotImplementedError(
+            "Snapshots are not supported in the local Qdrant. Please use server Qdrant if you need full snapshots."
         )
 
-    def recover_from_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        snapshot_recover: m.SnapshotRecover = None,
-    ) -> m.InlineResponse2003:
-        """
-        Recover local collection data from a snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
-        """
-        return self._build_for_recover_from_snapshot(
-            collection_name=collection_name,
-            wait=wait,
-            snapshot_recover=snapshot_recover,
+    def recover_snapshot(self, collection_name: str, location: str, **kwargs: Any) -> bool:
+        raise NotImplementedError(
+            "Snapshots are not supported in the local Qdrant. Please use server Qdrant if you need full snapshots."
         )
 
-    def recover_from_uploaded_snapshot(
-        self,
-        collection_name: str,
-        wait: bool = None,
-        priority: SnapshotPriority = None,
-        snapshot: IO[Any] = None,
-    ) -> m.InlineResponse2003:
-        """
-        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
-        """
-        return self._build_for_recover_from_uploaded_snapshot(
-            collection_name=collection_name,
-            wait=wait,
-            priority=priority,
-            snapshot=snapshot,
+    def lock_storage(self, reason: str, **kwargs: Any) -> types.LocksOption:
+        raise NotImplementedError(
+            "Locks are not supported in the local Qdrant. Please use server Qdrant if you need full snapshots."
         )
 
-    def update_aliases(
-        self,
-        timeout: int = None,
-        change_aliases_operation: m.ChangeAliasesOperation = None,
-    ) -> m.InlineResponse2003:
-        return self._build_for_update_aliases(
-            timeout=timeout,
-            change_aliases_operation=change_aliases_operation,
+    def unlock_storage(self, **kwargs: Any) -> types.LocksOption:
+        raise NotImplementedError(
+            "Locks are not supported in the local Qdrant. Please use server Qdrant if you need full snapshots."
         )
 
-    def update_collection(
-        self,
-        collection_name: str,
-        timeout: int = None,
-        update_collection: m.UpdateCollection = None,
-    ) -> m.InlineResponse2003:
-        """
-        Update parameters of the existing collection
-        """
-        return self._build_for_update_collection(
-            collection_name=collection_name,
-            timeout=timeout,
-            update_collection=update_collection,
-        )
-
-    def update_collection_cluster(
-        self,
-        collection_name: str,
-        timeout: int = None,
-        cluster_operations: m.ClusterOperations = None,
-    ) -> m.InlineResponse2003:
-        return self._build_for_update_collection_cluster(
-            collection_name=collection_name,
-            timeout=timeout,
-            cluster_operations=cluster_operations,
+    def get_locks(self, **kwargs: Any) -> types.LocksOption:
+        return types.LocksOption(
+            error_message=None,
+            write=False,
         )
```

### Comparing `qdrant_client-1.3.1/qdrant_client/http/api/points_api.py` & `qdrant_client-1.3.2/qdrant_client/http/api/points_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,153 +1,37 @@
 # flake8: noqa E501
-from enum import Enum
-from pathlib import PurePath
-from types import GeneratorType
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Set, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, Set, Union
 
-from pydantic.json import ENCODERS_BY_TYPE
-from pydantic.main import BaseModel
+from qdrant_client._pydantic_compat import to_json
 from qdrant_client.http.models import *
 from qdrant_client.http.models import models as m
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 file = None
 
 
-def generate_encoders_by_class_tuples(type_encoder_map: Dict[Any, Callable]) -> Dict[Callable, Tuple]:
-    encoders_by_classes: Dict[Callable, List] = {}
-    for type_, encoder in type_encoder_map.items():
-        encoders_by_classes.setdefault(encoder, []).append(type_)
-    encoders_by_class_tuples: Dict[Callable, Tuple] = {}
-    for encoder, classes in encoders_by_classes.items():
-        encoders_by_class_tuples[encoder] = tuple(classes)
-    return encoders_by_class_tuples
-
-
-encoders_by_class_tuples = generate_encoders_by_class_tuples(ENCODERS_BY_TYPE)
-
-
 def jsonable_encoder(
     obj: Any,
     include: Union[SetIntStr, DictIntStrAny] = None,
     exclude=None,
     by_alias: bool = True,
     skip_defaults: bool = None,
     exclude_unset: bool = False,
-    include_none: bool = True,
-    custom_encoder=None,
-    sqlalchemy_safe: bool = True,
-) -> Any:
-    if exclude is None:
-        exclude = set()
-    if custom_encoder is None:
-        custom_encoder = {}
-    if include is not None and not isinstance(include, set):
-        include = set(include)
-    if exclude is not None and not isinstance(exclude, set):
-        exclude = set(exclude)
-    if isinstance(obj, BaseModel):
-        encoder = getattr(obj.Config, "json_encoders", {})
-        if custom_encoder:
-            encoder.update(custom_encoder)
-        obj_dict = obj.dict(
+):
+    if hasattr(obj, "json") or hasattr(obj, "model_dump_json"):
+        return to_json(
+            obj,
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=bool(exclude_unset or skip_defaults),
         )
 
-        return jsonable_encoder(
-            obj_dict,
-            include_none=include_none,
-            custom_encoder=encoder,
-            sqlalchemy_safe=sqlalchemy_safe,
-        )
-    if isinstance(obj, Enum):
-        return obj.value
-    if isinstance(obj, PurePath):
-        return str(obj)
-    if isinstance(obj, (str, int, float, type(None))):
-        return obj
-    if isinstance(obj, dict):
-        encoded_dict = {}
-        for key, value in obj.items():
-            if (
-                (not sqlalchemy_safe or (not isinstance(key, str)) or (not key.startswith("_sa")))
-                and (value is not None or include_none)
-                and ((include and key in include) or key not in exclude)
-            ):
-                encoded_key = jsonable_encoder(
-                    key,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-                encoded_value = jsonable_encoder(
-                    value,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-                encoded_dict[encoded_key] = encoded_value
-        return encoded_dict
-    if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
-        encoded_list = []
-        for item in obj:
-            encoded_list.append(
-                jsonable_encoder(
-                    item,
-                    include=include,
-                    exclude=exclude,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-            )
-        return encoded_list
-
-    if custom_encoder:
-        if type(obj) in custom_encoder:
-            return custom_encoder[type(obj)](obj)
-        else:
-            for encoder_type, encoder in custom_encoder.items():
-                if isinstance(obj, encoder_type):
-                    return encoder(obj)
-
-    if type(obj) in ENCODERS_BY_TYPE:
-        return ENCODERS_BY_TYPE[type(obj)](obj)
-    for encoder, classes_tuple in encoders_by_class_tuples.items():
-        if isinstance(obj, classes_tuple):
-            return encoder(obj)
-
-    errors: List[Exception] = []
-    try:
-        data = dict(obj)
-    except Exception as e:
-        errors.append(e)
-        try:
-            data = vars(obj)
-        except Exception as e:
-            errors.append(e)
-            raise ValueError(errors)
-    return jsonable_encoder(
-        data,
-        by_alias=by_alias,
-        exclude_unset=exclude_unset,
-        include_none=include_none,
-        custom_encoder=custom_encoder,
-        sqlalchemy_safe=sqlalchemy_safe,
-    )
+    return obj
 
 
 if TYPE_CHECKING:
     from qdrant_client.http.api_client import ApiClient
 
 
 class _PointsApi:
@@ -170,45 +54,49 @@
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
         if ordering is not None:
             query_params["ordering"] = str(ordering)
 
+        headers = {}
         body = jsonable_encoder(points_selector)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2006,
             method="POST",
             url="/collections/{collection_name}/points/payload/clear",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_count_points(
         self,
         collection_name: str,
         count_request: m.CountRequest = None,
     ):
         """
         Count points which matches given filtering condition
         """
         path_params = {
             "collection_name": str(collection_name),
         }
 
+        headers = {}
         body = jsonable_encoder(count_request)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20017,
             method="POST",
             url="/collections/{collection_name}/points/count",
             path_params=path_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_delete_payload(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
@@ -223,23 +111,25 @@
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
         if ordering is not None:
             query_params["ordering"] = str(ordering)
 
+        headers = {}
         body = jsonable_encoder(delete_payload)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2006,
             method="POST",
             url="/collections/{collection_name}/points/payload/delete",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_delete_points(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
@@ -254,23 +144,25 @@
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
         if ordering is not None:
             query_params["ordering"] = str(ordering)
 
+        headers = {}
         body = jsonable_encoder(points_selector)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2006,
             method="POST",
             url="/collections/{collection_name}/points/delete",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_delete_vectors(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
@@ -285,23 +177,25 @@
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
         if ordering is not None:
             query_params["ordering"] = str(ordering)
 
+        headers = {}
         body = jsonable_encoder(delete_vectors)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2006,
             method="POST",
             url="/collections/{collection_name}/points/vectors/delete",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_get_point(
         self,
         collection_name: str,
         id: m.ExtendedPointId,
         consistency: m.ReadConsistency = None,
@@ -339,23 +233,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if consistency is not None:
             query_params["consistency"] = str(consistency)
 
+        headers = {}
         body = jsonable_encoder(point_request)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20012,
             method="POST",
             url="/collections/{collection_name}/points",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_overwrite_payload(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
@@ -370,23 +266,25 @@
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
         if ordering is not None:
             query_params["ordering"] = str(ordering)
 
+        headers = {}
         body = jsonable_encoder(set_payload)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2006,
             method="PUT",
             url="/collections/{collection_name}/points/payload",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_recommend_batch_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         recommend_request_batch: m.RecommendRequestBatch = None,
@@ -398,23 +296,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if consistency is not None:
             query_params["consistency"] = str(consistency)
 
+        headers = {}
         body = jsonable_encoder(recommend_request_batch)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20015,
             method="POST",
             url="/collections/{collection_name}/points/recommend/batch",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_recommend_point_groups(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         recommend_groups_request: m.RecommendGroupsRequest = None,
@@ -426,23 +326,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if consistency is not None:
             query_params["consistency"] = str(consistency)
 
+        headers = {}
         body = jsonable_encoder(recommend_groups_request)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20016,
             method="POST",
             url="/collections/{collection_name}/points/recommend/groups",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_recommend_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         recommend_request: m.RecommendRequest = None,
@@ -454,23 +356,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if consistency is not None:
             query_params["consistency"] = str(consistency)
 
+        headers = {}
         body = jsonable_encoder(recommend_request)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20014,
             method="POST",
             url="/collections/{collection_name}/points/recommend",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_scroll_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         scroll_request: m.ScrollRequest = None,
@@ -482,23 +386,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if consistency is not None:
             query_params["consistency"] = str(consistency)
 
+        headers = {}
         body = jsonable_encoder(scroll_request)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20013,
             method="POST",
             url="/collections/{collection_name}/points/scroll",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_search_batch_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         search_request_batch: m.SearchRequestBatch = None,
@@ -510,23 +416,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if consistency is not None:
             query_params["consistency"] = str(consistency)
 
+        headers = {}
         body = jsonable_encoder(search_request_batch)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20015,
             method="POST",
             url="/collections/{collection_name}/points/search/batch",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_search_point_groups(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         search_groups_request: m.SearchGroupsRequest = None,
@@ -538,23 +446,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if consistency is not None:
             query_params["consistency"] = str(consistency)
 
+        headers = {}
         body = jsonable_encoder(search_groups_request)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20016,
             method="POST",
             url="/collections/{collection_name}/points/search/groups",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_search_points(
         self,
         collection_name: str,
         consistency: m.ReadConsistency = None,
         search_request: m.SearchRequest = None,
@@ -566,23 +476,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if consistency is not None:
             query_params["consistency"] = str(consistency)
 
+        headers = {}
         body = jsonable_encoder(search_request)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse20014,
             method="POST",
             url="/collections/{collection_name}/points/search",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_set_payload(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
@@ -597,23 +509,25 @@
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
         if ordering is not None:
             query_params["ordering"] = str(ordering)
 
+        headers = {}
         body = jsonable_encoder(set_payload)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2006,
             method="POST",
             url="/collections/{collection_name}/points/payload",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_update_vectors(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
@@ -628,23 +542,25 @@
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
         if ordering is not None:
             query_params["ordering"] = str(ordering)
 
+        headers = {}
         body = jsonable_encoder(update_vectors)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2006,
             method="PUT",
             url="/collections/{collection_name}/points/vectors",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_upsert_points(
         self,
         collection_name: str,
         wait: bool = None,
         ordering: WriteOrdering = None,
@@ -659,23 +575,25 @@
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
         if ordering is not None:
             query_params["ordering"] = str(ordering)
 
+        headers = {}
         body = jsonable_encoder(point_insert_operations)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2006,
             method="PUT",
             url="/collections/{collection_name}/points",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
 
 class AsyncPointsApi(_PointsApi):
     async def clear_payload(
         self,
         collection_name: str,
```

### Comparing `qdrant_client-1.3.1/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.3.2/qdrant_client/http/api/snapshots_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,153 +1,37 @@
 # flake8: noqa E501
-from enum import Enum
-from pathlib import PurePath
-from types import GeneratorType
-from typing import IO, TYPE_CHECKING, Any, Callable, Dict, List, Set, Tuple, Union
+from typing import IO, TYPE_CHECKING, Any, Dict, Set, Union
 
-from pydantic.json import ENCODERS_BY_TYPE
-from pydantic.main import BaseModel
+from qdrant_client._pydantic_compat import to_json
 from qdrant_client.http.models import *
 from qdrant_client.http.models import models as m
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 file = None
 
 
-def generate_encoders_by_class_tuples(type_encoder_map: Dict[Any, Callable]) -> Dict[Callable, Tuple]:
-    encoders_by_classes: Dict[Callable, List] = {}
-    for type_, encoder in type_encoder_map.items():
-        encoders_by_classes.setdefault(encoder, []).append(type_)
-    encoders_by_class_tuples: Dict[Callable, Tuple] = {}
-    for encoder, classes in encoders_by_classes.items():
-        encoders_by_class_tuples[encoder] = tuple(classes)
-    return encoders_by_class_tuples
-
-
-encoders_by_class_tuples = generate_encoders_by_class_tuples(ENCODERS_BY_TYPE)
-
-
 def jsonable_encoder(
     obj: Any,
     include: Union[SetIntStr, DictIntStrAny] = None,
     exclude=None,
     by_alias: bool = True,
     skip_defaults: bool = None,
     exclude_unset: bool = False,
-    include_none: bool = True,
-    custom_encoder=None,
-    sqlalchemy_safe: bool = True,
-) -> Any:
-    if exclude is None:
-        exclude = set()
-    if custom_encoder is None:
-        custom_encoder = {}
-    if include is not None and not isinstance(include, set):
-        include = set(include)
-    if exclude is not None and not isinstance(exclude, set):
-        exclude = set(exclude)
-    if isinstance(obj, BaseModel):
-        encoder = getattr(obj.Config, "json_encoders", {})
-        if custom_encoder:
-            encoder.update(custom_encoder)
-        obj_dict = obj.dict(
+):
+    if hasattr(obj, "json") or hasattr(obj, "model_dump_json"):
+        return to_json(
+            obj,
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=bool(exclude_unset or skip_defaults),
         )
 
-        return jsonable_encoder(
-            obj_dict,
-            include_none=include_none,
-            custom_encoder=encoder,
-            sqlalchemy_safe=sqlalchemy_safe,
-        )
-    if isinstance(obj, Enum):
-        return obj.value
-    if isinstance(obj, PurePath):
-        return str(obj)
-    if isinstance(obj, (str, int, float, type(None))):
-        return obj
-    if isinstance(obj, dict):
-        encoded_dict = {}
-        for key, value in obj.items():
-            if (
-                (not sqlalchemy_safe or (not isinstance(key, str)) or (not key.startswith("_sa")))
-                and (value is not None or include_none)
-                and ((include and key in include) or key not in exclude)
-            ):
-                encoded_key = jsonable_encoder(
-                    key,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-                encoded_value = jsonable_encoder(
-                    value,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-                encoded_dict[encoded_key] = encoded_value
-        return encoded_dict
-    if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
-        encoded_list = []
-        for item in obj:
-            encoded_list.append(
-                jsonable_encoder(
-                    item,
-                    include=include,
-                    exclude=exclude,
-                    by_alias=by_alias,
-                    exclude_unset=exclude_unset,
-                    include_none=include_none,
-                    custom_encoder=custom_encoder,
-                    sqlalchemy_safe=sqlalchemy_safe,
-                )
-            )
-        return encoded_list
-
-    if custom_encoder:
-        if type(obj) in custom_encoder:
-            return custom_encoder[type(obj)](obj)
-        else:
-            for encoder_type, encoder in custom_encoder.items():
-                if isinstance(obj, encoder_type):
-                    return encoder(obj)
-
-    if type(obj) in ENCODERS_BY_TYPE:
-        return ENCODERS_BY_TYPE[type(obj)](obj)
-    for encoder, classes_tuple in encoders_by_class_tuples.items():
-        if isinstance(obj, classes_tuple):
-            return encoder(obj)
-
-    errors: List[Exception] = []
-    try:
-        data = dict(obj)
-    except Exception as e:
-        errors.append(e)
-        try:
-            data = vars(obj)
-        except Exception as e:
-            errors.append(e)
-            raise ValueError(errors)
-    return jsonable_encoder(
-        data,
-        by_alias=by_alias,
-        exclude_unset=exclude_unset,
-        include_none=include_none,
-        custom_encoder=custom_encoder,
-        sqlalchemy_safe=sqlalchemy_safe,
-    )
+    return obj
 
 
 if TYPE_CHECKING:
     from qdrant_client.http.api_client import ApiClient
 
 
 class _SnapshotsApi:
@@ -327,23 +211,25 @@
             "collection_name": str(collection_name),
         }
 
         query_params = {}
         if wait is not None:
             query_params["wait"] = str(wait).lower()
 
+        headers = {}
         body = jsonable_encoder(snapshot_recover)
-
+        if "Content-Type" not in headers:
+            headers["Content-Type"] = "application/json"
         return self.api_client.request(
             type_=m.InlineResponse2003,
             method="PUT",
             url="/collections/{collection_name}/snapshots/recover",
             path_params=path_params,
             params=query_params,
-            json=body,
+            data=body,
         )
 
     def _build_for_recover_from_uploaded_snapshot(
         self,
         collection_name: str,
         wait: bool = None,
         priority: SnapshotPriority = None,
```

### Comparing `qdrant_client-1.3.1/qdrant_client/http/api_client.py` & `qdrant_client-1.3.2/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/http/exceptions.py` & `qdrant_client-1.3.2/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/http/models/models.py` & `qdrant_client-1.3.2/qdrant_client/http/models/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,68 +10,68 @@
 
 from pydantic import BaseModel, Field
 from pydantic.types import StrictBool, StrictFloat, StrictInt, StrictStr
 
 Payload = Dict[Any, Any]
 
 
-class AbortTransferOperation(BaseModel):
+class AbortTransferOperation(BaseModel, extra="forbid"):
     abort_transfer: "MoveShard" = Field(..., description="")
 
 
-class AliasDescription(BaseModel):
+class AliasDescription(BaseModel, extra="forbid"):
     alias_name: str = Field(..., description="")
     collection_name: str = Field(..., description="")
 
 
-class AppBuildTelemetry(BaseModel):
+class AppBuildTelemetry(BaseModel, extra="forbid"):
     name: str = Field(..., description="")
     version: str = Field(..., description="")
     features: Optional["AppFeaturesTelemetry"] = Field(default=None, description="")
     system: Optional["RunningEnvironmentTelemetry"] = Field(default=None, description="")
     startup: datetime = Field(..., description="")
 
 
-class AppFeaturesTelemetry(BaseModel):
+class AppFeaturesTelemetry(BaseModel, extra="forbid"):
     debug: bool = Field(..., description="")
     web_feature: bool = Field(..., description="")
     service_debug_feature: bool = Field(..., description="")
     recovery_mode: bool = Field(..., description="")
 
 
-class Batch(BaseModel):
+class Batch(BaseModel, extra="forbid"):
     ids: List["ExtendedPointId"] = Field(..., description="")
     vectors: "BatchVectorStruct" = Field(..., description="")
     payloads: Optional[List["Payload"]] = Field(default=None, description="")
 
 
-class ChangeAliasesOperation(BaseModel):
+class ChangeAliasesOperation(BaseModel, extra="forbid"):
     """
     Operation for performing changes of collection aliases. Alias changes are atomic, meaning that no collection modifications can happen between alias operations.
     """
 
     actions: List["AliasOperations"] = Field(
         ...,
         description="Operation for performing changes of collection aliases. Alias changes are atomic, meaning that no collection modifications can happen between alias operations.",
     )
 
 
-class ClusterConfigTelemetry(BaseModel):
+class ClusterConfigTelemetry(BaseModel, extra="forbid"):
     grpc_timeout_ms: int = Field(..., description="")
     p2p: "P2pConfigTelemetry" = Field(..., description="")
     consensus: "ConsensusConfigTelemetry" = Field(..., description="")
 
 
-class ClusterStatusOneOf(BaseModel):
+class ClusterStatusOneOf(BaseModel, extra="forbid"):
     status: Literal[
         "disabled",
     ] = Field(..., description="")
 
 
-class ClusterStatusOneOf1(BaseModel):
+class ClusterStatusOneOf1(BaseModel, extra="forbid"):
     """
     Description of enabled cluster
     """
 
     status: Literal[
         "enabled",
     ] = Field(..., description="Description of enabled cluster")
@@ -81,56 +81,56 @@
     consensus_thread_status: "ConsensusThreadStatus" = Field(..., description="Description of enabled cluster")
     message_send_failures: Dict[str, "MessageSendErrors"] = Field(
         ...,
         description="Consequent failures of message send operations in consensus by peer address. On the first success to send to that peer - entry is removed from this hashmap.",
     )
 
 
-class ClusterStatusTelemetry(BaseModel):
+class ClusterStatusTelemetry(BaseModel, extra="forbid"):
     number_of_peers: int = Field(..., description="")
     term: int = Field(..., description="")
     commit: int = Field(..., description="")
     pending_operations: int = Field(..., description="")
     role: Optional["StateRole"] = Field(default=None, description="")
     is_voter: bool = Field(..., description="")
     peer_id: Optional[int] = Field(default=None, description="")
     consensus_thread_status: "ConsensusThreadStatus" = Field(..., description="")
 
 
-class ClusterTelemetry(BaseModel):
+class ClusterTelemetry(BaseModel, extra="forbid"):
     enabled: bool = Field(..., description="")
     status: Optional["ClusterStatusTelemetry"] = Field(default=None, description="")
     config: Optional["ClusterConfigTelemetry"] = Field(default=None, description="")
 
 
-class CollectionClusterInfo(BaseModel):
+class CollectionClusterInfo(BaseModel, extra="forbid"):
     """
     Current clustering distribution for the collection
     """
 
     peer_id: int = Field(..., description="ID of this peer")
     shard_count: int = Field(..., description="Total number of shards")
     local_shards: List["LocalShardInfo"] = Field(..., description="Local shards")
     remote_shards: List["RemoteShardInfo"] = Field(..., description="Remote shards")
     shard_transfers: List["ShardTransferInfo"] = Field(..., description="Shard transfers")
 
 
-class CollectionConfig(BaseModel):
+class CollectionConfig(BaseModel, extra="forbid"):
     params: "CollectionParams" = Field(..., description="")
     hnsw_config: "HnswConfig" = Field(..., description="")
     optimizer_config: "OptimizersConfig" = Field(..., description="")
     wal_config: "WalConfig" = Field(..., description="")
     quantization_config: Optional["QuantizationConfig"] = Field(default=None, description="")
 
 
-class CollectionDescription(BaseModel):
+class CollectionDescription(BaseModel, extra="forbid"):
     name: str = Field(..., description="")
 
 
-class CollectionInfo(BaseModel):
+class CollectionInfo(BaseModel, extra="forbid"):
     """
     Current statistics and configuration of the collection
     """
 
     status: "CollectionStatus" = Field(..., description="Current statistics and configuration of the collection")
     optimizer_status: "OptimizersStatus" = Field(
         ..., description="Current statistics and configuration of the collection"
@@ -149,138 +149,138 @@
     segments_count: int = Field(
         ..., description="Number of segments in collection. Each segment has independent vector as payload indexes"
     )
     config: "CollectionConfig" = Field(..., description="Current statistics and configuration of the collection")
     payload_schema: Dict[str, "PayloadIndexInfo"] = Field(..., description="Types of stored payload")
 
 
-class CollectionParams(BaseModel):
+class CollectionParams(BaseModel, extra="forbid"):
     vectors: "VectorsConfig" = Field(..., description="")
     shard_number: Optional[int] = Field(default=1, description="Number of shards the collection has")
     replication_factor: Optional[int] = Field(default=1, description="Number of replicas for each shard")
     write_consistency_factor: Optional[int] = Field(
         default=1,
         description="Defines how many replicas should apply the operation for us to consider it successful. Increasing this number will make the collection more resilient to inconsistencies, but will also make it fail if not enough replicas are available. Does not have any performance impact.",
     )
     on_disk_payload: Optional[bool] = Field(
         default=False,
         description="If true - point&#x27;s payload will not be stored in memory. It will be read from the disk every time it is requested. This setting saves RAM by (slightly) increasing the response time. Note: those payload values that are involved in filtering and are indexed - remain in RAM.",
     )
 
 
-class CollectionParamsDiff(BaseModel):
+class CollectionParamsDiff(BaseModel, extra="forbid"):
     replication_factor: Optional[int] = Field(default=None, description="Number of replicas for each shard")
     write_consistency_factor: Optional[int] = Field(
         default=None, description="Minimal number successful responses from replicas to consider operation successful"
     )
 
 
 class CollectionStatus(str, Enum):
     GREEN = "green"
     YELLOW = "yellow"
     RED = "red"
 
 
-class CollectionTelemetry(BaseModel):
+class CollectionTelemetry(BaseModel, extra="forbid"):
     id: str = Field(..., description="")
     init_time_ms: int = Field(..., description="")
     config: "CollectionConfig" = Field(..., description="")
     shards: List["ReplicaSetTelemetry"] = Field(..., description="")
     transfers: List["ShardTransferInfo"] = Field(..., description="")
 
 
-class CollectionsAggregatedTelemetry(BaseModel):
+class CollectionsAggregatedTelemetry(BaseModel, extra="forbid"):
     vectors: int = Field(..., description="")
     optimizers_status: "OptimizersStatus" = Field(..., description="")
     params: "CollectionParams" = Field(..., description="")
 
 
-class CollectionsAliasesResponse(BaseModel):
+class CollectionsAliasesResponse(BaseModel, extra="forbid"):
     aliases: List["AliasDescription"] = Field(..., description="")
 
 
-class CollectionsResponse(BaseModel):
+class CollectionsResponse(BaseModel, extra="forbid"):
     collections: List["CollectionDescription"] = Field(..., description="")
 
 
-class CollectionsTelemetry(BaseModel):
+class CollectionsTelemetry(BaseModel, extra="forbid"):
     number_of_collections: int = Field(..., description="")
     collections: Optional[List["CollectionTelemetryEnum"]] = Field(default=None, description="")
 
 
 class CompressionRatio(str, Enum):
     X4 = "x4"
     X8 = "x8"
     X16 = "x16"
     X32 = "x32"
     X64 = "x64"
 
 
-class ConsensusConfigTelemetry(BaseModel):
+class ConsensusConfigTelemetry(BaseModel, extra="forbid"):
     max_message_queue_size: int = Field(..., description="")
     tick_period_ms: int = Field(..., description="")
     bootstrap_timeout_sec: int = Field(..., description="")
 
 
-class ConsensusThreadStatusOneOf(BaseModel):
+class ConsensusThreadStatusOneOf(BaseModel, extra="forbid"):
     consensus_thread_status: Literal[
         "working",
     ] = Field(..., description="")
     last_update: datetime = Field(..., description="")
 
 
-class ConsensusThreadStatusOneOf1(BaseModel):
+class ConsensusThreadStatusOneOf1(BaseModel, extra="forbid"):
     consensus_thread_status: Literal[
         "stopped",
     ] = Field(..., description="")
 
 
-class ConsensusThreadStatusOneOf2(BaseModel):
+class ConsensusThreadStatusOneOf2(BaseModel, extra="forbid"):
     consensus_thread_status: Literal[
         "stopped_with_err",
     ] = Field(..., description="")
     err: str = Field(..., description="")
 
 
-class CountRequest(BaseModel):
+class CountRequest(BaseModel, extra="forbid"):
     """
     Count Request Counts the number of points which satisfy the given filter. If filter is not provided, the count of all points in the collection will be returned.
     """
 
     filter: Optional["Filter"] = Field(default=None, description="Look only for points which satisfies this conditions")
     exact: Optional[bool] = Field(
         default=True,
         description="If true, count exact number of points. If false, count approximate number of points faster. Approximate count might be unreliable during the indexing process. Default: true",
     )
 
 
-class CountResult(BaseModel):
+class CountResult(BaseModel, extra="forbid"):
     count: int = Field(..., description="Number of points which satisfy the conditions")
 
 
-class CreateAlias(BaseModel):
+class CreateAlias(BaseModel, extra="forbid"):
     """
     Create alternative name for a collection. Collection will be available under both names for search, retrieve,
     """
 
     collection_name: str = Field(
         ...,
         description="Create alternative name for a collection. Collection will be available under both names for search, retrieve,",
     )
     alias_name: str = Field(
         ...,
         description="Create alternative name for a collection. Collection will be available under both names for search, retrieve,",
     )
 
 
-class CreateAliasOperation(BaseModel):
+class CreateAliasOperation(BaseModel, extra="forbid"):
     create_alias: "CreateAlias" = Field(..., description="")
 
 
-class CreateCollection(BaseModel):
+class CreateCollection(BaseModel, extra="forbid"):
     """
     Operation for creating new collection and (optionally) specify index params
     """
 
     vectors: "VectorsConfig" = Field(
         ..., description="Operation for creating new collection and (optionally) specify index params"
     )
@@ -312,46 +312,46 @@
     )
     init_from: Optional["InitFrom"] = Field(default=None, description="Specify other collection to copy data from.")
     quantization_config: Optional["QuantizationConfig"] = Field(
         default=None, description="Quantization parameters. If none - quantization is disabled."
     )
 
 
-class CreateFieldIndex(BaseModel):
+class CreateFieldIndex(BaseModel, extra="forbid"):
     field_name: str = Field(..., description="")
     field_schema: Optional["PayloadFieldSchema"] = Field(default=None, description="")
 
 
-class DeleteAlias(BaseModel):
+class DeleteAlias(BaseModel, extra="forbid"):
     """
     Delete alias if exists
     """
 
     alias_name: str = Field(..., description="Delete alias if exists")
 
 
-class DeleteAliasOperation(BaseModel):
+class DeleteAliasOperation(BaseModel, extra="forbid"):
     """
     Delete alias if exists
     """
 
     delete_alias: "DeleteAlias" = Field(..., description="Delete alias if exists")
 
 
-class DeletePayload(BaseModel):
+class DeletePayload(BaseModel, extra="forbid"):
     keys: List[str] = Field(..., description="List of payload keys to remove from payload")
     points: Optional[List["ExtendedPointId"]] = Field(
         default=None, description="Deletes values from each point in this list"
     )
     filter: Optional["Filter"] = Field(
         default=None, description="Deletes values from points that satisfy this filter condition"
     )
 
 
-class DeleteVectors(BaseModel):
+class DeleteVectors(BaseModel, extra="forbid"):
     points: Optional[List["ExtendedPointId"]] = Field(
         default=None, description="Deletes values from each point in this list"
     )
     filter: Optional["Filter"] = Field(
         default=None, description="Deletes values from points that satisfy this filter condition"
     )
     vector: List[str] = Field(..., description="Vector names")
@@ -359,108 +359,108 @@
 
 class Distance(str, Enum):
     COSINE = "Cosine"
     EUCLID = "Euclid"
     DOT = "Dot"
 
 
-class DropReplicaOperation(BaseModel):
+class DropReplicaOperation(BaseModel, extra="forbid"):
     drop_replica: "Replica" = Field(..., description="")
 
 
-class ErrorResponse(BaseModel):
+class ErrorResponse(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Optional["ErrorResponseStatus"] = Field(default=None, description="")
     result: Optional[Any] = Field(default=None, description="")
 
 
-class ErrorResponseStatus(BaseModel):
+class ErrorResponseStatus(BaseModel, extra="forbid"):
     error: Optional[str] = Field(default=None, description="Description of the occurred error.")
 
 
-class FieldCondition(BaseModel):
+class FieldCondition(BaseModel, extra="forbid"):
     """
     All possible payload filtering conditions
     """
 
     key: str = Field(..., description="Payload key")
     match: Optional["Match"] = Field(default=None, description="Check if point has field with a given value")
     range: Optional["Range"] = Field(default=None, description="Check if points value lies in a given range")
     geo_bounding_box: Optional["GeoBoundingBox"] = Field(
         default=None, description="Check if points geo location lies in a given area"
     )
     geo_radius: Optional["GeoRadius"] = Field(default=None, description="Check if geo point is within a given radius")
     values_count: Optional["ValuesCount"] = Field(default=None, description="Check number of values of the field")
 
 
-class Filter(BaseModel):
+class Filter(BaseModel, extra="forbid"):
     should: Optional[List["Condition"]] = Field(
         default=None, description="At least one of those conditions should match"
     )
     must: Optional[List["Condition"]] = Field(default=None, description="All conditions must match")
     must_not: Optional[List["Condition"]] = Field(default=None, description="All conditions must NOT match")
 
 
-class FilterSelector(BaseModel):
+class FilterSelector(BaseModel, extra="forbid"):
     filter: "Filter" = Field(..., description="")
 
 
-class GeoBoundingBox(BaseModel):
+class GeoBoundingBox(BaseModel, extra="forbid"):
     """
     Geo filter request  Matches coordinates inside the rectangle, described by coordinates of lop-left and bottom-right edges
     """
 
     top_left: "GeoPoint" = Field(
         ...,
         description="Geo filter request  Matches coordinates inside the rectangle, described by coordinates of lop-left and bottom-right edges",
     )
     bottom_right: "GeoPoint" = Field(
         ...,
         description="Geo filter request  Matches coordinates inside the rectangle, described by coordinates of lop-left and bottom-right edges",
     )
 
 
-class GeoPoint(BaseModel):
+class GeoPoint(BaseModel, extra="forbid"):
     """
     Geo point payload schema
     """
 
     lon: float = Field(..., description="Geo point payload schema")
     lat: float = Field(..., description="Geo point payload schema")
 
 
-class GeoRadius(BaseModel):
+class GeoRadius(BaseModel, extra="forbid"):
     """
     Geo filter request  Matches coordinates inside the circle of `radius` and center with coordinates `center`
     """
 
     center: "GeoPoint" = Field(
         ...,
         description="Geo filter request  Matches coordinates inside the circle of `radius` and center with coordinates `center`",
     )
     radius: float = Field(..., description="Radius of the area in meters")
 
 
-class GroupsResult(BaseModel):
+class GroupsResult(BaseModel, extra="forbid"):
     groups: List["PointGroup"] = Field(..., description="")
 
 
-class GrpcTelemetry(BaseModel):
+class GrpcTelemetry(BaseModel, extra="forbid"):
     responses: Dict[str, "OperationDurationStatistics"] = Field(..., description="")
 
 
-class HasIdCondition(BaseModel):
+class HasIdCondition(BaseModel, extra="forbid"):
     """
     ID-based filtering condition
     """
 
     has_id: List["ExtendedPointId"] = Field(..., description="ID-based filtering condition")
 
 
-class HnswConfig(BaseModel):
+class HnswConfig(BaseModel, extra="forbid"):
     """
     Config of HNSW index
     """
 
     m: int = Field(
         ...,
         description="Number of edges per node in the index graph. Larger the value - more accurate the search, more space required.",
@@ -482,15 +482,15 @@
     )
     payload_m: Optional[int] = Field(
         default=None,
         description="Custom M param for hnsw graph built for payload index. If not set, default M will be used.",
     )
 
 
-class HnswConfigDiff(BaseModel):
+class HnswConfigDiff(BaseModel, extra="forbid"):
     m: Optional[int] = Field(
         default=None,
         description="Number of edges per node in the index graph. Larger the value - more accurate the search, more space required.",
     )
     ef_construct: Optional[int] = Field(
         default=None,
         description="Number of neighbours to consider during the index building. Larger the value - more accurate the search, more time required to build the index.",
@@ -509,340 +509,340 @@
     )
     payload_m: Optional[int] = Field(
         default=None,
         description="Custom M param for additional payload-aware HNSW links. If not set, default M will be used.",
     )
 
 
-class IndexesOneOf(BaseModel):
+class IndexesOneOf(BaseModel, extra="forbid"):
     """
     Do not use any index, scan whole vector collection during search. Guarantee 100% precision, but may be time consuming on large collections.
     """
 
     type: Literal["plain",] = Field(
         ...,
         description="Do not use any index, scan whole vector collection during search. Guarantee 100% precision, but may be time consuming on large collections.",
     )
     options: Any = Field(
         ...,
         description="Do not use any index, scan whole vector collection during search. Guarantee 100% precision, but may be time consuming on large collections.",
     )
 
 
-class IndexesOneOf1(BaseModel):
+class IndexesOneOf1(BaseModel, extra="forbid"):
     """
     Use filterable HNSW index for approximate search. Is very fast even on a very huge collections, but require additional space to store index and additional time to build it.
     """
 
     type: Literal["hnsw",] = Field(
         ...,
         description="Use filterable HNSW index for approximate search. Is very fast even on a very huge collections, but require additional space to store index and additional time to build it.",
     )
     options: "HnswConfig" = Field(
         ...,
         description="Use filterable HNSW index for approximate search. Is very fast even on a very huge collections, but require additional space to store index and additional time to build it.",
     )
 
 
-class InitFrom(BaseModel):
+class InitFrom(BaseModel, extra="forbid"):
     """
     Operation for creating new collection and (optionally) specify index params
     """
 
     collection: str = Field(
         ..., description="Operation for creating new collection and (optionally) specify index params"
     )
 
 
-class InlineResponse200(BaseModel):
+class InlineResponse200(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["TelemetryData"] = Field(default=None, description="")
 
 
-class InlineResponse2001(BaseModel):
+class InlineResponse2001(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["LocksOption"] = Field(default=None, description="")
 
 
-class InlineResponse20010(BaseModel):
+class InlineResponse20010(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["SnapshotDescription"] = Field(default=None, description="")
 
 
-class InlineResponse20011(BaseModel):
+class InlineResponse20011(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["Record"] = Field(default=None, description="")
 
 
-class InlineResponse20012(BaseModel):
+class InlineResponse20012(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional[List["Record"]] = Field(default=None, description="")
 
 
-class InlineResponse20013(BaseModel):
+class InlineResponse20013(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["ScrollResult"] = Field(default=None, description="")
 
 
-class InlineResponse20014(BaseModel):
+class InlineResponse20014(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional[List["ScoredPoint"]] = Field(default=None, description="")
 
 
-class InlineResponse20015(BaseModel):
+class InlineResponse20015(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional[List[List["ScoredPoint"]]] = Field(default=None, description="")
 
 
-class InlineResponse20016(BaseModel):
+class InlineResponse20016(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["GroupsResult"] = Field(default=None, description="")
 
 
-class InlineResponse20017(BaseModel):
+class InlineResponse20017(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["CountResult"] = Field(default=None, description="")
 
 
-class InlineResponse2002(BaseModel):
+class InlineResponse2002(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["ClusterStatus"] = Field(default=None, description="")
 
 
-class InlineResponse2003(BaseModel):
+class InlineResponse2003(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional[bool] = Field(default=None, description="")
 
 
-class InlineResponse2004(BaseModel):
+class InlineResponse2004(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["CollectionsResponse"] = Field(default=None, description="")
 
 
-class InlineResponse2005(BaseModel):
+class InlineResponse2005(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["CollectionInfo"] = Field(default=None, description="")
 
 
-class InlineResponse2006(BaseModel):
+class InlineResponse2006(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["UpdateResult"] = Field(default=None, description="")
 
 
-class InlineResponse2007(BaseModel):
+class InlineResponse2007(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["CollectionClusterInfo"] = Field(default=None, description="")
 
 
-class InlineResponse2008(BaseModel):
+class InlineResponse2008(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional["CollectionsAliasesResponse"] = Field(default=None, description="")
 
 
-class InlineResponse2009(BaseModel):
+class InlineResponse2009(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional[List["SnapshotDescription"]] = Field(default=None, description="")
 
 
-class InlineResponse202(BaseModel):
+class InlineResponse202(BaseModel, extra="forbid"):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "accepted",
     ] = Field(None, description="")
 
 
-class IsEmptyCondition(BaseModel):
+class IsEmptyCondition(BaseModel, extra="forbid"):
     """
     Select points with empty payload for a specified field
     """
 
     is_empty: "PayloadField" = Field(..., description="Select points with empty payload for a specified field")
 
 
-class IsNullCondition(BaseModel):
+class IsNullCondition(BaseModel, extra="forbid"):
     """
     Select points with null payload for a specified field
     """
 
     is_null: "PayloadField" = Field(..., description="Select points with null payload for a specified field")
 
 
-class LocalShardInfo(BaseModel):
+class LocalShardInfo(BaseModel, extra="forbid"):
     shard_id: int = Field(..., description="Local shard id")
     points_count: int = Field(..., description="Number of points in the shard")
     state: "ReplicaState" = Field(..., description="")
 
 
-class LocalShardTelemetry(BaseModel):
+class LocalShardTelemetry(BaseModel, extra="forbid"):
     variant_name: Optional[str] = Field(default=None, description="")
     segments: List["SegmentTelemetry"] = Field(..., description="")
     optimizations: "OptimizerTelemetry" = Field(..., description="")
 
 
-class LocksOption(BaseModel):
+class LocksOption(BaseModel, extra="forbid"):
     error_message: Optional[str] = Field(default=None, description="")
     write: bool = Field(..., description="")
 
 
-class LookupLocation(BaseModel):
+class LookupLocation(BaseModel, extra="forbid"):
     """
     Defines a location to use for looking up the vector. Specifies collection and vector field name.
     """
 
     collection: str = Field(..., description="Name of the collection used for lookup")
     vector: Optional[str] = Field(
         default=None,
         description="Optional name of the vector field within the collection. If not provided, the default vector field will be used.",
     )
 
 
-class MatchAny(BaseModel):
+class MatchAny(BaseModel, extra="forbid"):
     """
     Exact match on any of the given values
     """
 
     any: "AnyVariants" = Field(..., description="Exact match on any of the given values")
 
 
-class MatchExcept(BaseModel):
+class MatchExcept(BaseModel, extra="forbid"):
     """
     Should have at least one value not matching the any given values
     """
 
     except_: "AnyVariants" = Field(
         ..., description="Should have at least one value not matching the any given values", alias="except"
     )
 
 
-class MatchText(BaseModel):
+class MatchText(BaseModel, extra="forbid"):
     """
     Full-text match of the strings.
     """
 
     text: str = Field(..., description="Full-text match of the strings.")
 
 
-class MatchValue(BaseModel):
+class MatchValue(BaseModel, extra="forbid"):
     """
     Exact match of the given value
     """
 
     value: "ValueVariants" = Field(..., description="Exact match of the given value")
 
 
-class MessageSendErrors(BaseModel):
+class MessageSendErrors(BaseModel, extra="forbid"):
     """
     Message send failures for a particular peer
     """
 
     count: int = Field(..., description="Message send failures for a particular peer")
     latest_error: Optional[str] = Field(default=None, description="Message send failures for a particular peer")
 
 
-class MoveShard(BaseModel):
+class MoveShard(BaseModel, extra="forbid"):
     shard_id: int = Field(..., description="")
     to_peer_id: int = Field(..., description="")
     from_peer_id: int = Field(..., description="")
 
 
-class MoveShardOperation(BaseModel):
+class MoveShardOperation(BaseModel, extra="forbid"):
     move_shard: "MoveShard" = Field(..., description="")
 
 
-class NamedVector(BaseModel):
+class NamedVector(BaseModel, extra="forbid"):
     """
     Vector data with name
     """
 
     name: str = Field(..., description="Name of vector data")
     vector: List[float] = Field(..., description="Vector data")
 
 
-class Nested(BaseModel):
+class Nested(BaseModel, extra="forbid"):
     """
     Select points with payload for a specified nested field
     """
 
     key: str = Field(..., description="Select points with payload for a specified nested field")
     filter: "Filter" = Field(..., description="Select points with payload for a specified nested field")
 
 
-class NestedCondition(BaseModel):
+class NestedCondition(BaseModel, extra="forbid"):
     nested: "Nested" = Field(..., description="")
 
 
-class OperationDurationStatistics(BaseModel):
+class OperationDurationStatistics(BaseModel, extra="forbid"):
     count: int = Field(..., description="")
     fail_count: Optional[int] = Field(default=None, description="")
     avg_duration_micros: Optional[float] = Field(default=None, description="")
     min_duration_micros: Optional[float] = Field(default=None, description="")
     max_duration_micros: Optional[float] = Field(default=None, description="")
     last_responded: Optional[datetime] = Field(default=None, description="")
 
 
-class OptimizerTelemetry(BaseModel):
+class OptimizerTelemetry(BaseModel, extra="forbid"):
     status: "OptimizersStatus" = Field(..., description="")
     optimizations: "OperationDurationStatistics" = Field(..., description="")
 
 
-class OptimizersConfig(BaseModel):
+class OptimizersConfig(BaseModel, extra="forbid"):
     deleted_threshold: float = Field(
         ...,
         description="The minimal fraction of deleted vectors in a segment, required to perform segment optimization",
     )
     vacuum_min_vector_number: int = Field(
         ..., description="The minimal number of vectors in a segment, required to perform segment optimization"
     )
@@ -862,15 +862,15 @@
         default=None,
         description="Maximum size (in kilobytes) of vectors allowed for plain index, exceeding this threshold will enable vector indexing  Default value is 20,000, based on &lt;https://github.com/google-research/google-research/blob/master/scann/docs/algorithms.md&gt;.  To disable vector indexing, set to `0`.  Note: 1kB = 1 vector of size 256.",
     )
     flush_interval_sec: int = Field(..., description="Minimum interval between forced flushes.")
     max_optimization_threads: int = Field(..., description="Maximum available threads for optimization workers")
 
 
-class OptimizersConfigDiff(BaseModel):
+class OptimizersConfigDiff(BaseModel, extra="forbid"):
     deleted_threshold: Optional[float] = Field(
         default=None,
         description="The minimal fraction of deleted vectors in a segment, required to perform segment optimization",
     )
     vacuum_min_vector_number: Optional[int] = Field(
         default=None, description="The minimal number of vectors in a segment, required to perform segment optimization"
     )
@@ -896,136 +896,136 @@
     )
 
 
 class OptimizersStatusOneOf(str, Enum):
     OK = "ok"
 
 
-class OptimizersStatusOneOf1(BaseModel):
+class OptimizersStatusOneOf1(BaseModel, extra="forbid"):
     """
     Something wrong happened with optimizers
     """
 
     error: str = Field(..., description="Something wrong happened with optimizers")
 
 
-class P2pConfigTelemetry(BaseModel):
+class P2pConfigTelemetry(BaseModel, extra="forbid"):
     connection_pool_size: int = Field(..., description="")
 
 
-class PayloadField(BaseModel):
+class PayloadField(BaseModel, extra="forbid"):
     """
     Payload field
     """
 
     key: str = Field(..., description="Payload field name")
 
 
-class PayloadIndexInfo(BaseModel):
+class PayloadIndexInfo(BaseModel, extra="forbid"):
     """
     Display payload field type &amp; index information
     """
 
     data_type: "PayloadSchemaType" = Field(..., description="Display payload field type &amp; index information")
     params: Optional["PayloadSchemaParams"] = Field(
         default=None, description="Display payload field type &amp; index information"
     )
     points: int = Field(..., description="Number of points indexed with this index")
 
 
-class PayloadIndexTelemetry(BaseModel):
+class PayloadIndexTelemetry(BaseModel, extra="forbid"):
     field_name: Optional[str] = Field(default=None, description="")
     points_values_count: int = Field(..., description="")
     points_count: int = Field(..., description="")
     histogram_bucket_size: Optional[int] = Field(default=None, description="")
 
 
 class PayloadSchemaType(str, Enum):
     KEYWORD = "keyword"
     INTEGER = "integer"
     FLOAT = "float"
     GEO = "geo"
     TEXT = "text"
 
 
-class PayloadSelectorExclude(BaseModel):
+class PayloadSelectorExclude(BaseModel, extra="forbid"):
     exclude: List[str] = Field(..., description="Exclude this fields from returning payload")
 
 
-class PayloadSelectorInclude(BaseModel):
+class PayloadSelectorInclude(BaseModel, extra="forbid"):
     include: List[str] = Field(..., description="Only include this payload keys")
 
 
-class PayloadStorageTypeOneOf(BaseModel):
+class PayloadStorageTypeOneOf(BaseModel, extra="forbid"):
     type: Literal[
         "in_memory",
     ] = Field(..., description="")
 
 
-class PayloadStorageTypeOneOf1(BaseModel):
+class PayloadStorageTypeOneOf1(BaseModel, extra="forbid"):
     type: Literal[
         "on_disk",
     ] = Field(..., description="")
 
 
-class PeerInfo(BaseModel):
+class PeerInfo(BaseModel, extra="forbid"):
     """
     Information of a peer in the cluster
     """
 
     uri: str = Field(..., description="Information of a peer in the cluster")
 
 
-class PointGroup(BaseModel):
+class PointGroup(BaseModel, extra="forbid"):
     hits: List["ScoredPoint"] = Field(..., description="Scored points that have the same value of the group_by key")
     id: "GroupId" = Field(..., description="")
     lookup: Optional["Record"] = Field(default=None, description="Record that has been looked up using the group id")
 
 
-class PointIdsList(BaseModel):
+class PointIdsList(BaseModel, extra="forbid"):
     points: List["ExtendedPointId"] = Field(..., description="")
 
 
-class PointRequest(BaseModel):
+class PointRequest(BaseModel, extra="forbid"):
     ids: List["ExtendedPointId"] = Field(..., description="Look for points with ids")
     with_payload: Optional["WithPayloadInterface"] = Field(
         default=None, description="Select which payload to return with the response. Default: All"
     )
     with_vector: Optional["WithVector"] = Field(default=None, description="")
 
 
-class PointStruct(BaseModel):
+class PointStruct(BaseModel, extra="forbid"):
     id: "ExtendedPointId" = Field(..., description="")
     vector: "VectorStruct" = Field(..., description="")
     payload: Optional["Payload"] = Field(default=None, description="Payload values (optional)")
 
 
-class PointVectors(BaseModel):
+class PointVectors(BaseModel, extra="forbid"):
     id: "ExtendedPointId" = Field(..., description="")
     vector: "VectorStruct" = Field(..., description="")
 
 
-class PointsBatch(BaseModel):
+class PointsBatch(BaseModel, extra="forbid"):
     batch: "Batch" = Field(..., description="")
 
 
-class PointsList(BaseModel):
+class PointsList(BaseModel, extra="forbid"):
     points: List["PointStruct"] = Field(..., description="")
 
 
-class ProductQuantization(BaseModel):
+class ProductQuantization(BaseModel, extra="forbid"):
     product: "ProductQuantizationConfig" = Field(..., description="")
 
 
-class ProductQuantizationConfig(BaseModel):
+class ProductQuantizationConfig(BaseModel, extra="forbid"):
     compression: "CompressionRatio" = Field(..., description="")
     always_ram: Optional[bool] = Field(default=None, description="")
 
 
-class QuantizationSearchParams(BaseModel):
+class QuantizationSearchParams(BaseModel, extra="forbid"):
     """
     Additional parameters of the search
     """
 
     ignore: Optional[bool] = Field(
         default=False, description="If true, quantized vectors are ignored. Default is false."
     )
@@ -1035,15 +1035,15 @@
     )
     oversampling: Optional[float] = Field(
         default=None,
         description="Oversampling factor for quantization. Default is 1.0.  Defines how many extra vectors should be pre-selected using quantized index, and then re-scored using original vectors.  For example, if `oversampling` is 2.4 and `limit` is 100, then 240 vectors will be pre-selected using quantized index, and then top-100 will be returned after re-scoring.",
     )
 
 
-class RaftInfo(BaseModel):
+class RaftInfo(BaseModel, extra="forbid"):
     """
     Summary information about the current raft state
     """
 
     term: int = Field(
         ...,
         description="Raft divides time into terms of arbitrary length, each beginning with an election. If a candidate wins the election, it remains the leader for the rest of the term. The term number increases monotonically. Each server stores the current term number which is also exchanged in every communication.",
@@ -1055,15 +1055,15 @@
         ..., description="Number of consensus operations pending to be applied on this peer"
     )
     leader: Optional[int] = Field(default=None, description="Leader of the current term")
     role: Optional["StateRole"] = Field(default=None, description="Role of this peer in the current term")
     is_voter: bool = Field(..., description="Is this peer a voter or a learner")
 
 
-class Range(BaseModel):
+class Range(BaseModel, extra="forbid"):
     """
     Range filter request
     """
 
     lt: Optional[float] = Field(default=None, description="point.key &lt; range.lt")
     gt: Optional[float] = Field(default=None, description="point.key &gt; range.gt")
     gte: Optional[float] = Field(default=None, description="point.key &gt;= range.gte")
@@ -1072,15 +1072,15 @@
 
 class ReadConsistencyType(str, Enum):
     MAJORITY = "majority"
     QUORUM = "quorum"
     ALL = "all"
 
 
-class RecommendGroupsRequest(BaseModel):
+class RecommendGroupsRequest(BaseModel, extra="forbid"):
     positive: List["ExtendedPointId"] = Field(..., description="Look for vectors closest to those")
     negative: Optional[List["ExtendedPointId"]] = Field(default=[], description="Try to avoid vectors like this")
     filter: Optional["Filter"] = Field(default=None, description="Look only for points which satisfies this conditions")
     params: Optional["SearchParams"] = Field(default=None, description="Additional search params")
     with_payload: Optional["WithPayloadInterface"] = Field(
         default=None, description="Select which payload to return with the response. Default: None"
     )
@@ -1106,15 +1106,15 @@
     group_size: int = Field(..., description="Maximum amount of points to return per group")
     limit: int = Field(..., description="Maximum amount of groups to return")
     with_lookup: Optional["WithLookupInterface"] = Field(
         default=None, description="Look for points in another collection using the group ids"
     )
 
 
-class RecommendRequest(BaseModel):
+class RecommendRequest(BaseModel, extra="forbid"):
     """
     Recommendation request. Provides positive and negative examples of the vectors, which are already stored in the collection.  Service should look for the points which are closer to positive examples and at the same time further to negative examples. The concrete way of how to compare negative and positive distances is up to implementation in `segment` crate.
     """
 
     positive: List["ExtendedPointId"] = Field(..., description="Look for vectors closest to those")
     negative: Optional[List["ExtendedPointId"]] = Field(default=[], description="Try to avoid vectors like this")
     filter: Optional["Filter"] = Field(default=None, description="Look only for points which satisfies this conditions")
@@ -1140,102 +1140,102 @@
     )
     lookup_from: Optional["LookupLocation"] = Field(
         default=None,
         description="The location used to lookup vectors. If not specified - use current collection. Note: the other collection should have the same vector size as the current collection",
     )
 
 
-class RecommendRequestBatch(BaseModel):
+class RecommendRequestBatch(BaseModel, extra="forbid"):
     searches: List["RecommendRequest"] = Field(..., description="")
 
 
-class Record(BaseModel):
+class Record(BaseModel, extra="forbid"):
     """
     Point data
     """
 
     id: "ExtendedPointId" = Field(..., description="Point data")
     payload: Optional["Payload"] = Field(default=None, description="Payload - values assigned to the point")
     vector: Optional["VectorStruct"] = Field(default=None, description="Vector of the point")
 
 
-class RemoteShardInfo(BaseModel):
+class RemoteShardInfo(BaseModel, extra="forbid"):
     shard_id: int = Field(..., description="Remote shard id")
     peer_id: int = Field(..., description="Remote peer id")
     state: "ReplicaState" = Field(..., description="")
 
 
-class RemoteShardTelemetry(BaseModel):
+class RemoteShardTelemetry(BaseModel, extra="forbid"):
     shard_id: int = Field(..., description="")
     peer_id: Optional[int] = Field(default=None, description="")
     searches: "OperationDurationStatistics" = Field(..., description="")
     updates: "OperationDurationStatistics" = Field(..., description="")
 
 
-class RenameAlias(BaseModel):
+class RenameAlias(BaseModel, extra="forbid"):
     """
     Change alias to a new one
     """
 
     old_alias_name: str = Field(..., description="Change alias to a new one")
     new_alias_name: str = Field(..., description="Change alias to a new one")
 
 
-class RenameAliasOperation(BaseModel):
+class RenameAliasOperation(BaseModel, extra="forbid"):
     """
     Change alias to a new one
     """
 
     rename_alias: "RenameAlias" = Field(..., description="Change alias to a new one")
 
 
-class Replica(BaseModel):
+class Replica(BaseModel, extra="forbid"):
     shard_id: int = Field(..., description="")
     peer_id: int = Field(..., description="")
 
 
-class ReplicaSetTelemetry(BaseModel):
+class ReplicaSetTelemetry(BaseModel, extra="forbid"):
     id: int = Field(..., description="")
     local: Optional["LocalShardTelemetry"] = Field(default=None, description="")
     remote: List["RemoteShardTelemetry"] = Field(..., description="")
     replicate_states: Dict[str, "ReplicaState"] = Field(..., description="")
 
 
 class ReplicaState(str, Enum):
     ACTIVE = "Active"
     DEAD = "Dead"
     PARTIAL = "Partial"
     INITIALIZING = "Initializing"
     LISTENER = "Listener"
 
 
-class ReplicateShardOperation(BaseModel):
+class ReplicateShardOperation(BaseModel, extra="forbid"):
     replicate_shard: "MoveShard" = Field(..., description="")
 
 
-class RequestsTelemetry(BaseModel):
+class RequestsTelemetry(BaseModel, extra="forbid"):
     rest: "WebApiTelemetry" = Field(..., description="")
     grpc: "GrpcTelemetry" = Field(..., description="")
 
 
-class RunningEnvironmentTelemetry(BaseModel):
+class RunningEnvironmentTelemetry(BaseModel, extra="forbid"):
     distribution: Optional[str] = Field(default=None, description="")
     distribution_version: Optional[str] = Field(default=None, description="")
     is_docker: bool = Field(..., description="")
     cores: Optional[int] = Field(default=None, description="")
     ram_size: Optional[int] = Field(default=None, description="")
     disk_size: Optional[int] = Field(default=None, description="")
     cpu_flags: str = Field(..., description="")
 
 
-class ScalarQuantization(BaseModel):
+class ScalarQuantization(BaseModel, extra="forbid"):
     scalar: "ScalarQuantizationConfig" = Field(..., description="")
 
 
-class ScalarQuantizationConfig(BaseModel):
+class ScalarQuantizationConfig(BaseModel, extra="forbid"):
     type: "ScalarType" = Field(..., description="")
     quantile: Optional[float] = Field(
         default=None,
         description="Quantile for quantization. Expected value range in [0.5, 1.0]. If not set - use the whole range of values",
     )
     always_ram: Optional[bool] = Field(
         default=None,
@@ -1243,27 +1243,27 @@
     )
 
 
 class ScalarType(str, Enum):
     INT8 = "int8"
 
 
-class ScoredPoint(BaseModel):
+class ScoredPoint(BaseModel, extra="forbid"):
     """
     Search result
     """
 
     id: "ExtendedPointId" = Field(..., description="Search result")
     version: int = Field(..., description="Point version")
     score: float = Field(..., description="Points vector distance to the query vector")
     payload: Optional["Payload"] = Field(default=None, description="Payload - values assigned to the point")
     vector: Optional["VectorStruct"] = Field(default=None, description="Vector of the point")
 
 
-class ScrollRequest(BaseModel):
+class ScrollRequest(BaseModel, extra="forbid"):
     """
     Scroll request - paginate over all points which matches given condition
     """
 
     offset: Optional["ExtendedPointId"] = Field(default=None, description="Start ID to read points from.")
     limit: Optional[int] = Field(default=None, description="Page size. Default: 10")
     filter: Optional["Filter"] = Field(
@@ -1273,26 +1273,26 @@
         default=None, description="Select which payload to return with the response. Default: All"
     )
     with_vector: Optional["WithVector"] = Field(
         default=None, description="Scroll request - paginate over all points which matches given condition"
     )
 
 
-class ScrollResult(BaseModel):
+class ScrollResult(BaseModel, extra="forbid"):
     """
     Result of the points read request
     """
 
     points: List["Record"] = Field(..., description="List of retrieved points")
     next_page_offset: Optional["ExtendedPointId"] = Field(
         default=None, description="Offset which should be used to retrieve a next page result"
     )
 
 
-class SearchGroupsRequest(BaseModel):
+class SearchGroupsRequest(BaseModel, extra="forbid"):
     vector: "NamedVectorStruct" = Field(..., description="")
     filter: Optional["Filter"] = Field(default=None, description="Look only for points which satisfies this conditions")
     params: Optional["SearchParams"] = Field(default=None, description="Additional search params")
     with_payload: Optional["WithPayloadInterface"] = Field(
         default=None, description="Select which payload to return with the response. Default: None"
     )
     with_vector: Optional["WithVector"] = Field(
@@ -1309,31 +1309,31 @@
     group_size: int = Field(..., description="Maximum amount of points to return per group")
     limit: int = Field(..., description="Maximum amount of groups to return")
     with_lookup: Optional["WithLookupInterface"] = Field(
         default=None, description="Look for points in another collection using the group ids"
     )
 
 
-class SearchParams(BaseModel):
+class SearchParams(BaseModel, extra="forbid"):
     """
     Additional parameters of the search
     """
 
     hnsw_ef: Optional[int] = Field(
         default=None,
-        description="Params relevant to HNSW index /// Size of the beam in a beam-search. Larger the value - more accurate the result, more time required for search.",
+        description="Params relevant to HNSW index Size of the beam in a beam-search. Larger the value - more accurate the result, more time required for search.",
     )
     exact: Optional[bool] = Field(
         default=False,
         description="Search without approximation. If set to true, search may run long but with exact results.",
     )
     quantization: Optional["QuantizationSearchParams"] = Field(default=None, description="Quantization params")
 
 
-class SearchRequest(BaseModel):
+class SearchRequest(BaseModel, extra="forbid"):
     """
     Search request. Holds all conditions and parameters for the search of most similar points by vector similarity given the filtering restrictions.
     """
 
     vector: "NamedVectorStruct" = Field(
         ...,
         description="Search request. Holds all conditions and parameters for the search of most similar points by vector similarity given the filtering restrictions.",
@@ -1353,83 +1353,83 @@
     )
     score_threshold: Optional[float] = Field(
         default=None,
         description="Define a minimal score threshold for the result. If defined, less similar results will not be returned. Score of the returned result might be higher or smaller than the threshold depending on the Distance function used. E.g. for cosine similarity only higher scores will be returned.",
     )
 
 
-class SearchRequestBatch(BaseModel):
+class SearchRequestBatch(BaseModel, extra="forbid"):
     searches: List["SearchRequest"] = Field(..., description="")
 
 
-class SegmentConfig(BaseModel):
+class SegmentConfig(BaseModel, extra="forbid"):
     vector_data: Dict[str, "VectorDataConfig"] = Field(..., description="")
     payload_storage_type: "PayloadStorageType" = Field(..., description="")
 
 
-class SegmentInfo(BaseModel):
+class SegmentInfo(BaseModel, extra="forbid"):
     """
     Aggregated information about segment
     """
 
     segment_type: "SegmentType" = Field(..., description="Aggregated information about segment")
     num_vectors: int = Field(..., description="Aggregated information about segment")
     num_points: int = Field(..., description="Aggregated information about segment")
     num_deleted_vectors: int = Field(..., description="Aggregated information about segment")
     ram_usage_bytes: int = Field(..., description="Aggregated information about segment")
     disk_usage_bytes: int = Field(..., description="Aggregated information about segment")
     is_appendable: bool = Field(..., description="Aggregated information about segment")
     index_schema: Dict[str, "PayloadIndexInfo"] = Field(..., description="Aggregated information about segment")
 
 
-class SegmentTelemetry(BaseModel):
+class SegmentTelemetry(BaseModel, extra="forbid"):
     info: "SegmentInfo" = Field(..., description="")
     config: "SegmentConfig" = Field(..., description="")
     vector_index_searches: List["VectorIndexSearchesTelemetry"] = Field(..., description="")
     payload_field_indices: List["PayloadIndexTelemetry"] = Field(..., description="")
 
 
 class SegmentType(str, Enum):
     PLAIN = "plain"
     INDEXED = "indexed"
     SPECIAL = "special"
 
 
-class SetPayload(BaseModel):
+class SetPayload(BaseModel, extra="forbid"):
     payload: "Payload" = Field(..., description="")
     points: Optional[List["ExtendedPointId"]] = Field(
         default=None, description="Assigns payload to each point in this list"
     )
     filter: Optional["Filter"] = Field(
         default=None, description="Assigns payload to each point that satisfy this filter condition"
     )
 
 
-class ShardTransferInfo(BaseModel):
+class ShardTransferInfo(BaseModel, extra="forbid"):
     shard_id: int = Field(..., description="")
     from_: int = Field(..., description="", alias="from")
     to: int = Field(..., description="")
     sync: bool = Field(
         ...,
         description="If `true` transfer is a synchronization of a replicas If `false` transfer is a moving of a shard from one peer to another",
     )
 
 
-class SnapshotDescription(BaseModel):
+class SnapshotDescription(BaseModel, extra="forbid"):
     name: str = Field(..., description="")
     creation_time: Optional[str] = Field(default=None, description="")
     size: int = Field(..., description="")
 
 
 class SnapshotPriority(str, Enum):
     SNAPSHOT = "snapshot"
     REPLICA = "replica"
 
 
-class SnapshotRecover(BaseModel):
+class SnapshotRecover(BaseModel, extra="forbid"):
     location: str = Field(
         ...,
         description="Examples: - URL `http://localhost:8080/collections/my_collection/snapshots/my_snapshot` - Local path `file:///qdrant/snapshots/test_collection-2022-08-04-10-49-10.snapshot`",
     )
     priority: Optional["SnapshotPriority"] = Field(
         default=None,
         description="Defines which data should be used as a source of truth if there are other replicas in the cluster. If set to `Snapshot`, the snapshot will be used as a source of truth, and the current state will be overwritten. If set to `Replica`, the current state will be used as a source of truth, and after recovery if will be synchronized with the snapshot.",
@@ -1439,23 +1439,23 @@
 class StateRole(str, Enum):
     FOLLOWER = "Follower"
     CANDIDATE = "Candidate"
     LEADER = "Leader"
     PRECANDIDATE = "PreCandidate"
 
 
-class TelemetryData(BaseModel):
+class TelemetryData(BaseModel, extra="forbid"):
     id: str = Field(..., description="")
     app: "AppBuildTelemetry" = Field(..., description="")
     collections: "CollectionsTelemetry" = Field(..., description="")
     cluster: "ClusterTelemetry" = Field(..., description="")
     requests: "RequestsTelemetry" = Field(..., description="")
 
 
-class TextIndexParams(BaseModel):
+class TextIndexParams(BaseModel, extra="forbid"):
     type: "TextIndexType" = Field(..., description="")
     tokenizer: Optional["TokenizerType"] = Field(default=None, description="")
     min_token_len: Optional[int] = Field(default=None, description="")
     max_token_len: Optional[int] = Field(default=None, description="")
     lowercase: Optional[bool] = Field(default=None, description="If true, lowercase all tokens. Default: true")
 
 
@@ -1465,79 +1465,79 @@
 
 class TokenizerType(str, Enum):
     PREFIX = "prefix"
     WHITESPACE = "whitespace"
     WORD = "word"
 
 
-class UpdateCollection(BaseModel):
+class UpdateCollection(BaseModel, extra="forbid"):
     """
     Operation for updating parameters of the existing collection
     """
 
     optimizers_config: Optional["OptimizersConfigDiff"] = Field(
         default=None,
         description="Custom params for Optimizers.  If none - values from service configuration file are used. This operation is blocking, it will only proceed ones all current optimizations are complete",
     )
     params: Optional["CollectionParamsDiff"] = Field(
         default=None, description="Collection base params.  If none - values from service configuration file are used."
     )
 
 
-class UpdateResult(BaseModel):
+class UpdateResult(BaseModel, extra="forbid"):
     operation_id: int = Field(..., description="Sequential number of the operation")
     status: "UpdateStatus" = Field(..., description="")
 
 
 class UpdateStatus(str, Enum):
     ACKNOWLEDGED = "acknowledged"
     COMPLETED = "completed"
 
 
-class UpdateVectors(BaseModel):
+class UpdateVectors(BaseModel, extra="forbid"):
     points: List["PointVectors"] = Field(..., description="Points with named vectors")
 
 
-class ValuesCount(BaseModel):
+class ValuesCount(BaseModel, extra="forbid"):
     """
     Values count filter request
     """
 
     lt: Optional[int] = Field(default=None, description="point.key.length() &lt; values_count.lt")
     gt: Optional[int] = Field(default=None, description="point.key.length() &gt; values_count.gt")
     gte: Optional[int] = Field(default=None, description="point.key.length() &gt;= values_count.gte")
     lte: Optional[int] = Field(default=None, description="point.key.length() &lt;= values_count.lte")
 
 
-class VectorDataConfig(BaseModel):
+class VectorDataConfig(BaseModel, extra="forbid"):
     """
     Config of single vector data storage
     """
 
     size: int = Field(..., description="Size/dimensionality of the vectors used")
     distance: "Distance" = Field(..., description="Config of single vector data storage")
     storage_type: "VectorStorageType" = Field(..., description="Config of single vector data storage")
     index: "Indexes" = Field(..., description="Config of single vector data storage")
     quantization_config: Optional["QuantizationConfig"] = Field(
         default=None, description="Vector specific quantization config that overrides collection config"
     )
 
 
-class VectorIndexSearchesTelemetry(BaseModel):
+class VectorIndexSearchesTelemetry(BaseModel, extra="forbid"):
     index_name: Optional[str] = Field(default=None, description="")
     unfiltered_plain: "OperationDurationStatistics" = Field(..., description="")
     unfiltered_hnsw: "OperationDurationStatistics" = Field(..., description="")
     filtered_plain: "OperationDurationStatistics" = Field(..., description="")
     filtered_small_cardinality: "OperationDurationStatistics" = Field(..., description="")
     filtered_large_cardinality: "OperationDurationStatistics" = Field(..., description="")
     filtered_exact: "OperationDurationStatistics" = Field(..., description="")
     unfiltered_exact: "OperationDurationStatistics" = Field(..., description="")
 
 
-class VectorParams(BaseModel):
+class VectorParams(BaseModel, extra="forbid"):
     """
     Params of single vector data storage
     """
 
     size: int = Field(..., description="Size of a vectors used")
     distance: "Distance" = Field(..., description="Params of single vector data storage")
     hnsw_config: Optional["HnswConfigDiff"] = Field(
@@ -1562,31 +1562,31 @@
     MMAP = "Mmap"
 
 
 class VectorStorageTypeOneOf2(str, Enum):
     CHUNKEDMMAP = "ChunkedMmap"
 
 
-class WalConfig(BaseModel):
+class WalConfig(BaseModel, extra="forbid"):
     wal_capacity_mb: int = Field(..., description="Size of a single WAL segment in MB")
     wal_segments_ahead: int = Field(..., description="Number of WAL segments to create ahead of actually used ones")
 
 
-class WalConfigDiff(BaseModel):
+class WalConfigDiff(BaseModel, extra="forbid"):
     wal_capacity_mb: Optional[int] = Field(default=None, description="Size of a single WAL segment in MB")
     wal_segments_ahead: Optional[int] = Field(
         default=None, description="Number of WAL segments to create ahead of actually used ones"
     )
 
 
-class WebApiTelemetry(BaseModel):
+class WebApiTelemetry(BaseModel, extra="forbid"):
     responses: Dict[str, Dict[str, "OperationDurationStatistics"]] = Field(..., description="")
 
 
-class WithLookup(BaseModel):
+class WithLookup(BaseModel, extra="forbid"):
     collection: str = Field(..., description="Name of the collection to use for points lookup")
     with_payload: Optional["WithPayloadInterface"] = Field(
         default=None, description="Options for specifying which payload to include (or not)"
     )
     with_vectors: Optional["WithVector"] = Field(
         default=None, description="Options for specifying which vectors to include (or not)"
     )
```

### Comparing `qdrant_client-1.3.1/qdrant_client/local/distances.py` & `qdrant_client-1.3.2/qdrant_client/local/distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/local/geo.py` & `qdrant_client-1.3.2/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/local/local_collection.py` & `qdrant_client-1.3.2/qdrant_client/local/local_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import uuid
 from collections import OrderedDict, defaultdict
 from copy import deepcopy
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
+from qdrant_client._pydantic_compat import construct
 from qdrant_client.conversions import common_types as types
 from qdrant_client.http import models
 from qdrant_client.local.distances import (
     DistanceOrder,
     calculate_distance,
     distance_to_order,
 )
@@ -232,15 +233,16 @@
                 if required_order == DistanceOrder.BIGGER_IS_BETTER:
                     if score < score_threshold:
                         break
                 else:
                     if score > score_threshold:
                         break
 
-            scored_point = models.ScoredPoint.construct(
+            scored_point = construct(
+                models.ScoredPoint,
                 id=point_id,
                 score=score,
                 version=0,
                 payload=self._get_payload(idx, with_payload),
                 vector=self._get_vectors(idx, with_vectors),
             )
 
@@ -548,14 +550,17 @@
             vectors = {DEFAULT_VECTOR_NAME: point.vector}
         else:
             vectors = point.vector
 
         for vector_name, named_vectors in self.vectors.items():
             vector = vectors.get(vector_name)
             if vector is not None:
+                params = self.get_vector_params(vector_name)
+                if params.distance == models.Distance.COSINE:
+                    vector = np.array(vector) / np.linalg.norm(vector)
                 self.vectors[vector_name][idx] = vector
                 self.deleted_per_vector[vector_name][idx] = 0
             else:
                 self.deleted_per_vector[vector_name][idx] = 1
 
         self.deleted[idx] = 0
 
@@ -581,14 +586,17 @@
                 fake_vector = np.ones(named_vectors.shape[1])
                 named_vectors[idx] = fake_vector
                 self.deleted_per_vector[vector_name] = np.append(
                     self.deleted_per_vector[vector_name], 1
                 )
             else:
                 vector_np = np.array(vector)
+                params = self.get_vector_params(vector_name)
+                if params.distance == models.Distance.COSINE:
+                    vector_np = vector_np / np.linalg.norm(vector_np)
                 named_vectors[idx] = vector_np
                 self.vectors[vector_name] = named_vectors
                 self.deleted_per_vector[vector_name] = np.append(
                     self.deleted_per_vector[vector_name], 0
                 )
 
     def _upsert_point(self, point: models.PointStruct) -> None:
```

### Comparing `qdrant_client-1.3.1/qdrant_client/local/payload_filters.py` & `qdrant_client-1.3.2/qdrant_client/local/payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.3.2/qdrant_client/local/payload_value_extractor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/local/persistence.py` & `qdrant_client-1.3.2/qdrant_client/local/persistence.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/local/tests/test_payload_filters.py` & `qdrant_client-1.3.2/qdrant_client/local/tests/test_payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/parallel_processor.py` & `qdrant_client-1.3.2/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/proto/collections.proto` & `qdrant_client-1.3.2/qdrant_client/proto/collections.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.3.2/qdrant_client/proto/collections_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.3.2/qdrant_client/proto/json_with_int.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/proto/points.proto` & `qdrant_client-1.3.2/qdrant_client/proto/points.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/proto/points_service.proto` & `qdrant_client-1.3.2/qdrant_client/proto/points_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.3.2/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/qdrant_client.py` & `qdrant_client-1.3.2/qdrant_client/qdrant_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 from qdrant_client import grpc as grpc
 from qdrant_client.client_base import QdrantBase
 from qdrant_client.conversions import common_types as types
 from qdrant_client.http import ApiClient, SyncApis
 from qdrant_client.local.qdrant_local import QdrantLocal
@@ -1434,15 +1433,17 @@
             max_retries=max_retries,
             **kwargs,
         )
 
     def upload_collection(
         self,
         collection_name: str,
-        vectors: Union[types.NumpyArray, Dict[str, types.NumpyArray], Iterable[List[float]]],
+        vectors: Union[
+            Dict[str, types.NumpyArray], types.NumpyArray, Iterable[types.VectorStruct]
+        ],
         payload: Optional[Iterable[Dict[Any, Any]]] = None,
         ids: Optional[Iterable[types.PointId]] = None,
         batch_size: int = 64,
         parallel: int = 1,
         method: Optional[str] = None,
         max_retries: int = 3,
         **kwargs: Any,
```

### Comparing `qdrant_client-1.3.1/qdrant_client/qdrant_remote.py` & `qdrant_client-1.3.2/qdrant_client/qdrant_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 )
 
 import httpx
 import numpy as np
 from urllib3.util import Url, parse_url
 
 from qdrant_client import grpc as grpc
+from qdrant_client._pydantic_compat import construct
 from qdrant_client.client_base import QdrantBase
 from qdrant_client.connection import get_async_channel, get_channel
 from qdrant_client.conversions import common_types as types
 from qdrant_client.conversions.conversion import (
     GrpcToRest,
     RestToGrpc,
     grpc_payload_schema_to_field_type,
@@ -538,31 +539,32 @@
 
             return GrpcToRest.convert_groups_result(result)
         else:
             if isinstance(with_lookup, grpc.WithLookup):
                 with_lookup = GrpcToRest.convert_with_lookup(with_lookup)
 
             if isinstance(query_vector, tuple):
-                query_vector = rest_models.NamedVector.construct(
-                    name=query_vector[0], vector=query_vector[1]
+                query_vector = construct(
+                    rest_models.NamedVector, name=query_vector[0], vector=query_vector[1]
                 )
 
             if isinstance(query_vector, np.ndarray):
                 query_vector = query_vector.tolist()
 
             if isinstance(query_filter, grpc.Filter):
                 query_filter = GrpcToRest.convert_filter(model=query_filter)
 
             if isinstance(search_params, grpc.SearchParams):
                 search_params = GrpcToRest.convert_search_params(search_params)
 
             if isinstance(with_payload, grpc.WithPayloadSelector):
                 with_payload = GrpcToRest.convert_with_payload_selector(with_payload)
 
-            search_groups_request = rest_models.SearchGroupsRequest.construct(
+            search_groups_request = construct(
+                rest_models.SearchGroupsRequest,
                 vector=query_vector,
                 filter=query_filter,
                 params=search_params,
                 with_payload=with_payload,
                 with_vector=with_vectors,
                 score_threshold=score_threshold,
                 group_by=group_by,
@@ -884,15 +886,16 @@
 
             if isinstance(lookup_from, grpc.LookupLocation):
                 lookup_from = GrpcToRest.convert_lookup_location(lookup_from)
 
             result = self.openapi_client.points_api.recommend_point_groups(
                 collection_name=collection_name,
                 consistency=consistency,
-                recommend_groups_request=rest_models.RecommendGroupsRequest.construct(
+                recommend_groups_request=construct(
+                    rest_models.RecommendGroupsRequest,
                     positive=positive,
                     negative=negative,
                     filter=query_filter,
                     group_by=group_by,
                     limit=limit,
                     group_size=group_size,
                     params=search_params,
@@ -1155,15 +1158,16 @@
             return GrpcToRest.convert_update_result(grpc_result)
         else:
             _points, _filter = self._try_argument_to_rest_points_and_filter(points)
             return self.openapi_client.points_api.delete_vectors(
                 collection_name=collection_name,
                 wait=wait,
                 ordering=ordering,
-                delete_vectors=rest_models.DeleteVectors.construct(
+                delete_vectors=construct(
+                    rest_models.DeleteVectors,
                     vector=vectors,
                     points=_points,
                     filter=_filter,
                 ),
             ).result
 
     def retrieve(
@@ -1246,15 +1250,15 @@
             )
         elif isinstance(points, grpc.PointsSelector):
             points_selector = points
         elif isinstance(points, (rest_models.PointIdsList, rest_models.FilterSelector)):
             points_selector = RestToGrpc.convert_points_selector(points)
         elif isinstance(points, rest_models.Filter):
             points_selector = RestToGrpc.convert_points_selector(
-                rest_models.FilterSelector.construct(filter=points)
+                construct(rest_models.FilterSelector, filter=points)
             )
         elif isinstance(points, grpc.Filter):
             points_selector = grpc.PointsSelector(filter=points)
         else:
             raise ValueError(f"Unsupported points selector type: {type(points)}")
         return points_selector
 
@@ -1263,24 +1267,24 @@
         cls, points: types.PointsSelector
     ) -> rest_models.PointsSelector:
         if isinstance(points, list):
             _points = [
                 GrpcToRest.convert_point_id(idx) if isinstance(idx, grpc.PointId) else idx
                 for idx in points
             ]
-            points_selector = rest_models.PointIdsList.construct(points=_points)
+            points_selector = construct(rest_models.PointIdsList, points=_points)
         elif isinstance(points, grpc.PointsSelector):
             points_selector = GrpcToRest.convert_points_selector(points)
         elif isinstance(points, (rest_models.PointIdsList, rest_models.FilterSelector)):
             points_selector = points
         elif isinstance(points, rest_models.Filter):
-            points_selector = rest_models.FilterSelector.construct(filter=points)
+            points_selector = construct(rest_models.FilterSelector, filter=points)
         elif isinstance(points, grpc.Filter):
-            points_selector = rest_models.FilterSelector.construct(
-                filter=GrpcToRest.convert_filter(points)
+            points_selector = construct(
+                rest_models.FilterSelector, filter=GrpcToRest.convert_filter(points)
             )
         else:
             raise ValueError(f"Unsupported points selector type: {type(points)}")
         return points_selector
 
     @classmethod
     def _points_selector_to_points_list(
@@ -1792,14 +1796,15 @@
             replication_factor=replication_factor,
             write_consistency_factor=write_consistency_factor,
             on_disk_payload=on_disk_payload,
             hnsw_config=hnsw_config,
             optimizers_config=optimizers_config,
             wal_config=wal_config,
             quantization_config=quantization_config,
+            init_from=init_from,
             timeout=timeout,
         )
 
     @property
     def _updater_class(self) -> Type[BaseUploader]:
         if self._prefer_grpc:
             return GrpcBatchUploader
@@ -1864,15 +1869,17 @@
             records=records, batch_size=batch_size
         )
         self._upload_collection(batches_iterator, collection_name, max_retries, parallel, method)
 
     def upload_collection(
         self,
         collection_name: str,
-        vectors: Union[types.NumpyArray, Dict[str, types.NumpyArray], Iterable[List[float]]],
+        vectors: Union[
+            Dict[str, types.NumpyArray], types.NumpyArray, Iterable[types.VectorStruct]
+        ],
         payload: Optional[Iterable[Dict[Any, Any]]] = None,
         ids: Optional[Iterable[types.PointId]] = None,
         batch_size: int = 64,
         parallel: int = 1,
         method: Optional[str] = None,
         max_retries: int = 3,
         **kwargs: Any,
```

### Comparing `qdrant_client-1.3.1/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.3.2/qdrant_client/uploader/grpc_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.1/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.3.2/qdrant_client/uploader/rest_uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 from itertools import count
 from typing import Any, Generator, Iterable, Optional, Tuple, Union
 
+import numpy as np
+
 from qdrant_client.http import SyncApis
 from qdrant_client.http.models import Batch, PointsList, PointStruct
 from qdrant_client.uploader.uploader import BaseUploader
 
 
 def upload_batch(
     openapi_client: SyncApis,
@@ -19,15 +21,15 @@
         payload_batch = list(payload_batch)
     else:
         payload_batch = (None for _ in count())
 
     points = [
         PointStruct(
             id=idx,
-            vector=vector,
+            vector=(vector.tolist() if isinstance(vector, np.ndarray) else vector) or {},
             payload=payload,
         )
         for idx, vector, payload in zip(ids_batch, vectors_batch, payload_batch)
     ]
 
     for attempt in range(max_retries):
         try:
```

### Comparing `qdrant_client-1.3.1/qdrant_client/uploader/uploader.py` & `qdrant_client-1.3.2/qdrant_client/uploader/uploader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import itertools
 import math
 from abc import ABC
 from itertools import count, islice
-from typing import Dict, Generator, Iterable, List, Optional, Union
+from typing import Any, Dict, Generator, Iterable, List, Optional, Union
 
 import numpy as np
 
+from qdrant_client.conversions import common_types as types
 from qdrant_client.conversions.common_types import Record
 from qdrant_client.http.models import ExtendedPointId
 from qdrant_client.parallel_processor import Worker
 
 
 def iter_batch(iterable: Union[Iterable, Generator], size: int) -> Iterable:
     """
@@ -33,58 +34,54 @@
             vectors_batch = [record.vector for record in record_batch]
             payload_batch = [record.payload for record in record_batch]
             yield ids_batch, vectors_batch, payload_batch
 
     @classmethod
     def iterate_batches(
         cls,
-        vectors: Union[np.ndarray, Dict[str, np.ndarray], Iterable[List[float]]],
+        vectors: Union[
+            Dict[str, types.NumpyArray], types.NumpyArray, Iterable[types.VectorStruct]
+        ],
         payload: Optional[Iterable[dict]],
         ids: Optional[Iterable[ExtendedPointId]],
         batch_size: int,
     ) -> Iterable:
         if ids is None:
             ids = itertools.count()
 
         ids_batches = iter_batch(ids, batch_size)
         if payload is None:
             payload_batches: Union[Generator, Iterable] = (None for _ in count())
         else:
             payload_batches = iter_batch(payload, batch_size)
 
         if isinstance(vectors, np.ndarray):
-            vector_batches = _get_vector_batches_from_numpy(vectors, batch_size)
-        elif isinstance(vectors, dict):
-            vector_batches = _get_named_vector_batches_from_numpy(vectors, batch_size)
+            vector_batches: Iterable[Any] = cls._vector_batches_from_numpy(vectors, batch_size)
+        elif isinstance(vectors, dict) and any(
+            isinstance(value, np.ndarray) for value in vectors.values()
+        ):
+            vector_batches = cls._vector_batches_from_numpy_named_vectors(vectors, batch_size)
         else:
             vector_batches = iter_batch(vectors, batch_size)
 
         yield from zip(ids_batches, vector_batches, payload_batches)
 
-
-def _get_vector_batches_from_numpy(
-    vectors: np.ndarray, batch_size: int
-) -> Union[Generator, Iterable]:
-    num_vectors = vectors.shape[0]
-    num_batches = int(math.ceil(num_vectors / batch_size))
-    vector_batches: Union[Generator, Iterable] = (
-        vectors[i * batch_size : (i + 1) * batch_size].tolist() for i in range(num_batches)
-    )
-
-    return vector_batches
-
-
-def _get_named_vector_batches_from_numpy(
-    vectors: Dict[str, np.ndarray], batch_size: int
-) -> Union[Generator, Iterable]:
-    all_num_vectors = set([v.shape[0] for k, v in vectors.items()])
-    assert (
-        len(all_num_vectors) == 1
-    ), f"Dict of named vectors should have the same number of vectors, but got {all_num_vectors}"
-    num_vectors = list(all_num_vectors)[0]
-    num_batches = int(math.ceil(num_vectors / batch_size))
-    vector_names = vectors.keys()
-    vector_batches: Union[Generator, Iterable] = (
-        {name: vectors[name][i].tolist() for name in vector_names} for i in range(num_vectors)
-    )
-
-    return iter_batch(vector_batches, batch_size)
+    @staticmethod
+    def _vector_batches_from_numpy(vectors: types.NumpyArray, batch_size: int) -> Iterable[float]:
+        for i in range(0, vectors.shape[0], batch_size):
+            yield vectors[i : i + batch_size].tolist()
+
+    @staticmethod
+    def _vector_batches_from_numpy_named_vectors(
+        vectors: Dict[str, types.NumpyArray], batch_size: int
+    ) -> Iterable[Dict[str, List[float]]]:
+        assert (
+            len(set([arr.shape[0] for arr in vectors.values()])) == 1
+        ), "Each named vector should have the same number of vectors"
+
+        num_vectors = next(iter(vectors.values())).shape[0]
+        # Convert Dict[str, np.ndarray] to Generator(Dict[str, List[float]])
+        vector_batches = (
+            {name: vectors[name][i].tolist() for name in vectors.keys()}
+            for i in range(num_vectors)
+        )
+        yield from iter_batch(vector_batches, batch_size)
```

### Comparing `qdrant_client-1.3.1/PKG-INFO` & `qdrant_client-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.3.1
+Version: 1.3.2
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
 License: Apache-2.0
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.7,<3.12
@@ -17,16 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grpcio (>=1.41.0)
 Requires-Dist: grpcio-tools (>=1.41.0)
 Requires-Dist: httpx[http2] (>=0.14.0)
 Requires-Dist: numpy (<1.21) ; python_version < "3.8"
 Requires-Dist: numpy (>=1.21) ; python_version >= "3.8"
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
-Requires-Dist: pydantic (>=1.8,<2.0)
-Requires-Dist: typing-extensions (>=4.0.0,<4.6.0)
+Requires-Dist: pydantic (>=1.10.8)
 Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
 Project-URL: Repository, https://github.com/qdrant/qdrant-client
 Description-Content-Type: text/markdown
 
 
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.3.1 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.3.2 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
 qdrant/qdrant-client License: Apache-2.0 Keywords:
 vector,search,neural,matching,client Author: Andrey Vasnetsov Author-email:
 andrey@qdrant.tech Requires-Python: >=3.7,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: grpcio (>=1.41.0) Requires-Dist:
 grpcio-tools (>=1.41.0) Requires-Dist: httpx[http2] (>=0.14.0) Requires-Dist:
 numpy (<1.21) ; python_version < "3.8" Requires-Dist: numpy (>=1.21) ;
 python_version >= "3.8" Requires-Dist: portalocker (>=2.7.0,<3.0.0) Requires-
-Dist: pydantic (>=1.8,<2.0) Requires-Dist: typing-extensions (>=4.0.0,<4.6.0)
-Requires-Dist: urllib3 (>=1.26.14,<2.0.0) Project-URL: Repository, https://
-github.com/qdrant/qdrant-client Description-Content-Type: text/markdown
+Dist: pydantic (>=1.10.8) Requires-Dist: urllib3 (>=1.26.14,<2.0.0) Project-
+URL: Repository, https://github.com/qdrant/qdrant-client Description-Content-
+Type: text/markdown
                                    [Qdrant]
           Python Client library for the Qdrant vector search engine.
   [PyPI_version] [OpenAPI_Docs] [Apache_2.0_License] [Discord] [Roadmap_2023]
 # Python Qdrant Client Client library and SDK for the [Qdrant](https://
 github.com/qdrant/qdrant) vector search engine. Library contains type
 definitions for all Qdrant API and allows to make both Sync and Async requests.
 Client allows calls for all [Qdrant API methods](https://qdrant.github.io/
```

