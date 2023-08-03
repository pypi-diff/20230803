# Comparing `tmp/reana-commons-0.9.3a3.tar.gz` & `tmp/reana-commons-0.9.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reana-commons-0.9.3a3.tar", last modified: Fri Jun 23 14:26:30 2023, max compression
+gzip compressed data, was "reana-commons-0.9.3a4.tar", last modified: Thu Aug  3 14:42:51 2023, max compression
```

## Comparing `reana-commons-0.9.3a3.tar` & `reana-commons-0.9.3a4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.458793 reana-commons-0.9.3a3/
--rw-r--r--   0 madonado  (1000) madonado  (1000)      272 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/.flake8
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1161 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/AUTHORS.rst
--rw-r--r--   0 madonado  (1000) madonado  (1000)    10156 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/CHANGES.rst
--rw-r--r--   0 madonado  (1000) madonado  (1000)      676 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/CONTRIBUTING.rst
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1092 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/LICENSE
--rw-r--r--   0 madonado  (1000) madonado  (1000)      601 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/MANIFEST.in
--rw-r--r--   0 madonado  (1000) madonado  (1000)    13543 2023-06-23 14:26:30.458793 reana-commons-0.9.3a3/PKG-INFO
--rw-r--r--   0 madonado  (1000) madonado  (1000)     2114 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/README.rst
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.453793 reana-commons-0.9.3a3/docs/
--rw-r--r--   0 madonado  (1000) madonado  (1000)     6508 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/docs/conf.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1361 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/docs/index.rst
--rw-r--r--   0 madonado  (1000) madonado  (1000)      240 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/docs/requirements.txt
--rw-r--r--   0 madonado  (1000) madonado  (1000)      308 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/pytest.ini
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.455793 reana-commons-0.9.3a3/reana_commons/
--rw-r--r--   0 madonado  (1000) madonado  (1000)      377 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/__init__.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     8543 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/api_client.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)    16844 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/config.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     2588 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/consumer.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     2350 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/email.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     2950 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/errors.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1859 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/job_utils.py
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.456793 reana-commons-0.9.3a3/reana_commons/k8s/
--rw-r--r--   0 madonado  (1000) madonado  (1000)      265 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/__init__.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1925 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/api_client.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     4330 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/kerberos.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)    11521 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/secrets.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     3248 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/k8s/volumes.py
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.456793 reana-commons-0.9.3a3/reana_commons/openapi_specifications/
--rw-r--r--   0 madonado  (1000) madonado  (1000)    12023 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_job_controller.json
--rw-r--r--   0 madonado  (1000) madonado  (1000)   137719 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_server.json
--rw-r--r--   0 madonado  (1000) madonado  (1000)    50816 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_workflow_controller.json
--rw-r--r--   0 madonado  (1000) madonado  (1000)     6328 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/publisher.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     8302 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/serial.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     7051 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/snakemake.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     4101 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/specification.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)    17086 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/utils.py
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.457793 reana-commons-0.9.3a3/reana_commons/validation/
--rw-r--r--   0 madonado  (1000) madonado  (1000)      268 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/__init__.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     6129 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/compute_backends.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     2093 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/operational_options.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)    17863 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/parameters.py
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.457793 reana-commons-0.9.3a3/reana_commons/validation/schemas/
--rw-r--r--   0 madonado  (1000) madonado  (1000)     6528 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/schemas/reana_analysis_schema.json
--rw-r--r--   0 madonado  (1000) madonado  (1000)     2779 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/validation/utils.py
--rwxr-xr-x   0 madonado  (1000) madonado  (1000)      458 2023-06-23 14:25:16.000000 reana-commons-0.9.3a3/reana_commons/version.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     7404 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/workflow_engine.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     7536 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/workspace.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     2163 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/reana_commons/yadage.py
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.455793 reana-commons-0.9.3a3/reana_commons.egg-info/
--rw-r--r--   0 madonado  (1000) madonado  (1000)    13543 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/PKG-INFO
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1702 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/SOURCES.txt
--rw-r--r--   0 madonado  (1000) madonado  (1000)        1 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/dependency_links.txt
--rw-r--r--   0 madonado  (1000) madonado  (1000)        1 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/not-zip-safe
--rw-r--r--   0 madonado  (1000) madonado  (1000)      766 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/requires.txt
--rw-r--r--   0 madonado  (1000) madonado  (1000)       14 2023-06-23 14:26:30.000000 reana-commons-0.9.3a3/reana_commons.egg-info/top_level.txt
--rwxr-xr-x   0 madonado  (1000) madonado  (1000)     1172 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/run-tests.sh
--rw-r--r--   0 madonado  (1000) madonado  (1000)      136 2023-06-23 14:26:30.458793 reana-commons-0.9.3a3/setup.cfg
--rwxr-xr-x   0 madonado  (1000) madonado  (1000)     3331 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/setup.py
-drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-06-23 14:26:30.458793 reana-commons-0.9.3a3/tests/
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1317 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/conftest.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)      718 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_email.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     3200 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_job_utils.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     2700 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_mq.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1659 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_operational_options.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     3925 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_secrets_store.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1383 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_snakemake.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1674 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_specification.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     4726 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_utils.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)     1004 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_validation.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)      446 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_version.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)    10248 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tests/test_workspace.py
--rw-r--r--   0 madonado  (1000) madonado  (1000)      333 2023-06-22 07:54:05.000000 reana-commons-0.9.3a3/tox.ini
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.783759 reana-commons-0.9.3a4/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      272 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/.flake8
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1161 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/AUTHORS.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    10441 2023-08-03 14:41:17.000000 reana-commons-0.9.3a4/CHANGES.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      676 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/CONTRIBUTING.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1092 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/LICENSE
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      627 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/MANIFEST.in
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    13828 2023-08-03 14:42:51.783759 reana-commons-0.9.3a4/PKG-INFO
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2114 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/README.rst
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.778759 reana-commons-0.9.3a4/docs/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6508 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/docs/conf.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1361 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/docs/index.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      240 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/docs/requirements.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      308 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/pytest.ini
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.780759 reana-commons-0.9.3a4/reana_commons/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      377 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/__init__.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     8543 2023-07-20 13:31:13.000000 reana-commons-0.9.3a4/reana_commons/api_client.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    16844 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/config.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2588 2023-07-20 08:32:36.000000 reana-commons-0.9.3a4/reana_commons/consumer.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2350 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/reana_commons/email.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2950 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/errors.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1859 2023-07-20 09:37:42.000000 reana-commons-0.9.3a4/reana_commons/job_utils.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.781759 reana-commons-0.9.3a4/reana_commons/k8s/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      265 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/k8s/__init__.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1925 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/k8s/api_client.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     4330 2023-07-17 11:48:11.000000 reana-commons-0.9.3a4/reana_commons/k8s/kerberos.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    11521 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/k8s/secrets.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     3248 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/k8s/volumes.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.781759 reana-commons-0.9.3a4/reana_commons/openapi_specifications/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    11988 2023-08-03 14:41:17.000000 reana-commons-0.9.3a4/reana_commons/openapi_specifications/reana_job_controller.json
+-rw-r--r--   0 madonado  (1000) madonado  (1000)   138067 2023-08-03 14:41:17.000000 reana-commons-0.9.3a4/reana_commons/openapi_specifications/reana_server.json
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    50761 2023-08-03 14:41:17.000000 reana-commons-0.9.3a4/reana_commons/openapi_specifications/reana_workflow_controller.json
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6328 2023-07-20 08:32:36.000000 reana-commons-0.9.3a4/reana_commons/publisher.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     8302 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/serial.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     7051 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/snakemake.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     4101 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/reana_commons/specification.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    17086 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/reana_commons/utils.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.782759 reana-commons-0.9.3a4/reana_commons/validation/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      268 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/validation/__init__.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6129 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/validation/compute_backends.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2093 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/validation/operational_options.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    17863 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/validation/parameters.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.782759 reana-commons-0.9.3a4/reana_commons/validation/schemas/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6528 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/reana_commons/validation/schemas/reana_analysis_schema.json
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2779 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/validation/utils.py
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)      458 2023-08-03 14:41:17.000000 reana-commons-0.9.3a4/reana_commons/version.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     7404 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/workflow_engine.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     7536 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/workspace.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2163 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/reana_commons/yadage.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.780759 reana-commons-0.9.3a4/reana_commons.egg-info/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    13828 2023-08-03 14:42:51.000000 reana-commons-0.9.3a4/reana_commons.egg-info/PKG-INFO
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1702 2023-08-03 14:42:51.000000 reana-commons-0.9.3a4/reana_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)        1 2023-08-03 14:42:51.000000 reana-commons-0.9.3a4/reana_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)        1 2023-08-03 14:42:51.000000 reana-commons-0.9.3a4/reana_commons.egg-info/not-zip-safe
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      766 2023-08-03 14:42:51.000000 reana-commons-0.9.3a4/reana_commons.egg-info/requires.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)       14 2023-08-03 14:42:51.000000 reana-commons-0.9.3a4/reana_commons.egg-info/top_level.txt
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)     1172 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/run-tests.sh
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      136 2023-08-03 14:42:51.783759 reana-commons-0.9.3a4/setup.cfg
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)     3331 2023-08-03 14:41:17.000000 reana-commons-0.9.3a4/setup.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-03 14:42:51.783759 reana-commons-0.9.3a4/tests/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1317 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/conftest.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      718 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_email.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     3200 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_job_utils.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2700 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_mq.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1659 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_operational_options.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     3925 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_secrets_store.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1383 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_snakemake.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1674 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/tests/test_specification.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     4726 2023-07-20 08:43:18.000000 reana-commons-0.9.3a4/tests/test_utils.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1004 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_validation.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      446 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_version.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    10248 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tests/test_workspace.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      333 2023-06-22 07:54:05.000000 reana-commons-0.9.3a4/tox.ini
```

### Comparing `reana-commons-0.9.3a3/AUTHORS.rst` & `reana-commons-0.9.3a4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/CHANGES.rst` & `reana-commons-0.9.3a4/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,24 @@
 =======
 
 Version 0.9.3 (UNRELEASED)
 --------------------------
 
 - Adds OpenAPI specification support for ``prune_workspace`` endpoint that allows to delete files that are neither inputs nor outputs from the workspace.
 - Adds support for ``tests.files`` in ``reana.yaml`` allowing to specify Gherking feature files for testing.
