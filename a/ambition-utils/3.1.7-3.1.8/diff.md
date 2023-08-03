# Comparing `tmp/ambition-utils-3.1.7.tar.gz` & `tmp/ambition-utils-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambition-utils-3.1.7.tar", last modified: Mon Jul 24 13:58:37 2023, max compression
+gzip compressed data, was "ambition-utils-3.1.8.tar", last modified: Thu Aug  3 15:09:45 2023, max compression
```

## Comparing `ambition-utils-3.1.7.tar` & `ambition-utils-3.1.8.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.592221 ambition-utils-3.1.7/
--rw-r--r--   0 tneu       (501) staff       (20)     1075 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/LICENSE
--rw-r--r--   0 tneu       (501) staff       (20)       68 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/MANIFEST.in
--rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-07-24 13:58:37.592290 ambition-utils-3.1.7/PKG-INFO
--rw-r--r--   0 tneu       (501) staff       (20)     1114 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/README.rst
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.579753 ambition-utils-3.1.7/ambition_utils/
--rw-r--r--   0 tneu       (501) staff       (20)       48 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/__init__.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.580984 ambition-utils-3.1.7/ambition_utils/activity/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/activity/__init__.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.581583 ambition-utils-3.1.7/ambition_utils/activity/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)     2231 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/activity/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)     1656 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/activity/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     4446 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/activity/models.py
--rw-r--r--   0 tneu       (501) staff       (20)     2737 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/activity/tasks.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.581968 ambition-utils-3.1.7/ambition_utils/activity/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/activity/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      229 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/activity/tests/model_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)     2794 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/activity/tests/task_tests.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.582242 ambition-utils-3.1.7/ambition_utils/anomaly/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/anomaly/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     9762 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/anomaly/models.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.582895 ambition-utils-3.1.7/ambition_utils/anomaly/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     6036 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/anomaly_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)      202 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/apps.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.583197 ambition-utils-3.1.7/ambition_utils/anomaly/tests/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)     2644 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      928 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/models.py
--rw-r--r--   0 tneu       (501) staff       (20)      138 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/apps.py
--rw-r--r--   0 tneu       (501) staff       (20)     2545 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/fields.py
--rw-r--r--   0 tneu       (501) staff       (20)    13636 2023-01-26 16:48:58.000000 ambition-utils-3.1.7/ambition_utils/forms.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.583658 ambition-utils-3.1.7/ambition_utils/postgres_lock/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     3782 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/lock.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.584403 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)      487 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)      434 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
--rw-r--r--   0 tneu       (501) staff       (20)      581 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      875 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/models.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.584608 ambition-utils-3.1.7/ambition_utils/postgres_lock/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     4399 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/tests/lock_tests.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.585744 ambition-utils-3.1.7/ambition_utils/rrule/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/rrule/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      162 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/apps.py
--rw-r--r--   0 tneu       (501) staff       (20)      127 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/rrule/constants.py
--rw-r--r--   0 tneu       (501) staff       (20)     9900 2023-07-20 18:18:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/forms.py
--rw-r--r--   0 tneu       (501) staff       (20)      389 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/rrule/handler.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.587303 ambition-utils-3.1.7/ambition_utils/rrule/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)      927 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)      415 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
--rw-r--r--   0 tneu       (501) staff       (20)      936 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
--rw-r--r--   0 tneu       (501) staff       (20)      486 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)    18825 2023-07-20 21:45:03.000000 ambition-utils-3.1.7/ambition_utils/rrule/models.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.588442 ambition-utils-3.1.7/ambition_utils/rrule/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      200 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/apps.py
--rw-r--r--   0 tneu       (501) staff       (20)    18459 2023-07-20 18:18:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/form_tests.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.588755 ambition-utils-3.1.7/ambition_utils/rrule/tests/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)     1005 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)    56586 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/model_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)      713 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/models.py
--rw-r--r--   0 tneu       (501) staff       (20)     7349 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/sql.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.590078 ambition-utils-3.1.7/ambition_utils/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      190 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/apps.py
--rw-r--r--   0 tneu       (501) staff       (20)     2556 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/tests/field_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)    16249 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/tests/form_tests.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.590676 ambition-utils-3.1.7/ambition_utils/tests/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)      489 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)      685 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      364 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/models.py
--rw-r--r--   0 tneu       (501) staff       (20)     3144 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/sql_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)     3435 2022-11-29 21:40:08.000000 ambition-utils-3.1.7/ambition_utils/tests/time_helper_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)     4765 2022-11-29 21:40:08.000000 ambition-utils-3.1.7/ambition_utils/time_helpers.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.591284 ambition-utils-3.1.7/ambition_utils/transaction/
--rw-r--r--   0 tneu       (501) staff       (20)       46 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/transaction/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     2261 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/transaction/decorators.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.591564 ambition-utils-3.1.7/ambition_utils/transaction/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/transaction/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     2032 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/transaction/tests/durable_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)     2666 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/transaction/utils.py
--rw-r--r--   0 tneu       (501) staff       (20)       38 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/urls.py
--rw-r--r--   0 tneu       (501) staff       (20)       22 2023-07-20 21:59:50.000000 ambition-utils-3.1.7/ambition_utils/version.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.580468 ambition-utils-3.1.7/ambition_utils.egg-info/
--rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/PKG-INFO
--rw-r--r--   0 tneu       (501) staff       (20)     3085 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/SOURCES.txt
--rw-r--r--   0 tneu       (501) staff       (20)        1 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/dependency_links.txt
--rw-r--r--   0 tneu       (501) staff       (20)      262 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/requires.txt
--rw-r--r--   0 tneu       (501) staff       (20)       15 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/top_level.txt
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.592085 ambition-utils-3.1.7/requirements/
--rw-r--r--   0 tneu       (501) staff       (20)       31 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/requirements/docs.txt
--rw-r--r--   0 tneu       (501) staff       (20)       96 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/requirements/requirements-testing.txt
--rw-r--r--   0 tneu       (501) staff       (20)      160 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/requirements/requirements.txt
--rw-r--r--   0 tneu       (501) staff       (20)      252 2023-07-24 13:58:37.592647 ambition-utils-3.1.7/setup.cfg
--rw-r--r--   0 tneu       (501) staff       (20)     1914 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/setup.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.609560 ambition-utils-3.1.8/
+-rw-r--r--   0 tneu       (501) staff       (20)     1075 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/LICENSE
+-rw-r--r--   0 tneu       (501) staff       (20)       68 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/MANIFEST.in
+-rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-08-03 15:09:45.609631 ambition-utils-3.1.8/PKG-INFO
+-rw-r--r--   0 tneu       (501) staff       (20)     1114 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/README.rst
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.597344 ambition-utils-3.1.8/ambition_utils/
+-rw-r--r--   0 tneu       (501) staff       (20)       48 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/__init__.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.598469 ambition-utils-3.1.8/ambition_utils/activity/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/activity/__init__.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.599104 ambition-utils-3.1.8/ambition_utils/activity/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     2231 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/activity/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)     1656 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/activity/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4446 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/activity/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2737 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/activity/tasks.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.599475 ambition-utils-3.1.8/ambition_utils/activity/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/activity/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      229 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/activity/tests/model_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2794 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/activity/tests/task_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.599738 ambition-utils-3.1.8/ambition_utils/anomaly/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/anomaly/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     9762 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/anomaly/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.600468 ambition-utils-3.1.8/ambition_utils/anomaly/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     6036 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/anomaly_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)      202 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/apps.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.600787 ambition-utils-3.1.8/ambition_utils/anomaly/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     2644 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      928 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)      138 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2545 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/fields.py
+-rw-r--r--   0 tneu       (501) staff       (20)    13636 2023-01-26 16:48:58.000000 ambition-utils-3.1.8/ambition_utils/forms.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.601279 ambition-utils-3.1.8/ambition_utils/postgres_lock/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3782 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/lock.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.602014 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      487 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      434 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
+-rw-r--r--   0 tneu       (501) staff       (20)      581 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      875 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.602235 ambition-utils-3.1.8/ambition_utils/postgres_lock/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4399 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/tests/lock_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.603343 ambition-utils-3.1.8/ambition_utils/rrule/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/rrule/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      162 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)      127 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/rrule/constants.py
+-rw-r--r--   0 tneu       (501) staff       (20)     9900 2023-07-20 18:18:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/forms.py
+-rw-r--r--   0 tneu       (501) staff       (20)      389 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/rrule/handler.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.604541 ambition-utils-3.1.8/ambition_utils/rrule/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      927 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      415 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
+-rw-r--r--   0 tneu       (501) staff       (20)      936 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
+-rw-r--r--   0 tneu       (501) staff       (20)      486 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
+-rw-r--r--   0 tneu       (501) staff       (20)      412 2023-08-03 14:04:44.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0005_auto_20230802_1548.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)    18906 2023-08-03 14:04:44.000000 ambition-utils-3.1.8/ambition_utils/rrule/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.605796 ambition-utils-3.1.8/ambition_utils/rrule/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      200 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)    18459 2023-07-20 18:18:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/form_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.606192 ambition-utils-3.1.8/ambition_utils/rrule/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     1005 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)    60914 2023-08-03 14:04:44.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/model_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)      713 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     7349 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/sql.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.607418 ambition-utils-3.1.8/ambition_utils/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      190 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2556 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/tests/field_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)    16249 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/tests/form_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.607987 ambition-utils-3.1.8/ambition_utils/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      489 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      685 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      364 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3144 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/sql_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3435 2022-11-29 21:40:08.000000 ambition-utils-3.1.8/ambition_utils/tests/time_helper_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4765 2022-11-29 21:40:08.000000 ambition-utils-3.1.8/ambition_utils/time_helpers.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.608487 ambition-utils-3.1.8/ambition_utils/transaction/
+-rw-r--r--   0 tneu       (501) staff       (20)       46 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/transaction/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2261 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/transaction/decorators.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.608780 ambition-utils-3.1.8/ambition_utils/transaction/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/transaction/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2032 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/transaction/tests/durable_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2666 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/transaction/utils.py
+-rw-r--r--   0 tneu       (501) staff       (20)       38 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/urls.py
+-rw-r--r--   0 tneu       (501) staff       (20)       22 2023-08-03 14:06:21.000000 ambition-utils-3.1.8/ambition_utils/version.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.597983 ambition-utils-3.1.8/ambition_utils.egg-info/
+-rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/PKG-INFO
+-rw-r--r--   0 tneu       (501) staff       (20)     3144 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 tneu       (501) staff       (20)        1 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      262 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/requires.txt
+-rw-r--r--   0 tneu       (501) staff       (20)       15 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/top_level.txt
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.609433 ambition-utils-3.1.8/requirements/
+-rw-r--r--   0 tneu       (501) staff       (20)       31 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/requirements/docs.txt
+-rw-r--r--   0 tneu       (501) staff       (20)       96 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/requirements/requirements-testing.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      160 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/requirements/requirements.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      252 2023-08-03 15:09:45.610101 ambition-utils-3.1.8/setup.cfg
+-rw-r--r--   0 tneu       (501) staff       (20)     1914 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/setup.py
```

### Comparing `ambition-utils-3.1.7/LICENSE` & `ambition-utils-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/PKG-INFO` & `ambition-utils-3.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.7
+Version: 3.1.8
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Keywords: django,database,query,sql,postgres,upsert
 Platform: UNKNOWN
