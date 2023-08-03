# Comparing `tmp/google-cloud-artifact-registry-1.8.2.tar.gz` & `tmp/google-cloud-artifact-registry-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-artifact-registry-1.8.2.tar", last modified: Wed Jul  5 15:50:23 2023, max compression
+gzip compressed data, was "google-cloud-artifact-registry-1.8.3.tar", last modified: Thu Aug  3 19:06:09 2023, max compression
```

## Comparing `google-cloud-artifact-registry-1.8.2.tar` & `google-cloud-artifact-registry-1.8.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4914 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3973 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.024055 google-cloud-artifact-registry-1.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.024055 google-cloud-artifact-registry-1.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.024055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/
--rw-rw-r--   0 root         (0)     1003     5160 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.028055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/
--rw-rw-r--   0 root         (0)     1003     4658 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    13684 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.028055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.028055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/
--rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/__init__.py
--rw-rw-r--   0 root         (0)     1003   173720 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/async_client.py
--rw-rw-r--   0 root         (0)     1003   195059 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/client.py
--rw-rw-r--   0 root         (0)     1003    46028 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.028055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22688 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/base.py
--rw-rw-r--   0 root         (0)     1003    54735 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    56058 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   197642 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.032055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/
--rw-rw-r--   0 root         (0)     1003     4282 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6178 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/apt_artifact.py
--rw-rw-r--   0 root         (0)     1003    17062 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/artifact.py
--rw-rw-r--   0 root         (0)     1003     6289 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/file.py
--rw-rw-r--   0 root         (0)     1003     4185 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/package.py
--rw-rw-r--   0 root         (0)     1003    10021 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/repository.py
--rw-rw-r--   0 root         (0)     1003     1012 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003     3484 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/settings.py
--rw-rw-r--   0 root         (0)     1003     5826 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/tag.py
--rw-rw-r--   0 root         (0)     1003     7171 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/version.py
--rw-rw-r--   0 root         (0)     1003     3578 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/vpcsc_config.py
--rw-rw-r--   0 root         (0)     1003     5666 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/yum_artifact.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.032055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/
--rw-rw-r--   0 root         (0)     1003     3493 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     9842 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.032055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.036056 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/
--rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/__init__.py
--rw-rw-r--   0 root         (0)     1003   132770 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/async_client.py
--rw-rw-r--   0 root         (0)     1003   144067 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/client.py
--rw-rw-r--   0 root         (0)     1003    25699 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.036056 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22792 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/base.py
--rw-rw-r--   0 root         (0)     1003    42447 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43467 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   141462 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.036056 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     3141 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6209 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/apt_artifact.py
--rw-rw-r--   0 root         (0)     1003     5727 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/file.py
--rw-rw-r--   0 root         (0)     1003     4064 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/package.py
--rw-rw-r--   0 root         (0)     1003    10058 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/repository.py
--rw-rw-r--   0 root         (0)     1003     1017 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/service.py
--rw-rw-r--   0 root         (0)     1003     3499 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/settings.py
--rw-rw-r--   0 root         (0)     1003     5846 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/tag.py
--rw-rw-r--   0 root         (0)     1003     6729 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/version.py
--rw-rw-r--   0 root         (0)     1003     5697 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/yum_artifact.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/
--rw-r--r--   0 root         (0)     1003     4914 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3986 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:23.044056 google-cloud-artifact-registry-1.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3008 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   755115 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/test_artifact_registry.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003   502969 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/test_artifact_registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.065762 google-cloud-artifact-registry-1.8.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5029 2023-08-03 19:06:09.065762 google-cloud-artifact-registry-1.8.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4088 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.049761 google-cloud-artifact-registry-1.8.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.049761 google-cloud-artifact-registry-1.8.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.053762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry/
+-rw-rw-r--   0 root         (0)     1003     5160 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.053762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/
+-rw-rw-r--   0 root         (0)     1003     4658 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13684 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.053762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.053762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/
+-rw-rw-r--   0 root         (0)     1003      777 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/__init__.py
+-rw-rw-r--   0 root         (0)     1003   172980 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/async_client.py
+-rw-rw-r--   0 root         (0)     1003   194319 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/client.py
+-rw-rw-r--   0 root         (0)     1003    46028 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.057762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22688 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    54735 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    56058 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   197900 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.057762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4282 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6178 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/apt_artifact.py
+-rw-rw-r--   0 root         (0)     1003    17065 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/artifact.py
+-rw-rw-r--   0 root         (0)     1003     6290 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/file.py
+-rw-rw-r--   0 root         (0)     1003     4186 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/package.py
+-rw-rw-r--   0 root         (0)     1003    10022 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/repository.py
+-rw-rw-r--   0 root         (0)     1003     1012 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003     3485 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/settings.py
+-rw-rw-r--   0 root         (0)     1003     5827 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/tag.py
+-rw-rw-r--   0 root         (0)     1003     7172 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/version.py
+-rw-rw-r--   0 root         (0)     1003     3579 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/vpcsc_config.py
+-rw-rw-r--   0 root         (0)     1003     5666 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/yum_artifact.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.057762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     3493 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9842 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.057762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.061762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/
+-rw-rw-r--   0 root         (0)     1003      777 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/__init__.py
+-rw-rw-r--   0 root         (0)     1003   132031 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/async_client.py
+-rw-rw-r--   0 root         (0)     1003   143328 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/client.py
+-rw-rw-r--   0 root         (0)     1003    25699 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.061762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22792 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    42447 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43467 2023-08-03 19:03:09.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   141720 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.061762 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     3141 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6209 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/apt_artifact.py
+-rw-rw-r--   0 root         (0)     1003     5729 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/file.py
+-rw-rw-r--   0 root         (0)     1003     4065 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/package.py
+-rw-rw-r--   0 root         (0)     1003    10059 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/repository.py
+-rw-rw-r--   0 root         (0)     1003     1017 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/service.py
+-rw-rw-r--   0 root         (0)     1003     3500 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/settings.py
+-rw-rw-r--   0 root         (0)     1003     5847 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/tag.py
+-rw-rw-r--   0 root         (0)     1003     6730 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/version.py
+-rw-rw-r--   0 root         (0)     1003     5697 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/yum_artifact.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.065762 google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/
+-rw-r--r--   0 root         (0)     1003     5029 2023-08-03 19:06:08.000000 google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3986 2023-08-03 19:06:09.000000 google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:08.000000 google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:06:08.000000 google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:08.000000 google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-08-03 19:06:08.000000 google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:06:08.000000 google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-03 19:06:09.069763 google-cloud-artifact-registry-1.8.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3008 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.065762 google-cloud-artifact-registry-1.8.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.065762 google-cloud-artifact-registry-1.8.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.065762 google-cloud-artifact-registry-1.8.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.065762 google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   755115 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1/test_artifact_registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:09.065762 google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   502969 2023-08-03 19:03:10.000000 google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1beta2/test_artifact_registry.py
```

### Comparing `google-cloud-artifact-registry-1.8.2/LICENSE` & `google-cloud-artifact-registry-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.2/MANIFEST.in` & `google-cloud-artifact-registry-1.8.3/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2020 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/PKG-INFO` & `google-cloud-artifact-registry-1.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-artifact-registry
-Version: 1.8.2
+Version: 1.8.3
 Summary: Google Cloud Artifact Registry API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Artifact Registry.:  https://cloud.google.com/artifact-registry
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-artifact-registry/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -97,29 +100,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-artifact-registry
+    pip install google-cloud-artifact-registry
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-artifact-registry
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-artifact-registry
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Artifact Registry
    to see other available methods on the client.
 -  Read the `Artifact Registry Product documentation`_ to learn
