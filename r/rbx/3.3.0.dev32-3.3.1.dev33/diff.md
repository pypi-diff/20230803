# Comparing `tmp/rbx-3.3.0.dev32.tar.gz` & `tmp/rbx-3.3.1.dev33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbx-3.3.0.dev32.tar", last modified: Tue Jul 18 13:52:11 2023, max compression
+gzip compressed data, was "rbx-3.3.1.dev33.tar", last modified: Thu Aug  3 08:51:57 2023, max compression
```

## Comparing `rbx-3.3.0.dev32.tar` & `rbx-3.3.1.dev33.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.818238 rbx-3.3.0.dev32/rbx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/auth/keystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/aws/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx/buildtools/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 13:52:10.000000 rbx-3.3.0.dev32/rbx/buildtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx/buildtools/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/adsquare.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/broadsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/oxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/uslicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/gcp/cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/geo/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/geo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/geo/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/geo/packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/manifest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/manifest/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/manifest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/queues/
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/queues/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/queues/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/utils/mdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/web/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-18 13:52:10.000000 rbx-3.3.0.dev32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.367916 rbx-3.3.1.dev33/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 08:51:57.367916 rbx-3.3.1.dev33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.363916 rbx-3.3.1.dev33/rbx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.363916 rbx-3.3.1.dev33/rbx/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/auth/keystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.363916 rbx-3.3.1.dev33/rbx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/aws/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.363916 rbx-3.3.1.dev33/rbx/buildtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/buildtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 08:51:56.000000 rbx-3.3.1.dev33/rbx/buildtools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.363916 rbx-3.3.1.dev33/rbx/buildtools/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/buildtools/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/buildtools/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/buildtools/tasks/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/buildtools/tasks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/buildtools/tasks/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.363916 rbx-3.3.1.dev33/rbx/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/clients/adsquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/clients/broadsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/clients/oxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/clients/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/clients/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/clients/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/clients/uslicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.363916 rbx-3.3.1.dev33/rbx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/gcp/cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/gcp/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.367916 rbx-3.3.1.dev33/rbx/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/geo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/geo/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/geo/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.367916 rbx-3.3.1.dev33/rbx/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/manifest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/manifest/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/manifest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.367916 rbx-3.3.1.dev33/rbx/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/queues/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/queues/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.367916 rbx-3.3.1.dev33/rbx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/utils/mdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.367916 rbx-3.3.1.dev33/rbx/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-03 08:51:36.000000 rbx-3.3.1.dev33/rbx/web/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:51:57.363916 rbx-3.3.1.dev33/rbx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 08:51:57.000000 rbx-3.3.1.dev33/rbx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-03 08:51:57.000000 rbx-3.3.1.dev33/rbx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:51:57.000000 rbx-3.3.1.dev33/rbx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-03 08:51:57.000000 rbx-3.3.1.dev33/rbx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-03 08:51:57.000000 rbx-3.3.1.dev33/rbx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 08:51:57.000000 rbx-3.3.1.dev33/rbx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:51:57.367916 rbx-3.3.1.dev33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-03 08:51:56.000000 rbx-3.3.1.dev33/setup.py
```

### Comparing `rbx-3.3.0.dev32/LICENSE` & `rbx-3.3.1.dev33/LICENSE`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/PKG-INFO` & `rbx-3.3.1.dev33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.3.0.dev32
+Version: 3.3.1.dev33
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rbx-3.3.0.dev32/rbx/auth/decorators.py` & `rbx-3.3.1.dev33/rbx/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/auth/keystore.py` & `rbx-3.3.1.dev33/rbx/auth/keystore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from dataclasses import asdict, dataclass, field, InitVar
 import logging
 import os
 from unittest import mock
 
 import google.auth.credentials
+from google.api_core import retry
+from google.api_core.exceptions import RetryError
 from google.cloud.firestore import Client
 
-from ..clients import retry
+from ..clients.retry import Retry
 from ..exceptions import TransientException
 from ..settings import RBX_PROJECT
 
 logger = logging.getLogger("rbx.auth")
+default_retry = retry.Retry(initial=0.1, maximum=3.0, multiplier=1.3, deadline=10.0)
 
 
 class Keystore:
     """Manages API Keys stored in Google Cloud Firestore (Native Mode)."""
 
     def __init__(self):
         if os.getenv("GAE_ENV", "").startswith("standard"):
@@ -36,21 +39,21 @@
         """Given a DocumentSnapshot, return the fully loaded Key object."""
         return Key(**{"keystore": self, "key_id": document.id, **document.to_dict()})
 
     def add_campaign(self, campaign):
         """Add a campaign to the campaigns inventory."""
         self.add_campaigns([campaign])
 
-    @retry.Retry(deadline=300.0)
+    @Retry(deadline=120.0)
     def add_campaigns(self, campaigns):
         """Add campaigns to the campaigns inventory."""
         inventory = self.get_inventory()
         inventory.add(campaigns)
 
-    @retry.Retry(deadline=300.0)
+    @Retry(deadline=120.0)
     def create_key(
         self, email, name, campaigns=None, is_restricted=None, services=None
     ):
         """Make a new API key.
 
         A key is associated with a user via her email address. If a key already exists for that
         user, the key is updated instead.
@@ -62,19 +65,19 @@
                 "email": email,
                 "is_restricted": is_restricted if is_restricted is not None else True,
                 "name": name,
                 "services": services if services is not None else ["*.*"],
                 "status": "active",
             }
 
-            _, ref = self.collection.add(key)
-            if not ref.get().exists:
-                raise TransientException(f"Failed to create key for {email}")
-
-            key = self._key(ref.get())
+            try:
+                _, ref = self.collection.add(key, retry=default_retry)
+                key = self._key(ref.get(retry=default_retry))
+            except RetryError as e:
+                raise TransientException(e)
         else:
             key.update(
                 **{
                     "campaigns": campaigns or key.campaigns,
                     "is_restricted": is_restricted
                     if is_restricted is not None
                     else key.is_restricted,
@@ -96,45 +99,60 @@
         if not inventory:
             return []
 
         return inventory.values
 
     def get_inventory(self, key="campaigns"):
         """Retrieve a key from the inventory."""
-        document = self.inventory.document(key).get()
+        try:
+            document = self.inventory.document(key).get(retry=default_retry)
+        except RetryError as e:
+            raise TransientException(e)
+
         if not document.exists:
             return Inventory(key=key, keystore=self)
         else:
             return self._inventory(key, document)
 
     def get_key(self, key_id=None, email=None):
         """Retrieve a key by ID or email."""
         key = None
 
-        if key_id:
-            document = self.collection.document(key_id).get()
-            if document.exists:
-                key = self._key(document)
-
-        if email:
-            document = next(self.collection.where("email", "==", email).stream(), False)
-            if document:
-                key = self._key(document)
+        try:
+            if key_id:
+                document = self.collection.document(key_id).get(retry=default_retry)
+                if document.exists:
+                    key = self._key(document)
+
+            if email:
+                document = next(
+                    self.collection.where("email", "==", email).stream(
+                        retry=default_retry
+                    ),
+                    False,
+                )
+                if document:
+                    key = self._key(document)
+        except RetryError as e:
+            raise TransientException(e)
 
         # Unrestricted keys get access to all inventory
         if key and not key.is_restricted:
             key.campaigns = self.get_campaigns()
 
         return key
 
     def update_key(self, key, attributes):
         """Set the new Key values in Firestore."""
         assert isinstance(key, Key), f"excepted rbx.auth.Key, got {type(key)}"
         document = self.collection.document(key.key_id)
-        document.set(attributes, merge=True)
+        try:
+            document.set(attributes, merge=True, retry=default_retry)
+        except RetryError as e:
+            raise TransientException(e)
 
 
 @dataclass
 class Inventory:
     key: InitVar[str]
     keystore: InitVar[Keystore]
     values: list = field(default_factory=list)
@@ -143,15 +161,20 @@
         self.key = key
         self.keystore = keystore
 
     def add(self, added_values):
         values = set(self.values)
         values.update(set(added_values))
         document = self.keystore.inventory.document(self.key)
-        document.set({"values": sorted(list(values))}, merge=True)
+        try:
+            document.set(
+                {"values": sorted(list(values))}, merge=True, retry=default_retry
+            )
+        except RetryError as e:
+            raise TransientException(e)
 
 
 @dataclass
 class Key:
     key_id: InitVar[str]
     keystore: InitVar[Keystore]
     email: str
```