+- Changes the server OpenAPI specification to add the `maximum_interactive_session_inactivity_period` value to the `info` endpoint.
 - Changes email sending to allow configuring authentication and encryption options.
 - Fixes the verbs used to describe changes to the status of a workflow in order to avoid incorrect phrases such as ``workflow has been failed``.
 - Fixes the loading of Snakemake and CWL workflow specifications when no parameters are specified.
 
+Version 0.9.2.1 (2023-07-19)
+----------------------------
+
+- Changes ``PyYAML`` dependency version bounds in order to fix installation on Python 3.10+.
+
 Version 0.9.2 (2023-02-10)
 --------------------------
 
 - Fixes ``wcmatch`` dependency version specification.
 
 Version 0.9.1 (2023-01-18)
 --------------------------
```

### Comparing `reana-commons-0.9.3a3/CONTRIBUTING.rst` & `reana-commons-0.9.3a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/LICENSE` & `reana-commons-0.9.3a4/LICENSE`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/MANIFEST.in` & `reana-commons-0.9.3a4/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 include *.yaml
 include *.yml
 include .dockerignore
 include .flake8
 include LICENSE
 include pytest.ini
 include tox.ini
+exclude .readthedocs.yaml
 prune docs/_build
 recursive-include docs *.png
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include reana_commons *.json
 recursive-include reana_commons *.py
```