```

### Comparing `google-cloud-artifact-registry-1.8.2/README.rst` & `google-cloud-artifact-registry-1.8.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Artifact Registry.:  https://cloud.google.com/artifact-registry
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-artifact-registry/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -73,29 +76,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-artifact-registry
+    pip install google-cloud-artifact-registry
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-artifact-registry
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-artifact-registry
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Artifact Registry
    to see other available methods on the client.
 -  Read the `Artifact Registry Product documentation`_ to learn
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/gapic_version.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/gapic_metadata.json` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/gapic_version.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/__init__.py` & `google-cloud-artifact-registry-1.8.3/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/async_client.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -3426,50 +3426,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
@@ -3568,50 +3537,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/client.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -3899,50 +3899,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
@@ -4040,50 +4009,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/pagers.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/base.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc_asyncio.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/rest.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/services/artifact_registry/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -2071,62 +2071,62 @@
                 conditions in their IAM policies, see the `IAM
                 documentation <https://cloud.google.com/iam/help/conditions/resource-policies>`__.
 
                 **JSON example:**
 
                 ::
 
-                    {
-                      "bindings": [
-                        {
-                          "role": "roles/resourcemanager.organizationAdmin",
-                          "members": [
-                            "user:mike@example.com",
-                            "group:admins@example.com",
-                            "domain:google.com",
-                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                          ]
-                        },
-                        {
-                          "role": "roles/resourcemanager.organizationViewer",
-                          "members": [
-                            "user:eve@example.com"
-                          ],
-                          "condition": {
-                            "title": "expirable access",
-                            "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')",
-                          }
-                        }
-                      ],
-                      "etag": "BwWWja0YfJA=",
-                      "version": 3
-                    }
+                       {
+                         "bindings": [
+                           {
+                             "role": "roles/resourcemanager.organizationAdmin",
+                             "members": [
+                               "user:mike@example.com",
+                               "group:admins@example.com",
+                               "domain:google.com",
+                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                             ]
+                           },
+                           {
+                             "role": "roles/resourcemanager.organizationViewer",
+                             "members": [
+                               "user:eve@example.com"
+                             ],
+                             "condition": {
+                               "title": "expirable access",
+                               "description": "Does not grant access after Sep 2020",
+                               "expression": "request.time <
+                               timestamp('2020-10-01T00:00:00.000Z')",
+                             }
+                           }
+                         ],
+                         "etag": "BwWWja0YfJA=",
+                         "version": 3
+                       }
 
                 **YAML example:**
 
                 ::
 
