# Comparing `tmp/runpod-0.9.9.tar.gz` & `tmp/runpod-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpod-0.9.9.tar", last modified: Thu May 25 13:27:12 2023, max compression
+gzip compressed data, was "runpod-1.0.0.tar", last modified: Thu Aug  3 15:29:55 2023, max compression
```

## Comparing `runpod-0.9.9.tar` & `runpod-1.0.0.tar`

### file list

```diff
@@ -1,89 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.783007 runpod-0.9.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.775006 runpod-0.9.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-25 13:27:01.000000 runpod-0.9.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.775006 runpod-0.9.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-25 13:27:01.000000 runpod-0.9.9/.github/workflows/CD_publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-25 13:27:01.000000 runpod-0.9.9/.github/workflows/CI_codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-25 13:27:01.000000 runpod-0.9.9/.github/workflows/CI_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-25 13:27:01.000000 runpod-0.9.9/.github/workflows/ci_pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-25 13:27:01.000000 runpod-0.9.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-25 13:27:01.000000 runpod-0.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-25 13:27:12.783007 runpod-0.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-25 13:27:01.000000 runpod-0.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.771006 runpod-0.9.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.775006 runpod-0.9.9/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/api/quries.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.775006 runpod-0.9.9/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/images/env_var_location.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.775006 runpod-0.9.9/docs/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/serverless/local_testing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.775006 runpod-0.9.9/docs/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/serverless/utils/rp_cleanup.md
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/serverless/utils/rp_download.md
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/serverless/utils/rp_upload.md
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/serverless/utils/rp_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/serverless/worker.md
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 13:27:01.000000 runpod-0.9.9/docs/serverless/worker_realtime.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.775006 runpod-0.9.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-25 13:27:01.000000 runpod-0.9.9/examples/call_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-25 13:27:01.000000 runpod-0.9.9/examples/call_endpoint_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 13:27:01.000000 runpod-0.9.9/examples/graphql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-25 13:27:01.000000 runpod-0.9.9/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-25 13:27:01.000000 runpod-0.9.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 13:27:01.000000 runpod-0.9.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.775006 runpod-0.9.9/runpod/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod/api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/api_wrapper/ctl_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/api_wrapper/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod/api_wrapper/mutations/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/api_wrapper/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/api_wrapper/mutations/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod/api_wrapper/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/api_wrapper/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/api_wrapper/queries/gpus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod/endpoint/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/endpoint/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/endpoint/asyncio/asyncio_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/endpoint/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod/serverless/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/modules/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/modules/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/modules/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/modules/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/modules/rp_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/modules/rp_tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/modules/worker_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/utils/rp_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/utils/rp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/utils/rp_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/utils/rp_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-25 13:27:01.000000 runpod-0.9.9/runpod/serverless/work_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.779007 runpod-0.9.9/runpod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-25 13:27:12.000000 runpod-0.9.9/runpod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-25 13:27:12.000000 runpod-0.9.9/runpod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:27:12.000000 runpod-0.9.9/runpod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 13:27:12.000000 runpod-0.9.9/runpod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 13:27:12.000000 runpod-0.9.9/runpod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-25 13:27:12.783007 runpod-0.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-25 13:27:01.000000 runpod-0.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.783007 runpod-0.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.783007 runpod-0.9.9/tests/test_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/test_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/test_endpoint/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:27:12.783007 runpod-0.9.9/tests/test_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/test_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/test_serverless/test_module_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/test_serverless/test_pod_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/test_serverless/test_util_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/test_whatever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-25 13:27:01.000000 runpod-0.9.9/tests/whatever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.706942 runpod-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.694942 runpod-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.694942 runpod-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-03 15:29:22.000000 runpod-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-03 15:29:22.000000 runpod-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-03 15:29:22.000000 runpod-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.694942 runpod-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-03 15:29:22.000000 runpod-1.0.0/.github/workflows/CD-publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-03 15:29:22.000000 runpod-1.0.0/.github/workflows/CD-test_publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-03 15:29:22.000000 runpod-1.0.0/.github/workflows/CI-codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 15:29:22.000000 runpod-1.0.0/.github/workflows/CI-pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 15:29:22.000000 runpod-1.0.0/.github/workflows/CI-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-03 15:29:22.000000 runpod-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-03 15:29:22.000000 runpod-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 15:29:22.000000 runpod-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-03 15:29:55.710942 runpod-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-03 15:29:22.000000 runpod-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 15:29:22.000000 runpod-1.0.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.690941 runpod-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.694942 runpod-1.0.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/api/quries.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.694942 runpod-1.0.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/images/env_var_location.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.694942 runpod-1.0.0/docs/serverless/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.694942 runpod-1.0.0/docs/serverless/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/functions/error_handling.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/functions/logging.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/local_testing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/docs/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/utils/rp_cleanup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/utils/rp_debugger.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/utils/rp_download.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/utils/rp_upload.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/utils/rp_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/worker.md
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-03 15:29:22.000000 runpod-1.0.0/docs/serverless/worker_realtime.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-03 15:29:22.000000 runpod-1.0.0/examples/call_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-03 15:29:22.000000 runpod-1.0.0/examples/call_endpoint_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-03 15:29:22.000000 runpod-1.0.0/examples/graphql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 15:29:22.000000 runpod-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 15:29:22.000000 runpod-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/runpod/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/runpod/api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/api_wrapper/ctl_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/api_wrapper/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/runpod/api_wrapper/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/api_wrapper/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/api_wrapper/mutations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/runpod/api_wrapper/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/api_wrapper/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/api_wrapper/queries/gpus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/runpod/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/cli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/runpod/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.702942 runpod-1.0.0/runpod/endpoint/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/endpoint/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/endpoint/asyncio/asyncio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/endpoint/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.702942 runpod-1.0.0/runpod/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.702942 runpod-1.0.0/runpod/serverless/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/rp_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/rp_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/rp_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/rp_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/rp_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/rp_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/rp_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/rp_tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/modules/worker_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.702942 runpod-1.0.0/runpod/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/utils/rp_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/utils/rp_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/utils/rp_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/utils/rp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/utils/rp_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/utils/rp_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-08-03 15:29:22.000000 runpod-1.0.0/runpod/serverless/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.698942 runpod-1.0.0/runpod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-03 15:29:55.000000 runpod-1.0.0/runpod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-03 15:29:55.000000 runpod-1.0.0/runpod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:29:55.000000 runpod-1.0.0/runpod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 15:29:55.000000 runpod-1.0.0/runpod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-03 15:29:55.000000 runpod-1.0.0/runpod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 15:29:55.000000 runpod-1.0.0/runpod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-03 15:29:55.710942 runpod-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-03 15:29:22.000000 runpod-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.702942 runpod-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.702942 runpod-1.0.0/tests/test_api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_api_wrapper/test_ctl_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_api_wrapper/test_mutations_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.702942 runpod-1.0.0/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_cli/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.706942 runpod-1.0.0/tests/test_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_endpoint/test_asyncio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_endpoint/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.706942 runpod-1.0.0/tests/test_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.706942 runpod-1.0.0/tests/test_serverless/test_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_modules/test_tips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:29:55.706942 runpod-1.0.0/tests/test_serverless/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_utils/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_utils/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_utils/test_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_utils/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_utils/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_utils/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_serverless/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/test_whatever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-03 15:29:22.000000 runpod-1.0.0/tests/whatever.py
```

### Comparing `runpod-0.9.9/.github/workflows/CD_publish-to-pypi.yml` & `runpod-1.0.0/.github/workflows/CD-test_publish_to_pypi.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-name: CD | Publish Python 🐍 distributions 📦 to PyPI and TestPyPI
+name: CD | Test Publish Python 🐍 distributions 📦 to TestPyPI
 
 on:
-  release:
-    types: [published]
+  push:
+    branches:
+      - "staging"
 
   workflow_dispatch:
 
 jobs:
   build-n-publish:
-    name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
+    name: Build and publish Python 🐍 distributions 📦 to TestPyPI
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
-      - name: Set up Python 3.9
-        uses: actions/setup-python@v4.3.1
+      - name: Set up Python 3.11.0
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.9
+          python-version: 3.11.0
 
       - name: Install pypa/build
         run: >-
           python -m
           pip install
           build
           --user
@@ -35,13 +36,7 @@
           .
 
       - name: Publish distribution 📦 to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
-
-      - name: Publish distribution 📦 to PyPI
-        # if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `runpod-0.9.9/.github/workflows/CI_codeql.yml` & `runpod-1.0.0/.github/workflows/CI-codeql.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/.github/workflows/ci_pylint.yml` & `runpod-1.0.0/.github/workflows/CI-pylint.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 name: CI | Code Quality
 
 on:
   push:
     branches-ignore:
-      - "master-ci"
+      - "main-ci"
       - "release"
   pull_request:
     branches:
-      - master
+      - main
 
   workflow_dispatch:
-    name: Run code quality checks manually
 
 jobs:
   lint:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up Python 3.11
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.11.0
 
       - name: Install Dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
           pip install pylint
+          pip install pytest
 
       - name: Pylint Source
         run: |
           find . -type f -name '*.py' | xargs pylint --extension-pkg-whitelist='pydantic'
```

### Comparing `runpod-0.9.9/.gitignore` & `runpod-1.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 env
 .env
+.env310
 .vscode
 test_wrapper.py
+test_logging.py
+/ignore
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `runpod-0.9.9/LICENSE` & `runpod-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/PKG-INFO` & `runpod-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,62 @@
-Metadata-Version: 2.1
-Name: runpod
-Version: 0.9.9
-Summary: Official Python library for RunPod API & SDK.
-Home-page: https://github.com/runpod/runpod-python
-Author: RunPod
-Author-email: support@runpod.io
-License: MIT
-Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
-Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <div align="center">
 <h1>RunPod | Python Library </h1>
 
-[![CI | Code Quality](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml)
+[![PyPI Package](https://badge.fury.io/py/runpod.svg)](https://badge.fury.io/py/runpod)
+&nbsp;
+[![Downloads](https://static.pepy.tech/personalized-badge/runpod?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/runpod)
+
+[![CI | Code Quality](https://github.com/runpod/runpod-python/actions/workflows/CI-pylint.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI-pylint.yml)
+&nbsp;
+[![CI | Unit Tests](https://github.com/runpod/runpod-python/actions/workflows/CI-tests.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI-tests.yml)
 &nbsp;
-[![CI | Unit Tests](https://github.com/runpod/runpod-python/actions/workflows/CI_tests.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI_tests.yml)
+[![CI | CodeQL](https://github.com/runpod/runpod-python/actions/workflows/CI-codeql.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI-codeql.yml)
 
 </div>
 
-Official Python library for RunPod API &amp; SDK.
+Welcome to the official Python library for RunPod API &amp; SDK.
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
-- [Installation](#installation)
-- [SDK - Serverless Worker](#sdk---serverless-worker)
+- [💻 | Installation](#--installation)
+- [⚡ | Serverless Worker (SDK)](#--serverless-worker-sdk)
   - [Quick Start](#quick-start)
-- [API Language Library](#api-language-library)
+  - [Local Test Worker](#local-test-worker)
+- [📚 | API Language Library (GraphQL Wrapper)](#--api-language-library-graphql-wrapper)
   - [Endpoints](#endpoints)
-  - [GPU Pod Control](#gpu-pod-control)
-- [Directory](#directory)
-- [Community and Contributing](#community-and-contributing)
+  - [GPU Cloud (Pods)](#gpu-cloud-pods)
+- [📁 | Directory](#--directory)
+- [🤝 | Community and Contributing](#--community-and-contributing)
 
-## Installation
+## 💻 | Installation
 
 ```bash
+# Install the latest release version
 pip install runpod
+
+# or
+
+# Install the latest development version (main branch)
+pip install git+https://github.com/runpod/runpod-python.git
 ```
 
-## SDK - Serverless Worker
+*Python 3.10 or higher is required to use the latest version of this package.*
+
+## ⚡ | Serverless Worker (SDK)
 
 This python package can also be used to create a serverless worker that can be deployed to RunPod as a custom endpoint API.
 
 ### Quick Start
 
 Create an python script in your project that contains your model definition and the RunPod worker start code. Run this python code as your default container start command:
 
 ```python
+# my_worker.py
+
 import runpod
 
 def is_even(job):
 
     job_input = job["input"]
     the_number = job_input["number"]
 
@@ -77,15 +71,23 @@
 runpod.serverless.start({"handler": is_even})
 ```
 
 Make sure that this file is ran when your container starts. This can be accomplished by calling it in the docker command when you setup a template at [runpod.io/console/serverless/user/templates](https://www.runpod.io/console/serverless/user/templates) or by setting it as the default command in your Dockerfile.
 
 See our [blog post](https://www.runpod.io/blog/serverless-create-a-basic-api) for creating a basic Serverless API, or view the [details docs](https://docs.runpod.io/serverless-ai/custom-apis) for more information.
 
-## API Language Library
+### Local Test Worker
+
+You can also test your worker locally before deploying it to RunPod. This is useful for debugging and testing.
+
+```bash
+python my_worker.py --rp_serve_api
+```
+
+## 📚 | API Language Library (GraphQL Wrapper)
 
 When interacting with the RunPod API you can use this library to make requests to the API.
 
 ```python
 import runpod
 
 runpod.api_key = "your_runpod_api_key_found_under_settings"
@@ -116,15 +118,15 @@
     {"your_model_input_key": "your_model_input_value"}
 )
 
 # Returns the job results if completed within 90 seconds, otherwise, returns the job status.
 print(run_request )
 ```
 
-### GPU Pod Control
+### GPU Cloud (Pods)
 
 ```python
 import runpod
 
 runpod.api_key = "your_runpod_api_key_found_under_settings"
 
 # Create a pod
@@ -136,26 +138,29 @@
 # Start the pod
 runpod.start_pod(pod.id)
 
 # Terminate the pod
 runpod.terminate_pod(pod.id)
 ```
 
-## Directory
+## 📁 | Directory
 
 ```BASH
 .
 ├── docs               # Documentation
+├── examples           # Examples
 ├── runpod             # Package source code
+│   ├── api_wrapper    # Language library - API (GraphQL)
+│   ├── cli            # Command Line Interface Functions
 │   ├── endpoint       # Language library - Endpoints
 │   └── serverless     # SDK - Serverless Worker
 └── tests              # Package tests
 ```
 
-## Community and Contributing
+## 🤝 | Community and Contributing
 
 We welcome both pull requests and issues on [GitHub](https://github.com/runpod/runpod-python). Bug fixes and new features are encouraged.
 
 <div align="center">
 
 <a target="_blank" href="https://discord.gg/pJ3P2DbUUq">![Discord Banner 2](https://discordapp.com/api/guilds/912829806415085598/widget.png?style=banner2)</a>
```