### Comparing `reana-commons-0.9.3a3/PKG-INFO` & `reana-commons-0.9.3a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reana-commons
-Version: 0.9.3a3
+Version: 0.9.3a4
 Summary: REANA-Commons.
 Home-page: https://github.com/reanahub/reana-commons
 Author: REANA
 Author-email: info@reana.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -96,18 +96,24 @@
 =======
 
 Version 0.9.3 (UNRELEASED)
 --------------------------
 
 - Adds OpenAPI specification support for ``prune_workspace`` endpoint that allows to delete files that are neither inputs nor outputs from the workspace.
 - Adds support for ``tests.files`` in ``reana.yaml`` allowing to specify Gherking feature files for testing.
+- Changes the server OpenAPI specification to add the `maximum_interactive_session_inactivity_period` value to the `info` endpoint.
 - Changes email sending to allow configuring authentication and encryption options.
 - Fixes the verbs used to describe changes to the status of a workflow in order to avoid incorrect phrases such as ``workflow has been failed``.
 - Fixes the loading of Snakemake and CWL workflow specifications when no parameters are specified.
 
+Version 0.9.2.1 (2023-07-19)
+----------------------------
+
+- Changes ``PyYAML`` dependency version bounds in order to fix installation on Python 3.10+.
+
 Version 0.9.2 (2023-02-10)
 --------------------------
 
 - Fixes ``wcmatch`` dependency version specification.
 
 Version 0.9.1 (2023-01-18)
 --------------------------
