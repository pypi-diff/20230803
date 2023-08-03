# Comparing `tmp/modelaapi-0.6.233.tar.gz` & `tmp/modelaapi-0.6.234.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.233.tar", last modified: Thu Aug  3 16:42:14 2023, max compression
+gzip compressed data, was "modelaapi-0.6.234.tar", last modified: Thu Aug  3 18:08:34 2023, max compression
```

## Comparing `modelaapi-0.6.233.tar` & `modelaapi-0.6.234.tar`

### file list

```diff
@@ -1,581 +1,581 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.233/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.233/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.233/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.233/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.233/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.233/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-03 16:42:14.422753 modelaapi-0.6.233/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.233/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6763 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24765 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    41839 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.366754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    52674 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    91844 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35286 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    40354 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18422 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    55370 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    97138 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.370754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8164 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4594 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4881 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3133 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12730 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4263 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.374754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23069 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11572 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7286 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    20675 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.378754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    59638 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62238 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)   104684 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4969 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4644 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5326 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5395 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4276 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.382754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.386754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10704 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6390 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    18037 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.386754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.386754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5885 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.386754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.386754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    66312 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.386754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.386754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3961 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.386754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5613 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4141 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2012 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.358754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.358754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/health/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/health/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)     2035 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1010 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3056 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19563 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.390754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17943 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4516 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4951 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13520 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2363 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.394754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.358754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclassrun/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclassrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)    11990 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6559 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    23986 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4035 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1956 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.398754 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1204 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4282 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3917 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4820 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1294 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5788 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.402753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6533 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5338 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3883 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4364 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4597 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3815 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4459 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.406753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6909 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6597 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3580 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12936 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.410753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4784 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3696 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-08-02 18:33:15.000000 modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-08-02 18:33:15.000000 modelaapi-0.6.233/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      310 2023-08-02 18:33:15.000000 modelaapi-0.6.233/google/api/annotations_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-08-02 18:33:15.000000 modelaapi-0.6.233/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2272 2023-08-02 18:33:15.000000 modelaapi-0.6.233/google/api/http_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/api/apps/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21422 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/api/apps/v1/generated_pb2.pyi
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.414753 modelaapi-0.6.233/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   150106 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/api/core/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6650 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/api/rbac/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      579 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23310 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1267 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      135 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.418753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      577 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.362754 modelaapi-0.6.233/k8s/io/apps/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/apps/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.362754 modelaapi-0.6.233/k8s/io/core/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.362754 modelaapi-0.6.233/k8s/io/pkg/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.362754 modelaapi-0.6.233/k8s/io/pkg/api/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.362754 modelaapi-0.6.233/k8s/io/pkg/apis/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.362754 modelaapi-0.6.233/k8s/io/pkg/apis/meta/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.362754 modelaapi-0.6.233/k8s/io/pkg/util/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.362754 modelaapi-0.6.233/k8s/io/rbac/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/k8s/io/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-02 18:33:15.000000 modelaapi-0.6.233/k8s/io/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.233/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.233/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.233/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.233/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.233/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-08-03 16:42:11.000000 modelaapi-0.6.233/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 16:42:14.422753 modelaapi-0.6.233/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-03 16:42:14.000000 modelaapi-0.6.233/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    24585 2023-08-03 16:42:14.000000 modelaapi-0.6.233/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-08-03 16:42:14.000000 modelaapi-0.6.233/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-08-03 16:42:14.000000 modelaapi-0.6.233/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.233/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-08-03 16:42:14.000000 modelaapi-0.6.233/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-08-03 16:42:14.000000 modelaapi-0.6.233/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.233/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-08-03 16:42:14.426753 modelaapi-0.6.233/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5473 2023-07-21 18:09:27.000000 modelaapi-0.6.233/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.234/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.234/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.234/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.234/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.234/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.234/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-03 18:08:34.927729 modelaapi-0.6.234/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.234/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6763 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24765 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    41839 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    52674 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    91844 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35286 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    40354 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18422 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    55370 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    97138 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8164 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4594 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4881 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3133 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12730 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4263 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23069 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11572 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7286 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20675 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    61254 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    64734 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)   104658 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4969 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4644 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5326 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5395 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4276 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11708 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7194 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20179 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5885 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    66312 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3961 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5613 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4141 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2012 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.887729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.887729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2035 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1010 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3056 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19563 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17943 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4516 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4951 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13520 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2363 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.887729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11990 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6559 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23986 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4035 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1956 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1204 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4282 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3917 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4820 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1294 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5788 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6533 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5338 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3883 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4364 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4597 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3815 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4459 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6909 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6597 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3580 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12936 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4784 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3696 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      310 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/annotations_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2272 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/http_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/apps/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21422 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/apps/v1/generated_pb2.pyi
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   150106 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6650 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      579 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23310 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1267 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      135 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      577 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/apps/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apps/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/core/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/api/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/apis/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/apis/meta/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/util/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/rbac/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-08-03 18:08:33.000000 modelaapi-0.6.234/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24585 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.234/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.234/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-08-03 18:08:34.931729 modelaapi-0.6.234/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5473 2023-07-21 18:09:27.000000 modelaapi-0.6.234/setup.py
```

### Comparing `modelaapi-0.6.233/CONTRIBUTING.rst` & `modelaapi-0.6.234/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/LICENSE.txt` & `modelaapi-0.6.234/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/Makefile` & `modelaapi-0.6.234/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/PKG-INFO` & `modelaapi-0.6.234/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.233
+Version: 0.6.234
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.233
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.234
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.233
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.234
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.233/README.md` & `modelaapi-0.6.234/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi` & `modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_inference_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xa2\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x03\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xf4\x03\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xae\x03\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xfd\x03\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xf6\x07\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x07 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\x0b \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xef\x02\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x8d\x04\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"~\n\x1c\x44sCreateModelProfileResponse\x12^\n\x0fprofileLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x83\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\x8e\x04\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"~\n\x1c\x44sCreateStudyProfileResponse\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe8\x06\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xf9\x02\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x06target\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0c\n\x04rows\x18\x05 \x01(\x05\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xe6\x04\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12V\n\x0ftrainingDataset\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xc3\x03\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x14\n\x0ctrainingHash\x18\x04 \x01(\t\x12\x13\n\x0btestingHash\x18\x05 \x01(\t\x12\x16\n\x0evalidationHash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\x12\\\n\rtrainLocation\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12[\n\x0ctestLocation\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x61\n\x12validationLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xa7\x02\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\r\n\x05rungs\x18\x04 \x01(\x05\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\x91\x02\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x86\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xd7\x08\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xc3\x01\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Q\n\x07reports\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xe8\x02\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12P\n\x06report\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\x8b\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe9\x03\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x11\n\tdefaultHP\x18\x07 \x01(\x08\x12\x11\n\talgorithm\x18\x08 \x01(\t\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xeb\x02\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xc9\x03\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x87\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12O\n\x06models\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xd5\x03\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x10\n\x08\x61lgnames\x18\x06 \x03(\t\x12\x0b\n\x03\x61ll\x18\x07 \x01(\x08\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xdc\x03\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xbc\x03\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xb9\x01\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x16\n\x14\x44sStudyEndedResponse\"\x92\x02\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"r\n\x17SaveOptimizerDBResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x8d\x02\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x14\n\x12\x44sSnapshotResponse\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xca\x03\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelClass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelClassRun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x08\x65ntities\x18\x04 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\x05 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"r\n\x17GenTrainingDataResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xa5\x04\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xf1\x04\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xb6\x04\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xfb\x02\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf0?\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xa2\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x03\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xf4\x03\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xae\x03\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xfd\x03\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xf6\x07\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x06 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\t \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\n \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xc8\x03\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe6\x04\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"~\n\x1c\x44sCreateModelProfileResponse\x12^\n\x0fprofileLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x83\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xe7\x04\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"~\n\x1c\x44sCreateStudyProfileResponse\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe8\x06\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xd2\x03\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12U\n\x06target\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0c\n\x04rows\x18\x06 \x01(\x05\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xcf\x05\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12^\n\x0ftrainingDataset\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12]\n\x0etestingDataset\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"\xc3\x03\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x14\n\x0ctrainingHash\x18\x04 \x01(\t\x12\x13\n\x0btestingHash\x18\x05 \x01(\t\x12\x16\n\x0evalidationHash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\x12\\\n\rtrainLocation\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12[\n\x0ctestLocation\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x61\n\x12validationLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x80\x03\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\r\n\x05rungs\x18\x05 \x01(\x05\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xea\x02\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x86\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xd7\x08\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xc3\x01\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Q\n\x07reports\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc1\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe4\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xc2\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x07 \x01(\x05\x12\x11\n\tdefaultHP\x18\x08 \x01(\x08\x12\x11\n\talgorithm\x18\t \x01(\t\x12V\n\nalgorithms\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xeb\x02\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xc9\x03\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe0\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xae\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x10\n\x08\x61lgnames\x18\x07 \x03(\t\x12\x0b\n\x03\x61ll\x18\x08 \x01(\x08\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb5\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xb9\x01\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x16\n\x14\x44sStudyEndedResponse\"\x92\x02\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"r\n\x17SaveOptimizerDBResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x8d\x02\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x14\n\x12\x44sSnapshotResponse\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xca\x03\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelClass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelClassRun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x08\x65ntities\x18\x04 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\x05 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"r\n\x17GenTrainingDataResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xa5\x04\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xf1\x04\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xb6\x04\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xfb\x02\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf0?\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.data.v1.data_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z.github.com/metaprov/modelaapi/services/data/v1'
@@ -103,177 +103,177 @@
   _DSRUNRECIPERESPONSE._serialized_start=4445
   _DSRUNRECIPERESPONSE._serialized_end=4544
   _DATASOURCERESPONSE._serialized_start=4546
   _DATASOURCERESPONSE._serialized_end=4566
   _DATASETRESPONSE._serialized_start=4568
   _DATASETRESPONSE._serialized_end=4585
   _DSCREATEDATASETPROFILEREQUEST._serialized_start=4588
-  _DSCREATEDATASETPROFILEREQUEST._serialized_end=4955
-  _DSCREATEDATASETPROFILERESPONSE._serialized_start=4958
-  _DSCREATEDATASETPROFILERESPONSE._serialized_end=5265
-  _DSCREATEMODELPROFILEREQUEST._serialized_start=5268
-  _DSCREATEMODELPROFILEREQUEST._serialized_end=5793
-  _DSCREATEMODELPROFILERESPONSE._serialized_start=5795
-  _DSCREATEMODELPROFILERESPONSE._serialized_end=5921
-  _DSMERGEFORECASTFILEREQUEST._serialized_start=5924
-  _DSMERGEFORECASTFILEREQUEST._serialized_end=6951
+  _DSCREATEDATASETPROFILEREQUEST._serialized_end=5044
+  _DSCREATEDATASETPROFILERESPONSE._serialized_start=5047
+  _DSCREATEDATASETPROFILERESPONSE._serialized_end=5354
+  _DSCREATEMODELPROFILEREQUEST._serialized_start=5357
+  _DSCREATEMODELPROFILEREQUEST._serialized_end=5971
+  _DSCREATEMODELPROFILERESPONSE._serialized_start=5973
+  _DSCREATEMODELPROFILERESPONSE._serialized_end=6099
+  _DSMERGEFORECASTFILEREQUEST._serialized_start=6102
+  _DSMERGEFORECASTFILEREQUEST._serialized_end=7129
   _DSMERGEFORECASTFILEREQUEST_SECRETENTRY._serialized_start=945
   _DSMERGEFORECASTFILEREQUEST_SECRETENTRY._serialized_end=990
   _DSMERGEFORECASTFILEREQUEST_DBSECRETENTRY._serialized_start=4396
   _DSMERGEFORECASTFILEREQUEST_DBSECRETENTRY._serialized_end=4443
-  _DSMERGEFORECASTFILERESPONSE._serialized_start=6953
-  _DSMERGEFORECASTFILERESPONSE._serialized_end=6995
-  _DSCREATESTUDYPROFILEREQUEST._serialized_start=6998
-  _DSCREATESTUDYPROFILEREQUEST._serialized_end=7524
-  _DSCREATESTUDYPROFILERESPONSE._serialized_start=7526
-  _DSCREATESTUDYPROFILERESPONSE._serialized_end=7652
-  _RUNTESTSUITEREQUEST._serialized_start=7655
-  _RUNTESTSUITEREQUEST._serialized_end=8527
-  _RUNTESTSUITERESPONSE._serialized_start=8529
-  _RUNTESTSUITERESPONSE._serialized_end=8641
-  _DSGENERATEDATASETREQUEST._serialized_start=8644
-  _DSGENERATEDATASETREQUEST._serialized_end=9021
-  _DSGENERATEDATASETRESPONSE._serialized_start=9023
-  _DSGENERATEDATASETRESPONSE._serialized_end=9137
-  _DSSPLITDATASETREQUEST._serialized_start=9140
-  _DSSPLITDATASETREQUEST._serialized_end=9754
-  _DSSPLITDATASETRESPONSE._serialized_start=9757
-  _DSSPLITDATASETRESPONSE._serialized_end=10208
-  _DSSPLITDATASETTORUNGSREQUEST._serialized_start=10211
-  _DSSPLITDATASETTORUNGSREQUEST._serialized_end=10506
-  _DSSPLITDATASETTORUNGSRESPONSE._serialized_start=10508
-  _DSSPLITDATASETTORUNGSRESPONSE._serialized_end=10539
-  _GROUPBYDATASETREQUEST._serialized_start=10542
-  _GROUPBYDATASETREQUEST._serialized_end=10815
-  _GROUPBYDATASETRESPONSE._serialized_start=10817
-  _GROUPBYDATASETRESPONSE._serialized_end=10854
-  _DSINFERSCHEMAREQUEST._serialized_start=10857
-  _DSINFERSCHEMAREQUEST._serialized_end=11070
-  _DSINFERSCHEMARESPONSE._serialized_start=11072
-  _DSINFERSCHEMARESPONSE._serialized_end=11178
-  _DSGETTABLEVIEWREQUEST._serialized_start=11181
-  _DSGETTABLEVIEWREQUEST._serialized_end=11401
-  _DSGETTABLEVIEWRESPONSE._serialized_start=11403
-  _DSGETTABLEVIEWRESPONSE._serialized_end=11507
-  _CREATEMODELREPORTREQUEST._serialized_start=11510
-  _CREATEMODELREPORTREQUEST._serialized_end=12028
-  _CREATEFORECASTREPORTREQUEST._serialized_start=12031
-  _CREATEFORECASTREPORTREQUEST._serialized_end=13142
+  _DSMERGEFORECASTFILERESPONSE._serialized_start=7131
+  _DSMERGEFORECASTFILERESPONSE._serialized_end=7173
+  _DSCREATESTUDYPROFILEREQUEST._serialized_start=7176
+  _DSCREATESTUDYPROFILEREQUEST._serialized_end=7791
+  _DSCREATESTUDYPROFILERESPONSE._serialized_start=7793
+  _DSCREATESTUDYPROFILERESPONSE._serialized_end=7919
+  _RUNTESTSUITEREQUEST._serialized_start=7922
+  _RUNTESTSUITEREQUEST._serialized_end=8794
+  _RUNTESTSUITERESPONSE._serialized_start=8796
+  _RUNTESTSUITERESPONSE._serialized_end=8908
+  _DSGENERATEDATASETREQUEST._serialized_start=8911
+  _DSGENERATEDATASETREQUEST._serialized_end=9377
+  _DSGENERATEDATASETRESPONSE._serialized_start=9379
+  _DSGENERATEDATASETRESPONSE._serialized_end=9493
+  _DSSPLITDATASETREQUEST._serialized_start=9496
+  _DSSPLITDATASETREQUEST._serialized_end=10215
+  _DSSPLITDATASETRESPONSE._serialized_start=10218
+  _DSSPLITDATASETRESPONSE._serialized_end=10669
+  _DSSPLITDATASETTORUNGSREQUEST._serialized_start=10672
+  _DSSPLITDATASETTORUNGSREQUEST._serialized_end=11056
+  _DSSPLITDATASETTORUNGSRESPONSE._serialized_start=11058
+  _DSSPLITDATASETTORUNGSRESPONSE._serialized_end=11089
+  _GROUPBYDATASETREQUEST._serialized_start=11092
+  _GROUPBYDATASETREQUEST._serialized_end=11454
+  _GROUPBYDATASETRESPONSE._serialized_start=11456
+  _GROUPBYDATASETRESPONSE._serialized_end=11493
+  _DSINFERSCHEMAREQUEST._serialized_start=11496
+  _DSINFERSCHEMAREQUEST._serialized_end=11709
+  _DSINFERSCHEMARESPONSE._serialized_start=11711
+  _DSINFERSCHEMARESPONSE._serialized_end=11817
+  _DSGETTABLEVIEWREQUEST._serialized_start=11820
+  _DSGETTABLEVIEWREQUEST._serialized_end=12040
+  _DSGETTABLEVIEWRESPONSE._serialized_start=12042
+  _DSGETTABLEVIEWRESPONSE._serialized_end=12146
+  _CREATEMODELREPORTREQUEST._serialized_start=12149
+  _CREATEMODELREPORTREQUEST._serialized_end=12667
+  _CREATEFORECASTREPORTREQUEST._serialized_start=12670
+  _CREATEFORECASTREPORTREQUEST._serialized_end=13781
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_start=945
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_end=990
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_start=4396
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_end=4443
-  _CREATESUMMARYREPORTREQUEST._serialized_start=13145
-  _CREATESUMMARYREPORTREQUEST._serialized_end=13340
-  _CREATEREPORTRESPONSE._serialized_start=13342
-  _CREATEREPORTRESPONSE._serialized_end=13377
-  _CREATEDATASETREPORTREQUEST._serialized_start=13380
-  _CREATEDATASETREPORTREQUEST._serialized_end=13740
-  _CREATESTUDYREPORTREQUEST._serialized_start=13743
-  _CREATESTUDYREPORTREQUEST._serialized_end=14266
-  _ASKMODELREQUEST._serialized_start=14269
-  _ASKMODELREQUEST._serialized_end=14758
-  _GETTIMESERIESDATASETKEYSREQUEST._serialized_start=14761
-  _GETTIMESERIESDATASETKEYSREQUEST._serialized_end=15124
-  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_start=15126
-  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_end=15174
-  _ASKFORECASTMODELREQUEST._serialized_start=15177
-  _ASKFORECASTMODELREQUEST._serialized_end=15634
-  _ASKFORECASTMODELRESPONSE._serialized_start=15636
-  _ASKFORECASTMODELRESPONSE._serialized_end=15742
-  _ASKENSEMBLEREQUEST._serialized_start=15745
-  _ASKENSEMBLEREQUEST._serialized_end=16264
-  _ASKENSEMBLERESPONSE._serialized_start=16266
-  _ASKENSEMBLERESPONSE._serialized_end=16367
-  _ASKBASELINEREQUEST._serialized_start=16370
-  _ASKBASELINEREQUEST._serialized_end=16839
-  _ASKBASELINERESPONSE._serialized_start=16841
-  _ASKBASELINERESPONSE._serialized_end=16942
-  _ASKALLMODELSFORTASKREQUEST._serialized_start=16945
-  _ASKALLMODELSFORTASKREQUEST._serialized_end=17421
-  _ASKALLMODELSFORTASKRESPONSE._serialized_start=17423
-  _ASKALLMODELSFORTASKRESPONSE._serialized_end=17532
-  _TELLMODELREQUEST._serialized_start=17535
-  _TELLMODELREQUEST._serialized_end=17979
-  _TELLMODELRESPONSE._serialized_start=17981
-  _TELLMODELRESPONSE._serialized_end=18016
-  _DSSHUTDOWNREQUEST._serialized_start=18018
-  _DSSHUTDOWNREQUEST._serialized_end=18037
-  _DSSHUTDOWNRESPONSE._serialized_start=18039
-  _DSSHUTDOWNRESPONSE._serialized_end=18059
-  _DSTESTCONNECTIONREQUEST._serialized_start=18062
-  _DSTESTCONNECTIONREQUEST._serialized_end=18408
+  _CREATESUMMARYREPORTREQUEST._serialized_start=13784
+  _CREATESUMMARYREPORTREQUEST._serialized_end=13979
+  _CREATEREPORTRESPONSE._serialized_start=13981
+  _CREATEREPORTRESPONSE._serialized_end=14016
+  _CREATEDATASETREPORTREQUEST._serialized_start=14019
+  _CREATEDATASETREPORTREQUEST._serialized_end=14468
+  _CREATESTUDYREPORTREQUEST._serialized_start=14471
+  _CREATESTUDYREPORTREQUEST._serialized_end=15083
+  _ASKMODELREQUEST._serialized_start=15086
+  _ASKMODELREQUEST._serialized_end=15664
+  _GETTIMESERIESDATASETKEYSREQUEST._serialized_start=15667
+  _GETTIMESERIESDATASETKEYSREQUEST._serialized_end=16030
+  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_start=16032
+  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_end=16080
+  _ASKFORECASTMODELREQUEST._serialized_start=16083
+  _ASKFORECASTMODELREQUEST._serialized_end=16540
+  _ASKFORECASTMODELRESPONSE._serialized_start=16542
+  _ASKFORECASTMODELRESPONSE._serialized_end=16648
+  _ASKENSEMBLEREQUEST._serialized_start=16651
+  _ASKENSEMBLEREQUEST._serialized_end=17259
+  _ASKENSEMBLERESPONSE._serialized_start=17261
+  _ASKENSEMBLERESPONSE._serialized_end=17362
+  _ASKBASELINEREQUEST._serialized_start=17365
+  _ASKBASELINEREQUEST._serialized_end=17923
+  _ASKBASELINERESPONSE._serialized_start=17925
+  _ASKBASELINERESPONSE._serialized_end=18026
+  _ASKALLMODELSFORTASKREQUEST._serialized_start=18029
+  _ASKALLMODELSFORTASKREQUEST._serialized_end=18594
+  _ASKALLMODELSFORTASKRESPONSE._serialized_start=18596
+  _ASKALLMODELSFORTASKRESPONSE._serialized_end=18705
+  _TELLMODELREQUEST._serialized_start=18708
+  _TELLMODELREQUEST._serialized_end=19241
+  _TELLMODELRESPONSE._serialized_start=19243
+  _TELLMODELRESPONSE._serialized_end=19278
+  _DSSHUTDOWNREQUEST._serialized_start=19280
+  _DSSHUTDOWNREQUEST._serialized_end=19299
+  _DSSHUTDOWNRESPONSE._serialized_start=19301
+  _DSSHUTDOWNRESPONSE._serialized_end=19321
+  _DSTESTCONNECTIONREQUEST._serialized_start=19324
+  _DSTESTCONNECTIONREQUEST._serialized_end=19670
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_start=945
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_end=990
-  _DSTESTCONNECTIONRESPONSE._serialized_start=18410
-  _DSTESTCONNECTIONRESPONSE._serialized_end=18465
-  _DSSTUDYENDEDREQUEST._serialized_start=18468
-  _DSSTUDYENDEDREQUEST._serialized_end=18653
-  _DSSTUDYENDEDRESPONSE._serialized_start=18655
-  _DSSTUDYENDEDRESPONSE._serialized_end=18677
-  _SAVEOPTIMIZERDBREQUEST._serialized_start=18680
-  _SAVEOPTIMIZERDBREQUEST._serialized_end=18954
-  _SAVEOPTIMIZERDBRESPONSE._serialized_start=18956
-  _SAVEOPTIMIZERDBRESPONSE._serialized_end=19070
-  _DSGETDATABASESREQUEST._serialized_start=19072
-  _DSGETDATABASESREQUEST._serialized_end=19182
-  _DSGETDATABASESRESPONSE._serialized_start=19184
-  _DSGETDATABASESRESPONSE._serialized_end=19227
-  _DSGETTABLESREQUEST._serialized_start=19229
-  _DSGETTABLESREQUEST._serialized_end=19336
-  _DSGETTABLESRESPONSE._serialized_start=19338
-  _DSGETTABLESRESPONSE._serialized_end=19375
-  _DSEXECUTESQLREQUEST._serialized_start=19377
-  _DSEXECUTESQLREQUEST._serialized_end=19498
-  _DSEXECUTESQLRESPONSE._serialized_start=19500
-  _DSEXECUTESQLRESPONSE._serialized_end=19602
-  _DSSNAPSHOTREQUEST._serialized_start=19605
-  _DSSNAPSHOTREQUEST._serialized_end=19874
-  _DSSNAPSHOTRESPONSE._serialized_start=19876
-  _DSSNAPSHOTRESPONSE._serialized_end=19896
-  _ASKMODELRESPONSE._serialized_start=19898
-  _ASKMODELRESPONSE._serialized_end=19996
-  _GENTRAININGDATAREQUEST._serialized_start=19999
-  _GENTRAININGDATAREQUEST._serialized_end=20457
-  _GENTRAININGDATARESPONSE._serialized_start=20459
-  _GENTRAININGDATARESPONSE._serialized_end=20573
-  _SYNCONLINESTOREREQUEST._serialized_start=20576
-  _SYNCONLINESTOREREQUEST._serialized_end=21451
+  _DSTESTCONNECTIONRESPONSE._serialized_start=19672
+  _DSTESTCONNECTIONRESPONSE._serialized_end=19727
+  _DSSTUDYENDEDREQUEST._serialized_start=19730
+  _DSSTUDYENDEDREQUEST._serialized_end=19915
+  _DSSTUDYENDEDRESPONSE._serialized_start=19917
+  _DSSTUDYENDEDRESPONSE._serialized_end=19939
+  _SAVEOPTIMIZERDBREQUEST._serialized_start=19942
+  _SAVEOPTIMIZERDBREQUEST._serialized_end=20216
+  _SAVEOPTIMIZERDBRESPONSE._serialized_start=20218
+  _SAVEOPTIMIZERDBRESPONSE._serialized_end=20332
+  _DSGETDATABASESREQUEST._serialized_start=20334
+  _DSGETDATABASESREQUEST._serialized_end=20444
+  _DSGETDATABASESRESPONSE._serialized_start=20446
+  _DSGETDATABASESRESPONSE._serialized_end=20489
+  _DSGETTABLESREQUEST._serialized_start=20491
+  _DSGETTABLESREQUEST._serialized_end=20598
+  _DSGETTABLESRESPONSE._serialized_start=20600
+  _DSGETTABLESRESPONSE._serialized_end=20637
+  _DSEXECUTESQLREQUEST._serialized_start=20639
+  _DSEXECUTESQLREQUEST._serialized_end=20760
+  _DSEXECUTESQLRESPONSE._serialized_start=20762
+  _DSEXECUTESQLRESPONSE._serialized_end=20864
+  _DSSNAPSHOTREQUEST._serialized_start=20867
+  _DSSNAPSHOTREQUEST._serialized_end=21136
+  _DSSNAPSHOTRESPONSE._serialized_start=21138
+  _DSSNAPSHOTRESPONSE._serialized_end=21158
+  _ASKMODELRESPONSE._serialized_start=21160
+  _ASKMODELRESPONSE._serialized_end=21258
+  _GENTRAININGDATAREQUEST._serialized_start=21261
+  _GENTRAININGDATAREQUEST._serialized_end=21719
+  _GENTRAININGDATARESPONSE._serialized_start=21721
+  _GENTRAININGDATARESPONSE._serialized_end=21835
+  _SYNCONLINESTOREREQUEST._serialized_start=21838
+  _SYNCONLINESTOREREQUEST._serialized_end=22713
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_start=4396
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_end=4443
-  _SYNCONLINESTORERESPONSE._serialized_start=21453
-  _SYNCONLINESTORERESPONSE._serialized_end=21478
-  _GENONLINESTOREDATASETREQUEST._serialized_start=21481
-  _GENONLINESTOREDATASETREQUEST._serialized_end=22374
+  _SYNCONLINESTORERESPONSE._serialized_start=22715
+  _SYNCONLINESTORERESPONSE._serialized_end=22740
+  _GENONLINESTOREDATASETREQUEST._serialized_start=22743
+  _GENONLINESTOREDATASETREQUEST._serialized_end=23636
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_start=4396
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_end=4443
-  _GENONLINESTOREDATASETRESPONSE._serialized_start=22376
-  _GENONLINESTOREDATASETRESPONSE._serialized_end=22496
-  _BATCHPREDICTREQUEST._serialized_start=22499
-  _BATCHPREDICTREQUEST._serialized_end=23536
+  _GENONLINESTOREDATASETRESPONSE._serialized_start=23638
+  _GENONLINESTOREDATASETRESPONSE._serialized_end=23758
+  _BATCHPREDICTREQUEST._serialized_start=23761
+  _BATCHPREDICTREQUEST._serialized_end=24798
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_start=4396
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_end=4443
-  _BATCHPREDICTRESPONSE._serialized_start=23538
-  _BATCHPREDICTRESPONSE._serialized_end=23574
-  _SAVEDATASETREQUEST._serialized_start=23577
-  _SAVEDATASETREQUEST._serialized_end=24126
-  _SAVEMODELREQUEST._serialized_start=24129
-  _SAVEMODELREQUEST._serialized_end=24754
-  _SAVEPREDICTIONREQUEST._serialized_start=24757
-  _SAVEPREDICTIONREQUEST._serialized_end=25323
-  _SAVEPREDICTORREQUEST._serialized_start=25326
-  _SAVEPREDICTORREQUEST._serialized_end=25705
-  _CREATEMETRICSSTOREREQUEST._serialized_start=25708
-  _CREATEMETRICSSTOREREQUEST._serialized_end=25840
-  _CREATEMETRICSSTORERESPONSE._serialized_start=25842
-  _CREATEMETRICSSTORERESPONSE._serialized_end=25870
-  _SAVERESPONSE._serialized_start=25872
-  _SAVERESPONSE._serialized_end=25900
-  _DATASERVICE._serialized_start=25903
-  _DATASERVICE._serialized_end=34079
+  _BATCHPREDICTRESPONSE._serialized_start=24800
+  _BATCHPREDICTRESPONSE._serialized_end=24836
+  _SAVEDATASETREQUEST._serialized_start=24839
+  _SAVEDATASETREQUEST._serialized_end=25388
+  _SAVEMODELREQUEST._serialized_start=25391
+  _SAVEMODELREQUEST._serialized_end=26016
+  _SAVEPREDICTIONREQUEST._serialized_start=26019
+  _SAVEPREDICTIONREQUEST._serialized_end=26585
+  _SAVEPREDICTORREQUEST._serialized_start=26588
+  _SAVEPREDICTORREQUEST._serialized_end=26967
+  _CREATEMETRICSSTOREREQUEST._serialized_start=26970
+  _CREATEMETRICSSTOREREQUEST._serialized_end=27102
+  _CREATEMETRICSSTORERESPONSE._serialized_start=27104
+  _CREATEMETRICSSTORERESPONSE._serialized_end=27132
+  _SAVERESPONSE._serialized_start=27134
+  _SAVERESPONSE._serialized_end=27162
+  _DATASERVICE._serialized_start=27165
+  _DATASERVICE._serialized_end=35341
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,76 +9,82 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class AskAllModelsForTaskRequest(_message.Message):
-    __slots__ = ["algorithms", "budget", "dataset", "datasource", "product", "study", "task"]
+    __slots__ = ["algorithms", "budget", "dataset", "datasource", "product", "snapshot", "study", "task"]
     ALGORITHMS_FIELD_NUMBER: _ClassVar[int]
     BUDGET_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     TASK_FIELD_NUMBER: _ClassVar[int]
     algorithms: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1_1_1_1.Algorithm]
     budget: int
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
     task: str
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., budget: _Optional[int] = ..., task: _Optional[str] = ..., algorithms: _Optional[_Iterable[_Union[_generated_pb2_1_1_1_1.Algorithm, _Mapping]]] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., budget: _Optional[int] = ..., task: _Optional[str] = ..., algorithms: _Optional[_Iterable[_Union[_generated_pb2_1_1_1_1.Algorithm, _Mapping]]] = ...) -> None: ...
 
 class AskAllModelsForTaskResponse(_message.Message):
     __slots__ = ["model"]
     MODEL_FIELD_NUMBER: _ClassVar[int]
     model: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1.Model]
     def __init__(self, model: _Optional[_Iterable[_Union[_generated_pb2_1.Model, _Mapping]]] = ...) -> None: ...
 
 class AskBaselineRequest(_message.Message):
-    __slots__ = ["algnames", "algorithms", "all", "dataset", "datasource", "product", "study"]
+    __slots__ = ["algnames", "algorithms", "all", "dataset", "datasource", "product", "snapshot", "study"]
     ALGNAMES_FIELD_NUMBER: _ClassVar[int]
     ALGORITHMS_FIELD_NUMBER: _ClassVar[int]
     ALL_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     algnames: _containers.RepeatedScalarFieldContainer[str]
     algorithms: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1_1_1_1.Algorithm]
     all: bool
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., algnames: _Optional[_Iterable[str]] = ..., all: bool = ..., algorithms: _Optional[_Iterable[_Union[_generated_pb2_1_1_1_1.Algorithm, _Mapping]]] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., algnames: _Optional[_Iterable[str]] = ..., all: bool = ..., algorithms: _Optional[_Iterable[_Union[_generated_pb2_1_1_1_1.Algorithm, _Mapping]]] = ...) -> None: ...
 
 class AskBaselineResponse(_message.Message):
     __slots__ = ["model"]
     MODEL_FIELD_NUMBER: _ClassVar[int]
     model: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1.Model]
     def __init__(self, model: _Optional[_Iterable[_Union[_generated_pb2_1.Model, _Mapping]]] = ...) -> None: ...
 
 class AskEnsembleRequest(_message.Message):
-    __slots__ = ["algorithms", "dataset", "datasource", "models", "product", "study"]
+    __slots__ = ["algorithms", "dataset", "datasource", "models", "product", "snapshot", "study"]
     ALGORITHMS_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     MODELS_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     algorithms: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1_1_1_1.Algorithm]
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     models: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1.Model]
     product: _generated_pb2.DataProduct
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., models: _Optional[_Iterable[_Union[_generated_pb2_1.Model, _Mapping]]] = ..., algorithms: _Optional[_Iterable[_Union[_generated_pb2_1_1_1_1.Algorithm, _Mapping]]] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., models: _Optional[_Iterable[_Union[_generated_pb2_1.Model, _Mapping]]] = ..., algorithms: _Optional[_Iterable[_Union[_generated_pb2_1_1_1_1.Algorithm, _Mapping]]] = ...) -> None: ...
 
 class AskEnsembleResponse(_message.Message):
     __slots__ = ["model"]
     MODEL_FIELD_NUMBER: _ClassVar[int]
     model: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1.Model]
     def __init__(self, model: _Optional[_Iterable[_Union[_generated_pb2_1.Model, _Mapping]]] = ...) -> None: ...
 
@@ -101,32 +107,34 @@
 class AskForecastModelResponse(_message.Message):
     __slots__ = ["model"]
     MODEL_FIELD_NUMBER: _ClassVar[int]
     model: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1.Model]
     def __init__(self, model: _Optional[_Iterable[_Union[_generated_pb2_1.Model, _Mapping]]] = ...) -> None: ...
 
 class AskModelRequest(_message.Message):
-    __slots__ = ["algorithm", "algorithms", "budget", "dataset", "datasource", "defaultHP", "product", "study"]
+    __slots__ = ["algorithm", "algorithms", "budget", "dataset", "datasource", "defaultHP", "product", "snapshot", "study"]
     ALGORITHMS_FIELD_NUMBER: _ClassVar[int]
     ALGORITHM_FIELD_NUMBER: _ClassVar[int]
     BUDGET_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     DEFAULTHP_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     algorithm: str
     algorithms: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1_1_1_1.Algorithm]
     budget: int
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     defaultHP: bool
     product: _generated_pb2.DataProduct
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., budget: _Optional[int] = ..., defaultHP: bool = ..., algorithm: _Optional[str] = ..., algorithms: _Optional[_Iterable[_Union[_generated_pb2_1_1_1_1.Algorithm, _Mapping]]] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., budget: _Optional[int] = ..., defaultHP: bool = ..., algorithm: _Optional[str] = ..., algorithms: _Optional[_Iterable[_Union[_generated_pb2_1_1_1_1.Algorithm, _Mapping]]] = ...) -> None: ...
 
 class AskModelResponse(_message.Message):
     __slots__ = ["model"]
     MODEL_FIELD_NUMBER: _ClassVar[int]
     model: _generated_pb2_1.Model
     def __init__(self, model: _Optional[_Union[_generated_pb2_1.Model, _Mapping]] = ...) -> None: ...
 
@@ -171,24 +179,26 @@
 class BatchPredictResponse(_message.Message):
     __slots__ = ["rows"]
     ROWS_FIELD_NUMBER: _ClassVar[int]
     rows: int
     def __init__(self, rows: _Optional[int] = ...) -> None: ...
 
 class CreateDatasetReportRequest(_message.Message):
-    __slots__ = ["dataset", "datasource", "product", "report"]
+    __slots__ = ["dataset", "datasource", "product", "report", "snapshot"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     REPORT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
     report: _generated_pb2_1.Report
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., report: _Optional[_Union[_generated_pb2_1.Report, _Mapping]] = ...) -> None: ...
+    snapshot: _generated_pb2.DatasetSnapshot
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., report: _Optional[_Union[_generated_pb2_1.Report, _Mapping]] = ...) -> None: ...
 
 class CreateForecastReportRequest(_message.Message):
     __slots__ = ["bucket", "connection", "dataset", "datasource", "dbConnection", "dbSecret", "forecast", "group", "product", "report", "secret", "study"]
     class DbSecretEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
@@ -259,28 +269,30 @@
 class CreateReportResponse(_message.Message):
     __slots__ = ["pdf"]
     PDF_FIELD_NUMBER: _ClassVar[int]
     pdf: bytes
     def __init__(self, pdf: _Optional[bytes] = ...) -> None: ...
 
 class CreateStudyReportRequest(_message.Message):
-    __slots__ = ["dataset", "datasource", "models", "product", "report", "study"]
+    __slots__ = ["dataset", "datasource", "models", "product", "report", "snapshot", "study"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     MODELS_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     REPORT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     models: _generated_pb2_1.ModelList
     product: _generated_pb2.DataProduct
     report: _generated_pb2_1.Report
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., models: _Optional[_Union[_generated_pb2_1.ModelList, _Mapping]] = ..., report: _Optional[_Union[_generated_pb2_1.Report, _Mapping]] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., models: _Optional[_Union[_generated_pb2_1.ModelList, _Mapping]] = ..., report: _Optional[_Union[_generated_pb2_1.Report, _Mapping]] = ...) -> None: ...
 
 class CreateSummaryReportRequest(_message.Message):
     __slots__ = ["product", "reports"]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     REPORTS_FIELD_NUMBER: _ClassVar[int]
     product: _generated_pb2.DataProduct
     reports: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1.Report]
@@ -291,72 +303,78 @@
     def __init__(self) -> None: ...
 
 class DatasetResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class DsCreateDatasetProfileRequest(_message.Message):
-    __slots__ = ["bucket", "dataset", "datasource", "product"]
+    __slots__ = ["bucket", "dataset", "datasource", "product", "snapshot"]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     bucket: _generated_pb2_1_1_1.VirtualBucket
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ...) -> None: ...
+    snapshot: _generated_pb2.DatasetSnapshot
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ...) -> None: ...
 
 class DsCreateDatasetProfileResponse(_message.Message):
     __slots__ = ["anomalyLocation", "profile", "profileLocation"]
     ANOMALYLOCATION_FIELD_NUMBER: _ClassVar[int]
     PROFILELOCATION_FIELD_NUMBER: _ClassVar[int]
     PROFILE_FIELD_NUMBER: _ClassVar[int]
     anomalyLocation: _generated_pb2_1_1_1_1.FileLocation
     profile: _common_pb2.DatasetProfile
     profileLocation: _generated_pb2_1_1_1_1.FileLocation
     def __init__(self, profile: _Optional[_Union[_common_pb2.DatasetProfile, _Mapping]] = ..., profileLocation: _Optional[_Union[_generated_pb2_1_1_1_1.FileLocation, _Mapping]] = ..., anomalyLocation: _Optional[_Union[_generated_pb2_1_1_1_1.FileLocation, _Mapping]] = ...) -> None: ...
 
 class DsCreateModelProfileRequest(_message.Message):
-    __slots__ = ["bucket", "dataset", "datasource", "model", "product", "study"]
+    __slots__ = ["bucket", "dataset", "datasource", "model", "product", "snapshot", "study"]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     MODEL_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     bucket: _generated_pb2_1_1_1.VirtualBucket
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     model: _generated_pb2_1.Model
     product: _generated_pb2.DataProduct
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., model: _Optional[_Union[_generated_pb2_1.Model, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., model: _Optional[_Union[_generated_pb2_1.Model, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ...) -> None: ...
 
 class DsCreateModelProfileResponse(_message.Message):
     __slots__ = ["profileLocation"]
     PROFILELOCATION_FIELD_NUMBER: _ClassVar[int]
     profileLocation: _generated_pb2_1_1_1_1.FileLocation
     def __init__(self, profileLocation: _Optional[_Union[_generated_pb2_1_1_1_1.FileLocation, _Mapping]] = ...) -> None: ...
 
 class DsCreateStudyProfileRequest(_message.Message):
-    __slots__ = ["bucket", "dataset", "datasource", "models", "product", "study"]
+    __slots__ = ["bucket", "dataset", "datasource", "models", "product", "snapshot", "study"]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     MODELS_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     bucket: _generated_pb2_1_1_1.VirtualBucket
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     models: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1.Model]
     product: _generated_pb2.DataProduct
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ..., models: _Optional[_Iterable[_Union[_generated_pb2_1.Model, _Mapping]]] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ..., models: _Optional[_Iterable[_Union[_generated_pb2_1.Model, _Mapping]]] = ...) -> None: ...
 
 class DsCreateStudyProfileResponse(_message.Message):
     __slots__ = ["profileLocation"]
     PROFILELOCATION_FIELD_NUMBER: _ClassVar[int]
     profileLocation: _generated_pb2_1_1_1_1.FileLocation
     def __init__(self, profileLocation: _Optional[_Union[_generated_pb2_1_1_1_1.FileLocation, _Mapping]] = ...) -> None: ...
 
@@ -371,26 +389,28 @@
 class DsExecuteSqlResponse(_message.Message):
     __slots__ = ["tableview"]
     TABLEVIEW_FIELD_NUMBER: _ClassVar[int]
     tableview: _common_pb2.TableView
     def __init__(self, tableview: _Optional[_Union[_common_pb2.TableView, _Mapping]] = ...) -> None: ...
 
 class DsGenerateDatasetRequest(_message.Message):
-    __slots__ = ["dataset", "datasource", "product", "rows", "target"]
+    __slots__ = ["dataset", "datasource", "product", "rows", "snapshot", "target"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     ROWS_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     TARGET_FIELD_NUMBER: _ClassVar[int]
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
     rows: int
+    snapshot: _generated_pb2.DatasetSnapshot
     target: _generated_pb2_1_1_1_1.DataLocation
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., target: _Optional[_Union[_generated_pb2_1_1_1_1.DataLocation, _Mapping]] = ..., rows: _Optional[int] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., target: _Optional[_Union[_generated_pb2_1_1_1_1.DataLocation, _Mapping]] = ..., rows: _Optional[int] = ...) -> None: ...
 
 class DsGenerateDatasetResponse(_message.Message):
     __slots__ = ["target"]
     TARGET_FIELD_NUMBER: _ClassVar[int]
     target: _generated_pb2_1_1_1_1.DataLocation
     def __init__(self, target: _Optional[_Union[_generated_pb2_1_1_1_1.DataLocation, _Mapping]] = ...) -> None: ...
 
@@ -666,30 +686,32 @@
     def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ...) -> None: ...
 
 class DsSnapshotResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class DsSplitDatasetRequest(_message.Message):
-    __slots__ = ["bucket", "dataset", "datasource", "product", "study", "testingDataset", "trainingDataset"]
+    __slots__ = ["bucket", "dataset", "datasource", "product", "snapshot", "study", "testingDataset", "trainingDataset"]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     TESTINGDATASET_FIELD_NUMBER: _ClassVar[int]
     TRAININGDATASET_FIELD_NUMBER: _ClassVar[int]
     bucket: _generated_pb2_1_1_1.VirtualBucket
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
-    testingDataset: _generated_pb2.Dataset
-    trainingDataset: _generated_pb2.Dataset
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ..., trainingDataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., testingDataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ...) -> None: ...
+    testingDataset: _generated_pb2.DatasetSnapshot
+    trainingDataset: _generated_pb2.DatasetSnapshot
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ..., trainingDataset: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., testingDataset: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ...) -> None: ...
 
 class DsSplitDatasetResponse(_message.Message):
     __slots__ = ["indexFile", "testLocation", "testing", "testingHash", "trainLocation", "training", "trainingHash", "validation", "validationHash", "validationLocation"]
     INDEXFILE_FIELD_NUMBER: _ClassVar[int]
     TESTINGHASH_FIELD_NUMBER: _ClassVar[int]
     TESTING_FIELD_NUMBER: _ClassVar[int]
     TESTLOCATION_FIELD_NUMBER: _ClassVar[int]