-                    bindings:
-                    - members:
-                      - user:mike@example.com
-                      - group:admins@example.com
-                      - domain:google.com
-                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin
-                    - members:
-                      - user:eve@example.com
-                      role: roles/resourcemanager.organizationViewer
-                      condition:
-                        title: expirable access
-                        description: Does not grant access after Sep 2020
-                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
-                    etag: BwWWja0YfJA=
-                    version: 3
+                       bindings:
+                       - members:
+                         - user:mike@example.com
+                         - group:admins@example.com
+                         - domain:google.com
+                         - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                         role: roles/resourcemanager.organizationAdmin
+                       - members:
+                         - user:eve@example.com
+                         role: roles/resourcemanager.organizationViewer
+                         condition:
+                           title: expirable access
+                           description: Does not grant access after Sep 2020
+                           expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+                       etag: BwWWja0YfJA=
+                       version: 3
 
                 For a description of IAM and its features, see the `IAM
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
@@ -3963,62 +3963,62 @@
                 conditions in their IAM policies, see the `IAM
                 documentation <https://cloud.google.com/iam/help/conditions/resource-policies>`__.
 
                 **JSON example:**
 
                 ::
 
-                    {
-                      "bindings": [
-                        {
-                          "role": "roles/resourcemanager.organizationAdmin",
-                          "members": [
-                            "user:mike@example.com",
-                            "group:admins@example.com",
-                            "domain:google.com",
-                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                          ]
-                        },
-                        {
-                          "role": "roles/resourcemanager.organizationViewer",
-                          "members": [
-                            "user:eve@example.com"
-                          ],
-                          "condition": {
-                            "title": "expirable access",
-                            "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')",
-                          }
-                        }
-                      ],
-                      "etag": "BwWWja0YfJA=",
-                      "version": 3
-                    }
+                       {
+                         "bindings": [
+                           {
+                             "role": "roles/resourcemanager.organizationAdmin",
+                             "members": [
+                               "user:mike@example.com",
+                               "group:admins@example.com",
+                               "domain:google.com",
+                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                             ]
+                           },
+                           {
+                             "role": "roles/resourcemanager.organizationViewer",
+                             "members": [
+                               "user:eve@example.com"
+                             ],
+                             "condition": {
+                               "title": "expirable access",
+                               "description": "Does not grant access after Sep 2020",
+                               "expression": "request.time <
+                               timestamp('2020-10-01T00:00:00.000Z')",
+                             }
+                           }
+                         ],
+                         "etag": "BwWWja0YfJA=",
+                         "version": 3
+                       }
 
                 **YAML example:**
 
                 ::
 