```

### Comparing `ambition-utils-3.1.7/README.rst` & `ambition-utils-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/activity/migrations/0001_initial.py` & `ambition-utils-3.1.8/ambition_utils/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/activity/migrations/0002_auto_20180427_1819.py` & `ambition-utils-3.1.8/ambition_utils/activity/migrations/0002_auto_20180427_1819.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/activity/models.py` & `ambition-utils-3.1.8/ambition_utils/activity/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/activity/tasks.py` & `ambition-utils-3.1.8/ambition_utils/activity/tasks.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/activity/tests/task_tests.py` & `ambition-utils-3.1.8/ambition_utils/activity/tests/task_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/anomaly/models.py` & `ambition-utils-3.1.8/ambition_utils/anomaly/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/anomaly/tests/anomaly_tests.py` & `ambition-utils-3.1.8/ambition_utils/anomaly/tests/anomaly_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/anomaly/tests/migrations/0001_initial.py` & `ambition-utils-3.1.8/ambition_utils/anomaly/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/anomaly/tests/models.py` & `ambition-utils-3.1.8/ambition_utils/anomaly/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/fields.py` & `ambition-utils-3.1.8/ambition_utils/fields.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/forms.py` & `ambition-utils-3.1.8/ambition_utils/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/postgres_lock/lock.py` & `ambition-utils-3.1.8/ambition_utils/postgres_lock/lock.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py` & `ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/postgres_lock/models.py` & `ambition-utils-3.1.8/ambition_utils/postgres_lock/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/postgres_lock/tests/lock_tests.py` & `ambition-utils-3.1.8/ambition_utils/postgres_lock/tests/lock_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/rrule/forms.py` & `ambition-utils-3.1.8/ambition_utils/rrule/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/rrule/migrations/0001_initial.py` & `ambition-utils-3.1.8/ambition_utils/rrule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py` & `ambition-utils-3.1.8/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/rrule/models.py` & `ambition-utils-3.1.8/ambition_utils/rrule/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,14 +131,17 @@
     related_object_id = models.IntegerField(null=True, db_index=True)
     related_object_content_type = models.ForeignKey(ContentType, null=True, on_delete=models.PROTECT)
     related_object = GenericForeignKey('related_object_content_type', 'related_object_id')
 
     # The name of the method to call on the related_object when the recurrence has expired
     related_object_handler_name = models.TextField(default=None, null=True, blank=True)
 
