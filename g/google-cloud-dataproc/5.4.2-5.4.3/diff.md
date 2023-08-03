# Comparing `tmp/google-cloud-dataproc-5.4.2.tar.gz` & `tmp/google-cloud-dataproc-5.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataproc-5.4.2.tar", last modified: Wed Jul  5 15:07:01 2023, max compression
+gzip compressed data, was "google-cloud-dataproc-5.4.3.tar", last modified: Thu Aug  3 17:53:57 2023, max compression
```

## Comparing `google-cloud-dataproc-5.4.2.tar` & `google-cloud-dataproc-5.4.3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.667206 google-cloud-dataproc-5.4.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4620 2023-07-05 15:07:01.667206 google-cloud-dataproc-5.4.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3701 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.643207 google-cloud-dataproc-5.4.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.643207 google-cloud-dataproc-5.4.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/google/cloud/dataproc/
--rw-rw-r--   0 root         (0)     1003    15051 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/
--rw-rw-r--   0 root         (0)     1003    11355 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15797 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.651207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    56180 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    64864 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     6171 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.651207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1566 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11320 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24453 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24765 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    64105 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.651207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/
--rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    48423 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    58292 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/client.py
--rw-rw-r--   0 root         (0)     1003     5645 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.651207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1432 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9285 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22939 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23286 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    57614 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/
--rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    80455 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    89325 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/client.py
--rw-rw-r--   0 root         (0)     1003     5692 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1460 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13322 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28663 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29113 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    80094 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/
--rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    67560 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    74242 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/client.py
--rw-rw-r--   0 root         (0)     1003     5512 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13052 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26071 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26482 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    72086 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/
--rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    46647 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    55885 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.659206 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1496 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8990 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22495 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22822 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    54940 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.659206 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/
--rw-rw-r--   0 root         (0)     1003      805 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    73291 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    82170 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/client.py
--rw-rw-r--   0 root         (0)     1003     6101 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.659206 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/
--rw-rw-r--   0 root         (0)     1003     1552 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13977 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30186 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    30591 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    78720 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/
--rw-rw-r--   0 root         (0)     1003     7071 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16523 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/autoscaling_policies.py
--rw-rw-r--   0 root         (0)     1003    20835 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/batches.py
--rw-rw-r--   0 root         (0)     1003    81651 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/clusters.py
--rw-rw-r--   0 root         (0)     1003    56007 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/jobs.py
--rw-rw-r--   0 root         (0)     1003     6061 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/node_groups.py
--rw-rw-r--   0 root         (0)     1003     9425 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/operations.py
--rw-rw-r--   0 root         (0)     1003    27760 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/shared.py
--rw-rw-r--   0 root         (0)     1003    38762 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/workflow_templates.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/
--rw-r--r--   0 root         (0)     1003     4620 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5438 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:07:01.667206 google-cloud-dataproc-5.4.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2972 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/tests/system/gapic/v1/
--rw-rw-r--   0 root         (0)     1003     1109 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/system/gapic/v1/test_system_cluster_controller_v1.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.667206 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   220145 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_autoscaling_policy_service.py
--rw-rw-r--   0 root         (0)     1003   196675 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_batch_controller.py
--rw-rw-r--   0 root         (0)     1003   301083 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_cluster_controller.py
--rw-rw-r--   0 root         (0)     1003   256059 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_job_controller.py
--rw-rw-r--   0 root         (0)     1003   169636 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_node_group_controller.py
--rw-rw-r--   0 root         (0)     1003   333025 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_workflow_template_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.809831 google-cloud-dataproc-5.4.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4691 2023-08-03 17:53:57.809831 google-cloud-dataproc-5.4.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3772 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.785831 google-cloud-dataproc-5.4.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.785831 google-cloud-dataproc-5.4.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.789831 google-cloud-dataproc-5.4.3/google/cloud/dataproc/
+-rw-rw-r--   0 root         (0)     1003    15051 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.793831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/
+-rw-rw-r--   0 root         (0)     1003    11355 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15797 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.793831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.793831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    56180 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    64864 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6171 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.793831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1566 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11320 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24453 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24765 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    64105 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.793831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/
+-rw-rw-r--   0 root         (0)     1003      773 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    48423 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58292 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/client.py
+-rw-rw-r--   0 root         (0)     1003     5645 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.797831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1432 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9285 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22939 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23286 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    57614 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.797831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/
+-rw-rw-r--   0 root         (0)     1003      781 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    80455 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    89325 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/client.py
+-rw-rw-r--   0 root         (0)     1003     5692 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.797831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1460 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13322 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28663 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29113 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    80094 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.797831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/
+-rw-rw-r--   0 root         (0)     1003      765 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67560 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74242 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/client.py
+-rw-rw-r--   0 root         (0)     1003     5512 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.801831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13052 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26071 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26482 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    72086 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.801831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/
+-rw-rw-r--   0 root         (0)     1003      789 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46647 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    55885 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.801831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1496 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8990 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22495 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22822 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    54940 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.801831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/
+-rw-rw-r--   0 root         (0)     1003      805 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    73291 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    82170 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6101 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.805831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1552 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13977 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30186 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    30591 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    78720 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.805831 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/
+-rw-rw-r--   0 root         (0)     1003     7071 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16523 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/autoscaling_policies.py
+-rw-rw-r--   0 root         (0)     1003    20835 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/batches.py
+-rw-rw-r--   0 root         (0)     1003    81664 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/clusters.py
+-rw-rw-r--   0 root         (0)     1003    56039 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/jobs.py
+-rw-rw-r--   0 root         (0)     1003     6061 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/node_groups.py
+-rw-rw-r--   0 root         (0)     1003     9425 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/operations.py
+-rw-rw-r--   0 root         (0)     1003    27760 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/shared.py
+-rw-rw-r--   0 root         (0)     1003    38763 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/workflow_templates.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.805831 google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/
+-rw-r--r--   0 root         (0)     1003     4691 2023-08-03 17:53:57.000000 google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5438 2023-08-03 17:53:57.000000 google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 17:53:57.000000 google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 17:53:57.000000 google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 17:53:57.000000 google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-08-03 17:53:57.000000 google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 17:53:57.000000 google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-03 17:53:57.809831 google-cloud-dataproc-5.4.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2972 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.805831 google-cloud-dataproc-5.4.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.789831 google-cloud-dataproc-5.4.3/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.789831 google-cloud-dataproc-5.4.3/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.805831 google-cloud-dataproc-5.4.3/tests/system/gapic/v1/
+-rw-rw-r--   0 root         (0)     1003     1109 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/system/gapic/v1/test_system_cluster_controller_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.805831 google-cloud-dataproc-5.4.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.805831 google-cloud-dataproc-5.4.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 17:53:57.809831 google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   220145 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_autoscaling_policy_service.py
+-rw-rw-r--   0 root         (0)     1003   196675 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_batch_controller.py
+-rw-rw-r--   0 root         (0)     1003   301083 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_cluster_controller.py
+-rw-rw-r--   0 root         (0)     1003   256059 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_job_controller.py
+-rw-rw-r--   0 root         (0)     1003   169636 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_node_group_controller.py
+-rw-rw-r--   0 root         (0)     1003   333025 2023-08-03 17:51:57.000000 google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_workflow_template_service.py
```

### Comparing `google-cloud-dataproc-5.4.2/LICENSE` & `google-cloud-dataproc-5.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.2/MANIFEST.in` & `google-cloud-dataproc-5.4.3/MANIFEST.in`

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

### Comparing `google-cloud-dataproc-5.4.2/PKG-INFO` & `google-cloud-dataproc-5.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataproc
-Version: 5.4.2
+Version: 5.4.3
 Summary: Google Cloud Dataproc API client library
 Home-page: https://github.com/googleapis/python-dataproc
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Google Cloud Dataproc API.:  https://cloud.google.com/dataproc
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
+.. _samples/: https://github.com/googleapis/python-dataproc/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-dataproc
+    pip install google-cloud-dataproc
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-dataproc
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-dataproc
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Google Cloud Dataproc API
    to see other available methods on the client.
 -  Read the `Google Cloud Dataproc API Product documentation`_ to learn