### Comparing `runpod-0.9.9/docs/api/quries.md` & `runpod-1.0.0/docs/api/quries.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/docs/images/env_var_location.png` & `runpod-1.0.0/docs/images/env_var_location.png`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/docs/serverless/local_testing.md` & `runpod-1.0.0/docs/serverless/local_testing.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/docs/serverless/utils/rp_download.md` & `runpod-1.0.0/docs/serverless/utils/rp_download.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/docs/serverless/utils/rp_upload.md` & `runpod-1.0.0/docs/serverless/utils/rp_upload.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/docs/serverless/utils/rp_validator.md` & `runpod-1.0.0/docs/serverless/utils/rp_validator.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - `default` (defaults `None`) - A default value to use if the input is not provided.
 - `type` (required) - The type of the input
 - `constraints` (optional) - A lambda function that takes in the input and returns true or false
 
 ## Example Usage
 
 ```python
-from runpod.serverless.utils.validator import validate
+from runpod.serverless.utils.rp_validator import validate
 
 # Define the schema for the expected inputs
 schema = {
     "input1": {
         "type": str,    # expected type
         "required": True,    # is input required
     },
```

### Comparing `runpod-0.9.9/docs/serverless/worker.md` & `runpod-1.0.0/docs/serverless/worker.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # The Serverless Worker
 
-## Logging
+Both RunPod official endpoints as well as custom built endpoints function by means of a worker that fetches available jobs, passes them into a handler and then returns the output.
 
-The worker outputs logs to the console at different points in the workers lifecycle. These logs can be used to debug issues with the worker or handler. There are four logging levels that can be used to control the verbosity of the logs:
+A worker entry point is a python file containing the command `runpod.serverless.start(config)`. An minimal worker file is shown below:
 
-   1. `DEBUG` (Default) - Outputs all logs, including debug logs.
-
-   2. `INFO` - Outputs all logs except debug logs.
-
-   3. `WARNING` - Outputs only warning and error logs.
+```python
+import runpod
 
-   4. `ERROR` - Outputs only error logs.
+def handler(job):
+    # Handle the job and return the output
+    return {"output": "Job completed successfully"}
 
-To set the logging level, set the `RUNPOD_DEBUG_LEVEL` environment variable to one of the above logging levels. For example, to set the logging level to `INFO`, set the `RUNPOD_DEBUG_LEVEL` environment variable to `INFO`.
+runpod.serverless.start({"handler": handler})
+```
 
-## Error Handling
+## config
 
-The worker is designed to handle errors raised by the handler gracefully. If the handler raises an error, the worker will capture this error and return it as the job output along with the stack trace.
+The `config` parameter is a dictionary containing the following keys:
 
-If you want to return a custom error within the handler, this can be accomplished by returning a dictionary with a top-level key of `error` and a value of the error message. The worker will then return this error message as the job output.
+| Key       | Type       | Description                                                  |
+|-----------|------------|--------------------------------------------------------------|
+| `handler` | `function` | The handler function that will be called with the job input. |
 
-### Example
+### handler
 
-```python
-def handler_with_custom_error(job):
-    if job["id"] == "invalid_job":
-        return {"error": "Invalid job ID"}
-    else:
-        # Handle the job and return the output
-        return {"output": "Job completed successfully"}
-```
+The handler function can either had a standard return or be a generator function. If the handler is a generator function, it will be called with the job input and the generator will be iterated over until it is exhausted.
 
 ## Worker Refresh
 
 For more complex operations where you are downloading files or making changes to the worker, it can be beneficial to refresh the worker between jobs. This can be accomplished by enabling a `refresh_worker` worker flag in one of two ways:
 
    1. Enable on start with `runpod.serverless.start({"handler": handler, "refresh_worker": True})`, this will refresh the worker after every job return, even if the handler raises an error.