+    # An optional number of days to offset occurrences by
+    day_offset = models.SmallIntegerField(blank=True, null=True)
+
     # Custom object manager
     objects = RRuleManager()
 
     def get_time_zone_object(self):
         """
         Returns the time zone object from pytz
         """
@@ -210,30 +213,35 @@
 
         # Always cache
         params['cache'] = True
 
         # Return the rrule
         return rrule(**params)
 
-    def get_next_occurrence(self, last_occurrence=None, force=False):
+    def get_next_occurrence(self, last_occurrence=None, calculate_offset=True, force=False):
         """
         Builds the rrule and returns the next date in the series or None of it is the end of the series
         :param last_occurrence: The last occurrence that was generated
+        :param calculate_offset: Should the given offset be calculated?
         :param force: If the next occurrence is none, force the rrule to generate another
         :rtype: rrule or None
         """
         # Get the last occurrence
         last_occurrence = last_occurrence or self.last_occurrence or datetime.utcnow()
 
         # Get the rule set
         rule_set = self.get_rrule_set()
 
         # Convert to local time zone for getting next occurrence, otherwise time zones ahead of utc will return the same
         last_occurrence = fleming.convert_to_tz(last_occurrence, self.get_time_zone_object(), return_naive=True)
 
+        # Un-offset the last occurrence to match the rule_set's dates for .after() before offsetting again later
+        if calculate_offset:
+            last_occurrence = self.offset(last_occurrence, reverse=True)
+
         # Generate the next occurrence
         next_occurrence = rule_set.after(last_occurrence)
 
         # If next occurrence is none and force is true, force the rrule to generate another date
         if next_occurrence is None and force:
             # Keep a reference to the original rrule_params
             original_rrule_params = {}