```

### Comparing `google-cloud-dataproc-5.4.2/README.rst` & `google-cloud-dataproc-5.4.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Google Cloud Dataproc API.:  https://cloud.google.com/dataproc
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
+.. _samples/: https://github.com/googleapis/python-dataproc/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-dataproc
+    pip install google-cloud-dataproc
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-dataproc
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-dataproc
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Google Cloud Dataproc API
    to see other available methods on the client.
 -  Read the `Google Cloud Dataproc API Product documentation`_ to learn
```

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc/gapic_version.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "5.4.2"  # {x-release-please-version}
+__version__ = "5.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/gapic_metadata.json` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/gapic_version.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "5.4.2"  # {x-release-please-version}
+__version__ = "5.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/async_client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/async_client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/pagers.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/pagers.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/base.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/base.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/rest.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/rest.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/__init__.py`

 * *Files 12% similar despite different names*

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/async_client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/async_client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/pagers.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/pagers.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/__init__.py`

 * *Files 8% similar despite different names*

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/base.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/base.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/grpc.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/grpc.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/rest.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/batch_controller/transports/rest.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/async_client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/async_client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/pagers.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/pagers.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/base.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/base.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/rest.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/cluster_controller/transports/rest.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/async_client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/async_client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/pagers.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/pagers.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/base.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/base.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/grpc.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/grpc.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/rest.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/job_controller/transports/rest.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/async_client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/async_client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/__init__.py`

 * *Files 8% similar despite different names*

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/base.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/base.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/rest.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/node_group_controller/transports/rest.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/async_client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/async_client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/client.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/client.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/pagers.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/pagers.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/base.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/base.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/rest.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/services/workflow_template_service/transports/rest.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/__init__.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/autoscaling_policies.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/autoscaling_policies.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/batches.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/batches.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/clusters.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/clusters.py`

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
@@ -1280,16 +1280,18 @@
 
 class KerberosConfig(proto.Message):
     r"""Specifies Kerberos related configuration.
 
     Attributes:
         enable_kerberos (bool):
             Optional. Flag to indicate whether to
-            Kerberize the cluster (default: false). Set this
-            field to true to enable Kerberos on a cluster.
+            Kerberize the cluster (default:
+
+            false). Set this field to true to enable
+            Kerberos on a cluster.
         root_principal_password_uri (str):
             Optional. The Cloud Storage URI of a KMS
             encrypted file containing the root principal
             password.
         kms_key_uri (str):
             Optional. The uri of the KMS key used to
             encrypt various sensitive files.
```

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/jobs.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/jobs.py`

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
@@ -60,16 +60,18 @@
     r"""The runtime logging config of the job.
 
     Attributes:
         driver_log_levels (MutableMapping[str, google.cloud.dataproc_v1.types.LoggingConfig.Level]):
             The per-package log levels for the driver.
             This may include "root" package name to
             configure rootLogger. Examples:
-              'com.google = FATAL', 'root = INFO',
-            'org.apache = DEBUG'
+
+            - 'com.google = FATAL'
+            - 'root = INFO'
+            - 'org.apache = DEBUG'
     """
 
     class Level(proto.Enum):
         r"""The Log4j level for job execution. When running an `Apache
         Hive <https://hive.apache.org/>`__ job, Cloud Dataproc configures
         the Hive client to an equivalent verbosity level.
 
