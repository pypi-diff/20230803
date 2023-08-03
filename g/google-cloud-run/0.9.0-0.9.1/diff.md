# Comparing `tmp/google-cloud-run-0.9.0.tar.gz` & `tmp/google-cloud-run-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-run-0.9.0.tar", last modified: Thu Jul  6 22:15:55 2023, max compression
+gzip compressed data, was "google-cloud-run-0.9.1.tar", last modified: Thu Aug  3 14:34:42 2023, max compression
```

## Comparing `google-cloud-run-0.9.0.tar` & `google-cloud-run-0.9.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.302425 google-cloud-run-0.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4478 2023-07-06 22:15:55.302425 google-cloud-run-0.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3587 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.282423 google-cloud-run-0.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.282423 google-cloud-run-0.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.286424 google-cloud-run-0.9.0/google/cloud/run/
--rw-rw-r--   0 root         (0)     1003     4984 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.286424 google-cloud-run-0.9.0/google/cloud/run_v2/
--rw-rw-r--   0 root         (0)     1003     4323 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    11056 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.286424 google-cloud-run-0.9.0/google/cloud/run_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.290424 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/
--rw-rw-r--   0 root         (0)     1003      753 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/__init__.py
--rw-rw-r--   0 root         (0)     1003    32619 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/async_client.py
--rw-rw-r--   0 root         (0)     1003    44778 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/client.py
--rw-rw-r--   0 root         (0)     1003     5724 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.290424 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8120 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17896 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18214 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    38166 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.290424 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/
--rw-rw-r--   0 root         (0)     1003      729 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/__init__.py
--rw-rw-r--   0 root         (0)     1003    62838 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/async_client.py
--rw-rw-r--   0 root         (0)     1003    75369 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/client.py
--rw-rw-r--   0 root         (0)     1003     5454 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.290424 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/
--rw-rw-r--   0 root         (0)     1003     1260 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10638 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24322 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24783 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    74484 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.290424 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/
--rw-rw-r--   0 root         (0)     1003      749 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/__init__.py
--rw-rw-r--   0 root         (0)     1003    32630 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/async_client.py
--rw-rw-r--   0 root         (0)     1003    45650 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/client.py
--rw-rw-r--   0 root         (0)     1003     5679 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.294424 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/
--rw-rw-r--   0 root         (0)     1003     1330 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8080 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17882 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18199 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    38176 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.294424 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/
--rw-rw-r--   0 root         (0)     1003      745 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/__init__.py
--rw-rw-r--   0 root         (0)     1003    61155 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/async_client.py
--rw-rw-r--   0 root         (0)     1003    74285 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/client.py
--rw-rw-r--   0 root         (0)     1003     5634 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.294424 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11098 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23863 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24318 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    70807 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.294424 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/
--rw-rw-r--   0 root         (0)     1003      733 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/__init__.py
--rw-rw-r--   0 root         (0)     1003    27316 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/async_client.py
--rw-rw-r--   0 root         (0)     1003    40166 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/client.py
--rw-rw-r--   0 root         (0)     1003     5499 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.298425 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/
--rw-rw-r--   0 root         (0)     1003     1274 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7324 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15918 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16151 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    30136 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.298425 google-cloud-run-0.9.0/google/cloud/run_v2/types/
--rw-rw-r--   0 root         (0)     1003     3581 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10542 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/condition.py
--rw-rw-r--   0 root         (0)     1003    13565 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/execution.py
--rw-rw-r--   0 root         (0)     1003     4307 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/execution_template.py
--rw-rw-r--   0 root         (0)     1003    18011 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/job.py
--rw-rw-r--   0 root         (0)     1003    23222 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/k8s_min.py
--rw-rw-r--   0 root         (0)     1003    14333 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/revision.py
--rw-rw-r--   0 root         (0)     1003     6438 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/revision_template.py
--rw-rw-r--   0 root         (0)     1003    20322 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/service.py
--rw-rw-r--   0 root         (0)     1003    13995 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/task.py
--rw-rw-r--   0 root         (0)     1003     4207 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/task_template.py
--rw-rw-r--   0 root         (0)     1003     3750 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/traffic_target.py
--rw-rw-r--   0 root         (0)     1003     5608 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/google/cloud/run_v2/types/vendor_settings.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.302425 google-cloud-run-0.9.0/google_cloud_run.egg-info/
--rw-r--r--   0 root         (0)     1003     4478 2023-07-06 22:15:55.000000 google-cloud-run-0.9.0/google_cloud_run.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3882 2023-07-06 22:15:55.000000 google-cloud-run-0.9.0/google_cloud_run.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-06 22:15:55.000000 google-cloud-run-0.9.0/google_cloud_run.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-06 22:15:55.000000 google-cloud-run-0.9.0/google_cloud_run.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-06 22:15:55.000000 google-cloud-run-0.9.0/google_cloud_run.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-06 22:15:55.000000 google-cloud-run-0.9.0/google_cloud_run.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-06 22:15:55.000000 google-cloud-run-0.9.0/google_cloud_run.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-06 22:15:55.302425 google-cloud-run-0.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2952 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.302425 google-cloud-run-0.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.302425 google-cloud-run-0.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.302425 google-cloud-run-0.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 22:15:55.302425 google-cloud-run-0.9.0/tests/unit/gapic/run_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/unit/gapic/run_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   153449 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_executions.py
--rw-rw-r--   0 root         (0)     1003   261584 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_jobs.py
--rw-rw-r--   0 root         (0)     1003   150586 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_revisions.py
--rw-rw-r--   0 root         (0)     1003   247638 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_services.py
--rw-rw-r--   0 root         (0)     1003   131392 2023-07-06 22:14:00.000000 google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.675844 google-cloud-run-0.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4544 2023-08-03 14:34:42.675844 google-cloud-run-0.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3653 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.659846 google-cloud-run-0.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.659846 google-cloud-run-0.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.659846 google-cloud-run-0.9.1/google/cloud/run/
+-rw-rw-r--   0 root         (0)     1003     4984 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.663845 google-cloud-run-0.9.1/google/cloud/run_v2/
+-rw-rw-r--   0 root         (0)     1003     4323 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11056 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.663845 google-cloud-run-0.9.1/google/cloud/run_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.663845 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/
+-rw-rw-r--   0 root         (0)     1003      753 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32621 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44780 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/client.py
+-rw-rw-r--   0 root         (0)     1003     5724 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.663845 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8120 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17896 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18214 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    38166 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.663845 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/
+-rw-rw-r--   0 root         (0)     1003      729 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62098 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74629 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/client.py
+-rw-rw-r--   0 root         (0)     1003     5454 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.663845 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/
+-rw-rw-r--   0 root         (0)     1003     1260 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10638 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24322 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24783 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    74742 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.667845 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/
+-rw-rw-r--   0 root         (0)     1003      749 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32633 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    45653 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/client.py
+-rw-rw-r--   0 root         (0)     1003     5679 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.667845 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/
+-rw-rw-r--   0 root         (0)     1003     1330 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8080 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17882 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18199 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    38176 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.667845 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/
+-rw-rw-r--   0 root         (0)     1003      745 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60415 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/async_client.py
+-rw-rw-r--   0 root         (0)     1003    73545 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/client.py
+-rw-rw-r--   0 root         (0)     1003     5634 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.667845 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11098 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23863 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24318 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    71065 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.667845 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/
+-rw-rw-r--   0 root         (0)     1003      733 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27318 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40168 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/client.py
+-rw-rw-r--   0 root         (0)     1003     5499 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.671844 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/
+-rw-rw-r--   0 root         (0)     1003     1274 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7324 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15918 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16151 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    30136 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.671844 google-cloud-run-0.9.1/google/cloud/run_v2/types/
+-rw-rw-r--   0 root         (0)     1003     3581 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10542 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/condition.py
+-rw-rw-r--   0 root         (0)     1003    13567 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/execution.py
+-rw-rw-r--   0 root         (0)     1003     4307 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/execution_template.py
+-rw-rw-r--   0 root         (0)     1003    18012 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/job.py
+-rw-rw-r--   0 root         (0)     1003    23223 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/k8s_min.py
+-rw-rw-r--   0 root         (0)     1003    14336 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/revision.py
+-rw-rw-r--   0 root         (0)     1003     6438 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/revision_template.py
+-rw-rw-r--   0 root         (0)     1003    20322 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/service.py
+-rw-rw-r--   0 root         (0)     1003    13997 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/task.py
+-rw-rw-r--   0 root         (0)     1003     4207 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/task_template.py
+-rw-rw-r--   0 root         (0)     1003     3750 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/traffic_target.py
+-rw-rw-r--   0 root         (0)     1003     5608 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/google/cloud/run_v2/types/vendor_settings.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.671844 google-cloud-run-0.9.1/google_cloud_run.egg-info/
+-rw-r--r--   0 root         (0)     1003     4544 2023-08-03 14:34:42.000000 google-cloud-run-0.9.1/google_cloud_run.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3882 2023-08-03 14:34:42.000000 google-cloud-run-0.9.1/google_cloud_run.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 14:34:42.000000 google-cloud-run-0.9.1/google_cloud_run.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 14:34:42.000000 google-cloud-run-0.9.1/google_cloud_run.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 14:34:42.000000 google-cloud-run-0.9.1/google_cloud_run.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-08-03 14:34:42.000000 google-cloud-run-0.9.1/google_cloud_run.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 14:34:42.000000 google-cloud-run-0.9.1/google_cloud_run.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-03 14:34:42.675844 google-cloud-run-0.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2952 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.671844 google-cloud-run-0.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.671844 google-cloud-run-0.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.671844 google-cloud-run-0.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 14:34:42.675844 google-cloud-run-0.9.1/tests/unit/gapic/run_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/unit/gapic/run_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   153449 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_executions.py
+-rw-rw-r--   0 root         (0)     1003   261584 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_jobs.py
+-rw-rw-r--   0 root         (0)     1003   150586 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_revisions.py
+-rw-rw-r--   0 root         (0)     1003   247638 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_services.py
+-rw-rw-r--   0 root         (0)     1003   131392 2023-08-03 14:32:52.000000 google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_tasks.py
```

### Comparing `google-cloud-run-0.9.0/LICENSE` & `google-cloud-run-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.9.0/MANIFEST.in` & `google-cloud-run-0.9.1/MANIFEST.in`

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

### Comparing `google-cloud-run-0.9.0/PKG-INFO` & `google-cloud-run-0.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-run
-Version: 0.9.0
+Version: 0.9.1
 Summary: Google Cloud Run API client library
 Home-page: https://github.com/googleapis/python-run
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Cloud Run API.:  https://cloud.google.com/run/docs
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
+.. _samples/: https://github.com/googleapis/python-run/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-run
+    pip install google-cloud-run
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-run
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-run
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Cloud Run API
    to see other available methods on the client.
 -  Read the `Cloud Run API Product documentation`_ to learn