@@ -252,14 +260,17 @@
             # Restore the rrule params
             self.rrule_params = original_rrule_params
 
         # If there is a next occurrence, convert to utc
         if next_occurrence:
             next_occurrence = self.convert_to_utc(next_occurrence)
 
+            if calculate_offset:
+                next_occurrence = self.offset(next_occurrence)
+
         # Return the next occurrence
         return next_occurrence
 
     def update_next_occurrence(self, save=True):
         """
         Sets the next_occurrence property to the next time in the series and sets the last_occurrence property
         to the previous value of next_occurrence. If the save option is True, the model will be saved. The
@@ -272,14 +283,15 @@
             return None
 
         # Only handle if the current date is >= next occurrence
         if datetime.utcnow() < self.next_occurrence:
             return False
 
         self.last_occurrence = self.next_occurrence
+
         self.next_occurrence = self.get_next_occurrence(self.last_occurrence)
 
         # Only save if the flag is true
         if save:
             self.save(update_fields=['last_occurrence', 'next_occurrence'])
 
     def convert_to_utc(self, dt):
@@ -291,30 +303,47 @@
         dt = fleming.attach_tz_if_none(dt, self.get_time_zone_object())
 
         # Convert to utc
         dt = fleming.convert_to_tz(dt, pytz.utc, return_naive=True)
 
         return dt
 
+    def offset(self, dt, reverse=False) -> datetime:
+        """
+        Offsets a given datetime by the number of days specified by day_offset.
+        :param dt: The datetime to offset by day_offset
+        :param reverse: Reverse the offset calculation.
+        :return dt:
+        """
+        # The offset gets multiplied by 1 or -1 depending on offset direction
+        multiplier = -1 if reverse else 1
+
+        return fleming.add_timedelta(
+            dt,
+            timedelta(days=self.day_offset * multiplier),
+            within_tz=self.time_zone
+        ) if self.day_offset else dt
+
     def refresh_next_occurrence(self, current_time=None):
         """
         Sets the next occurrence date based on the current rrule param definition. The date will be after the
         specified current_time or utcnow.
         :param current_time: Optional datetime object to compute the next time from
         """
         # Get the current time or go off the specified current time
         current_time = current_time or datetime.utcnow()
 
         # Next occurrence is in utc here
         next_occurrence = self.get_next_occurrence(last_occurrence=current_time)
 
         if next_occurrence:
-            # Only set if the new time is still greater than now
+            # Only set if the new time is still greater than now.
+            # Offset date if applicable.
             if next_occurrence > datetime.utcnow():
-                self.next_occurrence = next_occurrence
+                self.next_occurrence = self.offset(next_occurrence)
         else:
             self.next_occurrence = next_occurrence
 
     def pre_save_hooks(self):
         self.set_date_objects()
 
     def set_date_objects(self):
@@ -331,14 +360,17 @@
         if is_new:
             # Get the first scheduled time according to the rrule (this converts from utc back to local time)
             self.next_occurrence = self.get_rrule_set()[0]
 
             # Convert back to utc before saving
             self.next_occurrence = self.convert_to_utc(self.next_occurrence)
 
+        # Offset, if applicable, for old and new.
+        self.next_occurrence = self.offset(self.next_occurrence)
+
     def set_date_objects_for_params(self, params, is_new=False):
         """
         Give an rrule params object, ensure that the date keys are properly set and properly converted to strings
         """
         # Check for no params
         if not params:
             return params
@@ -392,23 +424,24 @@
         try:
             # Capture the rule's first date for use in RRule.after() in the loop.
             rule_set = self.get_rrule_set()
 
             # Evaluate if the first date should be retained.
             d = self.convert_to_utc(rule_set[0])
             if not start_date or d > start_date:
-                dates.append(d)
+                dates.append(self.offset(d))
 
             # Continue evaluating and appending dates to satisfy desired number,
             # retaining date for evaluation in the next iteration.
+            # The offset is ignored for this comparison and applied at appending.
             while len(dates) < num_dates:
-                d = self.get_next_occurrence(last_occurrence=d)
+                d = self.get_next_occurrence(last_occurrence=d, calculate_offset=False)
                 if d:
                     if not start_date or d > start_date:
-                        dates.append(d)
+                        dates.append(self.offset(d))
                 else:
                     break
         except Exception:  # pragma: no cover
             pass
 
         # Return the generated dates
         return dates
@@ -430,49 +463,20 @@
         clone = copy.deepcopy(self)
         clone.id = None
         clone.save()
         return clone
 
     def clone_with_day_offset(self, day_offset: int) -> RRule:
         """