```

### Comparing `runpod-0.9.9/docs/serverless/worker_realtime.md` & `runpod-1.0.0/docs/serverless/worker_realtime.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/examples/call_endpoint_asyncio.py` & `runpod-1.0.0/examples/call_endpoint_asyncio.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/examples/graphql_wrapper.py` & `runpod-1.0.0/examples/graphql_wrapper.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/runpod/api_wrapper/graphql.py` & `runpod-1.0.0/runpod/api_wrapper/graphql.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/runpod/api_wrapper/mutations/pods.py` & `runpod-1.0.0/runpod/api_wrapper/mutations/pods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 RunPod | API Wrapper | Mutations | Pods
 """
 # pylint: disable=too-many-arguments, too-many-locals, too-many-branches
 
 
 def generate_pod_deployment_mutation(
-        name, image_name, gpu_type_id, cloud_type=None, gpu_count=None,
-        volume_in_gb=None, container_disk_in_gb=None, min_vcpu_count=None,
+        name, image_name, gpu_type_id, cloud_type=None, data_center_id=None, country_code=None,
+        gpu_count=None, volume_in_gb=None, container_disk_in_gb=None, min_vcpu_count=None,
         min_memory_in_gb=None, docker_args=None, ports=None, volume_mount_path=None,
-        env=None):
+        env=None, support_public_ip=None):
     '''
     Generates a mutation to deploy a pod on demand.
     '''
     input_fields = []
 
     if cloud_type is not None:
         input_fields.append(f"cloudType: {cloud_type}")
+    if data_center_id is not None:
+        input_fields.append(f'dataCenterId: "{data_center_id}"')
+    if country_code is not None:
+        input_fields.append(f'countryCode: "{country_code}"')
     if gpu_count is not None:
         input_fields.append(f"gpuCount: {gpu_count}")
     if volume_in_gb is not None:
         input_fields.append(f"volumeInGb: {volume_in_gb}")
     if container_disk_in_gb is not None:
         input_fields.append(f"containerDiskInGb: {container_disk_in_gb}")
     if min_vcpu_count is not None:
@@ -38,14 +42,16 @@
         input_fields.append(f'ports: "{ports}"')
     if volume_mount_path is not None:
         input_fields.append(f'volumeMountPath: "{volume_mount_path}"')
     if env is not None:
         env_string = ", ".join(
             [f'{{ key: "{key}", value: "{value}" }}' for key, value in env.items()])
         input_fields.append(f"env: [{env_string}]")
+    if support_public_ip is not None:
+        input_fields.append(f"supportPublicIp: {support_public_ip}")
 
     input_string = ", ".join(input_fields)
 
     return f"""
     mutation {{
       podFindAndDeployOnDemand(
         input: {{
```

### Comparing `runpod-0.9.9/runpod/api_wrapper/queries/gpus.py` & `runpod-1.0.0/runpod/api_wrapper/queries/gpus.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/runpod/endpoint/asyncio/asyncio_runner.py` & `runpod-1.0.0/runpod/endpoint/asyncio/asyncio_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     def __init__(self, endpoint_id: str, job_id: str, session: aiohttp.ClientSession):
         from runpod import api_key, endpoint_url_base  # pylint: disable=import-outside-toplevel,cyclic-import
 
         self.endpoint_id = endpoint_id
         self.job_id = job_id
         self.status_url = f"{endpoint_url_base}/{self.endpoint_id}/status/{self.job_id}"
+        self.cancel_url = f"{endpoint_url_base}/{self.endpoint_id}/cancel/{self.job_id}"
         self.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {api_key}"
         }
         self.session = session
 
     async def status(self) -> str:
@@ -43,14 +44,24 @@
         """
         while await self.status() not in ["COMPLETED", "FAILED"]:
             await asyncio.sleep(1)
 
         async with self.session.get(self.status_url, headers=self.headers) as resp:
             return (await resp.json())["output"]
 
+    async def cancel(self) -> dict:
+        """Cancels current job
+
+        Returns:
+            Output of cancel operation
+        """
+
+        async with self.session.post(self.cancel_url, headers=self.headers) as resp:
+            return await resp.json()
+
 
 class Endpoint:
     """Class for running endpoint"""
 
     def __init__(self, endpoint_id: str, session: aiohttp.ClientSession):
         from runpod import api_key, endpoint_url_base  # pylint: disable=import-outside-toplevel
```

### Comparing `runpod-0.9.9/runpod/serverless/modules/job.py` & `runpod-1.0.0/runpod/serverless/modules/rp_job.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,168 @@
 """
 Job related helpers.
 """
 
+import inspect
+from typing import Any, Callable, Dict, Generator, Optional, Union
+
 import os
-import time
 import json
 import traceback
+from aiohttp import ClientSession
 
-import runpod.serverless.modules.logging as log
-from .worker_state import JOB_GET_URL, get_done_url
-from .retry import retry
+from runpod.serverless.modules.rp_logger import RunPodLogger
+from .worker_state import WORKER_ID, Jobs
 from .rp_tips import check_return_size
 
-_IS_LOCAL_TEST = os.environ.get("RUNPOD_WEBHOOK_GET_JOB", None) is None
+JOB_GET_URL = str(os.environ.get('RUNPOD_WEBHOOK_GET_JOB')).replace('$ID', WORKER_ID)
 
+log = RunPodLogger()
+job_list = Jobs()
 
-def _get_local():
-    """
-    Returns contents of test_input.json.
-    """
-    if not os.path.exists("test_input.json"):
-        log.warn("test_input.json not found, skipping local testing")
-        return None
 
-    with open("test_input.json", "r", encoding="UTF-8") as file:
-        test_inputs = json.loads(file.read())
+def _job_get_url():
+    """
+    Prepare the URL for making a 'get' request to the serverless API (sls).
 
-    if "id" not in test_inputs:
-        test_inputs["id"] = "local_test"
+    This function constructs the appropriate URL for sending a 'get' request to the serverless API,
+    ensuring that the request will be correctly routed and processed by the API.
 
-    log.debug(f"Retrieved local job: {test_inputs}")
-    return test_inputs
+    Returns:
+        str: The prepared URL for the 'get' request to the serverless API.
+    """
+    job_in_progress = '1' if job_list.get_job_list() else '0'
+    return JOB_GET_URL + f"&job_in_progress={job_in_progress}"
 
 
-async def get_job(session, config):
+async def get_job(session: ClientSession, retry=True) -> Optional[Dict[str, Any]]:
     """
     Get the job from the queue.
+    Will continue trying to get a job until one is available.
+
+    Inputs:
+    - session | The aiohttp session
+
+    Note: Retry True just for ease of, if testing improved this can be removed.
     """
     next_job = None
 
-    try:
-        if config.get("test_input", None) is not None:
-            log.warn("test_input set, using test_input as job input")
-            next_job = config["test_input"]
-            next_job["id"] = "test_input_provided"
-        elif _IS_LOCAL_TEST:
-            log.warn("RUNPOD_WEBHOOK_GET_JOB not set, switching to get_local")
-            next_job = _get_local()
-        else:
-            async with session.get(JOB_GET_URL) as response:
+    while next_job is None:
+        try:
+            async with session.get(_job_get_url()) as response:
+                if response.status == 204:
+                    log.debug("No content, no job to process.")
+                    if not retry:
+                        return None
+                    continue
+
+                if response.status not in [200, 400]:
+                    log.error(f"Failed to get job, status code: {response.status}")
+                    if not retry:
+                        return None
+                    continue
+
                 next_job = await response.json()
-                log.debug(f"Retrieved remote job: {next_job}")
+                log.debug(f"Received Job | {next_job}")
 
-        if next_job.get("id", None) is None:
-            log.error("Job has no id, unable to process.")
-            next_job = None
-
-        if next_job is not None:
-            log.info(f"Received job: {next_job['id']}")
-    except Exception as err:  # pylint: disable=broad-except
-        log.error(f"Error while getting job: {err}")
+            # Check if the job is valid
+            job_id = next_job.get("id", None)
+            job_input = next_job.get("input", None)
+
+            if None in [job_id, job_input]:
+                missing_fields = []
+                if job_id is None:
+                    missing_fields.append("id")
+                if job_input is None:
+                    missing_fields.append("input")
+
+                log.error(f"Job has missing field(s): {', '.join(missing_fields)}.")
+                next_job = None
+
+        except Exception as err:  # pylint: disable=broad-except
+            log.error(f"Error while getting job: {err}")
+
+        if next_job is None:
+            log.debug("No job available, waiting for the next one.")
+            if not retry:
+                return None
+
+    log.debug(f"{next_job['id']} | Valid Job Confirmed")
+
+    if next_job:
+        job_list.add_job(next_job["id"])
+        log.debug(f"{next_job['id']} | Added Job ID")
 
     return next_job
 
 
-def run_job(handler, job):
+async def run_job(handler: Callable, job: Dict[str, Any]) -> Dict[str, Any]:
     """
     Run the job using the handler.
     Returns the job output or error.
     """
-    start_time = time.time()
-    log.info(f'Started working on job {job["id"]} at {start_time} UTC')
-
-    run_result = {"error": "Failed to return job output or capture error."}
+    log.info(f'{job["id"]} | Started')
 
     try:
-        job_output = handler(job)
-        log.debug(f'Job {job["id"]} handler output: {job_output}')
+        result = handler(job)
+        job_output = await result if inspect.isawaitable(result) else result
 
-        if isinstance(job_output, bool):
-            run_result = {"output": job_output}
-        elif "error" in job_output:
-            run_result = {"error": str(job_output["error"])}
-        elif "refresh_worker" in job_output:
-            job_output.pop("refresh_worker")
-            run_result = {
-                "stopPod": True,
-                "output": job_output
-            }
-        else:
+        log.debug(f'{job["id"]} | Handler output: {job_output}')
+
+        run_result = {"output": job_output}
+
+        if isinstance(job_output, dict):
+
+            if job_output.get("error", False):
+                run_result = {"error": str(job_output["error"])}
+
+            if job_output.get("refresh_worker", False):
+                job_output.pop("refresh_worker")
+                run_result = {
+                    "stopPod": True,
+                    "output": job_output
+                }
+
+        elif isinstance(job_output, bool):
             run_result = {"output": job_output}
 
         check_return_size(run_result)  # Checks the size of the return body.
     except Exception as err:    # pylint: disable=broad-except
-        log.error(f'Error while running job {job["id"]}: {err}')
-        run_result = {"error": f"handler: {str(err)} \ntraceback: {traceback.format_exc()}"}
-    finally:
-        end_time = time.time()
-        log.info(f'Finished working on job {job["id"]} at {end_time} UTC')
-        log.info(f"Job {job['id']} took {end_time - start_time} seconds to complete")
-        log.debug(f"Run result: {run_result}")
+        error_content = json.dumps(
+            {
+                "error_type": str(type(err)),
+                "error_message": str(err),
+                "error_traceback": traceback.format_exc(),
+                "host_name": os.environ.get("RUNPOD_POD_HOSTNAME", "unknown"),
+                "pod_id": os.environ.get("RUNPOD_POD_ID", "unknown")
+            }, indent=4)
 
-        return run_result  # pylint: disable=lost-exception
-
-
-@retry(max_attempts=3, base_delay=1, max_delay=3)
-async def retry_send_result(session, job_data):
-    """
-    Wrapper for sending results.
-    """
-    headers = {
-        "charset": "utf-8",
-        "Content-Type": "application/x-www-form-urlencoded"
-    }
+        log.error(f'{job["id"]} | Captured Handler Exception')
+        log.error(error_content)
 
-    log.debug("Initiating result API call")
-    async with session.post(get_done_url(),
-                            data=job_data,
-                            headers=headers,
-                            raise_for_status=True) as resp:
-        result = await resp.text()
-        log.debug(f"Result API response: {result}")
+        run_result = {"error": error_content}
+    finally:
+        log.debug(f'{job["id"]} | run_job return: {run_result}')
 
-    log.info("Completed result API call")
+        return run_result  # pylint: disable=lost-exception
 
 
-async def send_result(session, job_data, job):
+async def run_job_generator(
+        handler: Callable,
+        job: Dict[str, Any]) -> Generator[Dict[str, Union[str, Any]], None, None]:
     '''
-    Return the job results.
+    Run generator job.
+    Yields output partials from the generator.
     '''
     try:
-        job_data = json.dumps(job_data, ensure_ascii=False)
-        if not _IS_LOCAL_TEST:
-            log.info(f"Sending job results for {job['id']}: {job_data}")
-            await retry_send_result(session, job_data)
+        job_output = handler(job)
+        if inspect.isasyncgenfunction(handler):
+            async for output_partial in job_output:
+                yield {"output": output_partial}
         else:
-            log.warn(f"Local test job results for {job['id']}: {job_data}")
-
-    except Exception as err:  # pylint: disable=broad-except
-        log.error(f"Error while returning job result {job['id']}: {err}")
-    else:
-        log.info(f"Successfully returned job result {job['id']}")
+            for output_partial in job_output:
+                yield {"output": output_partial}
+    except Exception as err:    # pylint: disable=broad-except
+        log.error(f'Error while running job {job["id"]}: {err}')
+        yield {"error": f"handler: {str(err)} \ntraceback: {traceback.format_exc()}"}
+    finally:
+        log.info(f'{job["id"]} | Finished ')
```

### Comparing `runpod-0.9.9/runpod/serverless/modules/retry.py` & `runpod-1.0.0/runpod/serverless/modules/retry.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/runpod/serverless/utils/rp_cleanup.py` & `runpod-1.0.0/runpod/serverless/utils/rp_cleanup.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/runpod/serverless/utils/rp_download.py` & `runpod-1.0.0/runpod/serverless/utils/rp_download.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,51 +14,78 @@
 from urllib.parse import urlparse
 from email import message_from_string
 from concurrent.futures import ThreadPoolExecutor
 
 import backoff
 import requests
 
+HEADERS = {"User-Agent": "runpod-python/0.0.0 (https://runpod.io; support@runpod.io)"}
 
-def download_files_from_urls(job_id: str, urls: Union[str, List[str]]) -> List[str]:
+
+def calculate_chunk_size(file_size: int) -> int:
     '''
+    Calculates the chunk size based on the file size.
+    '''
+    if file_size <= 1024*1024:  # 1 MB
+        return 1024  # 1 KB
+    if file_size <= 1024*1024*1024:  # 1 GB
+        return 1024*1024  # 1 MB
+
+    return 1024*1024*10  # 10 MB
+
+
+def download_files_from_urls(job_id: str, urls: Union[str, List[str]]) -> List[str]:
+    """
     Accepts a single URL or a list of URLs and downloads the files.
     Returns the list of downloaded file absolute paths.
     Saves the files in a directory called "downloaded_files" in the job directory.
-    '''
+    """
     download_directory = os.path.abspath(os.path.join('jobs', job_id, 'downloaded_files'))
     os.makedirs(download_directory, exist_ok=True)
 
     @backoff.on_exception(backoff.expo, requests.exceptions.RequestException, max_tries=3)
-    def download_file(url: str) -> bytes:
-        with requests.get(url, timeout=5) as response:
+    def download_file(url: str, path_to_save: str) -> str:
+        with requests.get(url, headers=HEADERS, stream=True, timeout=5) as response:
             response.raise_for_status()
             content_disposition = response.headers.get('Content-Disposition')
-            msg = message_from_string(f'Content-Disposition: {content_disposition}')
-            params = dict(msg.items()) if content_disposition else {}
-            file_extension = os.path.splitext(params.get('filename', ''))[1]
-            return response.content, file_extension
+            file_extension = ''
+            if content_disposition:
+                msg = message_from_string(f'Content-Disposition: {content_disposition}')
+                params = dict(msg.items())
+                file_extension = os.path.splitext(params.get('filename', ''))[1]
+
+            # If no extension could be determined from 'Content-Disposition', get it from the URL
+            if not file_extension:
+                file_extension = os.path.splitext(urlparse(url).path)[1]
+
+            file_size = int(response.headers.get('Content-Length', 0))
+            chunk_size = calculate_chunk_size(file_size)
+
+            # write the content in chunks to the file
+            with open(path_to_save + file_extension, 'wb') as file_path:
+                for chunk in response.iter_content(chunk_size=chunk_size):
+                    if chunk:  # filter out keep-alive chunks
+                        file_path.write(chunk)
+
+            return file_extension
 
     def download_file_to_path(url: str) -> str:
         if url is None:
             return None
 
+        file_name = f'{uuid.uuid4()}'
+        output_file_path = os.path.join(download_directory, file_name)
+
         try:
-            file_data, file_extension = download_file(url)
+            file_extension = download_file(url, output_file_path)
         except requests.exceptions.RequestException as err:
             print(f"Failed to download {url}: {err}")
             return None
 
-        file_name = f'{uuid.uuid4()}{file_extension}'
-        output_file_path = os.path.join(download_directory, file_name)
-
-        with open(output_file_path, 'wb') as output_file:
-            output_file.write(file_data)
-
-        return os.path.abspath(output_file_path)
+        return os.path.abspath(f"{output_file_path}{file_extension}")
 
     if isinstance(urls, str):
         urls = [urls]
 
     with ThreadPoolExecutor() as executor:
         downloaded_files = list(executor.map(download_file_to_path, urls))
 
@@ -74,15 +101,15 @@
     Returns an object that contains:
     - The absolute path to the downloaded file
     - File type
     - Original file name
     '''
     os.makedirs('job_files', exist_ok=True)
 
-    download_response = requests.get(file_url, timeout=30)
+    download_response = requests.get(file_url, headers=HEADERS, timeout=30)
 
     original_file_name = []
     if "Content-Disposition" in download_response.headers.keys():
         original_file_name = re.findall(
             "filename=(.+)",
             download_response.headers["Content-Disposition"]
         )
```

### Comparing `runpod-0.9.9/runpod/serverless/utils/rp_upload.py` & `runpod-1.0.0/runpod/serverless/utils/rp_upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ''' PodWorker | modules | upload.py '''
+# pylint: disable=too-many-arguments
 
 import os
 import io
 import time
 import uuid
+import shutil
 import logging
 import threading
 import multiprocessing
 from io import BytesIO
 from typing import Optional, Tuple
 
 import boto3
@@ -19,15 +21,16 @@
 
 logger = logging.getLogger("runpod upload utility")
 FMT = "%(filename)-20s:%(lineno)-4d %(asctime)s %(message)s"
 logging.basicConfig(level=logging.INFO, format=FMT, handlers=[logging.StreamHandler()])
 
 
 # --------------------------- S3 Bucket Connection --------------------------- #
-def get_boto_client(bucket_creds: Optional[dict] = None) -> Tuple[boto3.client, TransferConfig]:
+def get_boto_client(
+    bucket_creds: Optional[dict] = None) -> Tuple[boto3.client, TransferConfig]: # pragma: no cover
     '''
     Returns a boto3 client and transfer config for the bucket.
     '''
     bucket_session = session.Session()
 
     boto_config = Config(
         signature_version='s3v4',
@@ -66,15 +69,15 @@
 
     return boto_client, transfer_config
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Upload Image                                 #
 # ---------------------------------------------------------------------------- #
-def upload_image(job_id, image_location, result_index=0, results_list=None):
+def upload_image(job_id, image_location, result_index=0, results_list=None): # pragma: no cover
     '''
     Upload image to bucket storage.
     '''
     image_name = str(uuid.uuid4())[:8]
     boto_client, _ = get_boto_client()
 
     if boto_client is None:
@@ -118,15 +121,15 @@
 
         return presigned_url
 
 
 # ---------------------------------------------------------------------------- #
 #                                Files To Upload                               #
 # ---------------------------------------------------------------------------- #
-def files(job_id, file_list):
+def files(job_id, file_list): # pragma: no cover
     '''
     Uploads a list of files in parallel.
     Once all files are uploaded, the function returns the presigned URLs list.
     '''
     upload_progress = []  # List of threads
     file_urls = [None] * len(file_list)  # Resulting list of URLs for each file
 
@@ -143,15 +146,15 @@
     for upload in upload_progress:
         upload.join()
 
     return file_urls
 
 
 # --------------------------- Custom Bucket Upload --------------------------- #
-def bucket_upload(job_id, file_list, bucket_creds):
+def bucket_upload(job_id, file_list, bucket_creds): # pragma: no cover
     '''
     Uploads files to bucket storage.
     '''
     temp_bucket_session = session.Session()
 
     temp_boto_config = Config(
         signature_version='s3v4',
@@ -186,32 +189,52 @@
 
 
 # ------------------------- Single File Bucket Upload ------------------------ #
 def upload_file_to_bucket(
         file_name: str, file_location: str,
         bucket_creds: Optional[dict] = None,
         bucket_name: Optional[str] = None,
-        prefix: Optional[str] = None) -> str:
+        prefix: Optional[str] = None,
+        extra_args: Optional[dict] = None
+) -> str: # pragma: no cover
     '''
     Uploads a single file to bucket storage and returns a presigned URL.
     '''
     boto_client, transfer_config = get_boto_client(bucket_creds)
 
     if not bucket_name:
         bucket_name = time.strftime('%m-%y')
 
     key = f"{prefix}/{file_name}" if prefix else file_name
 
+    if boto_client is None:
+        print("No bucket endpoint set, saving to disk folder 'local_upload'")
+        print("If this is a live endpoint, please reference the following:")
+        print("https://github.com/runpod/runpod-python/blob/main/docs/serverless/utils/rp_upload.md")  # pylint: disable=line-too-long
+
+        os.makedirs("local_upload", exist_ok=True)
+        local_upload_location = f"local_upload/{file_name}"
+        shutil.copyfile(file_location, local_upload_location)
+
+        return local_upload_location
+
     file_size = os.path.getsize(file_location)
     with tqdm(total=file_size, unit='B', unit_scale=True, desc=file_name) as progress_bar:
-        boto_client.upload_file(
-            file_location, bucket_name, key,
-            Config=transfer_config,
-            Callback=progress_bar.update
-        )
+        upload_file_args = {
+            "Filename": file_location,
+            "Bucket": bucket_name,
+            "Key": key,
+            "Config": transfer_config,
+            "Callback": progress_bar.update
+        }
+
+        if extra_args:
+            upload_file_args["ExtraArgs"] = extra_args
+
+        boto_client.upload_file(**upload_file_args)
 
     presigned_url = boto_client.generate_presigned_url(
         'get_object',
         Params={
             'Bucket': bucket_name,
             'Key': key
         }, ExpiresIn=604800)
@@ -220,15 +243,15 @@
 
 
 # --------------------------- Upload Memory Object --------------------------- #
 def upload_in_memory_object(
         file_name: str, file_data: bytes,
         bucket_creds: Optional[dict] = None,
         bucket_name: Optional[str] = None,
-        prefix: Optional[str] = None) -> str:
+        prefix: Optional[str] = None) -> str: # pragma: no cover
     '''
     Uploads an in-memory object (bytes) to bucket storage and returns a presigned URL.
     '''
     boto_client, transfer_config = get_boto_client(bucket_creds)
 
     if not bucket_name:
         bucket_name = time.strftime('%m-%y')
```

### Comparing `runpod-0.9.9/runpod/serverless/utils/rp_validator.py` & `runpod-1.0.0/runpod/serverless/utils/rp_validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,74 +16,89 @@
 CONSTRAINTS_ERROR = "{} does not meet the constraints."
 SCHEMA_ERROR = "Schema error, {} is not a dictionary."
 
 
 def _add_error(error_list: List[str], message: str) -> None:
     error_list.append(message)
 
-
-def validate(raw_input: Dict[str, Any], schema: Dict[str, Any]
-             ) -> Dict[str, Union[Dict[str, Any], List[str]]]:
-    '''
-    Validates the input.
-    Checks to see if the provided inputs match the expected types.
-    Checks to see if the required inputs are included.
-    Sets the default values for the inputs that are not provided.
-    Validates the inputs using the lambda constraints.
-
-    Returns either the list of errors or a validated_job_input.
-    {"errors": ["error1", "error2"]}
-    or
-    {"validated_input": {"input1": "value1", "input2": "value2"}
-    '''
-    error_list = []
-    validated_input = raw_input.copy()
-
-    # Check for unexpected inputs.
+def _check_for_unexpected_inputs(raw_input, schema, error_list):
     for key in raw_input:
         if key not in schema:
             _add_error(error_list, UNEXPECTED_INPUT_ERROR.format(key))
 
-    # Check that items are dictionaries.
+
+def _validate_and_transform_schema_items(schema, error_list):
     for key, rules in schema.items():
         if not isinstance(rules, dict):
             try:
                 schema[key] = json.loads(rules)
             except json.decoder.JSONDecodeError:
                 _add_error(error_list, SCHEMA_ERROR.format(key))
 
-    # Checks for missing required inputs or sets the default values.
+
+def _validate_required_inputs_and_set_defaults(raw_input, schema, validated_input, error_list):
     for key, rules in schema.items():
         if 'type' not in rules:
             _add_error(error_list, MISSING_TYPE_ERROR.format(key))
 
         if 'required' not in rules:
             _add_error(error_list, MISSING_REQUIRED_ERROR.format(key))
         elif rules['required'] and key not in raw_input:
             _add_error(error_list, MISSING_REQUIRED_ERROR.format(key))
-        elif rules['required'] and key not in raw_input and "default" not in rules:
-            _add_error(error_list, MISSING_DEFAULT_ERROR.format(key))
-        elif not rules['required'] and key not in raw_input and "default" not in rules:
-            _add_error(error_list, MISSING_DEFAULT_ERROR.format(key))
         elif not rules['required'] and key not in raw_input:
-            validated_input[key] = raw_input.get(key, rules['default'])
+            if "default" in rules:
+                validated_input[key] = rules['default']
+            else:
+                _add_error(error_list, MISSING_DEFAULT_ERROR.format(key))
 
+
+def _validate_input_against_schema(schema, validated_input, error_list):
     for key, rules in schema.items():
-        # Enforce floats to be floats.
-        if rules['type'] is float and type(validated_input[key]) in [int, float]:
-            validated_input[key] = float(validated_input[key])
-
-        # Check for the correct type.
-        if not isinstance(validated_input[key], rules['type']) and raw_input.get(key, False):
-            _add_error(
-                error_list, f"{key} should be {rules['type']} type, not {type(raw_input[key])}.")
+        if key in validated_input:
+            # Enforce floats to be floats.
+            try:
+                if rules['type'] is float and type(validated_input[key]) in [int, float]:
+                    validated_input[key] = float(validated_input[key])
+            except TypeError:
+                continue
+
+            # Check for the correct type.
+            is_instance = isinstance(validated_input[key], rules['type'])
+            if validated_input[key] is not None and not is_instance:
+                _add_error(
+                    error_list,
+                    f"{key} should be {rules['type']} type, not {type(validated_input[key])}."
+                )
 
         # Check lambda constraints.
-        if "constraints" in rules:
-            if not rules['constraints'](validated_input[key]):
-                _add_error(error_list, CONSTRAINTS_ERROR.format(key))
+        if "constraints" in rules and not rules['constraints'](validated_input.get(key)):
+            _add_error(error_list, CONSTRAINTS_ERROR.format(key))
+
+def validate(
+    raw_input: Dict[str, Any], schema: Dict[str, Any]
+) -> Dict[str, Union[Dict[str, Any], List[str]]]:
+    '''
+    Validates the input.
+    Checks to see if the provided inputs match the expected types.
+    Checks to see if the required inputs are included.
+    Sets the default values for the inputs that are not provided.
+    Validates the inputs using the lambda constraints.
+
+    Returns either the list of errors or a validated_job_input.
+    {"errors": ["error1", "error2"]}
+    or
+    {"validated_input": {"input1": "value1", "input2": "value2"}
+    '''
+    error_list = []
+    validated_input = raw_input.copy()
+
+    # Separate the process into functions for better readability
+    _check_for_unexpected_inputs(raw_input, schema, error_list)
+    _validate_and_transform_schema_items(schema, error_list)
+    _validate_required_inputs_and_set_defaults(raw_input, schema, validated_input, error_list)
+    _validate_input_against_schema(schema, validated_input, error_list)
 
     validation_return = {"validated_input": validated_input}
     if error_list:
         validation_return = {"errors": error_list}
 
     return validation_return
```

### Comparing `runpod-0.9.9/runpod.egg-info/PKG-INFO` & `runpod-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,85 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 0.9.9
-Summary: Official Python library for RunPod API & SDK.
+Version: 1.0.0
+Summary: 🐍 | Python library for RunPod API and serverless worker SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <div align="center">
 <h1>RunPod | Python Library </h1>
 
-[![CI | Code Quality](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml)
+[![PyPI Package](https://badge.fury.io/py/runpod.svg)](https://badge.fury.io/py/runpod)
 &nbsp;
-[![CI | Unit Tests](https://github.com/runpod/runpod-python/actions/workflows/CI_tests.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI_tests.yml)
+[![Downloads](https://static.pepy.tech/personalized-badge/runpod?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/runpod)
+
+[![CI | Code Quality](https://github.com/runpod/runpod-python/actions/workflows/CI-pylint.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI-pylint.yml)
+&nbsp;
+[![CI | Unit Tests](https://github.com/runpod/runpod-python/actions/workflows/CI-tests.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI-tests.yml)
+&nbsp;
+[![CI | CodeQL](https://github.com/runpod/runpod-python/actions/workflows/CI-codeql.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/CI-codeql.yml)
 
 </div>
 
-Official Python library for RunPod API &amp; SDK.
+Welcome to the official Python library for RunPod API &amp; SDK.
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
-- [Installation](#installation)
-- [SDK - Serverless Worker](#sdk---serverless-worker)
+- [💻 | Installation](#--installation)
+- [⚡ | Serverless Worker (SDK)](#--serverless-worker-sdk)
   - [Quick Start](#quick-start)
-- [API Language Library](#api-language-library)
+  - [Local Test Worker](#local-test-worker)
+- [📚 | API Language Library (GraphQL Wrapper)](#--api-language-library-graphql-wrapper)
   - [Endpoints](#endpoints)
-  - [GPU Pod Control](#gpu-pod-control)
-- [Directory](#directory)
-- [Community and Contributing](#community-and-contributing)
+  - [GPU Cloud (Pods)](#gpu-cloud-pods)
+- [📁 | Directory](#--directory)
+- [🤝 | Community and Contributing](#--community-and-contributing)
 
-## Installation
+## 💻 | Installation
 
 ```bash
+# Install the latest release version
 pip install runpod
+
+# or
+
+# Install the latest development version (main branch)
+pip install git+https://github.com/runpod/runpod-python.git
 ```
 
-## SDK - Serverless Worker
+*Python 3.10 or higher is required to use the latest version of this package.*
+
+## ⚡ | Serverless Worker (SDK)
 
 This python package can also be used to create a serverless worker that can be deployed to RunPod as a custom endpoint API.
 
 ### Quick Start
 
 Create an python script in your project that contains your model definition and the RunPod worker start code. Run this python code as your default container start command:
 
 ```python
+# my_worker.py
+
 import runpod
 
 def is_even(job):
 
     job_input = job["input"]
     the_number = job_input["number"]
 
@@ -77,15 +94,23 @@
 runpod.serverless.start({"handler": is_even})
 ```
 
 Make sure that this file is ran when your container starts. This can be accomplished by calling it in the docker command when you setup a template at [runpod.io/console/serverless/user/templates](https://www.runpod.io/console/serverless/user/templates) or by setting it as the default command in your Dockerfile.
 
 See our [blog post](https://www.runpod.io/blog/serverless-create-a-basic-api) for creating a basic Serverless API, or view the [details docs](https://docs.runpod.io/serverless-ai/custom-apis) for more information.
 
-## API Language Library
+### Local Test Worker
+
+You can also test your worker locally before deploying it to RunPod. This is useful for debugging and testing.
+
+```bash
+python my_worker.py --rp_serve_api
+```
+
+## 📚 | API Language Library (GraphQL Wrapper)
 
 When interacting with the RunPod API you can use this library to make requests to the API.
 
 ```python
 import runpod
 
 runpod.api_key = "your_runpod_api_key_found_under_settings"
@@ -116,15 +141,15 @@
     {"your_model_input_key": "your_model_input_value"}
 )
 
 # Returns the job results if completed within 90 seconds, otherwise, returns the job status.
 print(run_request )
 ```
 
-### GPU Pod Control
+### GPU Cloud (Pods)
 
 ```python
 import runpod
 
 runpod.api_key = "your_runpod_api_key_found_under_settings"
 
 # Create a pod
@@ -136,26 +161,29 @@
 # Start the pod
 runpod.start_pod(pod.id)
 
 # Terminate the pod
 runpod.terminate_pod(pod.id)
 ```
 
-## Directory
+## 📁 | Directory
 
 ```BASH
 .
 ├── docs               # Documentation
+├── examples           # Examples
 ├── runpod             # Package source code
+│   ├── api_wrapper    # Language library - API (GraphQL)
+│   ├── cli            # Command Line Interface Functions
 │   ├── endpoint       # Language library - Endpoints
 │   └── serverless     # SDK - Serverless Worker
 └── tests              # Package tests
 ```
 
-## Community and Contributing
+## 🤝 | Community and Contributing
 
 We welcome both pull requests and issues on [GitHub](https://github.com/runpod/runpod-python). Bug fixes and new features are encouraged.
 
 <div align="center">
 
 <a target="_blank" href="https://discord.gg/pJ3P2DbUUq">![Discord Banner 2](https://discordapp.com/api/guilds/912829806415085598/widget.png?style=banner2)</a>
```

### Comparing `runpod-0.9.9/runpod.egg-info/SOURCES.txt` & `runpod-1.0.0/runpod.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,101 @@
 .gitignore
+CONTRIBUTING.md
 LICENSE
 README.md
-infer.py
+SECURITY.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 .github/dependabot.yml
-.github/workflows/CD_publish-to-pypi.yml
-.github/workflows/CI_codeql.yml
-.github/workflows/CI_tests.yml
-.github/workflows/ci_pylint.yml
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/CD-publish_to_pypi.yml
+.github/workflows/CD-test_publish_to_pypi.yml
+.github/workflows/CI-codeql.yml
+.github/workflows/CI-pylint.yml
+.github/workflows/CI-tests.yml
 docs/api/quries.md
 docs/images/env_var_location.png
 docs/serverless/local_testing.md
 docs/serverless/worker.md
 docs/serverless/worker_realtime.md
+docs/serverless/functions/error_handling.md
+docs/serverless/functions/logging.md
 docs/serverless/utils/rp_cleanup.md
+docs/serverless/utils/rp_debugger.md
 docs/serverless/utils/rp_download.md
 docs/serverless/utils/rp_upload.md
 docs/serverless/utils/rp_validator.md
 examples/call_endpoint.py
 examples/call_endpoint_asyncio.py
 examples/graphql_wrapper.py
 runpod/__init__.py
 runpod.egg-info/PKG-INFO
 runpod.egg-info/SOURCES.txt
 runpod.egg-info/dependency_links.txt
+runpod.egg-info/entry_points.txt
 runpod.egg-info/requires.txt
 runpod.egg-info/top_level.txt
 runpod/api_wrapper/__init__.py
 runpod/api_wrapper/ctl_commands.py
 runpod/api_wrapper/graphql.py
 runpod/api_wrapper/mutations/__init__.py
 runpod/api_wrapper/mutations/pods.py
 runpod/api_wrapper/queries/__init__.py
 runpod/api_wrapper/queries/gpus.py
+runpod/cli/__init__.py
+runpod/cli/config.py
 runpod/endpoint/__init__.py
 runpod/endpoint/runner.py
 runpod/endpoint/asyncio/__init__.py
 runpod/endpoint/asyncio/asyncio_runner.py
 runpod/serverless/__init__.py
-runpod/serverless/work_loop.py
+runpod/serverless/worker.py
 runpod/serverless/modules/__init__.py
-runpod/serverless/modules/heartbeat.py
-runpod/serverless/modules/job.py
-runpod/serverless/modules/logging.py
 runpod/serverless/modules/retry.py
 runpod/serverless/modules/rp_fastapi.py
+runpod/serverless/modules/rp_http.py
+runpod/serverless/modules/rp_job.py
+runpod/serverless/modules/rp_local.py
+runpod/serverless/modules/rp_logger.py
+runpod/serverless/modules/rp_ping.py
+runpod/serverless/modules/rp_scale.py
 runpod/serverless/modules/rp_tips.py
 runpod/serverless/modules/worker_state.py
 runpod/serverless/utils/__init__.py
 runpod/serverless/utils/rp_cleanup.py
+runpod/serverless/utils/rp_cuda.py
+runpod/serverless/utils/rp_debugger.py
 runpod/serverless/utils/rp_download.py
 runpod/serverless/utils/rp_upload.py
 runpod/serverless/utils/rp_validator.py
 tests/__init__.py
 tests/test_whatever.py
 tests/whatever.py
+tests/test_api_wrapper/test_ctl_commands.py
+tests/test_api_wrapper/test_mutations_pods.py
+tests/test_cli/__init__.py
+tests/test_cli/test_config.py
 tests/test_endpoint/__init__.py
+tests/test_endpoint/test_asyncio_runner.py
 tests/test_endpoint/test_runner.py
 tests/test_serverless/__init__.py
-tests/test_serverless/test_module_download.py
-tests/test_serverless/test_pod_worker.py
-tests/test_serverless/test_util_upload.py
+tests/test_serverless/test_worker.py
+tests/test_serverless/test_modules/__init__.py
+tests/test_serverless/test_modules/test_fastapi.py
+tests/test_serverless/test_modules/test_http.py
+tests/test_serverless/test_modules/test_job.py
+tests/test_serverless/test_modules/test_local.py
+tests/test_serverless/test_modules/test_logger.py
+tests/test_serverless/test_modules/test_ping.py
+tests/test_serverless/test_modules/test_retry.py
+tests/test_serverless/test_modules/test_state.py
+tests/test_serverless/test_modules/test_tips.py
+tests/test_serverless/test_utils/__init__.py
+tests/test_serverless/test_utils/test_cleanup.py
+tests/test_serverless/test_utils/test_cuda.py
+tests/test_serverless/test_utils/test_debugger.py
+tests/test_serverless/test_utils/test_download.py
+tests/test_serverless/test_utils/test_upload.py
+tests/test_serverless/test_utils/test_validate.py
```

### Comparing `runpod-0.9.9/setup.cfg` & `runpod-1.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = runpod
 version = 0.0.0  # Placeholder value, will be overridden by setuptools_scm
-description = Official Python library for RunPod API & SDK.
+description = 🐍 | Python library for RunPod API and serverless worker SDK.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = runpod, ai, gpu, serverless, SDK, API, python, library
 url = https://github.com/runpod/runpod-python
 project_urls = 
 	Bug Tracker = https://github.com/runpod/runpod-python/issues
 author = RunPod
@@ -20,28 +20,34 @@
 	Programming Language :: Python :: 3
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
-python_requires = >= 3.6
+python_requires = >= 3.10
 install_requires = 
-	backoff == 2.2.1
-	pillow >= 9.3.0
-	python-dotenv >= 0.21.0
-	requests >= 2.28.1
-	tqdm-loggable >= 0.1.3
-	boto3 >= 1.26.15
-	aiohttp >= 3.8.3
-	fastapi[all] >= 0.89.0
+	aiohttp >= 3.8.4
+	backoff >= 2.2.1
+	boto3 >= 1.26.165
+	pillow >= 9.5.0
+	py-cpuinfo >= 9.0.0
+	python-dotenv >= 1.0.0
+	requests >= 2.31.0
+	tomli >= 2.0.1
+	tqdm-loggable >= 0.1.4
+	fastapi[all] >= 0.99.0
 
 [options.extras_require]
 test = 
+	asynctest
+	nest_asyncio
 	pytest
+	pytest-cov
+	pytest-timeout
 	pytest-asyncio
 
 [setuptools_scm]
 write_to = runpod/_version.py
 
 [egg_info]
 tag_build =
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `runpod-0.9.9/tests/test_whatever.py` & `runpod-1.0.0/tests/test_whatever.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.9/tests/whatever.py` & `runpod-1.0.0/tests/whatever.py`

 * *Files identical despite different names*