### Comparing `rbx-3.3.0.dev32/rbx/aws/s3.py` & `rbx-3.3.1.dev33/rbx/aws/s3.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/buildtools/tasks/deploy.py` & `rbx-3.3.1.dev33/rbx/buildtools/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/buildtools/tasks/image.py` & `rbx-3.3.1.dev33/rbx/buildtools/tasks/image.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/buildtools/tasks/misc.py` & `rbx-3.3.1.dev33/rbx/buildtools/tasks/misc.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/clients/__init__.py` & `rbx-3.3.1.dev33/rbx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/clients/adsquare.py` & `rbx-3.3.1.dev33/rbx/clients/adsquare.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/clients/broadsign.py` & `rbx-3.3.1.dev33/rbx/clients/broadsign.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/clients/oxr.py` & `rbx-3.3.1.dev33/rbx/clients/oxr.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/clients/panels.py` & `rbx-3.3.1.dev33/rbx/clients/panels.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/clients/reporting.py` & `rbx-3.3.1.dev33/rbx/clients/reporting.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/clients/retry.py` & `rbx-3.3.1.dev33/rbx/clients/retry.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/clients/uslicer.py` & `rbx-3.3.1.dev33/rbx/clients/uslicer.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/exceptions.py` & `rbx-3.3.1.dev33/rbx/exceptions.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/gcp/cloud_tasks.py` & `rbx-3.3.1.dev33/rbx/gcp/cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/gcp/pubsub.py` & `rbx-3.3.1.dev33/rbx/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/gcp/storage.py` & `rbx-3.3.1.dev33/rbx/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/geo/__init__.py` & `rbx-3.3.1.dev33/rbx/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/geo/cli.py` & `rbx-3.3.1.dev33/rbx/geo/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/geo/maps.py` & `rbx-3.3.1.dev33/rbx/geo/maps.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/geo/packer.py` & `rbx-3.3.1.dev33/rbx/geo/packer.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/logging.py` & `rbx-3.3.1.dev33/rbx/logging.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/manifest/cli.py` & `rbx-3.3.1.dev33/rbx/manifest/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/manifest/processor.py` & `rbx-3.3.1.dev33/rbx/manifest/processor.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/manifest/utils.py` & `rbx-3.3.1.dev33/rbx/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/queues/__init__.py` & `rbx-3.3.1.dev33/rbx/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/queues/jobs.py` & `rbx-3.3.1.dev33/rbx/queues/jobs.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/queues/scheduler.py` & `rbx-3.3.1.dev33/rbx/queues/scheduler.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/utils/__init__.py` & `rbx-3.3.1.dev33/rbx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx/web/handlers.py` & `rbx-3.3.1.dev33/rbx/web/handlers.py`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx.egg-info/PKG-INFO` & `rbx-3.3.1.dev33/rbx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.3.0.dev32
+Version: 3.3.1.dev33
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rbx-3.3.0.dev32/rbx.egg-info/SOURCES.txt` & `rbx-3.3.1.dev33/rbx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/rbx.egg-info/requires.txt` & `rbx-3.3.1.dev33/rbx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.3.0.dev32/setup.py` & `rbx-3.3.1.dev33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 STORAGE = ["google-cloud-storage>=2.1,<3"]
 TASKS = ["google-cloud-tasks>=2.7,<3"]
 WEB = ["google-cloud-error-reporting>=1.9.2,<2"]
 
 
 setup(
     name="rbx",
-    version="3.3.0.dev32",
+    version="3.3.1.dev33",
     license="Apache 2.0",
     description="Scoota Platform utilities",
     long_description="A collection of common tools for Scoota services.",
     url="http://scoota.com/",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