@@ -708,24 +730,26 @@
     trainingHash: str
     validation: int
     validationHash: str
     validationLocation: _generated_pb2_1_1_1_1.FileLocation
     def __init__(self, training: _Optional[int] = ..., testing: _Optional[int] = ..., validation: _Optional[int] = ..., trainingHash: _Optional[str] = ..., testingHash: _Optional[str] = ..., validationHash: _Optional[str] = ..., indexFile: _Optional[str] = ..., trainLocation: _Optional[_Union[_generated_pb2_1_1_1_1.FileLocation, _Mapping]] = ..., testLocation: _Optional[_Union[_generated_pb2_1_1_1_1.FileLocation, _Mapping]] = ..., validationLocation: _Optional[_Union[_generated_pb2_1_1_1_1.FileLocation, _Mapping]] = ...) -> None: ...
 
 class DsSplitDatasetToRungsRequest(_message.Message):
-    __slots__ = ["dataset", "datasource", "product", "rungs"]
+    __slots__ = ["dataset", "datasource", "product", "rungs", "snapshot"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     RUNGS_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
     rungs: int
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., rungs: _Optional[int] = ...) -> None: ...
+    snapshot: _generated_pb2.DatasetSnapshot
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., rungs: _Optional[int] = ...) -> None: ...
 
 class DsSplitDatasetToRungsResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class DsStudyEndedRequest(_message.Message):
     __slots__ = ["product", "study"]