```

### Comparing `reana-commons-0.9.3a3/README.rst` & `reana-commons-0.9.3a4/README.rst`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/docs/conf.py` & `reana-commons-0.9.3a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/docs/index.rst` & `reana-commons-0.9.3a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/api_client.py` & `reana-commons-0.9.3a4/reana_commons/api_client.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/config.py` & `reana-commons-0.9.3a4/reana_commons/config.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/consumer.py` & `reana-commons-0.9.3a4/reana_commons/consumer.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/email.py` & `reana-commons-0.9.3a4/reana_commons/email.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/errors.py` & `reana-commons-0.9.3a4/reana_commons/errors.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/job_utils.py` & `reana-commons-0.9.3a4/reana_commons/job_utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/k8s/api_client.py` & `reana-commons-0.9.3a4/reana_commons/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/k8s/kerberos.py` & `reana-commons-0.9.3a4/reana_commons/k8s/kerberos.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/k8s/secrets.py` & `reana-commons-0.9.3a4/reana_commons/k8s/secrets.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/k8s/volumes.py` & `reana-commons-0.9.3a4/reana_commons/k8s/volumes.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_job_controller.json` & `reana-commons-0.9.3a4/reana_commons/openapi_specifications/reana_job_controller.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6527777777777778%*

 * *Differences: {"'info'": "{'version': '0.9.1a2'}", 'delete': "['parameters', 'tags']"}*

```diff
@@ -118,17 +118,16 @@
             ],
             "type": "object"
         }
     },
     "info": {
         "description": "REANA Job Controller API",
         "title": "reana-job-controller",
-        "version": "0.9.0a5"
+        "version": "0.9.1a2"
     },
-    "parameters": {},
     "paths": {
         "/apispec": {},
         "/job_cache": {
             "get": {
                 "description": "This resource takes a job specification and the workflow json, and checks if the job to be created, already exists in the cache.",
                 "operationId": "check_if_cached",
                 "parameters": [
@@ -409,10 +408,9 @@
                         }
                     }
                 },
                 "summary": "Returns the logs for a given job."
             }
         }
     },
-    "swagger": "2.0",
-    "tags": []
+    "swagger": "2.0"
 }
```

### Comparing `reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_server.json` & `reana-commons-0.9.3a4/reana_commons/openapi_specifications/reana_server.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4861110664580475%*

 * *Differences: {"'info'": "{'version': '0.9.1a3'}",*

 * * "'paths'": "{'/api/info': {'get': {'responses': {'200': {'schema': {'properties': "*

 * *            "{'maximum_interactive_session_inactivity_period': OrderedDict([('properties', "*

 * *            "OrderedDict([('title', OrderedDict([('type', 'string')])), ('value', "*

 * *            "OrderedDict([('type', 'string'), ('x-nullable', True)]))])), ('type', "*

 * *            "'object')])}}}}}}}",*

 * * 'delete': "['definitions', 'parameters', 'tags']"}*