-                    bindings:
-                    - members:
-                      - user:mike@example.com
-                      - group:admins@example.com
-                      - domain:google.com
-                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin
-                    - members:
-                      - user:eve@example.com
-                      role: roles/resourcemanager.organizationViewer
-                      condition:
-                        title: expirable access
-                        description: Does not grant access after Sep 2020
-                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
-                    etag: BwWWja0YfJA=
-                    version: 3
+                       bindings:
+                       - members:
+                         - user:mike@example.com
+                         - group:admins@example.com
+                         - domain:google.com
+                         - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                         role: roles/resourcemanager.organizationAdmin
+                       - members:
+                         - user:eve@example.com
+                         role: roles/resourcemanager.organizationViewer
+                         condition:
+                           title: expirable access
+                           description: Does not grant access after Sep 2020
+                           expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+                       etag: BwWWja0YfJA=
+                       version: 3
 
                 For a description of IAM and its features, see the `IAM
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/apt_artifact.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/apt_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/artifact.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -63,14 +63,15 @@
             where "us-west4" is the registry_location, "test-project" is
             the project_id, "test-repo" is the repository_name and
             "nginx@sha256:e9954c1fc875017be1c3e36eca16be2d9e9bccc4bf072163515467d6a823c7cf"
             is the image's digest.
         uri (str):
             Required. URL to access the image.
             Example:
+
             us-west4-docker.pkg.dev/test-project/test-repo/nginx@sha256:e9954c1fc875017be1c3e36eca16be2d9e9bccc4bf072163515467d6a823c7cf
         tags (MutableSequence[str]):
             Tags attached to this image.
         image_size_bytes (int):
             Calculated size of the image.
             This field is returned as the
             'metadata.imageSizeBytes' field in the Version
@@ -219,18 +220,20 @@
             com.google.guava:guava:31.0-jre", where "us-west4" is the
             registry_location, "test-project" is the project_id,
             "test-repo" is the repository_name and
             "com.google.guava:guava:31.0-jre" is the maven artifact.
         pom_uri (str):
             Required. URL to access the pom file of the
             artifact. Example:
+
             us-west4-maven.pkg.dev/test-project/test-repo/com/google/guava/guava/31.0/guava-31.0.pom
         group_id (str):
             Group ID for the artifact.
             Example:
+
             com.google.guava
         artifact_id (str):
             Artifact ID for the artifact.
         version (str):
             Version of this artifact.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time the artifact was created.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/file.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -71,14 +71,15 @@
 class File(proto.Message):
     r"""Files store content that is potentially associated with
     Packages or Versions.
 
     Attributes:
         name (str):
             The name of the file, for example:
+
             "projects/p1/locations/us-central1/repositories/repo1/files/a%2Fb%2Fc.txt".
             If the file ID part contains slashes, they are
             escaped.
         size_bytes (int):
             The size of the File in bytes.
         hashes (MutableSequence[google.cloud.artifactregistry_v1.types.Hash]):
             The hashes of the file content.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/package.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -34,14 +34,15 @@
 
 class Package(proto.Message):
     r"""Packages are named collections of versions.
 
     Attributes:
         name (str):
             The name of the package, for example:
+
             "projects/p1/locations/us-central1/repositories/repo1/packages/pkg1".
             If the package ID part contains slashes, the
             slashes are escaped.
         display_name (str):
             The display name of the package.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the package was created.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/repository.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,14 +45,15 @@
             Maven repository config contains repository
             level configuration for the repositories of
             maven type.
 
             This field is a member of `oneof`_ ``format_config``.
         name (str):
             The name of the repository, for example:
+
             "projects/p1/locations/us-central1/repositories/repo1".
         format_ (google.cloud.artifactregistry_v1.types.Repository.Format):
             The format of packages that are stored in the
             repository.
         description (str):
             The user-provided description of the
             repository.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/service.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/settings.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,15 +17,15 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.devtools.artifactregistry.v1",
+    package="google.devtools.artifactregistry.v1beta2",
     manifest={
         "ProjectSettings",
         "GetProjectSettingsRequest",
         "UpdateProjectSettingsRequest",
     },
 )
 
@@ -33,19 +33,20 @@
 class ProjectSettings(proto.Message):
     r"""The Artifact Registry settings that apply to a Project.
 
     Attributes:
         name (str):
             The name of the project's settings.
             Always of the form:
+
             projects/{project-id}/projectSettings
 
             In update request: never set
             In response: always set
-        legacy_redirection_state (google.cloud.artifactregistry_v1.types.ProjectSettings.RedirectionState):
+        legacy_redirection_state (google.cloud.artifactregistry_v1beta2.types.ProjectSettings.RedirectionState):
             The redirection state of the legacy
             repositories in this project.
     """
 
     class RedirectionState(proto.Enum):
         r"""The possible redirection states for legacy repositories.
 
@@ -91,15 +92,15 @@
     )
 
 
 class UpdateProjectSettingsRequest(proto.Message):
     r"""Sets the settings of the project.
 
     Attributes:
-        project_settings (google.cloud.artifactregistry_v1.types.ProjectSettings):
+        project_settings (google.cloud.artifactregistry_v1beta2.types.ProjectSettings):
             The project settings.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Field mask to support partial updates.
     """
 
     project_settings: "ProjectSettings" = proto.Field(
         proto.MESSAGE,
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/tag.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -44,14 +44,15 @@
             "projects/p1/locations/us-central1/repositories/repo1/packages/pkg1/tags/tag1".
             If the package part contains slashes, the slashes are
             escaped. The tag part can only have characters in
             [a-zA-Z0-9-._~:@], anything else must be URL encoded.
         version (str):
             The name of the version the tag refers to,
             for example:
+
             "projects/p1/locations/us-central1/repositories/repo1/packages/pkg1/versions/sha256:5243811"
             If the package or version ID parts contain
             slashes, the slashes are escaped.
     """
 
     name: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/version.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -60,14 +60,15 @@
     r"""The body of a version resource. A version resource represents
     a collection of components, such as files and other data. This
     may correspond to a version in many package management schemes.
 
     Attributes:
         name (str):
             The name of the version, for example:
+
             "projects/p1/locations/us-central1/repositories/repo1/packages/pkg1/versions/art1".
             If the package or version ID parts contain
             slashes, the slashes are escaped.
         description (str):
             Optional. Description of the version, as
             specified in its metadata.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/vpcsc_config.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/vpcsc_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -33,14 +33,15 @@
 class VPCSCConfig(proto.Message):
     r"""The Artifact Registry VPC SC config that apply to a Project.
 
     Attributes:
         name (str):
             The name of the project's VPC SC Config.
             Always of the form:
+
             projects/{projectID}/locations/{location}/vpcscConfig
             In update request: never set
             In response: always set
         vpcsc_policy (google.cloud.artifactregistry_v1.types.VPCSCConfig.VPCSCPolicy):
             The project per location VPC SC policy that
             defines the VPC SC behavior for the Remote
             Repository (Allow/Deny).
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/yum_artifact.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/yum_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/gapic_metadata.json` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/gapic_version.py` & `google-cloud-artifact-registry-1.8.3/tests/unit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/__init__.py` & `google-cloud-artifact-registry-1.8.3/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/async_client.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1838,14 +1838,15 @@
 
         Args:
             request (Optional[Union[google.cloud.artifactregistry_v1beta2.types.ListFilesRequest, dict]]):
                 The request object. The request to list files.
             parent (:class:`str`):
                 The name of the repository whose
                 files will be listed. For example:
+
                 "projects/p1/locations/us-central1/repositories/repo1
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -2650,50 +2651,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
@@ -2792,50 +2762,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/client.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -2111,14 +2111,15 @@
 
         Args:
             request (Union[google.cloud.artifactregistry_v1beta2.types.ListFilesRequest, dict]):
                 The request object. The request to list files.
             parent (str):
                 The name of the repository whose
                 files will be listed. For example:
+
                 "projects/p1/locations/us-central1/repositories/repo1
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -2878,50 +2879,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
@@ -3019,50 +2989,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/pagers.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/base.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc_asyncio.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/rest.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1616,62 +1616,62 @@
                 conditions in their IAM policies, see the `IAM
                 documentation <https://cloud.google.com/iam/help/conditions/resource-policies>`__.
 
                 **JSON example:**
 
                 ::
 
-                    {
-                      "bindings": [
-                        {
-                          "role": "roles/resourcemanager.organizationAdmin",
-                          "members": [
-                            "user:mike@example.com",
-                            "group:admins@example.com",
-                            "domain:google.com",
-                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                          ]
-                        },
-                        {
-                          "role": "roles/resourcemanager.organizationViewer",
-                          "members": [
-                            "user:eve@example.com"
-                          ],
-                          "condition": {
-                            "title": "expirable access",
-                            "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')",
-                          }
-                        }
-                      ],
-                      "etag": "BwWWja0YfJA=",
-                      "version": 3
-                    }
+                       {
+                         "bindings": [
+                           {
+                             "role": "roles/resourcemanager.organizationAdmin",
+                             "members": [
+                               "user:mike@example.com",
+                               "group:admins@example.com",
+                               "domain:google.com",
+                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                             ]
+                           },
+                           {
+                             "role": "roles/resourcemanager.organizationViewer",
+                             "members": [
+                               "user:eve@example.com"
+                             ],
+                             "condition": {
+                               "title": "expirable access",
+                               "description": "Does not grant access after Sep 2020",
+                               "expression": "request.time <
+                               timestamp('2020-10-01T00:00:00.000Z')",
+                             }
+                           }
+                         ],
+                         "etag": "BwWWja0YfJA=",
+                         "version": 3
+                       }
 
                 **YAML example:**
 
                 ::
 