@@ -860,22 +884,24 @@
 class GetTimeSeriesDatasetKeysResponse(_message.Message):
     __slots__ = ["keys"]
     KEYS_FIELD_NUMBER: _ClassVar[int]
     keys: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, keys: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class GroupByDatasetRequest(_message.Message):
-    __slots__ = ["dataset", "datasource", "product"]
+    __slots__ = ["dataset", "datasource", "product", "snapshot"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ...) -> None: ...
+    snapshot: _generated_pb2.DatasetSnapshot
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ...) -> None: ...
 
 class GroupByDatasetResponse(_message.Message):
     __slots__ = ["uri"]
     URI_FIELD_NUMBER: _ClassVar[int]
     uri: str
     def __init__(self, uri: _Optional[str] = ...) -> None: ...
 
@@ -1028,27 +1054,29 @@
     def __init__(self, storageConnection: _Optional[_Union[_generated_pb2_1_1_1.Connection, _Mapping]] = ..., storageBucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ..., storageSecret: _Optional[_Mapping[str, bytes]] = ..., dbConnection: _Optional[_Union[_generated_pb2_1_1_1.Connection, _Mapping]] = ..., dbSecret: _Optional[_Mapping[str, bytes]] = ..., model: _Optional[_Union[_generated_pb2_1.ModelClass, _Mapping]] = ..., fg: _Optional[_Union[_generated_pb2.FeatureGroup, _Mapping]] = ..., location: _Optional[_Union[_generated_pb2_1_1_1_1.DataLocation, _Mapping]] = ...) -> None: ...
 
 class SyncOnlineStoreResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class TellModelRequest(_message.Message):