```diff
@@ -1,15 +1,13 @@
 {
-    "definitions": {},
     "info": {
         "description": "Submit workflows to be run on REANA Cloud",
         "title": "REANA Server",
-        "version": "0.9.1a1"
+        "version": "0.9.1a3"
     },
-    "parameters": {},
     "paths": {
         "/account/settings/linkedaccounts/": {},
         "/account/settings/linkedaccounts/static/{filename}": {},
         "/account/settings/login": {},
         "/account/settings/security/": {},
         "/account/settings/sessions/revoke/": {},
         "/account/settings/static/{filename}": {},
@@ -451,14 +449,26 @@
                                         "value": {
                                             "type": "string",
                                             "x-nullable": true
                                         }
                                     },
                                     "type": "object"
                                 },
+                                "maximum_interactive_session_inactivity_period": {
+                                    "properties": {
+                                        "title": {
+                                            "type": "string"
+                                        },
+                                        "value": {
+                                            "type": "string",
+                                            "x-nullable": true
+                                        }
+                                    },
+                                    "type": "object"
+                                },
                                 "maximum_kubernetes_jobs_timeout": {
                                     "properties": {
                                         "title": {
                                             "type": "string"
                                         },
                                         "value": {
                                             "type": "string"
@@ -4434,10 +4444,9 @@
         "/oauth/login": {},
         "/oauth/login/{remote_app}/": {},
         "/oauth/signup/{remote_app}/": {},
         "/oauth/static/{filename}": {},
         "/signin": {},
         "/signup/": {}
     },
-    "swagger": "2.0",
-    "tags": []
+    "swagger": "2.0"
 }
```

### Comparing `reana-commons-0.9.3a3/reana_commons/openapi_specifications/reana_workflow_controller.json` & `reana-commons-0.9.3a4/reana_commons/openapi_specifications/reana_workflow_controller.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48611111111111116%*

 * *Differences: {"'info'": "{'version': '0.9.1a2'}", 'delete': "['definitions', 'parameters', 'tags']"}*

```diff
@@ -1,15 +1,13 @@
 {
-    "definitions": {},
     "info": {
         "description": "Submit and manage workflows",
         "title": "REANA Workflow Controller",
-        "version": "0.9.0a6"
+        "version": "0.9.1a2"
     },
-    "parameters": {},
     "paths": {
         "/api/workflows": {
             "get": {
                 "description": "This resource is expecting a user UUID. The information related to all workflows for a given user will be served as JSON",
                 "operationId": "get_workflows",
                 "parameters": [
                     {
@@ -1546,10 +1544,9 @@
                         }
                     }
                 },
                 "summary": "Returns the requested file."
             }
         }
     },
-    "swagger": "2.0",
-    "tags": []
+    "swagger": "2.0"
 }
```

### Comparing `reana-commons-0.9.3a3/reana_commons/publisher.py` & `reana-commons-0.9.3a4/reana_commons/publisher.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/serial.py` & `reana-commons-0.9.3a4/reana_commons/serial.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/snakemake.py` & `reana-commons-0.9.3a4/reana_commons/snakemake.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/specification.py` & `reana-commons-0.9.3a4/reana_commons/specification.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/utils.py` & `reana-commons-0.9.3a4/reana_commons/utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/validation/compute_backends.py` & `reana-commons-0.9.3a4/reana_commons/validation/compute_backends.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/validation/operational_options.py` & `reana-commons-0.9.3a4/reana_commons/validation/operational_options.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/validation/parameters.py` & `reana-commons-0.9.3a4/reana_commons/validation/parameters.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/validation/schemas/reana_analysis_schema.json` & `reana-commons-0.9.3a4/reana_commons/validation/schemas/reana_analysis_schema.json`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/validation/utils.py` & `reana-commons-0.9.3a4/reana_commons/validation/utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/workflow_engine.py` & `reana-commons-0.9.3a4/reana_commons/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/workspace.py` & `reana-commons-0.9.3a4/reana_commons/workspace.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons/yadage.py` & `reana-commons-0.9.3a4/reana_commons/yadage.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons.egg-info/PKG-INFO` & `reana-commons-0.9.3a4/reana_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reana-commons
-Version: 0.9.3a3
+Version: 0.9.3a4
 Summary: REANA-Commons.
 Home-page: https://github.com/reanahub/reana-commons
 Author: REANA
 Author-email: info@reana.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -96,18 +96,24 @@
 =======
 
 Version 0.9.3 (UNRELEASED)
 --------------------------
 
 - Adds OpenAPI specification support for ``prune_workspace`` endpoint that allows to delete files that are neither inputs nor outputs from the workspace.
 - Adds support for ``tests.files`` in ``reana.yaml`` allowing to specify Gherking feature files for testing.