-                    bindings:
-                    - members:
-                      - user:mike@example.com
-                      - group:admins@example.com
-                      - domain:google.com
-                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin
-                    - members:
-                      - user:eve@example.com
-                      role: roles/resourcemanager.organizationViewer
-                      condition:
-                        title: expirable access
-                        description: Does not grant access after Sep 2020
-                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
-                    etag: BwWWja0YfJA=
-                    version: 3
+                       bindings:
+                       - members:
+                         - user:mike@example.com
+                         - group:admins@example.com
+                         - domain:google.com
+                         - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                         role: roles/resourcemanager.organizationAdmin
+                       - members:
+                         - user:eve@example.com
+                         role: roles/resourcemanager.organizationViewer
+                         condition:
+                           title: expirable access
+                           description: Does not grant access after Sep 2020
+                           expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+                       etag: BwWWja0YfJA=
+                       version: 3
 
                 For a description of IAM and its features, see the `IAM
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
@@ -2757,62 +2757,62 @@
                 conditions in their IAM policies, see the `IAM
                 documentation <https://cloud.google.com/iam/help/conditions/resource-policies>`__.
 
                 **JSON example:**
 
                 ::
 
-                    {
-                      "bindings": [
-                        {
-                          "role": "roles/resourcemanager.organizationAdmin",
-                          "members": [
-                            "user:mike@example.com",
-                            "group:admins@example.com",
-                            "domain:google.com",
-                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                          ]
-                        },
-                        {
-                          "role": "roles/resourcemanager.organizationViewer",
-                          "members": [
-                            "user:eve@example.com"
-                          ],
-                          "condition": {
-                            "title": "expirable access",
-                            "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')",
-                          }
-                        }
-                      ],
-                      "etag": "BwWWja0YfJA=",
-                      "version": 3
-                    }
+                       {
+                         "bindings": [
+                           {
+                             "role": "roles/resourcemanager.organizationAdmin",
+                             "members": [
+                               "user:mike@example.com",
+                               "group:admins@example.com",
+                               "domain:google.com",
+                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                             ]
+                           },
+                           {
+                             "role": "roles/resourcemanager.organizationViewer",
+                             "members": [
+                               "user:eve@example.com"
+                             ],
+                             "condition": {
+                               "title": "expirable access",
+                               "description": "Does not grant access after Sep 2020",
+                               "expression": "request.time <
+                               timestamp('2020-10-01T00:00:00.000Z')",
+                             }
+                           }
+                         ],
+                         "etag": "BwWWja0YfJA=",
+                         "version": 3
+                       }
 
                 **YAML example:**
 
                 ::
 