-    __slots__ = ["dataset", "datasource", "failed", "model", "product", "study"]
+    __slots__ = ["dataset", "datasource", "failed", "model", "product", "snapshot", "study"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     FAILED_FIELD_NUMBER: _ClassVar[int]
     MODEL_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     failed: bool
     model: _generated_pb2_1.Model
     product: _generated_pb2.DataProduct
+    snapshot: _generated_pb2.DatasetSnapshot
     study: _generated_pb2_1.Study
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., model: _Optional[_Union[_generated_pb2_1.Model, _Mapping]] = ..., failed: bool = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ..., model: _Optional[_Union[_generated_pb2_1.Model, _Mapping]] = ..., failed: bool = ...) -> None: ...
 
 class TellModelResponse(_message.Message):
     __slots__ = ["pruned"]
     PRUNED_FIELD_NUMBER: _ClassVar[int]
     pruned: bool
     def __init__(self, pruned: bool = ...) -> None: ...
```

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,30 +441,28 @@
         """If a model is a partial model (sample < 100%)
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def TellModel(self, request, context):
-        """for bayaisn optimization, we tell the planner the result of the model evaluation
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def MergeForecastFile(self, request, context):
         """Merge the forecast back to one file.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DsTestConnection(self, request, context):
-        """test connection from python presepective
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ShutDown(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
```

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?github.com/metaprov/modelaapi/services/dataset/v1/dataset.proto\x12\x31github.com.metaprov.modelaapi.services.dataset.v1\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\"\xf4\x01\n\x13ListDatasetsRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x62\n\x06labels\x18\x02 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.dataset.v1.ListDatasetsRequest.LabelsEntry\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x10\n\x08order_by\x18\x05 \x01(\t\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x84\x01\n\x14ListDatasetsResponse\x12S\n\x08\x64\x61tasets\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetList\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xc5\x01\n\x11GetDatasetRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12`\n\x06labels\x18\x03 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetRequest.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x12GetDatasetResponse\x12N\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04yaml\x18\x02 \x01(\t\"f\n\x14\x43reateDatasetRequest\x12N\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x17\n\x15\x43reateDatasetResponse\"\x96\x01\n\x14UpdateDatasetRequest\x12N\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x17\n\x15UpdateDatasetResponse\"7\n\x14\x44\x65leteDatasetRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x17\n\x15\x44\x65leteDatasetResponse\"\x8b\x01\n\x18GetDatasetProfileRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\\\n\x08snapshot\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.SnapshotReference\"n\n\x19GetDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\x89\x01\n\x16\x44ownloadDatasetRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\\\n\x08snapshot\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.SnapshotReference\"&\n\x17\x44ownloadDatasetResponse\x12\x0b\n\x03raw\x18\x01 \x01(\x0c\"\x8d\x01\n\x1aGetDatasetAnomaliesRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\\\n\x08snapshot\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.SnapshotReference\"i\n\x1bGetDatasetAnomaliesResponse\x12J\n\x05table\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView2\xd2\r\n\x0e\x44\x61tasetService\x12\xc1\x01\n\x0cListDatasets\x12\x46.github.com.metaprov.modelaapi.services.dataset.v1.ListDatasetsRequest\x1aG.github.com.metaprov.modelaapi.services.dataset.v1.ListDatasetsResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/datasets/{namespace}\x12\xc2\x01\n\nGetDataset\x12\x44.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetRequest\x1a\x45.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/v1/datasets/{namespace}/{name}\x12\xbb\x01\n\rCreateDataset\x12G.github.com.metaprov.modelaapi.services.dataset.v1.CreateDatasetRequest\x1aH.github.com.metaprov.modelaapi.services.dataset.v1.CreateDatasetResponse\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v1/datasets:\x01*\x12\xf0\x01\n\rUpdateDataset\x12G.github.com.metaprov.modelaapi.services.dataset.v1.UpdateDatasetRequest\x1aH.github.com.metaprov.modelaapi.services.dataset.v1.UpdateDatasetResponse\"L\x82\xd3\xe4\x93\x02\x46\x1a\x41/v1/datasets/{dataset.metadata.namespace}/{dataset.metadata.name}:\x01*\x12\xbf\x01\n\rDeleteDataset\x12G.github.com.metaprov.modelaapi.services.dataset.v1.DeleteDatasetRequest\x1aH.github.com.metaprov.modelaapi.services.dataset.v1.DeleteDatasetResponse\"\x1b\x82\xd3\xe4\x93\x02\x15*\x13/v1/datasets/{name}\x12\xeb\x01\n\x11GetDatasetProfile\x12K.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetProfileRequest\x1aL.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetProfileResponse\";\x82\xd3\xe4\x93\x02\x35\"3/v1/datasets/{namespace}/{snapshot.dataset}:profile\x12\xe6\x01\n\x0f\x44ownloadDataset\x12I.github.com.metaprov.modelaapi.services.dataset.v1.DownloadDatasetRequest\x1aJ.github.com.metaprov.modelaapi.services.dataset.v1.DownloadDatasetResponse\"<\x82\xd3\xe4\x93\x02\x36\"4/v1/datasets/{namespace}/{snapshot.dataset}:download\x12\xec\x01\n\x0cGetAnomalies\x12M.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetAnomaliesRequest\x1aN.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetAnomaliesResponse\"=\x82\xd3\xe4\x93\x02\x37\"5/v1/datasets/{namespace}/{snapshot.dataset}:anomaliesB3Z1github.com/metaprov/modelaapi/services/dataset/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?github.com/metaprov/modelaapi/services/dataset/v1/dataset.proto\x12\x31github.com.metaprov.modelaapi.services.dataset.v1\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\"\xf4\x01\n\x13ListDatasetsRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x62\n\x06labels\x18\x02 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.dataset.v1.ListDatasetsRequest.LabelsEntry\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x10\n\x08order_by\x18\x05 \x01(\t\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x84\x01\n\x14ListDatasetsResponse\x12S\n\x08\x64\x61tasets\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetList\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xc5\x01\n\x11GetDatasetRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12`\n\x06labels\x18\x03 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetRequest.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x12GetDatasetResponse\x12N\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04yaml\x18\x02 \x01(\t\"f\n\x14\x43reateDatasetRequest\x12N\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x17\n\x15\x43reateDatasetResponse\"\x96\x01\n\x14UpdateDatasetRequest\x12N\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x17\n\x15UpdateDatasetResponse\"7\n\x14\x44\x65leteDatasetRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x17\n\x15\x44\x65leteDatasetResponse\"\x8b\x01\n\x18GetDatasetProfileRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\\\n\x08snapshot\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.SnapshotReference\"n\n\x19GetDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\x89\x01\n\x16\x44ownloadDatasetRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\\\n\x08snapshot\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.SnapshotReference\"&\n\x17\x44ownloadDatasetResponse\x12\x0b\n\x03raw\x18\x01 \x01(\x0c\"\x8d\x01\n\x1aGetDatasetAnomaliesRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\\\n\x08snapshot\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.SnapshotReference\"i\n\x1bGetDatasetAnomaliesResponse\x12J\n\x05table\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x8a\x01\n\x16\x43ompareDatasetsRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12]\n\tsnapshots\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.SnapshotReference\"m\n\x17\x43ompareDatasetsResponse\x12R\n\x08profiles\x18\x01 \x03(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile2\xb3\x0f\n\x0e\x44\x61tasetService\x12\xc1\x01\n\x0cListDatasets\x12\x46.github.com.metaprov.modelaapi.services.dataset.v1.ListDatasetsRequest\x1aG.github.com.metaprov.modelaapi.services.dataset.v1.ListDatasetsResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/datasets/{namespace}\x12\xc2\x01\n\nGetDataset\x12\x44.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetRequest\x1a\x45.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/v1/datasets/{namespace}/{name}\x12\xbb\x01\n\rCreateDataset\x12G.github.com.metaprov.modelaapi.services.dataset.v1.CreateDatasetRequest\x1aH.github.com.metaprov.modelaapi.services.dataset.v1.CreateDatasetResponse\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v1/datasets:\x01*\x12\xf0\x01\n\rUpdateDataset\x12G.github.com.metaprov.modelaapi.services.dataset.v1.UpdateDatasetRequest\x1aH.github.com.metaprov.modelaapi.services.dataset.v1.UpdateDatasetResponse\"L\x82\xd3\xe4\x93\x02\x46\x1a\x41/v1/datasets/{dataset.metadata.namespace}/{dataset.metadata.name}:\x01*\x12\xcb\x01\n\rDeleteDataset\x12G.github.com.metaprov.modelaapi.services.dataset.v1.DeleteDatasetRequest\x1aH.github.com.metaprov.modelaapi.services.dataset.v1.DeleteDatasetResponse\"\'\x82\xd3\xe4\x93\x02!*\x1f/v1/datasets/{namespace}/{name}\x12\xeb\x01\n\x11GetDatasetProfile\x12K.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetProfileRequest\x1aL.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetProfileResponse\";\x82\xd3\xe4\x93\x02\x35\"3/v1/datasets/{namespace}/{snapshot.dataset}:profile\x12\xe6\x01\n\x0f\x44ownloadDataset\x12I.github.com.metaprov.modelaapi.services.dataset.v1.DownloadDatasetRequest\x1aJ.github.com.metaprov.modelaapi.services.dataset.v1.DownloadDatasetResponse\"<\x82\xd3\xe4\x93\x02\x36\"4/v1/datasets/{namespace}/{snapshot.dataset}:download\x12\xec\x01\n\x0cGetAnomalies\x12M.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetAnomaliesRequest\x1aN.github.com.metaprov.modelaapi.services.dataset.v1.GetDatasetAnomaliesResponse\"=\x82\xd3\xe4\x93\x02\x37\"5/v1/datasets/{namespace}/{snapshot.dataset}:anomalies\x12\xd2\x01\n\x0f\x43ompareDatasets\x12I.github.com.metaprov.modelaapi.services.dataset.v1.CompareDatasetsRequest\x1aJ.github.com.metaprov.modelaapi.services.dataset.v1.CompareDatasetsResponse\"(\x82\xd3\xe4\x93\x02\"\" /v1/datasets/{namespace}:compareB3Z1github.com/metaprov/modelaapi/services/dataset/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.dataset.v1.dataset_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z1github.com/metaprov/modelaapi/services/dataset/v1'
@@ -36,21 +36,23 @@
   _DATASETSERVICE.methods_by_name['GetDataset']._options = None
   _DATASETSERVICE.methods_by_name['GetDataset']._serialized_options = b'\202\323\344\223\002!\022\037/v1/datasets/{namespace}/{name}'
   _DATASETSERVICE.methods_by_name['CreateDataset']._options = None
   _DATASETSERVICE.methods_by_name['CreateDataset']._serialized_options = b'\202\323\344\223\002\021\"\014/v1/datasets:\001*'
   _DATASETSERVICE.methods_by_name['UpdateDataset']._options = None
   _DATASETSERVICE.methods_by_name['UpdateDataset']._serialized_options = b'\202\323\344\223\002F\032A/v1/datasets/{dataset.metadata.namespace}/{dataset.metadata.name}:\001*'
   _DATASETSERVICE.methods_by_name['DeleteDataset']._options = None