+- Changes the server OpenAPI specification to add the `maximum_interactive_session_inactivity_period` value to the `info` endpoint.
 - Changes email sending to allow configuring authentication and encryption options.
 - Fixes the verbs used to describe changes to the status of a workflow in order to avoid incorrect phrases such as ``workflow has been failed``.
 - Fixes the loading of Snakemake and CWL workflow specifications when no parameters are specified.
 
+Version 0.9.2.1 (2023-07-19)
+----------------------------
+
+- Changes ``PyYAML`` dependency version bounds in order to fix installation on Python 3.10+.
+
 Version 0.9.2 (2023-02-10)
 --------------------------
 
 - Fixes ``wcmatch`` dependency version specification.
 
 Version 0.9.1 (2023-01-18)
 --------------------------
```

### Comparing `reana-commons-0.9.3a3/reana_commons.egg-info/SOURCES.txt` & `reana-commons-0.9.3a4/reana_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/reana_commons.egg-info/requires.txt` & `reana-commons-0.9.3a4/reana_commons.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 bravado<10.4,>=10.2
 checksumdir<1.2,>=1.1.4
 click>=7.0
 fs>=2.0
 jsonschema[format]<4.0.0,>=3.0.1
 kombu>=4.6
 mock<4,>=3.0
-PyYAML<6.0,>=5.1
+PyYAML<7.0,>=5.1
 Werkzeug>=0.14.1
 wcmatch<8.5,>=8.3
 
 [all]
 Sphinx>=1.5.1
 sphinx-rtd-theme>=0.1.9
 pytest-reana<0.10.0,>=0.9.0a6
```

### Comparing `reana-commons-0.9.3a3/run-tests.sh` & `reana-commons-0.9.3a4/run-tests.sh`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/setup.py` & `reana-commons-0.9.3a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     "bravado>=10.2,<10.4",
     "checksumdir>=1.1.4,<1.2",
     "click>=7.0",
     "fs>=2.0",
     "jsonschema[format]>=3.0.1,<4.0.0",
     "kombu>=4.6",
     "mock>=3.0,<4",
-    "PyYAML>=5.1,<6.0",
+    "PyYAML>=5.1,<7.0",
     "Werkzeug>=0.14.1",
     "wcmatch>=8.3,<8.5",
 ]
 
 packages = find_packages()
```

### Comparing `reana-commons-0.9.3a3/tests/conftest.py` & `reana-commons-0.9.3a4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_email.py` & `reana-commons-0.9.3a4/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_job_utils.py` & `reana-commons-0.9.3a4/tests/test_job_utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_mq.py` & `reana-commons-0.9.3a4/tests/test_mq.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_operational_options.py` & `reana-commons-0.9.3a4/tests/test_operational_options.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_secrets_store.py` & `reana-commons-0.9.3a4/tests/test_secrets_store.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_snakemake.py` & `reana-commons-0.9.3a4/tests/test_snakemake.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_specification.py` & `reana-commons-0.9.3a4/tests/test_specification.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_utils.py` & `reana-commons-0.9.3a4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_validation.py` & `reana-commons-0.9.3a4/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `reana-commons-0.9.3a3/tests/test_workspace.py` & `reana-commons-0.9.3a4/tests/test_workspace.py`

 * *Files identical despite different names*