-                    bindings:
-                    - members:
-                      - user:mike@example.com
-                      - group:admins@example.com
-                      - domain:google.com
-                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin
-                    - members:
-                      - user:eve@example.com
-                      role: roles/resourcemanager.organizationViewer
-                      condition:
-                        title: expirable access
-                        description: Does not grant access after Sep 2020
-                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
-                    etag: BwWWja0YfJA=
-                    version: 3
+                       bindings:
+                       - members:
+                         - user:mike@example.com
+                         - group:admins@example.com
+                         - domain:google.com
+                         - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                         role: roles/resourcemanager.organizationAdmin
+                       - members:
+                         - user:eve@example.com
+                         role: roles/resourcemanager.organizationViewer
+                         condition:
+                           title: expirable access
+                           description: Does not grant access after Sep 2020
+                           expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+                       etag: BwWWja0YfJA=
+                       version: 3
 
                 For a description of IAM and its features, see the `IAM
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/__init__.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/apt_artifact.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/apt_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/file.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -71,14 +71,15 @@
 class File(proto.Message):
     r"""Files store content that is potentially associated with
     Packages or Versions.
 
     Attributes:
         name (str):
             The name of the file, for example:
+
             "projects/p1/locations/us-central1/repositories/repo1/files/a%2Fb%2Fc.txt".
             If the file ID part contains slashes, they are
             escaped.
         size_bytes (int):
             The size of the File in bytes.
         hashes (MutableSequence[google.cloud.artifactregistry_v1beta2.types.Hash]):
             The hashes of the file content.
@@ -123,14 +124,15 @@
 class ListFilesRequest(proto.Message):
     r"""The request to list files.
 
     Attributes:
         parent (str):
             The name of the repository whose files will
             be listed. For example:
+
             "projects/p1/locations/us-central1/repositories/repo1
         filter (str):
             An expression for filtering the results of the request.
             Filter rules are case insensitive. The fields eligible for
             filtering are:
 
             -  ``name``
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/package.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -34,14 +34,15 @@
 
 class Package(proto.Message):
     r"""Packages are named collections of versions.
 
     Attributes:
         name (str):
             The name of the package, for example:
+
             "projects/p1/locations/us-central1/repositories/repo1/packages/pkg1".
         display_name (str):
             The display name of the package.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the package was created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             The time when the package was last updated.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/repository.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,14 +45,15 @@
             Maven repository config contains repository
             level configuration for the repositories of
             maven type.
 
             This field is a member of `oneof`_ ``format_config``.
         name (str):
             The name of the repository, for example:
+
             "projects/p1/locations/us-central1/repositories/repo1".
         format_ (google.cloud.artifactregistry_v1beta2.types.Repository.Format):
             The format of packages that are stored in the
             repository.
         description (str):
             The user-provided description of the
             repository.
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/service.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/settings.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1/types/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,15 +17,15 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.devtools.artifactregistry.v1beta2",
+    package="google.devtools.artifactregistry.v1",
     manifest={
         "ProjectSettings",
         "GetProjectSettingsRequest",
         "UpdateProjectSettingsRequest",
     },
 )
 
@@ -33,19 +33,20 @@
 class ProjectSettings(proto.Message):
     r"""The Artifact Registry settings that apply to a Project.
 
     Attributes:
         name (str):
             The name of the project's settings.
             Always of the form:
+
             projects/{project-id}/projectSettings
 
             In update request: never set
             In response: always set
-        legacy_redirection_state (google.cloud.artifactregistry_v1beta2.types.ProjectSettings.RedirectionState):
+        legacy_redirection_state (google.cloud.artifactregistry_v1.types.ProjectSettings.RedirectionState):
             The redirection state of the legacy
             repositories in this project.
     """
 
     class RedirectionState(proto.Enum):
         r"""The possible redirection states for legacy repositories.
 
@@ -91,15 +92,15 @@
     )
 
 
 class UpdateProjectSettingsRequest(proto.Message):
     r"""Sets the settings of the project.
 
     Attributes:
-        project_settings (google.cloud.artifactregistry_v1beta2.types.ProjectSettings):
+        project_settings (google.cloud.artifactregistry_v1.types.ProjectSettings):
             The project settings.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Field mask to support partial updates.
     """
 
     project_settings: "ProjectSettings" = proto.Field(
         proto.MESSAGE,
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/tag.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -44,14 +44,15 @@
             "projects/p1/locations/us-central1/repositories/repo1/packages/pkg1/tags/tag1".
             If the package part contains slashes, the slashes are
             escaped. The tag part can only have characters in
             [a-zA-Z0-9-._~:@], anything else must be URL encoded.
         version (str):
             The name of the version the tag refers to,
             for example:
+
             "projects/p1/locations/us-central1/repositories/repo1/packages/pkg1/versions/sha256:5243811"
             If the package or version ID parts contain
             slashes, the slashes are escaped.
     """
 
     name: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/version.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -59,14 +59,15 @@
     r"""The body of a version resource. A version resource represents
     a collection of components, such as files and other data. This
     may correspond to a version in many package management schemes.
 
     Attributes:
         name (str):
             The name of the version, for example:
+
             "projects/p1/locations/us-central1/repositories/repo1/packages/pkg1/versions/art1".
             If the package or version ID parts contain
             slashes, the slashes are escaped.
         description (str):
             Optional. Description of the version, as
             specified in its metadata.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
```

### Comparing `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/yum_artifact.py` & `google-cloud-artifact-registry-1.8.3/google/cloud/artifactregistry_v1beta2/types/yum_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/PKG-INFO` & `google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-artifact-registry
-Version: 1.8.2
+Version: 1.8.3
 Summary: Google Cloud Artifact Registry API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Artifact Registry.:  https://cloud.google.com/artifact-registry
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-artifact-registry/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -97,29 +100,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-artifact-registry
+    pip install google-cloud-artifact-registry
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-artifact-registry
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-artifact-registry
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Artifact Registry
    to see other available methods on the client.
 -  Read the `Artifact Registry Product documentation`_ to learn
```

### Comparing `google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/SOURCES.txt` & `google-cloud-artifact-registry-1.8.3/google_cloud_artifact_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.2/setup.py` & `google-cloud-artifact-registry-1.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/tests/__init__.py` & `google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/tests/unit/__init__.py` & `google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1beta2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/test_artifact_registry.py` & `google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1/test_artifact_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/test_artifact_registry.py` & `google-cloud-artifact-registry-1.8.3/tests/unit/gapic/artifactregistry_v1beta2/test_artifact_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