-  _DATASETSERVICE.methods_by_name['DeleteDataset']._serialized_options = b'\202\323\344\223\002\025*\023/v1/datasets/{name}'
+  _DATASETSERVICE.methods_by_name['DeleteDataset']._serialized_options = b'\202\323\344\223\002!*\037/v1/datasets/{namespace}/{name}'
   _DATASETSERVICE.methods_by_name['GetDatasetProfile']._options = None
   _DATASETSERVICE.methods_by_name['GetDatasetProfile']._serialized_options = b'\202\323\344\223\0025\"3/v1/datasets/{namespace}/{snapshot.dataset}:profile'
   _DATASETSERVICE.methods_by_name['DownloadDataset']._options = None
   _DATASETSERVICE.methods_by_name['DownloadDataset']._serialized_options = b'\202\323\344\223\0026\"4/v1/datasets/{namespace}/{snapshot.dataset}:download'
   _DATASETSERVICE.methods_by_name['GetAnomalies']._options = None
   _DATASETSERVICE.methods_by_name['GetAnomalies']._serialized_options = b'\202\323\344\223\0027\"5/v1/datasets/{namespace}/{snapshot.dataset}:anomalies'
+  _DATASETSERVICE.methods_by_name['CompareDatasets']._options = None
+  _DATASETSERVICE.methods_by_name['CompareDatasets']._serialized_options = b'\202\323\344\223\002\"\" /v1/datasets/{namespace}:compare'
   _LISTDATASETSREQUEST._serialized_start=418
   _LISTDATASETSREQUEST._serialized_end=662
   _LISTDATASETSREQUEST_LABELSENTRY._serialized_start=617
   _LISTDATASETSREQUEST_LABELSENTRY._serialized_end=662
   _LISTDATASETSRESPONSE._serialized_start=665
   _LISTDATASETSRESPONSE._serialized_end=797
   _GETDATASETREQUEST._serialized_start=800