```

### Comparing `google-cloud-run-0.9.0/README.rst` & `google-cloud-run-0.9.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Cloud Run API.:  https://cloud.google.com/run/docs
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
+.. _samples/: https://github.com/googleapis/python-run/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-run
+    pip install google-cloud-run
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-run
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-run
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Cloud Run API
    to see other available methods on the client.
 -  Read the `Cloud Run API Product documentation`_ to learn
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run/gapic_version.py` & `google-cloud-run-0.9.1/google/cloud/run/gapic_version.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/gapic_metadata.json` & `google-cloud-run-0.9.1/google/cloud/run_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/gapic_version.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/gapic_version.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/async_client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/async_client.py`

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
@@ -265,14 +265,15 @@
         Args:
             request (Optional[Union[google.cloud.run_v2.types.GetExecutionRequest, dict]]):
                 The request object. Request message for obtaining a
                 Execution by its full name.
             name (:class:`str`):
                 Required. The full name of the
                 Execution. Format:
+
                 projects/{project}/locations/{location}/jobs/{job}/executions/{execution},
                 where {project} can be project id or
                 number.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -497,14 +498,15 @@
         Args:
             request (Optional[Union[google.cloud.run_v2.types.DeleteExecutionRequest, dict]]):
                 The request object. Request message for deleting an
                 Execution.
             name (:class:`str`):
                 Required. The name of the Execution
                 to delete. Format:
+
                 projects/{project}/locations/{location}/jobs/{job}/executions/{execution},
                 where {project} can be project id or
                 number.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/client.py`

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
@@ -597,14 +597,15 @@
         Args:
             request (Union[google.cloud.run_v2.types.GetExecutionRequest, dict]):
                 The request object. Request message for obtaining a
                 Execution by its full name.
             name (str):
                 Required. The full name of the
                 Execution. Format:
+
                 projects/{project}/locations/{location}/jobs/{job}/executions/{execution},
                 where {project} can be project id or
                 number.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -829,14 +830,15 @@
         Args:
             request (Union[google.cloud.run_v2.types.DeleteExecutionRequest, dict]):
                 The request object. Request message for deleting an
                 Execution.
             name (str):
                 Required. The name of the Execution
                 to delete. Format:
+
                 projects/{project}/locations/{location}/jobs/{job}/executions/{execution},
                 where {project} can be project id or
                 number.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/pagers.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/pagers.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/base.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/base.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/grpc.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/grpc.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/executions/transports/rest.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/executions/transports/rest.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/__init__.py` & `google-cloud-run-0.9.1/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,15 @@
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
-from .async_client import JobsAsyncClient
-from .client import JobsClient
-
-__all__ = (
-    "JobsClient",
-    "JobsAsyncClient",
-)
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/async_client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/async_client.py`

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
@@ -1014,50 +1014,19 @@
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
@@ -1157,50 +1126,19 @@
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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/client.py`

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
@@ -1350,50 +1350,19 @@
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
@@ -1492,50 +1461,19 @@
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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/pagers.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/pagers.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/__init__.py`

 * *Files 3% similar despite different names*

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/base.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/base.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/grpc.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/grpc.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/jobs/transports/rest.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/transports/rest.py`

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
@@ -823,62 +823,62 @@
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
@@ -1260,62 +1260,62 @@
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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/async_client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/async_client.py`

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
@@ -266,14 +266,15 @@
         Args:
             request (Optional[Union[google.cloud.run_v2.types.GetRevisionRequest, dict]]):
                 The request object. Request message for obtaining a
                 Revision by its full name.
             name (:class:`str`):
                 Required. The full name of the
                 Revision. Format:
+
                 projects/{project}/locations/{location}/services/{service}/revisions/{revision}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -376,14 +377,15 @@
                 The request object. Request message for retrieving a list
                 of Revisions.
             parent (:class:`str`):
                 Required. The Service from which the
                 Revisions should be listed. To list all
                 Revisions across Services, use "-"
                 instead of Service name. Format:
+
                 projects/{project}/locations/{location}/services/{service}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -498,14 +500,15 @@
                 retired Revision. Revision lifecycle is
                 usually managed by making changes to the
                 parent Service. Only retired revisions
                 can be deleted with this API.
             name (:class:`str`):
                 Required. The name of the Revision to
                 delete. Format:
+
                 projects/{project}/locations/{location}/services/{service}/revisions/{revision}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/client.py`

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
@@ -598,14 +598,15 @@
         Args:
             request (Union[google.cloud.run_v2.types.GetRevisionRequest, dict]):
                 The request object. Request message for obtaining a
                 Revision by its full name.
             name (str):
                 Required. The full name of the
                 Revision. Format:
+
                 projects/{project}/locations/{location}/services/{service}/revisions/{revision}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -716,14 +717,15 @@
                 The request object. Request message for retrieving a list
                 of Revisions.
             parent (str):
                 Required. The Service from which the
                 Revisions should be listed. To list all
                 Revisions across Services, use "-"
                 instead of Service name. Format:
+
                 projects/{project}/locations/{location}/services/{service}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -846,14 +848,15 @@
                 retired Revision. Revision lifecycle is
                 usually managed by making changes to the
                 parent Service. Only retired revisions
                 can be deleted with this API.
             name (str):
                 Required. The name of the Revision to
                 delete. Format:
+
                 projects/{project}/locations/{location}/services/{service}/revisions/{revision}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/pagers.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/pagers.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/base.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/base.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/grpc.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/grpc.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/revisions/transports/rest.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/revisions/transports/rest.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/async_client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/async_client.py`

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
@@ -941,50 +941,19 @@
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
@@ -1084,50 +1053,19 @@
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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/client.py`

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
@@ -1295,50 +1295,19 @@
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
@@ -1437,50 +1406,19 @@
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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/pagers.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/pagers.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/__init__.py`

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
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/base.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/base.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/grpc.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/grpc.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/grpc_asyncio.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/services/transports/rest.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/services/transports/rest.py`

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
@@ -801,62 +801,62 @@
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
@@ -1147,62 +1147,62 @@
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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/async_client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/async_client.py`

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
@@ -261,14 +261,15 @@
         Args:
             request (Optional[Union[google.cloud.run_v2.types.GetTaskRequest, dict]]):
                 The request object. Request message for obtaining a Task
                 by its full name.
             name (:class:`str`):
                 Required. The full name of the Task.
                 Format:
+
                 projects/{project}/locations/{location}/jobs/{job}/executions/{execution}/tasks/{task}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -369,14 +370,15 @@
             parent (:class:`str`):
                 Required. The Execution from which
                 the Tasks should be listed. To list all
                 Tasks across Executions of a Job, use
                 "-" instead of Execution name. To list
                 all Tasks across Jobs, use "-" instead
                 of Job name. Format:
+
                 projects/{project}/locations/{location}/jobs/{job}/executions/{execution}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/client.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/client.py`

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
@@ -621,14 +621,15 @@
         Args:
             request (Union[google.cloud.run_v2.types.GetTaskRequest, dict]):
                 The request object. Request message for obtaining a Task
                 by its full name.
             name (str):
                 Required. The full name of the Task.
                 Format:
+
                 projects/{project}/locations/{location}/jobs/{job}/executions/{execution}/tasks/{task}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -729,14 +730,15 @@
             parent (str):
                 Required. The Execution from which
                 the Tasks should be listed. To list all
                 Tasks across Executions of a Job, use
                 "-" instead of Execution name. To list
                 all Tasks across Jobs, use "-" instead
                 of Job name. Format:
+
                 projects/{project}/locations/{location}/jobs/{job}/executions/{execution}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/pagers.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/pagers.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/base.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/base.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/grpc.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/grpc.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/services/tasks/transports/rest.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/tasks/transports/rest.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/condition.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/condition.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/execution.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/execution.py`

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
@@ -38,14 +38,15 @@
 class GetExecutionRequest(proto.Message):
     r"""Request message for obtaining a Execution by its full name.
 
     Attributes:
         name (str):
             Required. The full name of the Execution.
             Format:
+
             projects/{project}/locations/{location}/jobs/{job}/executions/{execution},
             where {project} can be project id or number.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
@@ -121,14 +122,15 @@
 class DeleteExecutionRequest(proto.Message):
     r"""Request message for deleting an Execution.
 
     Attributes:
         name (str):
             Required. The name of the Execution to
             delete. Format:
+
             projects/{project}/locations/{location}/jobs/{job}/executions/{execution},
             where {project} can be project id or number.
         validate_only (bool):
             Indicates that the request should be
             validated without actually deleting any
             resources.
         etag (str):
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/execution_template.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/execution_template.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/job.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/job.py`

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
@@ -263,14 +263,15 @@
     r"""Job represents the configuration of a single job, which
     references a container image that is run to completion.
 
     Attributes:
         name (str):
             The fully qualified name of this Job.
             Format:
+
             projects/{project}/locations/{location}/jobs/{job}
         uid (str):
             Output only. Server assigned unique
             identifier for the Execution. The value is a
             UUID4 string and guaranteed to remain unchanged
             until the resource is deleted.
         generation (int):
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/k8s_min.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/k8s_min.py`

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
@@ -501,14 +501,15 @@
             The Cloud SQL instance connection names, as
             can be found in
             https://console.cloud.google.com/sql/instances.
             Visit
             https://cloud.google.com/sql/docs/mysql/connect-run
             for more information on how to connect Cloud SQL
             and Cloud Run. Format:
+
             {project}:{location}:{instance}
     """
 
     instances: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/revision.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/revision.py`

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
@@ -39,14 +39,15 @@
 class GetRevisionRequest(proto.Message):
     r"""Request message for obtaining a Revision by its full name.
 
     Attributes:
         name (str):
             Required. The full name of the Revision.
             Format:
+
             projects/{project}/locations/{location}/services/{service}/revisions/{revision}
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
@@ -57,14 +58,15 @@
 
     Attributes:
         parent (str):
             Required. The Service from which the
             Revisions should be listed. To list all
             Revisions across Services, use "-" instead of
             Service name. Format:
+
             projects/{project}/locations/{location}/services/{service}
         page_size (int):
             Maximum number of revisions to return in this
             call.
         page_token (str):
             A page token received from a previous call to
             ListRevisions. All other parameters must match.
@@ -123,14 +125,15 @@
     parent Service. Only retired revisions can be deleted with this
     API.
 
     Attributes:
         name (str):
             Required. The name of the Revision to delete.
             Format:
+
             projects/{project}/locations/{location}/services/{service}/revisions/{revision}
         validate_only (bool):
             Indicates that the request should be
             validated without actually deleting any
             resources.
         etag (str):
             A system-generated fingerprint for this
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/revision_template.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/revision_template.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/service.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/service.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/task.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/task.py`

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
@@ -39,14 +39,15 @@
 class GetTaskRequest(proto.Message):
     r"""Request message for obtaining a Task by its full name.
 
     Attributes:
         name (str):
             Required. The full name of the Task.
             Format:
+
             projects/{project}/locations/{location}/jobs/{job}/executions/{execution}/tasks/{task}
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
@@ -58,14 +59,15 @@
     Attributes:
         parent (str):
             Required. The Execution from which the Tasks
             should be listed. To list all Tasks across
             Executions of a Job, use "-" instead of
             Execution name. To list all Tasks across Jobs,
             use "-" instead of Job name. Format:
+
             projects/{project}/locations/{location}/jobs/{job}/executions/{execution}
         page_size (int):
             Maximum number of Tasks to return in this
             call.
         page_token (str):
             A page token received from a previous call to
             ListTasks. All other parameters must match.
```

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/task_template.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/task_template.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/traffic_target.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/traffic_target.py`

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

### Comparing `google-cloud-run-0.9.0/google/cloud/run_v2/types/vendor_settings.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/types/vendor_settings.py`

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

### Comparing `google-cloud-run-0.9.0/google_cloud_run.egg-info/PKG-INFO` & `google-cloud-run-0.9.1/google_cloud_run.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-run
-Version: 0.9.0
+Version: 0.9.1
 Summary: Google Cloud Run API client library
 Home-page: https://github.com/googleapis/python-run
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Cloud Run API.:  https://cloud.google.com/run/docs
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
+.. _samples/: https://github.com/googleapis/python-run/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-run
+    pip install google-cloud-run
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-run
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-run
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Cloud Run API
    to see other available methods on the client.
 -  Read the `Cloud Run API Product documentation`_ to learn
```

### Comparing `google-cloud-run-0.9.0/google_cloud_run.egg-info/SOURCES.txt` & `google-cloud-run-0.9.1/google_cloud_run.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.9.0/setup.py` & `google-cloud-run-0.9.1/setup.py`

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

### Comparing `google-cloud-run-0.9.0/tests/__init__.py` & `google-cloud-run-0.9.1/tests/unit/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/tests/unit/__init__.py` & `google-cloud-run-0.9.1/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/tests/unit/gapic/__init__.py` & `google-cloud-run-0.9.1/tests/unit/gapic/run_v2/__init__.py`

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

### Comparing `google-cloud-run-0.9.0/tests/unit/gapic/run_v2/__init__.py` & `google-cloud-run-0.9.1/google/cloud/run_v2/services/jobs/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,22 @@
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
+from .async_client import JobsAsyncClient
+from .client import JobsClient
+
+__all__ = (
+    "JobsClient",
+    "JobsAsyncClient",
+)
```

### Comparing `google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_executions.py` & `google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_executions.py`

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

### Comparing `google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_jobs.py` & `google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_jobs.py`

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

### Comparing `google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_revisions.py` & `google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_revisions.py`

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

### Comparing `google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_services.py` & `google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_services.py`

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

### Comparing `google-cloud-run-0.9.0/tests/unit/gapic/run_v2/test_tasks.py` & `google-cloud-run-0.9.1/tests/unit/gapic/run_v2/test_tasks.py`

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