-        Creates a clone of a passed RRule object offset by a specified number of days
+        Creates a clone of a passed RRule object with day_offset set.
         :param day_offset: The number of days to offset the clone's start date. Can be negative.
         """
-
-        # Create a clone of itself
         clone = self.clone()
-
-        # Manually update the rrule.dtstart & next_occurrence with the offset.
-        clone.rrule_params['dtstart'] = parser.parse(clone.rrule_params['dtstart']) + timedelta(days=day_offset)
-        clone.next_occurrence = clone.next_occurrence + timedelta(days=day_offset)
-
-        # Update until param by offsetting if it exists
-        if 'until' in clone.rrule_params:
-            clone.rrule_params['until'] = parser.parse(clone.rrule_params['until']) + timedelta(days=day_offset)
-
-        def offset_day(day: int) -> int:
-            """
-            Calculates the representation of a given day of the week plus the provided offset
-            For example, Tuesday (1) - 3 days yields Saturday (5).
-            :param int day: 0-6 that corresponds to RRule's weekday constants, MO-SU.
-            """
-            return (7 + (day + day_offset)) % 7
-
-        # Update byweekday param by offsetting. byweekday can be an array or integer.
-        if 'byweekday' in clone.rrule_params:
-            if isinstance(clone.rrule_params['byweekday'], list):
-                clone.rrule_params['byweekday'] = [
-                    offset_day(day) for day in clone.rrule_params['byweekday']
-                ]
-            else:
-                clone.rrule_params['byweekday'] = offset_day(clone.rrule_params['byweekday'])
-
-        # Lock it.
+        clone.day_offset = day_offset
         clone.save()
-
         return clone
 
     @classmethod
     def get_dates_from_params(cls, rrule_params, time_zone=None, num_dates=20, start_date=None):
         time_zone = time_zone or pytz.utc
         rule = cls(rrule_params=rrule_params, time_zone=time_zone)
```

### Comparing `ambition-utils-3.1.7/ambition_utils/rrule/tests/form_tests.py` & `ambition-utils-3.1.8/ambition_utils/rrule/tests/form_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/rrule/tests/migrations/0001_initial.py` & `ambition-utils-3.1.8/ambition_utils/rrule/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/rrule/tests/model_tests.py` & `ambition-utils-3.1.8/ambition_utils/rrule/tests/model_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1206,20 +1206,18 @@
 
         # Assert that the rule created here is unchanged but the clones reflect their offsets.
         format = '%Y-%m-%d'
         self.assertEqual(rule.next_occurrence.strftime(format), '2022-06-22')
         self.assertEqual(future_clone.next_occurrence.strftime(format), '2022-06-24')
         self.assertEqual(past_clone.next_occurrence.strftime(format), '2022-06-20')
 
-        # Assert that the rule created here is unchanged but the clone's byweekday params reflect their offsets.
-        # Future: MWF -> WFSu
-        # Past: MWF -> SMW
+        # Assert that the rule and clones all reflect MWF
         self.assertEqual(rule.rrule_params['byweekday'], [0, 2, 4])
-        self.assertEqual(future_clone.rrule_params['byweekday'], [2, 4, 6])
-        self.assertEqual(past_clone.rrule_params['byweekday'], [5, 0, 2])
+        self.assertEqual(future_clone.rrule_params['byweekday'], [0, 2, 4])
+        self.assertEqual(past_clone.rrule_params['byweekday'], [0, 2, 4])
 
         # Assert the generated dates are as expected.
         self.assertEqual(
             rule.get_dates(num_dates=4),
             [
                 datetime.datetime(2022, 6, 22),  # Wednesday
                 datetime.datetime(2022, 6, 24),  # Friday
@@ -1297,21 +1295,21 @@
                 'until': datetime.datetime(2022, 10, 17)
             }
         )
 
         future_clone = rule.clone_with_day_offset(1)
         past_clone = rule.clone_with_day_offset(-1)
 
-        # Assert the updated until values are correct
+        # Assert the cloned until values are the same
         self.assertEqual(
-            parser.parse(rule.rrule_params['until']) + datetime.timedelta(days=1),
+            parser.parse(rule.rrule_params['until']),
             parser.parse(future_clone.rrule_params['until'])
         )
         self.assertEqual(
-            parser.parse(rule.rrule_params['until']) - datetime.timedelta(days=1),
+            parser.parse(rule.rrule_params['until']),
             parser.parse(past_clone.rrule_params['until'])
         )
 
         # Assert the generated dates are as expected for the original.
         self.assertEqual(
             rule.get_dates(),
             [
@@ -1354,30 +1352,30 @@
                 'until': datetime.datetime(2022, 11, 1, 10),
             },
             time_zone=pytz.timezone('Europe/Kiev')
         )
 
         # Europe/Kiev goes from UTC+3 to UTC+2 in the early hours of 10/30.
         self.assertEqual(
-            rule.generate_dates(),
+            rule.get_dates(),
             [
                 datetime.datetime(2022, 10, 29, 7),
                 datetime.datetime(2022, 10, 30, 8),
                 datetime.datetime(2022, 10, 31, 8),
                 datetime.datetime(2022, 11, 1, 8),
             ]
         )
 
         # Europe/Kiev goes to standard time (UTC+2) in the early hours of 1/30.
         # This offset should result in a datetime (UTC+3).
         past_clone = rule.clone_with_day_offset(-1)
 
         # One day before each date in the regular series.
         self.assertEqual(
-            past_clone.generate_dates(),
+            past_clone.get_dates(),
             [
                 datetime.datetime(2022, 10, 28, 7),
                 datetime.datetime(2022, 10, 29, 7),
                 datetime.datetime(2022, 10, 30, 8),
                 datetime.datetime(2022, 10, 31, 8),
             ]
         )
@@ -1419,14 +1417,145 @@
                 datetime.datetime(2022, 10, 28, 7),
                 datetime.datetime(2022, 10, 29, 7),
                 datetime.datetime(2022, 10, 30, 8),
                 datetime.datetime(2022, 10, 31, 8),
             ]
         )
 
+    def test_offset(self):
+        """
+        Assert the offset method adjusts a given date by the given number of days
+        """
+        self.assertEqual(
+            RRule(day_offset=1).offset(datetime.datetime(2023, 1, 1)),
+            datetime.datetime(2023, 1, 2)
+        )
+
+        self.assertEqual(
+            RRule(day_offset=-1).offset(datetime.datetime(2023, 1, 1)),
+            datetime.datetime(2022, 12, 31)
+        )
+
+        self.assertEqual(
+            RRule().offset(datetime.datetime(2023, 1, 1)),
+            datetime.datetime(2023, 1, 1)
+        )
+
+    def test_day_offset(self):
+        """
+        Assert that the field, day_offset, adjusts all generated dates.
+        """
+        params = {
+            'freq': rrule.MONTHLY,
+            'interval': 1,
+            'dtstart': datetime.datetime(2016, 12, 31),
+            'bymonthday': 1,
+            'until': datetime.datetime(2017, 4, 30),
+        }
+
+        rule = RRule(
+            rrule_params=params,
+            time_zone=pytz.timezone('US/Eastern'),
+            occurrence_handler_path='ambition_utils.rrule.tests.model_tests.MockHandler',
+            day_offset=1,
+        )
+        next_dates = rule.get_dates()
+
+        # Check a few dates
+        self.assertEqual(len(next_dates), 4)
+
+        self.assertEqual(next_dates[0], datetime.datetime(2017, 1, 2, 5))
+        self.assertEqual(next_dates[1], datetime.datetime(2017, 2, 2, 5))
+        self.assertEqual(next_dates[2], datetime.datetime(2017, 3, 2, 5))
+        self.assertEqual(next_dates[3], datetime.datetime(2017, 4, 2, 4))  # DST change for US/Eastern
+
+        # Run pre save again to make sure it doesn't mess up params
+        rule.pre_save_hooks()
+
+        # Get next dates to compare against
+        more_next_dates = rule.get_dates()
+        self.assertEqual(next_dates, more_next_dates)
+
+        rule = RRule(
+            rrule_params=params,
+            time_zone=pytz.timezone('US/Eastern'),
+            occurrence_handler_path='ambition_utils.rrule.tests.model_tests.MockHandler',
+            day_offset=-1,
+        )
+
+        next_dates = rule.get_dates()
+
+        # Check a few dates
+        self.assertEqual(len(next_dates), 4)
+
+        self.assertEqual(next_dates[0], datetime.datetime(2016, 12, 31, 5))
+        self.assertEqual(next_dates[1], datetime.datetime(2017, 1, 31, 5))
+        self.assertEqual(next_dates[2], datetime.datetime(2017, 2, 28, 5))
+        self.assertEqual(next_dates[3], datetime.datetime(2017, 3, 31, 4))  # DST change for US/Eastern
+
+        # Run pre save again to make sure it doesn't mess up params
+        rule.pre_save_hooks()
+
+        # Get next dates to compare against
+        more_next_dates = rule.get_dates()
+        self.assertEqual(next_dates, more_next_dates)
+
+    def test_next_occurrences_day_offset(self):
+        """
+        Make sure that the correct occurrences are selected when a day offset is configured.
+        """
+        params = {
+            'freq': rrule.WEEKLY,
+            'interval': 1,
+            'dtstart': datetime.datetime(2017, 1, 2),
+        }
+
+        rrule1 = G(
+            RRule,
+            rrule_params=params,
+            occurrence_handler_path='ambition_utils.rrule.tests.model_tests.HandlerOne',
+            day_offset=1
+        )
+
+        params = {
+            'freq': rrule.WEEKLY,
+            'interval': 1,
+            'dtstart': datetime.datetime(2017, 1, 2),
+        }
+
+        rrule2 = G(
+            RRule,
+            rrule_params=params,
+            occurrence_handler_path='ambition_utils.rrule.tests.model_tests.HandlerTwo',
+            day_offset=-1
+        )
+
+        self.assertEqual(rrule1.next_occurrence, datetime.datetime(2017, 1, 3))
+        self.assertEqual(rrule2.next_occurrence, datetime.datetime(2017, 1, 1))
+
+        with freeze_time('1-3-2017'):
+            RRule.objects.handle_overdue()
+
+            rrule1.refresh_from_db()
+            rrule2.refresh_from_db()
+
+            # Both should be progressed
+            self.assertEqual(rrule1.next_occurrence, datetime.datetime(2017, 1, 10))
+            self.assertEqual(rrule2.next_occurrence, datetime.datetime(2017, 1, 8))
+
+        with freeze_time('1-8-2017'):
+            RRule.objects.handle_overdue()
+
+            rrule1.refresh_from_db()
+            rrule2.refresh_from_db()
+
+            # Both should be progressed
+            self.assertEqual(rrule1.next_occurrence, datetime.datetime(2017, 1, 10))
+            self.assertEqual(rrule2.next_occurrence, datetime.datetime(2017, 1, 15))
+
 
 class RRuleWithExclusionTest(TestCase):
     def test_exclusion(self):
         weekly_program = Program.objects.create(name='Weekly Program')
         weekly_rrule = RRule.objects.create(
             rrule_params={
                 'freq': rrule.DAILY,
```

### Comparing `ambition-utils-3.1.7/ambition_utils/rrule/tests/models.py` & `ambition-utils-3.1.8/ambition_utils/rrule/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/sql.py` & `ambition-utils-3.1.8/ambition_utils/sql.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/tests/field_tests.py` & `ambition-utils-3.1.8/ambition_utils/tests/field_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/tests/form_tests.py` & `ambition-utils-3.1.8/ambition_utils/tests/form_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/tests/migrations/0002_auto_20230124_1754.py` & `ambition-utils-3.1.8/ambition_utils/tests/migrations/0002_auto_20230124_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/tests/sql_tests.py` & `ambition-utils-3.1.8/ambition_utils/tests/sql_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/tests/time_helper_tests.py` & `ambition-utils-3.1.8/ambition_utils/tests/time_helper_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/time_helpers.py` & `ambition-utils-3.1.8/ambition_utils/time_helpers.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/transaction/decorators.py` & `ambition-utils-3.1.8/ambition_utils/transaction/decorators.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/transaction/tests/durable_tests.py` & `ambition-utils-3.1.8/ambition_utils/transaction/tests/durable_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils/transaction/utils.py` & `ambition-utils-3.1.8/ambition_utils/transaction/utils.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.7/ambition_utils.egg-info/PKG-INFO` & `ambition-utils-3.1.8/ambition_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.7
+Version: 3.1.8
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Keywords: django,database,query,sql,postgres,upsert
 Platform: UNKNOWN
```

### Comparing `ambition-utils-3.1.7/ambition_utils.egg-info/SOURCES.txt` & `ambition-utils-3.1.8/ambition_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 ambition_utils/rrule/forms.py
 ambition_utils/rrule/handler.py
 ambition_utils/rrule/models.py
 ambition_utils/rrule/migrations/0001_initial.py
 ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
 ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
 ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
+ambition_utils/rrule/migrations/0005_auto_20230802_1548.py
 ambition_utils/rrule/migrations/__init__.py
 ambition_utils/rrule/tests/__init__.py
 ambition_utils/rrule/tests/apps.py
 ambition_utils/rrule/tests/form_tests.py
 ambition_utils/rrule/tests/model_tests.py
 ambition_utils/rrule/tests/models.py
 ambition_utils/rrule/tests/migrations/0001_initial.py
```

### Comparing `ambition-utils-3.1.7/setup.py` & `ambition-utils-3.1.8/setup.py`

 * *Files identical despite different names*