@@ -125,14 +127,15 @@
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         main_jar_file_uri (str):
             The HCFS URI of the jar file containing the
             main class. Examples:
+
             'gs://foo-bucket/analytics-binaries/extract-useful-metrics-mr.jar'
             'hdfs:/tmp/test-samples/custom-wordcount.jar'
             'file:///home/usr/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar'
 
             This field is a member of `oneof`_ ``driver``.
         main_class (str):
             The name of the driver's main class. The jar file containing
@@ -152,21 +155,22 @@
             Optional. HCFS (Hadoop Compatible Filesystem)
             URIs of files to be copied to the working
             directory of Hadoop drivers and distributed
             tasks. Useful for naively parallel tasks.
         archive_uris (MutableSequence[str]):
             Optional. HCFS URIs of archives to be
             extracted in the working directory of Hadoop
-            drivers and tasks. Supported file types: .jar,
-            .tar, .tar.gz, .tgz, or .zip.
+            drivers and tasks. Supported file types:
+
+            .jar, .tar, .tar.gz, .tgz, or .zip.
         properties (MutableMapping[str, str]):
             Optional. A mapping of property names to values, used to
             configure Hadoop. Properties that conflict with values set
             by the Dataproc API may be overwritten. Can include
-            properties set in /etc/hadoop/conf/*-site and classes in
+            properties set in ``/etc/hadoop/conf/*-site`` and classes in
             user code.
         logging_config (google.cloud.dataproc_v1.types.LoggingConfig):
             Optional. The runtime log config for job
             execution.
     """
 
     main_jar_file_uri: str = proto.Field(
@@ -241,16 +245,17 @@
         file_uris (MutableSequence[str]):
             Optional. HCFS URIs of files to be placed in
             the working directory of each executor. Useful
             for naively parallel tasks.
         archive_uris (MutableSequence[str]):
             Optional. HCFS URIs of archives to be
             extracted into the working directory of each
-            executor. Supported file types: .jar, .tar,
-            .tar.gz, .tgz, and .zip.
+            executor. Supported file types:
+
+            .jar, .tar, .tar.gz, .tgz, and .zip.
         properties (MutableMapping[str, str]):
             Optional. A mapping of property names to
             values, used to configure Spark. Properties that
             conflict with values set by the Dataproc API may
             be overwritten. Can include properties set in
             /etc/spark/conf/spark-defaults.conf and classes
             in user code.
@@ -321,16 +326,17 @@
         file_uris (MutableSequence[str]):
             Optional. HCFS URIs of files to be placed in
             the working directory of each executor. Useful
             for naively parallel tasks.
         archive_uris (MutableSequence[str]):
             Optional. HCFS URIs of archives to be
             extracted into the working directory of each
-            executor. Supported file types: .jar, .tar,
-            .tar.gz, .tgz, and .zip.
+            executor. Supported file types:
+
+            .jar, .tar, .tar.gz, .tgz, and .zip.
         properties (MutableMapping[str, str]):
             Optional. A mapping of property names to
             values, used to configure PySpark. Properties
             that conflict with values set by the Dataproc
             API may be overwritten. Can include properties
             set in
             /etc/spark/conf/spark-defaults.conf and classes
@@ -434,15 +440,15 @@
         script_variables (MutableMapping[str, str]):
             Optional. Mapping of query variable names to values
             (equivalent to the Hive command: ``SET name="value";``).
         properties (MutableMapping[str, str]):
             Optional. A mapping of property names and values, used to
             configure Hive. Properties that conflict with values set by
             the Dataproc API may be overwritten. Can include properties
-            set in /etc/hadoop/conf/*-site.xml,
+            set in ``/etc/hadoop/conf/*-site.xml``,
             /etc/hive/conf/hive-site.xml, and classes in user code.
         jar_file_uris (MutableSequence[str]):
             Optional. HCFS URIs of jar files to add to
             the CLASSPATH of the Hive server and Hadoop
             MapReduce (MR) tasks. Can contain Hive SerDes
             and UDFs.
     """
@@ -576,15 +582,15 @@
         script_variables (MutableMapping[str, str]):
             Optional. Mapping of query variable names to values
             (equivalent to the Pig command: ``name=[value]``).
         properties (MutableMapping[str, str]):
             Optional. A mapping of property names to values, used to
             configure Pig. Properties that conflict with values set by
             the Dataproc API may be overwritten. Can include properties
-            set in /etc/hadoop/conf/*-site.xml,
+            set in ``/etc/hadoop/conf/*-site.xml``,
             /etc/pig/conf/pig.properties, and classes in user code.
         jar_file_uris (MutableSequence[str]):
             Optional. HCFS URIs of jar files to add to
             the CLASSPATH of the Pig Client and Hadoop
             MapReduce (MR) tasks. Can contain Pig UDFs.
         logging_config (google.cloud.dataproc_v1.types.LoggingConfig):
             Optional. The runtime log config for job
@@ -644,16 +650,17 @@
         file_uris (MutableSequence[str]):
             Optional. HCFS URIs of files to be placed in
             the working directory of each executor. Useful
             for naively parallel tasks.
         archive_uris (MutableSequence[str]):
             Optional. HCFS URIs of archives to be
             extracted into the working directory of each
-            executor. Supported file types: .jar, .tar,
-            .tar.gz, .tgz, and .zip.
+            executor. Supported file types:
+
+            .jar, .tar, .tar.gz, .tgz, and .zip.
         properties (MutableMapping[str, str]):
             Optional. A mapping of property names to
             values, used to configure SparkR. Properties
             that conflict with values set by the Dataproc
             API may be overwritten. Can include properties
             set in
             /etc/spark/conf/spark-defaults.conf and classes
```

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/node_groups.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/node_groups.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/operations.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/operations.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/shared.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/shared.py`

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

### Comparing `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/workflow_templates.py` & `google-cloud-dataproc-5.4.3/google/cloud/dataproc_v1/types/workflow_templates.py`

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
@@ -433,14 +433,15 @@
         number=10,
     )
 
 
 class TemplateParameter(proto.Message):
     r"""A configurable parameter that replaces one or more fields in
     the template. Parameterizable fields:
+
     - Labels
     - File uris
     - Job properties
     - Job arguments
     - Script variables
     - Main class (in HadoopJob and SparkJob)
     - Zone (in ClusterSelector)
```

### Comparing `google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/PKG-INFO` & `google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataproc
-Version: 5.4.2
+Version: 5.4.3
 Summary: Google Cloud Dataproc API client library
 Home-page: https://github.com/googleapis/python-dataproc
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Google Cloud Dataproc API.:  https://cloud.google.com/dataproc
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
+.. _samples/: https://github.com/googleapis/python-dataproc/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-dataproc
+    pip install google-cloud-dataproc
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-dataproc
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-dataproc
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Google Cloud Dataproc API
    to see other available methods on the client.
 -  Read the `Google Cloud Dataproc API Product documentation`_ to learn
```

### Comparing `google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/SOURCES.txt` & `google-cloud-dataproc-5.4.3/google_cloud_dataproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.2/setup.py` & `google-cloud-dataproc-5.4.3/setup.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/__init__.py` & `google-cloud-dataproc-5.4.3/tests/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/system/gapic/v1/test_system_cluster_controller_v1.py` & `google-cloud-dataproc-5.4.3/tests/system/gapic/v1/test_system_cluster_controller_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/__init__.py` & `google-cloud-dataproc-5.4.3/tests/unit/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/gapic/__init__.py` & `google-cloud-dataproc-5.4.3/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/__init__.py` & `google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/__init__.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_autoscaling_policy_service.py` & `google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_autoscaling_policy_service.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_batch_controller.py` & `google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_batch_controller.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_cluster_controller.py` & `google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_cluster_controller.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_job_controller.py` & `google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_job_controller.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_node_group_controller.py` & `google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_node_group_controller.py`

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

### Comparing `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_workflow_template_service.py` & `google-cloud-dataproc-5.4.3/tests/unit/gapic/dataproc_v1/test_workflow_template_service.py`

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