@@ -79,10 +81,14 @@
   _DOWNLOADDATASETREQUEST._serialized_end=1896
   _DOWNLOADDATASETRESPONSE._serialized_start=1898
   _DOWNLOADDATASETRESPONSE._serialized_end=1936
   _GETDATASETANOMALIESREQUEST._serialized_start=1939
   _GETDATASETANOMALIESREQUEST._serialized_end=2080
   _GETDATASETANOMALIESRESPONSE._serialized_start=2082
   _GETDATASETANOMALIESRESPONSE._serialized_end=2187
-  _DATASETSERVICE._serialized_start=2190
-  _DATASETSERVICE._serialized_end=3936
+  _COMPAREDATASETSREQUEST._serialized_start=2190
+  _COMPAREDATASETSREQUEST._serialized_end=2328
+  _COMPAREDATASETSRESPONSE._serialized_start=2330
+  _COMPAREDATASETSRESPONSE._serialized_end=2439
+  _DATASETSERVICE._serialized_start=2442
+  _DATASETSERVICE._serialized_end=4413
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,32 @@
 from google.protobuf import empty_pb2 as _empty_pb2
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as _generated_pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as _generated_pb2_1
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as _common_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class CompareDatasetsRequest(_message.Message):
+    __slots__ = ["namespace", "snapshots"]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOTS_FIELD_NUMBER: _ClassVar[int]
+    namespace: str
+    snapshots: _containers.RepeatedCompositeFieldContainer[_generated_pb2_1.SnapshotReference]
+    def __init__(self, namespace: _Optional[str] = ..., snapshots: _Optional[_Iterable[_Union[_generated_pb2_1.SnapshotReference, _Mapping]]] = ...) -> None: ...
+
+class CompareDatasetsResponse(_message.Message):
+    __slots__ = ["profiles"]
+    PROFILES_FIELD_NUMBER: _ClassVar[int]
+    profiles: _containers.RepeatedCompositeFieldContainer[_common_pb2.DatasetProfile]
+    def __init__(self, profiles: _Optional[_Iterable[_Union[_common_pb2.DatasetProfile, _Mapping]]] = ...) -> None: ...
+
 class CreateDatasetRequest(_message.Message):
     __slots__ = ["dataset"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     dataset: _generated_pb2.Dataset
     def __init__(self, dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ...) -> None: ...
 
 class CreateDatasetResponse(_message.Message):
```

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,19 @@
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.DownloadDatasetResponse.FromString,
                 )
         self.GetAnomalies = channel.unary_unary(
                 '/github.com.metaprov.modelaapi.services.dataset.v1.DatasetService/GetAnomalies',
                 request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.GetDatasetAnomaliesRequest.SerializeToString,
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.GetDatasetAnomaliesResponse.FromString,
                 )
+        self.CompareDatasets = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.dataset.v1.DatasetService/CompareDatasets',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.CompareDatasetsRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.CompareDatasetsResponse.FromString,
+                )
 
 
 class DatasetServiceServicer(object):
     """///// Dataset Service ///////
 
     """
 
@@ -107,14 +112,20 @@
 
     def GetAnomalies(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def CompareDatasets(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DatasetServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListDatasets': grpc.unary_unary_rpc_method_handler(
                     servicer.ListDatasets,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.ListDatasetsRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.ListDatasetsResponse.SerializeToString,
@@ -150,14 +161,19 @@
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.DownloadDatasetResponse.SerializeToString,
             ),
             'GetAnomalies': grpc.unary_unary_rpc_method_handler(
                     servicer.GetAnomalies,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.GetDatasetAnomaliesRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.GetDatasetAnomaliesResponse.SerializeToString,
             ),
+            'CompareDatasets': grpc.unary_unary_rpc_method_handler(
+                    servicer.CompareDatasets,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.CompareDatasetsRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.CompareDatasetsResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'github.com.metaprov.modelaapi.services.dataset.v1.DatasetService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -297,7 +313,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.dataset.v1.DatasetService/GetAnomalies',
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.GetDatasetAnomaliesRequest.SerializeToString,
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.GetDatasetAnomaliesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CompareDatasets(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.dataset.v1.DatasetService/CompareDatasets',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.CompareDatasetsRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_dataset_dot_v1_dot_dataset__pb2.CompareDatasetsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/google/api/annotations_pb2.py` & `modelaapi-0.6.234/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/google/api/http_pb2.py` & `modelaapi-0.6.234/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/google/api/http_pb2.pyi` & `modelaapi-0.6.234/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.234/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/api/apps/v1/generated_pb2.pyi` & `modelaapi-0.6.234/k8s/io/api/apps/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/api/core/v1/generated_pb2.pyi` & `modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/api/rbac/v1/generated_pb2.pyi` & `modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi` & `modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/modelaapi/consts.py` & `modelaapi-0.6.234/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/modelaapi/custom_transformers.py` & `modelaapi-0.6.234/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/modelaapi/graykite_model.py` & `modelaapi-0.6.234/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/modelaapi/ts.py` & `modelaapi-0.6.234/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/modelaapi/version.py` & `modelaapi-0.6.234/modelaapi/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 233,
+    "micro": 234,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.233/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.234/modelaapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.233
+Version: 0.6.234
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.233
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.234
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.233
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.234
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.233/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.234/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/setup.cfg` & `modelaapi-0.6.234/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.233/setup.py` & `modelaapi-0.6.234/setup.py`

 * *Files identical despite different names*

